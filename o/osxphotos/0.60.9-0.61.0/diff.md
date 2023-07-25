# Comparing `tmp/osxphotos-0.60.9.tar.gz` & `tmp/osxphotos-0.61.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.9.tar", last modified: Mon Jul 17 01:15:27 2023, max compression
+gzip compressed data, was "osxphotos-0.61.0.tar", last modified: Tue Jul 25 13:48:52 2023, max compression
```

## Comparing `osxphotos-0.60.9.tar` & `osxphotos-0.61.0.tar`

### file list

```diff
@@ -1,238 +1,240 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:27.001562 osxphotos-0.60.9/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.9/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.9/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-17 01:15:27.001150 osxphotos-0.60.9/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   226697 2023-07-17 01:15:15.000000 osxphotos-0.60.9/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.9/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.951934 osxphotos-0.60.9/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.9/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.9/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    17162 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-17 01:15:06.000000 osxphotos-0.60.9/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.9/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.9/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.961505 osxphotos-0.60.9/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.9/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.9/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    27724 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.9/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   108212 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.9/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.9/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.9/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.9/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.9/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.9/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.9/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.962091 osxphotos-0.60.9/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.9/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1479305 2023-07-17 01:15:23.000000 osxphotos-0.60.9/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.9/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.9/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.9/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.9/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    93623 2023-07-15 14:18:05.000000 osxphotos-0.60.9/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    87376 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.964193 osxphotos-0.60.9/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10525 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   150545 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5681 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8828 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.9/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-17 01:15:14.000000 osxphotos-0.60.9/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.9/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.9/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    25757 2023-07-03 07:44:41.000000 osxphotos-0.60.9/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/platform.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.9/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.965558 osxphotos-0.60.9/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.9/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.9/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.9/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.9/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.9/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    14487 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.9/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.968771 osxphotos-0.60.9/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.9/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.953863 osxphotos-0.60.9/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6527 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-17 01:15:27.001674 osxphotos-0.60.9/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.9/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:27.000543 osxphotos-0.60.9/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:27.000830 osxphotos-0.60.9/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.9/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.9/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   275628 2023-07-15 14:18:05.000000 osxphotos-0.60.9/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.9/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.9/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.9/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.9/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.9/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.9/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.9/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.9/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.9/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.9/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.9/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.9/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.9/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_photosalbum_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.9/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.9/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.9/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.9/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.9/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)    48444 2023-07-16 22:09:19.000000 osxphotos-0.60.9/tests/test_sonoma_14_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.9/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.9/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.9/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.9/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.9/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.9/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.892767 osxphotos-0.61.0/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2023-07-25 05:05:05.000000 osxphotos-0.61.0/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2023-07-25 05:05:05.000000 osxphotos-0.61.0/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-25 13:48:52.892439 osxphotos-0.61.0/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   230303 2023-07-25 13:48:38.000000 osxphotos-0.61.0/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-07-25 05:05:05.000000 osxphotos-0.61.0/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.828211 osxphotos-0.61.0/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17341 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-25 13:48:33.000000 osxphotos-0.61.0/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.840606 osxphotos-0.61.0/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27724 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      715 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4215 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   111312 2023-07-25 13:44:50.000000 osxphotos-0.61.0/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5782 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10225 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23803 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5369 2023-07-25 13:44:50.000000 osxphotos-0.61.0/osxphotos/cli/sidecar.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      695 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.841258 osxphotos-0.61.0/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1479401 2023-07-25 13:48:48.000000 osxphotos-0.61.0/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    93837 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    87960 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.844204 osxphotos-0.61.0/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      224 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10525 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1785 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   150713 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5699 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8828 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-25 13:48:37.000000 osxphotos-0.61.0/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    25757 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)      696 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/platform.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.845263 osxphotos-0.61.0/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14487 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.846045 osxphotos-0.61.0/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-07-25 05:05:05.000000 osxphotos-0.61.0/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.829977 osxphotos-0.61.0/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-25 13:48:52.000000 osxphotos-0.61.0/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6594 2023-07-25 13:48:52.000000 osxphotos-0.61.0/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-25 13:48:52.000000 osxphotos-0.61.0/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-25 13:48:52.000000 osxphotos-0.61.0/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-25 13:48:52.000000 osxphotos-0.61.0/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-25 13:48:52.000000 osxphotos-0.61.0/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-25 13:48:52.892811 osxphotos-0.61.0/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-07-25 05:05:05.000000 osxphotos-0.61.0/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.891579 osxphotos-0.61.0/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-25 13:48:52.891990 osxphotos-0.61.0/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2023-07-25 05:05:14.000000 osxphotos-0.61.0/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2023-07-25 05:05:14.000000 osxphotos-0.61.0/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   275628 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15160 2023-07-25 13:44:50.000000 osxphotos-0.61.0/tests/test_cli_export_sidecar_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      861 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      931 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_photosalbum_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48444 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_sonoma_14_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      487 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-07-25 05:05:15.000000 osxphotos-0.61.0/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.9/LICENSE` & `osxphotos-0.61.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/PKG-INFO` & `osxphotos-0.61.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.9
+Version: 0.61.0
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.9/README.md` & `osxphotos-0.61.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1113,14 +1113,60 @@
                                   ext' to ignore the photo extension. Resulting
                                   sidecar files will have name in format
                                   'IMG_1234.xmp'. Warning: this may result in
                                   sidecar filename collisions if there are files
                                   of different types but the same name in the
                                   output directory, e.g. 'IMG_1234.JPG' and
                                   'IMG_1234.MOV'.
+  --sidecar-template MAKO_TEMPLATE_FILE SIDECAR_FILENAME_TEMPLATE WRITE_SKIPPED STRIP_WHITESPACE STRIP_LINES
+                                  Create a custom sidecar file for each photo
+                                  exported with user provided Mako template
+                                  (MAKO_TEMPLATE_FILE). MAKO_TEMPLATE_FILE must
+                                  be a valid Mako template (see
+                                  https://www.makotemplates.org/). The template
+                                  will passed the following variables: photo
+                                  (PhotoInfo object for the photo being
+                                  exported), sidecar_path (pathlib.Path object
+                                  for the path to the sidecar being written),
+                                  and photo_path (pathlib.Path object for the
+                                  path to the exported photo.
+                                  SIDECAR_FILENAME_TEMPLATE must be a valid
+                                  template string (see Templating System in
+                                  help) which will be rendered to generate the
+                                  filename of the sidecar file. The `{filepath}`
+                                  template variable may be used in the
+                                  SIDECAR_FILENAME_TEMPLATE to refer to the
+                                  filename of the photo being exported.
+                                  WRITE_SKIPPED is a boolean value (true/false,
+                                  yes/no, 1/0 are all valid values) and
+                                  indicates whether or not write the sidecar
+                                  file even if the photo is skipped during
+                                  export. If WRITE_SKIPPED is false, the sidecar
+                                  file will not be written if the photo is
+                                  skipped during export. If WRITE_SKIPPED is
+                                  true, the sidecar file will be written even if
+                                  the photo is skipped during export.
+                                  STRIP_WHITESPACE and STRIP_LINES are boolean
+                                  values (true/false, yes/no, 1/0 are all valid
+                                  values) and indicate whether or not to strip
+                                  whitespace and blank lines from the resulting
+                                  sidecar file. For example, to create a sidecar
+                                  file with extension .xmp using a template file
+                                  named 'sidecar.mako' and write a sidecar for
+                                  skipped photos and strip blank lines but not
+                                  whitespace: `--sidecar-template sidecar.mako
+                                  '{filepath}.xmp' yes no yes`. To do the same
+                                  but to drop the photo extension from the
+                                  sidecar filename: `--sidecar-template
+                                  sidecar.mako
+                                  '{filepath.parent}/{filepath.stem}.xmp' yes no
+                                  yes --sidecar-drop-ext`. For an example Mako
+                                  file see https://raw.githubusercontent.com/Rhe
+                                  tTbull/osxphotos/main/examples/custom_sidecar.
+                                  mako
   --exiftool                      Use exiftool to write metadata directly to
                                   exported photos. To use this option, exiftool
                                   must be installed and in the path.  exiftool
                                   may be installed from https://exiftool.org/.
                                   Cannot be used with --export-as-hardlink.
                                   Writes the following metadata:
                                   EXIF:ImageDescription, XMP:Description (see
@@ -2120,15 +2166,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.9'
+{osxphotos_version}             The osxphotos version, e.g. '0.61.0'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2607,15 +2653,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.9'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.61.0'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
@@ -2681,15 +2727,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://kradalby.no"><img src="https://avatars1.githubusercontent.com/u/98431?v=4?s=75" width="75px;" alt="Kristoffer Dalby"/><br /><sub><b>Kristoffer Dalby</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=kradalby" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Rott-Apple"><img src="https://avatars1.githubusercontent.com/u/67875570?v=4?s=75" width="75px;" alt="Rott-Apple"/><br /><sub><b>Rott-Apple</b></sub></a><br /><a href="#research-Rott-Apple" title="Research">🔬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/narensankar0529"><img src="https://avatars3.githubusercontent.com/u/74054766?v=4?s=75" width="75px;" alt="narensankar0529"/><br /><sub><b>narensankar0529</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Anarensankar0529" title="Bug reports">🐛</a> <a href="#userTesting-narensankar0529" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/martinhrpi"><img src="https://avatars2.githubusercontent.com/u/19407684?v=4?s=75" width="75px;" alt="Martin"/><br /><sub><b>Martin</b></sub></a><br /><a href="#research-martinhrpi" title="Research">🔬</a> <a href="#userTesting-martinhrpi" title="User Testing">📓</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/davidjroos"><img src="https://avatars.githubusercontent.com/u/15630844?v=4?s=75" width="75px;" alt="davidjroos "/><br /><sub><b>davidjroos </b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=davidjroos" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://neilpa.me"><img src="https://avatars.githubusercontent.com/u/42419?v=4?s=75" width="75px;" alt="Neil Pankey"/><br /><sub><b>Neil Pankey</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=neilpa" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://neilpa.me"><img src="https://avatars.githubusercontent.com/u/42419?v=4?s=75" width="75px;" alt="Neil Pankey"/><br /><sub><b>Neil Pankey</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=neilpa" title="Code">💻</a> <a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aneilpa" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://aaronweb.net/"><img src="https://avatars.githubusercontent.com/u/604665?v=4?s=75" width="75px;" alt="Aaron van Geffen"/><br /><sub><b>Aaron van Geffen</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=AaronVanGeffen" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ubrandes"><img src="https://avatars.githubusercontent.com/u/59647284?v=4?s=75" width="75px;" alt="ubrandes "/><br /><sub><b>ubrandes </b></sub></a><br /><a href="#ideas-ubrandes" title="Ideas, Planning, & Feedback">🤔</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://blog.dewost.com/"><img src="https://avatars.githubusercontent.com/u/17090228?v=4?s=75" width="75px;" alt="Philippe Dewost"/><br /><sub><b>Philippe Dewost</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=pdewost" title="Documentation">📖</a> <a href="#example-pdewost" title="Examples">💡</a> <a href="#ideas-pdewost" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kaduskj"><img src="https://avatars.githubusercontent.com/u/983067?v=4?s=75" width="75px;" alt="kaduskj"/><br /><sub><b>kaduskj</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Akaduskj" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mkirkland4874"><img src="https://avatars.githubusercontent.com/u/36466711?v=4?s=75" width="75px;" alt="mkirkland4874"/><br /><sub><b>mkirkland4874</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Amkirkland4874" title="Bug reports">🐛</a> <a href="#example-mkirkland4874" title="Examples">💡</a></td>
```

### Comparing `osxphotos-0.60.9/README.rst` & `osxphotos-0.61.0/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/__init__.py` & `osxphotos-0.61.0/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/_constants.py` & `osxphotos-0.61.0/osxphotos/_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 # Ranges for model version by Photos version
 _PHOTOS_5_MODEL_VERSION = [13000, 13999]
 _PHOTOS_6_MODEL_VERSION = [14000, 14999]
 _PHOTOS_7_MODEL_VERSION = [15000, 15999]  # Dev preview: 15134, 12.1: 15331
 _PHOTOS_8_MODEL_VERSION = [16000, 16999]  # Ventura dev preview: 16119
 _PHOTOS_9_MODEL_VERSION = [17000, 17999]  # Sonoma dev preview: 17120
 
+# the preview versions of 12.0.0 had a difference schema for syndication info so need to check model version before processing
+_PHOTOS_SYNDICATION_MODEL_VERSION = 15323 # 12.0.1
+
 # some table names differ between Photos 5 and later versions
 _DB_TABLE_NAMES = {
     5: {
         "ASSET": "ZGENERICASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_37KEYWORDS",
         "ALBUM_JOIN": "Z_26ASSETS.Z_34ASSETS",
         "ALBUM_SORT_ORDER": "Z_26ASSETS.Z_FOK_34ASSETS",
```

### Comparing `osxphotos-0.60.9/osxphotos/adjustmentsinfo.py` & `osxphotos-0.61.0/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/albuminfo.py` & `osxphotos-0.61.0/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/__init__.py` & `osxphotos-0.61.0/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/about.py` & `osxphotos-0.61.0/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/add_locations.py` & `osxphotos-0.61.0/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/albums.py` & `osxphotos-0.61.0/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/batch_edit.py` & `osxphotos-0.61.0/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/cli.py` & `osxphotos-0.61.0/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/cli_commands.py` & `osxphotos-0.61.0/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/cli_params.py` & `osxphotos-0.61.0/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.61.0/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/color_themes.py` & `osxphotos-0.61.0/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/common.py` & `osxphotos-0.61.0/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/darkmode.py` & `osxphotos-0.61.0/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/debug_dump.py` & `osxphotos-0.61.0/osxphotos/cli/debug_dump.py`

 * *Files 20% similar despite different names*

```diff
@@ -89,21 +89,33 @@
             pprint.pprint(photosdb._dbfaces_pk)
             print("_dbpersons_pk:")
             pprint.pprint(photosdb._dbpersons_pk)
             print("_dbpersons_fullname:")
             pprint.pprint(photosdb._dbpersons_fullname)
         elif attr == "photos":
             photos = photosdb.query(options=query_options)
-            uuid = [photo.uuid for photo in photos]
-            for uuid_ in uuid:
-                print(f"_dbphotos['{uuid_}']:")
+            for p in photos:
+                # print info on each photo
+                # catch any errors and continue (because if we're using debug-dump, it might be because of an error)
+                print(f"photo: {p.uuid}")
+                print(f"_dbphotos['{p.uuid}']:")
                 try:
-                    pprint.pprint(photosdb._dbphotos[uuid_])
+                    print(photosdb._dbphotos[p.uuid])
                 except KeyError:
-                    print(f"Did not find uuid {uuid_} in _dbphotos")
+                    print(f"Did not find uuid {p.uuid} in _dbphotos")
+                print("PhotoInfo:")
+                try:
+                    print(p.asdict(shallow=False))
+                except Exception as e:
+                    print(f"Error dumping PhotoInfo.asdict(): {e}")
+                print("ZASSET")
+                print(p.tables().ZASSET.rows_dict())
+                print("ZADDITIONALASSETATTRIBUTES")
+                print(p.tables().ZADDITIONALASSETATTRIBUTES.rows_dict())
+                print("-" * 40)
         else:
             try:
                 val = getattr(photosdb, attr)
                 print(f"{attr}:")
                 pprint.pprint(val)
             except Exception:
                 print(f"Did not find attribute {attr} in PhotosDB")
```

### Comparing `osxphotos-0.60.9/osxphotos/cli/docs.py` & `osxphotos-0.61.0/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/dump.py` & `osxphotos-0.61.0/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.61.0/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/export.py` & `osxphotos-0.61.0/osxphotos/cli/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,18 @@
     OSXPHOTOS_CRASH_LOG,
     OSXPHOTOS_HIDDEN,
     get_photos_db,
     noop,
 )
 from .help import ExportCommand, get_help_msg
 from .list import _list_libraries
-from .param_types import ExportDBType, FunctionCall, TemplateString
+from .param_types import BooleanString, ExportDBType, FunctionCall, TemplateString
 from .report_writer import ReportWriterNoOp, export_report_writer_factory
 from .rich_progress import rich_progress
+from .sidecar import generate_user_sidecar
 from .verbose import get_verbose_console, verbose_print
 
 
 @click.command(cls=ExportCommand)
 @DB_OPTION
 @VERBOSE_OPTION
 @TIMESTAMP_OPTION
@@ -300,15 +301,16 @@
 @click.option(
     "--export-aae",
     is_flag=True,
     help="Also export an adjustments file detailing edits made to the original. "
     "The resulting file is named photoname.AAE. "
     "Note that to import these files back to Photos succesfully, you also need to "
     "export the edited photo and match the filename format Photos.app expects: "
-    "--filename 'IMG_{edited_version?E,}{id:04d}' --edited-suffix ''")
+    "--filename 'IMG_{edited_version?E,}{id:04d}' --edited-suffix ''",
+)
 @click.option(
     "--sidecar",
     default=None,
     multiple=True,
     metavar="FORMAT",
     type=click.Choice(["xmp", "json", "exiftool"], case_sensitive=False),
     help="Create sidecar for each photo exported; valid FORMAT values: xmp, json, exiftool; "
@@ -335,14 +337,49 @@
     "By default, sidecar files are named in format 'photo_filename.photo_ext.sidecar_ext', "
     "e.g. 'IMG_1234.JPG.xmp'. Use '--sidecar-drop-ext' to ignore the photo extension. "
     "Resulting sidecar files will have name in format 'IMG_1234.xmp'. "
     "Warning: this may result in sidecar filename collisions if there are files of different "
     "types but the same name in the output directory, e.g. 'IMG_1234.JPG' and 'IMG_1234.MOV'.",
 )
 @click.option(
+    "--sidecar-template",
+    metavar="MAKO_TEMPLATE_FILE SIDECAR_FILENAME_TEMPLATE WRITE_SKIPPED STRIP_WHITESPACE STRIP_LINES",
+    multiple=True,
+    type=click.Tuple(
+        [
+            click.Path(dir_okay=False, file_okay=True, exists=True),
+            TemplateString(),
+            BooleanString(),
+            BooleanString(),
+            BooleanString(),
+        ]
+    ),
+    help="Create a custom sidecar file for each photo exported with user provided Mako template (MAKO_TEMPLATE_FILE). "
+    "MAKO_TEMPLATE_FILE must be a valid Mako template (see https://www.makotemplates.org/). "
+    "The template will passed the following variables: photo (PhotoInfo object for the photo being exported), "
+    "sidecar_path (pathlib.Path object for the path to the sidecar being written), and "
+    "photo_path (pathlib.Path object for the path to the exported photo. "
+    "SIDECAR_FILENAME_TEMPLATE must be a valid template string (see Templating System in help) "
+    "which will be rendered to generate the filename of the sidecar file. "
+    "The `{filepath}` template variable may be used in the SIDECAR_FILENAME_TEMPLATE to refer to the filename of the "
+    "photo being exported. "
+    "WRITE_SKIPPED is a boolean value (true/false, yes/no, 1/0 are all valid values) and indicates whether or not "
+    "write the sidecar file even if the photo is skipped during export. "
+    "If WRITE_SKIPPED is false, the sidecar file will not be written if the photo is skipped during export. "
+    "If WRITE_SKIPPED is true, the sidecar file will be written even if the photo is skipped during export. "
+    "STRIP_WHITESPACE and STRIP_LINES are boolean values (true/false, yes/no, 1/0 are all valid values) "
+    "and indicate whether or not to strip whitespace and blank lines from the resulting sidecar file. "
+    "For example, to create a sidecar file with extension .xmp using a template file named 'sidecar.mako' "
+    "and write a sidecar for skipped photos and strip blank lines but not whitespace: "
+    "`--sidecar-template sidecar.mako '{filepath}.xmp' yes no yes`. "
+    "To do the same but to drop the photo extension from the sidecar filename: "
+    "`--sidecar-template sidecar.mako '{filepath.parent}/{filepath.stem}.xmp' yes no yes --sidecar-drop-ext`. "
+    "For an example Mako file see https://raw.githubusercontent.com/RhetTbull/osxphotos/main/examples/custom_sidecar.mako",
+)
+@click.option(
     "--exiftool",
     is_flag=True,
     help="Use exiftool to write metadata directly to exported photos. "
     "To use this option, exiftool must be installed and in the path.  "
     "exiftool may be installed from https://exiftool.org/.  "
     "Cannot be used with --export-as-hardlink.  Writes the following metadata: "
     "EXIF:ImageDescription, XMP:Description (see also --description-template); "
@@ -859,14 +896,15 @@
     save_config,
     screenshot,
     selfie,
     shared,
     export_aae,
     sidecar,
     sidecar_drop_ext,
+    sidecar_template,
     skip_bursts,
     skip_edited,
     skip_live,
     skip_original_if_edited,
     skip_raw,
     skip_uuid,
     skip_uuid_from_file,
@@ -1086,14 +1124,15 @@
         screenshot = cfg.screenshot
         selected = cfg.selected
         selfie = cfg.selfie
         shared = cfg.shared
         export_aae = cfg.export_aae
         sidecar = cfg.sidecar
         sidecar_drop_ext = cfg.sidecar_drop_ext
+        sidecar_template = cfg.sidecar_template
         skip_bursts = cfg.skip_bursts
         skip_edited = cfg.skip_edited
         skip_live = cfg.skip_live
         skip_original_if_edited = cfg.skip_original_if_edited
         skip_raw = cfg.skip_raw
         skip_uuid = cfg.skip_uuid
         skip_uuid_from_file = cfg.skip_uuid_from_file
@@ -1469,26 +1508,41 @@
                 f"Exporting [num]{num_photos}[/] photos{limit_str}", total=num_photos
             )
             for p in photos:
                 photo_num += 1
                 kwargs["photo"] = p
                 kwargs["photo_num"] = photo_num
                 export_results = export_photo(**kwargs)
+
+                # generate custom sidecars if needed
+                if sidecar_template:
+                    export_results += generate_user_sidecar(
+                        photo=p,
+                        export_results=export_results,
+                        sidecar_template=sidecar_template,
+                        exiftool_path=exiftool_path,
+                        export_dir=dest,
+                        dry_run=dry_run,
+                        verbose=verbose,
+                    )
+
+                # run post functions
                 if post_function:
                     for function in post_function:
                         # post function is tuple of (function, filename.py::function_name)
                         verbose(f"Calling post-function [bold]{function[1]}")
                         if not dry_run:
                             try:
                                 function[0](p, export_results, verbose)
                             except Exception as e:
                                 rich_echo_error(
                                     f"[error]Error running post-function [italic]{function[1]}[/italic]: {e}"
                                 )
 
+                # run post command
                 run_post_command(
                     photo=p,
                     post_command=post_command,
                     export_results=export_results,
                     export_dir=dest,
                     dry_run=dry_run,
                     exiftool_path=exiftool_path,
@@ -1663,14 +1717,16 @@
             + results.aae_written
             + results.sidecar_json_written
             + results.sidecar_json_skipped
             + results.sidecar_exiftool_written
             + results.sidecar_exiftool_skipped
             + results.sidecar_xmp_written
             + results.sidecar_xmp_skipped
+            + results.sidecar_user_written
+            + results.sidecar_user_skipped
             # include missing so a file that was already in export directory
             # but was missing on --update doesn't get deleted
             # (better to have old version than none)
             + results.missing
             # include files that have error in case they exist from previous export
             + [r[0] for r in results.error]
             + db_files
@@ -1762,15 +1818,15 @@
     export_preview=False,
     preview_suffix=None,
     preview_if_missing=False,
     photo_num=1,
     num_photos=1,
     tmpdir=None,
     update_errors=False,
-):
+) -> ExportResults:
     """Helper function for export that does the actual export
 
     Args:
         photo: PhotoInfo object
         dest: destination path as string
         album_keyword: bool; if True, exports album names as keywords in metadata
         convert_to_jpeg: bool; if True, converts non-jpeg images to jpeg
@@ -1813,14 +1869,15 @@
         skip_original_if_edited: bool; if True does not export original if photo has been edited
         touch_file: bool; sets file's modification time to match photo date
         update: bool, only export updated photos
         update_errors: bool, attempt to re-export photos that previously produced errors even if they otherwise would not be exported
         use_photos_export: bool; if True forces the use of AppleScript to export even if photo not missing
         verbose: callable for verbose output
         tmpdir: optional str; temporary directory to use for export
+
     Returns:
         list of path(s) of exported photo or None if photo was missing
 
     Raises:
         ValueError on invalid filename_template
     """
     export_original = not (skip_original_if_edited and photo.hasadjustments)
@@ -2185,15 +2242,15 @@
     touch_file,
     update,
     update_errors,
     use_photos_export,
     use_photokit,
     verbose,
     tmpdir,
-):
+) -> ExportResults:
     """Export photo to directory dest_path"""
 
     results = ExportResults()
 
     # don't try to export photos in the trash if they're missing
     photo_path = photo.path if export_original else photo.path_edited
     if photo.intrash and not photo_path and not preview_if_missing:
@@ -2735,17 +2792,14 @@
     export_dir,
     dry_run,
     exiftool_path,
     export_db,
     verbose,
 ):
     # todo: pass in RenderOptions from export? (e.g. so it contains strip, etc?)
-    # todo: need a shell_quote template type:
-    # {shell_quote,{filepath}/foo/bar}
-    # that quotes everything in the default value
     for category, command_template in post_command:
         files = getattr(export_results, category)
         for f in files:
             # some categories, like error, return a tuple of (file, error str)
             if isinstance(f, tuple):
                 f = f[0]
             render_options = RenderOptions(export_dir=export_dir, filepath=f)
```

### Comparing `osxphotos-0.60.9/osxphotos/cli/exportdb.py` & `osxphotos-0.61.0/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/grep.py` & `osxphotos-0.61.0/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/help.py` & `osxphotos-0.61.0/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/import_cli.py` & `osxphotos-0.61.0/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/info.py` & `osxphotos-0.61.0/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.61.0/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/keywords.py` & `osxphotos-0.61.0/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/kvstore.py` & `osxphotos-0.61.0/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/labels.py` & `osxphotos-0.61.0/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/list.py` & `osxphotos-0.61.0/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/orphans.py` & `osxphotos-0.61.0/osxphotos/cli/orphans.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,30 @@
 
     # shared derivatives
     directory = joinpath(
         "resources", "cloudsharing", "resources", "derivatives", "masters"
     )
     scan_for_files(directory, uuids_in_library)
 
+    # scopes directory (Photos 7+)
+    if photosdb.photos_version >= 7:
+        verbose_("Scanning scopes cloudsharing files")
+        directory = joinpath(
+            photosdb.library_path, "scopes", "cloudsharing", "resources"
+        )
+        scan_for_files(directory, uuids_in_library)
+
+        verbose_("Scanning scopes syndication files")
+        directory = joinpath(photosdb.library_path, "scopes", "syndication")
+        scan_for_files(directory, uuids_in_library)
+
+        verbose_("Scanning scopes momentshared files")
+        directory = joinpath(photosdb.library_path, "scopes", "momentshared")
+        scan_for_files(directory, uuids_in_library)
+
     # find orphans
     possible_orphans = []
     for uuid, files in uuids_in_library.items():
         if uuid not in uuids_in_db:
             possible_orphans.extend(files)
 
     echo(
```

### Comparing `osxphotos-0.60.9/osxphotos/cli/param_types.py` & `osxphotos-0.61.0/osxphotos/cli/param_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from osxphotos.phototemplate import PhotoTemplate, RenderOptions
 from osxphotos.timeutils import time_string_to_datetime, utc_offset_string_to_seconds
 from osxphotos.timezones import Timezone
 from osxphotos.utils import expand_and_validate_filepath, load_function
 
 __all__ = [
     "BitMathSize",
+    "BooleanString",
     "DateOffset",
     "DateTimeISO8601",
     "DeprecatedPath",
     "ExportDBType",
     "FunctionCall",
     "Latitude",
     "Longitude",
@@ -298,7 +299,23 @@
             if longitude < -180 or longitude > 180:
                 raise ValueError
             return longitude
         except Exception:
             self.fail(
                 f"Invalid longitude {value}. Must be a floating point number between -180 and 180."
             )
+
+
+class BooleanString(click.ParamType):
+    """A boolean string in the format True/False, Yes/No, T/F, Y/N, 1/0 (case insensitive)"""
+
+    name = "BooleanString"
+
+    def convert(self, value, param, ctx):
+        if value.lower() in ["true", "yes", "t", "y", "1"]:
+            return True
+        elif value.lower() in ["false", "no", "f", "n", "0"]:
+            return False
+        else:
+            self.fail(
+                f"Invalid boolean string {value}. Must be one of True/False, Yes/No, T/F, Y/N, 1/0 (case insensitive)."
+            )
```

### Comparing `osxphotos-0.60.9/osxphotos/cli/persons.py` & `osxphotos-0.61.0/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/photo_inspect.py` & `osxphotos-0.61.0/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/places.py` & `osxphotos-0.61.0/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/print_photo_info.py` & `osxphotos-0.61.0/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/query.py` & `osxphotos-0.61.0/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/repl.py` & `osxphotos-0.61.0/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/report_writer.py` & `osxphotos-0.61.0/osxphotos/cli/report_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
             "exiftool_warning",
             "exiftool_error",
             "extended_attributes_written",
             "extended_attributes_skipped",
             "cleanup_deleted_file",
             "cleanup_deleted_directory",
             "exported_album",
+            "sidecar_user",
         ]
 
         mode = "a" if append else "w"
         self._output_fh = open(self.output_file, mode)
 
         self._csv_writer = csv.DictWriter(self._output_fh, fieldnames=report_columns)
         if not append:
@@ -193,17 +194,17 @@
 
         all_results = prepare_export_results_for_writing(export_results)
         for data in list(all_results.values()):
             data["report_id"] = self.report_id
             cursor = self._conn.cursor()
             cursor.execute(
                 "INSERT INTO report "
-                "(datetime, filename, exported, new, updated, skipped, exif_updated, touched, converted_to_jpeg, sidecar_xmp, sidecar_json, sidecar_exiftool, missing, error, exiftool_warning, exiftool_error, extended_attributes_written, extended_attributes_skipped, cleanup_deleted_file, cleanup_deleted_directory, exported_album, report_id) "
+                "(datetime, filename, exported, new, updated, skipped, exif_updated, touched, converted_to_jpeg, sidecar_xmp, sidecar_json, sidecar_exiftool, missing, error, exiftool_warning, exiftool_error, extended_attributes_written, extended_attributes_skipped, cleanup_deleted_file, cleanup_deleted_directory, exported_album, report_id, sidecar_user) "  # noqa
                 "VALUES "
-                "(:datetime, :filename, :exported, :new, :updated, :skipped, :exif_updated, :touched, :converted_to_jpeg, :sidecar_xmp, :sidecar_json, :sidecar_exiftool, :missing, :error, :exiftool_warning, :exiftool_error, :extended_attributes_written, :extended_attributes_skipped, :cleanup_deleted_file, :cleanup_deleted_directory, :exported_album, :report_id);",
+                "(:datetime, :filename, :exported, :new, :updated, :skipped, :exif_updated, :touched, :converted_to_jpeg, :sidecar_xmp, :sidecar_json, :sidecar_exiftool, :missing, :error, :exiftool_warning, :exiftool_error, :extended_attributes_written, :extended_attributes_skipped, :cleanup_deleted_file, :cleanup_deleted_directory, :exported_album, :report_id, :sidecar_user);",  # noqa
                 data,
             )
         self._conn.commit()
 
     def close(self):
         """Close the output file"""
         self._conn.close()
@@ -258,14 +259,21 @@
         self._conn.commit()
 
         # migrate report table to add report_id if needed (#731)
         if "report_id" not in sqlite_columns(self._conn, "report"):
             self._conn.cursor().execute("ALTER TABLE report ADD COLUMN report_id TEXT;")
             self._conn.commit()
 
+        # migrate report table and add sidecar_user column if needed (#1123)
+        if "sidecar_user" not in sqlite_columns(self._conn, "report"):
+            self._conn.cursor().execute(
+                "ALTER TABLE report ADD COLUMN sidecar_user INTEGER;"
+            )
+            self._conn.commit()
+
         # create report_summary view
         c.execute(
             """
             CREATE VIEW IF NOT EXISTS report_summary AS
             SELECT
                 report_id,
                 datetime(MIN(datetime)) start_time,
@@ -343,14 +351,15 @@
                 "exiftool_warning": "",
                 "exiftool_error": "",
                 "extended_attributes_written": false,
                 "extended_attributes_skipped": false,
                 "cleanup_deleted_file": false,
                 "cleanup_deleted_directory": false,
                 "exported_album": "",
+                "sidecar_user": false,
             }
 
     for result in export_results.exported:
         all_results[str(result)]["exported"] = true
 
     for result in export_results.new:
         all_results[str(result)]["new"] = true
@@ -417,14 +426,22 @@
 
     for result in export_results.deleted_directories:
         all_results[str(result)]["cleanup_deleted_directory"] = true
 
     for result, album in export_results.exported_album:
         all_results[str(result)]["exported_album"] = album
 
+    for result in export_results.sidecar_user_written:
+        all_results[str(result)]["sidecar_user"] = true
+        all_results[str(result)]["exported"] = true
+
+    for result in export_results.sidecar_user_skipped:
+        all_results[str(result)]["sidecar_user"] = true
+        all_results[str(result)]["skipped"] = true
+
     return all_results
 
 
 def export_report_writer_factory(
     output_file: Union[str, bytes, os.PathLike], append: bool = False
 ) -> ReportWriterABC:
     """Return a ReportWriter instance appropriate for the output file type"""
```

### Comparing `osxphotos-0.60.9/osxphotos/cli/rich_progress.py` & `osxphotos-0.61.0/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/show_command.py` & `osxphotos-0.61.0/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/snap_diff.py` & `osxphotos-0.61.0/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/sync.py` & `osxphotos-0.61.0/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/sync_results.py` & `osxphotos-0.61.0/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/theme.py` & `osxphotos-0.61.0/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/timewarp.py` & `osxphotos-0.61.0/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/tutorial.py` & `osxphotos-0.61.0/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/uuid.py` & `osxphotos-0.61.0/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/verbose.py` & `osxphotos-0.61.0/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/cli/version.py` & `osxphotos-0.61.0/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/compare_exif.py` & `osxphotos-0.61.0/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/configoptions.py` & `osxphotos-0.61.0/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/crash_reporter.py` & `osxphotos-0.61.0/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/datetime_formatter.py` & `osxphotos-0.61.0/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/datetime_utils.py` & `osxphotos-0.61.0/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/debug.py` & `osxphotos-0.61.0/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/docs/docs.zip` & `osxphotos-0.61.0/osxphotos/docs/docs.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1479305 bytes, number of entries: 99
--rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
-drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jul-17 01:15 docs/_modules/index.html
-drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
--rw-r--r--  3.0 unx   333770 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/photoexporter.html
--rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
--rw-r--r--  3.0 unx   201029 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/export_db.html
--rw-r--r--  3.0 unx    14791 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/scoreinfo.html
-drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
--rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
--rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
--rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
--rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
--rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
--rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
--rw-r--r--  3.0 unx    52397 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   321986 tx defN 23-Jul-17 01:15 docs/_modules/osxphotos/photoinfo.html
--rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
--rw-r--r--  3.0 unx    29242 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   529210 tx defN 23-Jul-17 01:15 docs/_modules/osxphotos/photosdb/photosdb.html
--rw-r--r--  3.0 unx    39730 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosalbum.html
--rw-r--r--  3.0 unx    99009 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/placeinfo.html
--rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
--rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
--rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
--rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
--rw-r--r--  3.0 unx    62444 tx defN 23-Jul-17 01:15 docs/_modules/osxphotos/queryoptions.html
--rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
--rw-r--r--  3.0 unx    66040 tx defN 23-Jul-16 22:13 docs/_modules/osxphotos/_constants.html
-drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
--rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jul-17 01:15 docs/_sources/template_help.rst.txt
--rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
--rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
--rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
--rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
--rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
--rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
--rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
--rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
--rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
-drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
--rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
--rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
--rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
--rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Jul-17 01:15 docs/_static/documentation_options.js
--rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
--rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
--rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
--rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
--rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
--rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jul-17 01:15 docs/_static/copybutton.js
--rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
--rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jul-17 01:15 docs/_static/language_data.js
--rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
+Zip file size: 1479401 bytes, number of entries: 99
+-rw-r--r--  3.0 unx   331458 tx defN 23-Jul-25 05:05 docs/API_README.html
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 13:48 docs/_modules/
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jul-25 13:48 docs/_modules/index.html
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 13:48 docs/_modules/osxphotos/
+-rw-r--r--  3.0 unx   334470 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/photoexporter.html
+-rw-r--r--  3.0 unx   296439 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/phototemplate.html
+-rw-r--r--  3.0 unx   201029 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/export_db.html
+-rw-r--r--  3.0 unx    14791 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/scoreinfo.html
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 05:05 docs/_modules/osxphotos/photoinfo/
+-rw-r--r--  3.0 unx    14017 tx defN 23-Jul-25 05:05 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
+-rw-r--r--  3.0 unx   284197 tx defN 23-Jul-25 05:05 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
+-rw-r--r--  3.0 unx   195566 tx defN 23-Jul-25 05:05 docs/_modules/osxphotos/photoinfo/photoinfo.html
+-rw-r--r--  3.0 unx    33978 tx defN 23-Jul-25 05:05 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
+-rw-r--r--  3.0 unx    17959 tx defN 23-Jul-25 05:05 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
+-rw-r--r--  3.0 unx    43160 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/searchinfo.html
+-rw-r--r--  3.0 unx    52397 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/fileutil.html
+-rw-r--r--  3.0 unx   323894 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx    13131 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/exifinfo.html
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 13:48 docs/_modules/osxphotos/photosdb/
+-rw-r--r--  3.0 unx    29242 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
+-rw-r--r--  3.0 unx   529703 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx    39730 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/photosalbum.html
+-rw-r--r--  3.0 unx    99009 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/placeinfo.html
+-rw-r--r--  3.0 unx    22060 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/momentinfo.html
+-rw-r--r--  3.0 unx    82289 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/albuminfo.html
+-rw-r--r--  3.0 unx    78750 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/exiftool.html
+-rw-r--r--  3.0 unx    26012 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/debug.html
+-rw-r--r--  3.0 unx    62444 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/queryoptions.html
+-rw-r--r--  3.0 unx    81200 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/personinfo.html
+-rw-r--r--  3.0 unx    66337 tx defN 23-Jul-25 13:48 docs/_modules/osxphotos/_constants.html
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 13:48 docs/_sources/
+-rw-r--r--  3.0 unx      198 tx defN 23-Jul-25 05:05 docs/_sources/cli.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jul-25 13:48 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31240 tx defN 23-Jul-25 05:05 docs/_sources/tutorial.md.txt
+-rw-r--r--  3.0 unx       52 tx defN 23-Jul-25 05:05 docs/_sources/modules.rst.txt
+-rw-r--r--  3.0 unx    41238 tx defN 23-Jul-25 13:48 docs/_sources/tutorial.rst.txt
+-rw-r--r--  3.0 unx       93 tx defN 23-Jul-25 05:05 docs/_sources/reference.rst.txt
+-rw-r--r--  3.0 unx     7548 tx defN 23-Jul-25 05:05 docs/_sources/package_overview.rst.txt
+-rw-r--r--  3.0 unx      149 tx defN 23-Jul-25 05:05 docs/_sources/cli_export.rst.txt
+-rw-r--r--  3.0 unx   147706 tx defN 23-Jul-25 05:05 docs/_sources/API_README.rst.txt
+-rw-r--r--  3.0 unx      502 tx defN 23-Jul-25 05:05 docs/_sources/index.rst.txt
+-rw-r--r--  3.0 unx     4241 tx defN 23-Jul-25 05:05 docs/_sources/overview.rst.txt
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 13:48 docs/_static/
+-rw-r--r--  3.0 unx       90 bx defN 22-Dec-03 06:57 docs/_static/plus.png
+-rw-r--r--  3.0 unx     4712 tx defN 22-Dec-03 06:57 docs/_static/sphinx_highlight.js
+-rw-r--r--  3.0 unx    19530 tx defN 22-Dec-03 06:57 docs/_static/underscore.js
+-rw-r--r--  3.0 unx    11185 tx defN 23-Jul-25 05:05 docs/_static/alabaster.css
+-rw-r--r--  3.0 unx      421 tx defN 23-Jul-25 13:48 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx    18215 tx defN 22-Dec-03 06:57 docs/_static/searchtools.js
+-rw-r--r--  3.0 unx     1266 tx defN 22-Dec-03 06:57 docs/_static/debug.css
+-rw-r--r--  3.0 unx      313 tx defN 22-Dec-03 06:57 docs/_static/check-solid.svg
+-rw-r--r--  3.0 unx     9031 tx defN 22-Dec-03 06:57 docs/_static/clipboard.min.js
+-rw-r--r--  3.0 unx      286 bx stor 22-Dec-03 06:57 docs/_static/file.png
+-rw-r--r--  3.0 unx     4418 tx defN 22-Dec-03 06:57 docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jul-25 13:48 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx   287630 tx defN 23-Jul-25 05:05 docs/_static/jquery-3.5.1.js
+-rw-r--r--  3.0 unx       42 tx stor 23-Jul-25 05:05 docs/_static/custom.css
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jul-25 13:48 docs/_static/language_data.js
+-rw-r--r--  3.0 unx      411 tx defN 22-Dec-03 06:57 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
--rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
-drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
+-rw-r--r--  3.0 unx       90 bx defN 22-Dec-03 06:57 docs/_static/minus.png
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 13:48 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
--rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
+-rw-r--r--  3.0 unx     5529 tx defN 22-Dec-03 06:57 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
--rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
--rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
--rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Jul-17 01:15 docs/_static/basic.css
-drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
--rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
--rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
--rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jul-17 01:15 docs/_static/pygments.css
+-rw-r--r--  3.0 unx     7809 tx defN 22-Dec-03 06:57 docs/_static/styles/furo-extensions.css.map
+-rw-r--r--  3.0 unx     6034 tx defN 22-Dec-03 06:57 docs/_static/skeleton.css
+-rw-r--r--  3.0 unx   288580 tx defN 22-Dec-03 06:57 docs/_static/jquery-3.6.0.js
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jul-25 13:48 docs/_static/basic.css
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 13:48 docs/_static/scripts/
+-rw-r--r--  3.0 unx      187 tx defN 22-Dec-03 06:57 docs/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--  3.0 unx    28242 tx defN 22-Dec-03 06:57 docs/_static/scripts/furo.js.map
+-rw-r--r--  3.0 unx        0 bx stor 22-Dec-03 06:57 docs/_static/scripts/furo-extensions.js
+-rw-r--r--  3.0 unx     5265 tx defN 22-Dec-03 06:57 docs/_static/scripts/furo.js
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jul-25 13:48 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
--rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
--rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
--rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
--rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   428174 tx defN 23-Jul-17 01:15 docs/cli.html
--rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   254995 tx defN 23-Jul-17 01:15 docs/genindex.html
--rw-r--r--  3.0 unx   110750 tx defN 23-Jul-17 01:15 docs/index.html
--rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9859 bx stor 23-Jul-17 01:15 docs/objects.inv
--rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jul-17 01:15 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jul-17 01:15 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jul-17 01:15 docs/py-modindex.html
--rw-r--r--  3.0 unx   472096 tx defN 23-Jul-17 01:15 docs/reference.html
-drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
--rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
--rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
--rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jul-17 01:15 docs/search.html
--rw-r--r--  3.0 unx   225831 tx defN 23-Jul-17 01:15 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jul-17 01:15 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jul-17 01:15 docs/tutorial.html
-99 files, 7039540 bytes uncompressed, 1460573 bytes compressed:  79.3%
+-rw-r--r--  3.0 unx     4472 tx defN 22-Dec-03 06:57 docs/_static/doctools.js
+-rw-r--r--  3.0 unx    67692 tx defN 23-Jul-25 05:05 docs/_static/underscore-1.12.0.js
+-rw-r--r--  3.0 unx    89501 tx defN 22-Dec-03 06:57 docs/_static/jquery.js
+-rw-r--r--  3.0 unx    68420 tx defN 22-Dec-03 06:57 docs/_static/underscore-1.13.1.js
+-rw-r--r--  3.0 unx   430599 tx defN 23-Jul-25 13:48 docs/cli.html
+-rw-r--r--  3.0 unx    85854 tx defN 23-Jul-25 05:05 docs/cli_export.html
+-rw-r--r--  3.0 unx   255294 tx defN 23-Jul-25 13:48 docs/genindex.html
+-rw-r--r--  3.0 unx   110750 tx defN 23-Jul-25 13:48 docs/index.html
+-rw-r--r--  3.0 unx     2984 tx defN 23-Jul-25 05:05 docs/modules.html
+-rw-r--r--  3.0 unx     9863 bx stor 23-Jul-25 13:48 docs/objects.inv
+-rw-r--r--  3.0 unx   267506 bx defN 23-Jul-25 05:05 docs/osxphotos.pdf
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jul-25 13:48 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jul-25 13:48 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jul-25 13:48 docs/py-modindex.html
+-rw-r--r--  3.0 unx   472533 tx defN 23-Jul-25 13:48 docs/reference.html
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jul-25 05:05 docs/screencast/
+-rw-r--r--  3.0 unx     8007 tx defN 23-Jul-25 05:05 docs/screencast/terminalizer-demo.yml
+-rw-r--r--  3.0 unx    77927 bx defN 23-Jul-25 05:05 docs/screencast/osx-screenshot.png
+-rw-r--r--  3.0 unx   224316 bx defN 23-Jul-25 05:05 docs/screencast/demo.gif
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jul-25 13:48 docs/search.html
+-rw-r--r--  3.0 unx   217861 tx defN 23-Jul-25 13:48 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jul-25 13:48 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jul-25 13:48 docs/tutorial.html
+99 files, 7047150 bytes uncompressed, 1460669 bytes compressed:  79.3%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.9 documentation</title>
+        <title>Overview: module code - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoexporter.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoexporter - osxphotos 0.60.7 documentation</title>
+        <title>osxphotos.photoexporter - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -483,14 +483,16 @@
         <span class="s2">&quot;aae_written&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_exiftool_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_exiftool_written&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_json_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_json_written&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_xmp_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;sidecar_xmp_written&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;sidecar_user_written&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;sidecar_user_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;skipped_album&quot;</span><span class="p">,</span>
         <span class="s2">&quot;to_touch&quot;</span><span class="p">,</span>
         <span class="s2">&quot;touched&quot;</span><span class="p">,</span>
         <span class="s2">&quot;updated&quot;</span><span class="p">,</span>
         <span class="s2">&quot;xattr_skipped&quot;</span><span class="p">,</span>
         <span class="s2">&quot;xattr_written&quot;</span><span class="p">,</span>
@@ -514,14 +516,16 @@
         <span class="n">aae_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_exiftool_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_exiftool_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_json_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_json_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_xmp_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">sidecar_xmp_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+        <span class="n">sidecar_user_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+        <span class="n">sidecar_user_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">skipped_album</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">to_touch</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">touched</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">updated</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">xattr_skipped</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">xattr_written</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
@@ -554,14 +558,16 @@
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">aae_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_json_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_json_skipped</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_exiftool_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_exiftool_skipped</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_xmp_written</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_xmp_skipped</span>
+            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_user_written</span>
+            <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">sidecar_user_skipped</span>
             <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">missing</span>
         <span class="p">)</span>
         <span class="n">files</span> <span class="o">+=</span> <span class="p">[</span><span class="n">x</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">exiftool_warning</span><span class="p">]</span>
         <span class="n">files</span> <span class="o">+=</span> <span class="p">[</span><span class="n">x</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">exiftool_error</span><span class="p">]</span>
         <span class="n">files</span> <span class="o">+=</span> <span class="p">[</span><span class="n">x</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">error</span><span class="p">]</span>
 
         <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">files</span><span class="p">))</span></div>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -377,14 +377,16 @@
         "aae_written",
         "sidecar_exiftool_skipped",
         "sidecar_exiftool_written",
         "sidecar_json_skipped",
         "sidecar_json_written",
         "sidecar_xmp_skipped",
         "sidecar_xmp_written",
+        "sidecar_user_written",
+        "sidecar_user_skipped",
         "skipped",
         "skipped_album",
         "to_touch",
         "touched",
         "updated",
         "xattr_skipped",
         "xattr_written",
@@ -408,14 +410,16 @@
         aae_written=None,
         sidecar_exiftool_skipped=None,
         sidecar_exiftool_written=None,
         sidecar_json_skipped=None,
         sidecar_json_written=None,
         sidecar_xmp_skipped=None,
         sidecar_xmp_written=None,
+        sidecar_user_written=None,
+        sidecar_user_skipped=None,
         skipped=None,
         skipped_album=None,
         to_touch=None,
         touched=None,
         updated=None,
         xattr_skipped=None,
         xattr_written=None,
@@ -448,14 +452,16 @@
             + self.aae_written
             + self.sidecar_json_written
             + self.sidecar_json_skipped
             + self.sidecar_exiftool_written
             + self.sidecar_exiftool_skipped
             + self.sidecar_xmp_written
             + self.sidecar_xmp_skipped
+            + self.sidecar_user_written
+            + self.sidecar_user_skipped
             + self.missing
         )
         files += [x[0] for x in self.exiftool_warning]
         files += [x[0] for x in self.exiftool_error]
         files += [x[0] for x in self.error]
 
         return list(set(files))
```

#### docs/_modules/osxphotos/phototemplate.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.phototemplate - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos.phototemplate - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/export_db.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.export_db - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.export_db - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/scoreinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.scoreinfo - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.scoreinfo - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/searchinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.searchinfo - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.searchinfo - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/fileutil.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.fileutil - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.fileutil - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.60.9 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -366,15 +366,19 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_path</span> <span class="o">=</span> <span class="n">photopath</span>
             <span class="k">return</span> <span class="n">photopath</span>
 
     <span class="k">def</span> <span class="nf">_path_5</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns candidate path for original photo on Photos &gt;= version 5&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;shared&quot;</span><span class="p">]:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_5_shared</span><span class="p">()</span>
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_shared_moment</span><span class="p">():</span>
+        <span class="k">if</span> <span class="p">(</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span>
+            <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&gt;=</span> <span class="mi">7</span>
+            <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_shared_moment</span><span class="p">()</span>
+        <span class="p">):</span>
             <span class="c1"># path for photos in shared moments if it&#39;s in the shared moment folder</span>
             <span class="c1"># the file may also be in the originals folder which the next check will catch</span>
             <span class="c1"># check shared_moment first as a photo can be both a shared moment and syndicated</span>
             <span class="c1"># and if so, will be in the shared moment folder</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_shared_moment</span><span class="p">()</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
             <span class="c1"># path for &quot;shared with you&quot; syndicated photos that have not yet been saved to the library</span>
@@ -415,31 +419,31 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="n">shared_path</span><span class="p">,</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;directory&quot;</span><span class="p">],</span>
             <span class="n">filename</span><span class="p">,</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">_path_syndication</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return path for syndicated photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
-        <span class="c1"># Photos 8+ stores syndicated photos in a separate directory</span>
+        <span class="sd">&quot;&quot;&quot;Return path for syndicated photo on Photos &gt;= version 7&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 7+ stores syndicated photos in a separate directory</span>
         <span class="c1"># in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID.ext</span>
         <span class="c1"># where X is first digit of UUID</span>
         <span class="n">syndication_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/syndication/originals&quot;</span>
         <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
         <span class="n">path</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="n">syndication_path</span><span class="p">,</span>
             <span class="n">uuid_dir</span><span class="p">,</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">,</span>
         <span class="p">)</span>
         <span class="k">return</span> <span class="n">path</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
 
     <span class="k">def</span> <span class="nf">_path_shared_moment</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return path for shared moment photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
-        <span class="c1"># Photos 8+ stores shared moment photos in a separate directory</span>
+        <span class="sd">&quot;&quot;&quot;Return path for shared moment photo on Photos &gt;= version 7&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 7+ stores shared moment photos in a separate directory</span>
         <span class="c1"># in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID.ext</span>
         <span class="c1"># where X is first digit of UUID</span>
         <span class="n">momentshared_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/momentshared/originals&quot;</span>
         <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
         <span class="n">path</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="n">momentshared_path</span><span class="p">,</span>
@@ -564,15 +568,15 @@
             <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Unknown type </span><span class="si">{</span><span class="n">type_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
             <span class="n">library</span><span class="p">,</span> <span class="s2">&quot;resources&quot;</span><span class="p">,</span> <span class="s2">&quot;media&quot;</span><span class="p">,</span> <span class="s2">&quot;version&quot;</span><span class="p">,</span> <span class="n">folder_id</span><span class="p">,</span> <span class="n">nn_id</span><span class="p">,</span> <span class="n">filename</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">_path_edited_4</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
-        <span class="sd">&quot;&quot;&quot;return path_edited for Photos &lt;= 4; modified version of code in PhotoInfo to debug #859&quot;&quot;&quot;</span>
+        <span class="sd">&quot;&quot;&quot;return path_edited for Photos &lt;= 4; #859&quot;&quot;&quot;</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;hasAdjustments&quot;</span><span class="p">]:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
         <span class="k">if</span> <span class="n">edit_id</span> <span class="o">:=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;edit_resource_id&quot;</span><span class="p">]:</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="n">photopath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_predicted_path_edited_4</span><span class="p">()</span>
@@ -669,15 +673,15 @@
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">path_raw</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;absolute path of associated RAW image or None if there is not one&quot;&quot;&quot;</span>
 
         <span class="c1"># In Photos 5, raw is in same folder as original but with _4.ext</span>
         <span class="c1"># Unless &quot;Copy Items to the Photos Library&quot; is not checked</span>
-        <span class="c1"># then RAW image is not renamed but has same name is jpeg buth with raw extension</span>
+        <span class="c1"># then RAW image is not renamed but has same name is jpeg but with raw extension</span>
         <span class="c1"># Current implementation finds images with the correct raw UTI extension</span>
         <span class="c1"># in same folder as the original and with same stem as original in form: original_stem*.raw_ext</span>
         <span class="c1"># TODO: I don&#39;t like this -- would prefer a more deterministic approach but until I have more</span>
         <span class="c1"># data on how Photos stores and retrieves RAW images, this seems to be working</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;isMissing&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>  <span class="c1"># path would be meaningless until downloaded</span>
@@ -1124,15 +1128,15 @@
 
         <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_4</span><span class="p">()</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">path</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismissing</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
                 <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_shared_5</span><span class="p">()</span>
-            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span><span class="p">:</span>
+            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&gt;=</span> <span class="mi">7</span><span class="p">:</span>
                 <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_shared_moment</span><span class="p">()</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
                 <span class="c1"># syndicated (&quot;Shared with you&quot;) photos not yet saved to library</span>
                 <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_syndicated</span><span class="p">()</span>
 
             <span class="n">filename</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">path</span><span class="p">)</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="n">filename</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span><span class="p">)</span>
@@ -1188,32 +1192,32 @@
                     <span class="c1"># TODO: should this be a warning or debug?</span>
                     <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">return</span> <span class="n">photopath</span>
 
     <span class="k">def</span> <span class="nf">_path_live_syndicated</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return path for live syndicated photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
-        <span class="c1"># Photos 8+ stores live syndicated photos in a separate directory</span>
+        <span class="sd">&quot;&quot;&quot;Return path for live syndicated photo on Photos &gt;= version 7&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 7+ stores live syndicated photos in a separate directory</span>
         <span class="c1"># in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID_3.mov</span>
         <span class="c1"># where X is first digit of UUID</span>
         <span class="n">syndication_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/syndication/originals&quot;</span>
         <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
         <span class="n">filename</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span>
         <span class="n">live_photo</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="n">syndication_path</span><span class="p">,</span>
             <span class="n">uuid_dir</span><span class="p">,</span>
             <span class="n">filename</span><span class="p">,</span>
         <span class="p">)</span>
         <span class="k">return</span> <span class="n">live_photo</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">live_photo</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
 
     <span class="k">def</span> <span class="nf">_path_live_shared_moment</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return path for live shared moment photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
-        <span class="c1"># Photos 8+ stores live shared moment photos in a separate directory</span>
+        <span class="sd">&quot;&quot;&quot;Return path for live shared moment photo on Photos &gt;= version 7&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 7+ stores live shared moment photos in a separate directory</span>
         <span class="c1"># in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID_3.mov</span>
         <span class="c1"># where X is first digit of UUID</span>
         <span class="n">shared_moment_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/momentshared/originals&quot;</span>
         <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
         <span class="n">filename</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span>
         <span class="n">live_photo</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
@@ -1229,15 +1233,15 @@
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_derivatives_4</span><span class="p">()</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_derivatives_5_shared</span><span class="p">()</span>
 
         <span class="n">directory</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>  <span class="c1"># first char of uuid</span>
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span><span class="p">:</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&gt;=</span> <span class="mi">7</span><span class="p">:</span>
             <span class="c1"># shared moments</span>
             <span class="n">derivative_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/momentshared/resources/derivatives&quot;</span>
             <span class="n">thumb_path</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">derivative_path</span><span class="si">}</span><span class="s2">/masters/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">_4_5005_c.jpeg&quot;</span>
             <span class="p">)</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
             <span class="c1"># syndicated (&quot;Shared with you&quot;) photos not yet saved to library</span>
@@ -1591,45 +1595,45 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_search_info_normalized</span> <span class="o">=</span> <span class="n">SearchInfo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">normalized</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_search_info_normalized</span>
 
     <span class="nd">@cached_property</span>
     <span class="k">def</span> <span class="nf">syndicated</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;Return true if photo was shared via syndication (e.g. via Messages, etc.);</span>
 <span class="sd">        these are photos that appear in &quot;Shared with you&quot; album.</span>
-<span class="sd">        Photos 8+ only; returns None if not Photos 8+.</span>
+<span class="sd">        Photos 7+ only; returns None if not Photos 7+.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&lt;</span> <span class="mi">8</span><span class="p">:</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&lt;</span> <span class="mi">7</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="p">(</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_syndication_uuid</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;syndication_identifier&quot;</span><span class="p">]</span>
                 <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span>
             <span class="p">)</span>
         <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">False</span>
 
     <span class="nd">@cached_property</span>
     <span class="k">def</span> <span class="nf">saved_to_library</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;Return True if syndicated photo has been saved to library;</span>
 <span class="sd">        returns False if photo is not syndicated or has not been saved to the library.</span>
-<span class="sd">        Returns None if not Photos 8+.</span>
-<span class="sd">        Syndicated photos are photos that appear in &quot;Shared with you&quot; album; Photos 8+ only.</span>
+<span class="sd">        Returns None if not Photos 7+.</span>
+<span class="sd">        Syndicated photos are photos that appear in &quot;Shared with you&quot; album; Photos 7+ only.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&lt;</span> <span class="mi">8</span><span class="p">:</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&lt;</span> <span class="mi">7</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_syndication_uuid</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;syndication_history&quot;</span><span class="p">]</span> <span class="o">!=</span> <span class="mi">0</span>
         <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">False</span>
 
     <span class="nd">@cached_property</span>
     <span class="k">def</span> <span class="nf">shared_moment</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
-        <span class="sd">&quot;&quot;&quot;Returns True if photo is part of a shared moment otherwise False&quot;&quot;&quot;</span>
+        <span class="sd">&quot;&quot;&quot;Returns True if photo is part of a shared moment otherwise False (Photos 7+ only)&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;moment_share&quot;</span><span class="p">])</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">labels</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;returns list of labels applied to photo by Photos image categorization</span>
 <span class="sd">        only valid on Photos 5, on older libraries returns empty list</span>
 <span class="sd">        &quot;&quot;&quot;</span>
@@ -2126,14 +2130,18 @@
         <span class="n">exif_info</span> <span class="o">=</span> <span class="n">dataclasses</span><span class="o">.</span><span class="n">asdict</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">exif_info</span><span class="p">)</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exif_info</span> <span class="k">else</span> <span class="p">{}</span>
         <span class="n">face_info</span> <span class="o">=</span> <span class="p">[</span><span class="n">face</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">face</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">face_info</span><span class="p">]</span>
         <span class="n">folders</span> <span class="o">=</span> <span class="p">{</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="p">:</span> <span class="n">album</span><span class="o">.</span><span class="n">folder_names</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album_info</span><span class="p">}</span>
         <span class="n">likes</span> <span class="o">=</span> <span class="p">[</span><span class="n">like</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">like</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">likes</span><span class="p">]</span>
         <span class="n">place</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">place</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">place</span> <span class="k">else</span> <span class="p">{}</span>
         <span class="n">score</span> <span class="o">=</span> <span class="n">dataclasses</span><span class="o">.</span><span class="n">asdict</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">score</span><span class="p">)</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">score</span> <span class="k">else</span> <span class="p">{}</span>
 
+        <span class="c1"># do not add any new properties to data_dict as this is used by export to determine</span>
+        <span class="c1"># if a photo needs to be re-exported and adding new properties may cause all photos</span>
+        <span class="c1"># to be re-exported</span>
+        <span class="c1"># see below `if not shallow:`</span>
         <span class="n">dict_data</span> <span class="o">=</span> <span class="p">{</span>
             <span class="s2">&quot;albums&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">,</span>
             <span class="s2">&quot;burst&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst</span><span class="p">,</span>
             <span class="s2">&quot;cloud_guid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">cloud_guid</span><span class="p">,</span>
             <span class="s2">&quot;cloud_owner_hashed_id&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">cloud_owner_hashed_id</span><span class="p">,</span>
             <span class="s2">&quot;comments&quot;</span><span class="p">:</span> <span class="n">comments</span><span class="p">,</span>
             <span class="s2">&quot;date_added&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">date_added</span><span class="p">,</span>
@@ -2200,14 +2208,15 @@
             <span class="s2">&quot;uti&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uti</span><span class="p">,</span>
             <span class="s2">&quot;uuid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">,</span>
             <span class="s2">&quot;visible&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">visible</span><span class="p">,</span>
             <span class="s2">&quot;width&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">width</span><span class="p">,</span>
         <span class="p">}</span>
 
         <span class="c1"># non-shallow keys</span>
+        <span class="c1"># add any new properties here</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">shallow</span><span class="p">:</span>
             <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;album_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">album</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album_info</span><span class="p">]</span>
             <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;path_derivatives&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_derivatives</span>
             <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;adjustments&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">adjustments</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">adjustments</span> <span class="k">else</span> <span class="p">{}</span>
             <span class="p">)</span>
             <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;burst_album_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">a</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">a</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_album_info</span><span class="p">]</span>
@@ -2227,14 +2236,17 @@
                 <span class="bp">self</span><span class="o">.</span><span class="n">search_info</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">search_info</span> <span class="k">else</span> <span class="p">{}</span>
             <span class="p">)</span>
             <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;search_info_normalized&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">search_info_normalized</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span>
                 <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">search_info_normalized</span>
                 <span class="k">else</span> <span class="p">{}</span>
             <span class="p">)</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;syndicated&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;saved_to_library&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;shared_moment&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span>
 
         <span class="k">return</span> <span class="n">dict_data</span></div>
 
 <div class="viewcode-block" id="PhotoInfo.json"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.json">[docs]</a>    <span class="k">def</span> <span class="nf">json</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">indent</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">shallow</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;Return JSON representation</span>
 
 <span class="sd">        Args:</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -211,15 +211,19 @@
             self._path = photopath
             return photopath
 
     def _path_5(self):
         """Returns candidate path for original photo on Photos >= version 5"""
         if self._info["shared"]:
             return self._path_5_shared()
-        if self.shared_moment and self._path_shared_moment():
+        if (
+            self.shared_moment
+            and self._db.photos_version >= 7
+            and self._path_shared_moment()
+        ):
             # path for photos in shared moments if it's in the shared moment
 folder
             # the file may also be in the originals folder which the next check
 will catch
             # check shared_moment first as a photo can be both a shared moment
 and syndicated
             # and if so, will be in the shared moment folder
@@ -264,32 +268,32 @@
             self._db._library_path,
             shared_path,
             self._info["directory"],
             filename,
         )
 
     def _path_syndication(self):
-        """Return path for syndicated photo on Photos >= version 8"""
-        # Photos 8+ stores syndicated photos in a separate directory
+        """Return path for syndicated photo on Photos >= version 7"""
+        # Photos 7+ stores syndicated photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/
 UUID.ext
         # where X is first digit of UUID
         syndication_path = "scopes/syndication/originals"
         uuid_dir = self.uuid[0]
         path = os.path.join(
             self._db._library_path,
             syndication_path,
             uuid_dir,
             self.filename,
         )
         return path if os.path.isfile(path) else None
 
     def _path_shared_moment(self):
-        """Return path for shared moment photo on Photos >= version 8"""
-        # Photos 8+ stores shared moment photos in a separate directory
+        """Return path for shared moment photo on Photos >= version 7"""
+        # Photos 7+ stores shared moment photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/
 UUID.ext
         # where X is first digit of UUID
         momentshared_path = "scopes/momentshared/originals"
         uuid_dir = self.uuid[0]
         path = os.path.join(
             self._db._library_path,
@@ -424,16 +428,15 @@
 
         return os.path.join(
             library, "resources", "media", "version", folder_id, nn_id,
 filename
         )
 
     def _path_edited_4(self) -> str | None:
-        """return path_edited for Photos <= 4; modified version of code in
-PhotoInfo to debug #859"""
+        """return path_edited for Photos <= 4; #859"""
 
         if not self._info["hasAdjustments"]:
             return None
 
         if edit_id := self._info["edit_resource_id"]:
             try:
                 photopath = self._get_predicted_path_edited_4()
@@ -534,15 +537,15 @@
 
     @property
     def path_raw(self):
         """absolute path of associated RAW image or None if there is not one"""
 
         # In Photos 5, raw is in same folder as original but with _4.ext
         # Unless "Copy Items to the Photos Library" is not checked
-        # then RAW image is not renamed but has same name is jpeg buth with raw
+        # then RAW image is not renamed but has same name is jpeg but with raw
 extension
         # Current implementation finds images with the correct raw UTI
 extension
         # in same folder as the original and with same stem as original in
 form: original_stem*.raw_ext
         # TODO: I don't like this -- would prefer a more deterministic approach
 but until I have more
@@ -1028,15 +1031,15 @@
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
             if self.shared:
                 return self._path_live_photo_shared_5()
-            if self.shared_moment:
+            if self.shared_moment and self._db.photos_version >= 7:
                 return self._path_live_shared_moment()
             if self.syndicated and not self.saved_to_library:
                 # syndicated ("Shared with you") photos not yet saved to
 library
                 return self._path_live_syndicated()
 
             filename = pathlib.Path(self.path)
@@ -1096,16 +1099,16 @@
                     # TODO: should this be a warning or debug?
                     photopath = None
         else:
             photopath = None
         return photopath
 
     def _path_live_syndicated(self):
-        """Return path for live syndicated photo on Photos >= version 8"""
-        # Photos 8+ stores live syndicated photos in a separate directory
+        """Return path for live syndicated photo on Photos >= version 7"""
+        # Photos 7+ stores live syndicated photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/
 UUID_3.mov
         # where X is first digit of UUID
         syndication_path = "scopes/syndication/originals"
         uuid_dir = self.uuid[0]
         filename = f"{pathlib.Path(self.filename).stem}_3.mov"
         live_photo = os.path.join(
@@ -1113,16 +1116,16 @@
             syndication_path,
             uuid_dir,
             filename,
         )
         return live_photo if os.path.isfile(live_photo) else None
 
     def _path_live_shared_moment(self):
-        """Return path for live shared moment photo on Photos >= version 8"""
-        # Photos 8+ stores live shared moment photos in a separate directory
+        """Return path for live shared moment photo on Photos >= version 7"""
+        # Photos 7+ stores live shared moment photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/
 UUID_3.mov
         # where X is first digit of UUID
         shared_moment_path = "scopes/momentshared/originals"
         uuid_dir = self.uuid[0]
         filename = f"{pathlib.Path(self.filename).stem}_3.mov"
         live_photo = os.path.join(
@@ -1140,15 +1143,15 @@
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
 
         if self.shared:
             return self._path_derivatives_5_shared()
 
         directory = self._uuid[0]  # first char of uuid
-        if self.shared_moment:
+        if self.shared_moment and self._db.photos_version >= 7:
             # shared moments
             derivative_path = "scopes/momentshared/resources/derivatives"
             thumb_path = (
                 f"{derivative_path}/masters/{directory}/
 {self.uuid}_4_5005_c.jpeg"
             )
         elif self.syndicated and not self.saved_to_library:
@@ -1531,17 +1534,17 @@
             return self._search_info_normalized
 
     @cached_property
     def syndicated(self) -> bool | None:
         """Return true if photo was shared via syndication (e.g. via Messages,
 etc.);
         these are photos that appear in "Shared with you" album.
-        Photos 8+ only; returns None if not Photos 8+.
+        Photos 7+ only; returns None if not Photos 7+.
         """
-        if self._db.photos_version < 8:
+        if self._db.photos_version < 7:
             return None
 
         try:
             return (
                 self._db._db_syndication_uuid[self.uuid]
 ["syndication_identifier"]
                 is not None
@@ -1550,30 +1553,31 @@
             return False
 
     @cached_property
     def saved_to_library(self) -> bool | None:
         """Return True if syndicated photo has been saved to library;
         returns False if photo is not syndicated or has not been saved to the
 library.
-        Returns None if not Photos 8+.
+        Returns None if not Photos 7+.
         Syndicated photos are photos that appear in "Shared with you" album;
-Photos 8+ only.
+Photos 7+ only.
         """
-        if self._db.photos_version < 8:
+        if self._db.photos_version < 7:
             return None
 
         try:
             return self._db._db_syndication_uuid[self.uuid]
 ["syndication_history"] != 0
         except KeyError:
             return False
 
     @cached_property
     def shared_moment(self) -> bool:
-        """Returns True if photo is part of a shared moment otherwise False"""
+        """Returns True if photo is part of a shared moment otherwise False
+(Photos 7+ only)"""
         return bool(self._info["moment_share"])
 
     @property
     def labels(self):
         """returns list of labels applied to photo by Photos image
 categorization
         only valid on Photos 5, on older libraries returns empty list
@@ -2132,14 +2136,20 @@
         face_info = [face.asdict() for face in self.face_info]
         folders = {album.title: album.folder_names for album in
 self.album_info}
         likes = [like.asdict() for like in self.likes]
         place = self.place.asdict() if self.place else {}
         score = dataclasses.asdict(self.score) if self.score else {}
 
+        # do not add any new properties to data_dict as this is used by export
+to determine
+        # if a photo needs to be re-exported and adding new properties may
+cause all photos
+        # to be re-exported
+        # see below `if not shallow:`
         dict_data = {
             "albums": self.albums,
             "burst": self.burst,
             "cloud_guid": self.cloud_guid,
             "cloud_owner_hashed_id": self.cloud_owner_hashed_id,
             "comments": comments,
             "date_added": self.date_added,
@@ -2206,14 +2216,15 @@
             "uti": self.uti,
             "uuid": self.uuid,
             "visible": self.visible,
             "width": self.width,
         }
 
         # non-shallow keys
+        # add any new properties here
         if not shallow:
             dict_data["album_info"] = [album.asdict() for album in
 self.album_info]
             dict_data["path_derivatives"] = self.path_derivatives
             dict_data["adjustments"] = (
                 self.adjustments.asdict() if self.adjustments else {}
             )
@@ -2235,14 +2246,17 @@
                 self.search_info.asdict() if self.search_info else {}
             )
             dict_data["search_info_normalized"] = (
                 self.search_info_normalized.asdict()
                 if self.search_info_normalized
                 else {}
             )
+            dict_data["syndicated"] = self.syndicated
+            dict_data["saved_to_library"] = self.saved_to_library
+            dict_data["shared_moment"] = self.shared_moment
 
         return dict_data
 
 
 [docs]    def json(self, indent: int | None = None, shallow: bool = True) -
 > str:
         """Return JSON representation
```

#### docs/_modules/osxphotos/exifinfo.html

```diff
@@ -1,40 +1,204 @@
+<!doctype html>
+<html class="no-js" lang="en">
+  <head><meta charset="utf-8"/>
+    <meta name="viewport" content="width=device-width,initial-scale=1"/>
+    <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
+
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
+        <title>osxphotos.exifinfo - osxphotos 0.61.0 documentation</title>
+      <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
+    <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
+    
+    
 
-<!DOCTYPE html>
 
-<html>
-  <head>
-    <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>osxphotos.exifinfo &#8212; osxphotos 0.47.9 documentation</title>
-    <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css" />
-    <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
-    <script src="../../_static/jquery.js"></script>
-    <script src="../../_static/underscore.js"></script>
-    <script src="../../_static/doctools.js"></script>
-    <link rel="index" title="Index" href="../../genindex.html" />
-    <link rel="search" title="Search" href="../../search.html" />
-   
-  <link rel="stylesheet" href="../../_static/custom.css" type="text/css" />
+<style>
+  body {
+    --color-code-background: #f8f8f8;
+  --color-code-foreground: black;
   
+  }
+  @media not print {
+    body[data-theme="dark"] {
+      --color-code-background: #202020;
+  --color-code-foreground: #d0d0d0;
   
-  <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
+    }
+    @media (prefers-color-scheme: dark) {
+      body:not([data-theme="light"]) {
+        --color-code-background: #202020;
+  --color-code-foreground: #d0d0d0;
+  
+      }
+    }
+  }
+</style></head>
+  <body>
+    
+    <script>
+      document.body.dataset.theme = localStorage.getItem("theme") || "auto";
+    </script>
+    
 
-  </head><body>
+<svg xmlns="http://www.w3.org/2000/svg" style="display: none;">
+  <symbol id="svg-toc" viewBox="0 0 24 24">
+    <title>Contents</title>
+    <svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 1024 1024">
+      <path d="M408 442h480c4.4 0 8-3.6 8-8v-56c0-4.4-3.6-8-8-8H408c-4.4 0-8 3.6-8 8v56c0 4.4 3.6 8 8 8zm-8 204c0 4.4 3.6 8 8 8h480c4.4 0 8-3.6 8-8v-56c0-4.4-3.6-8-8-8H408c-4.4 0-8 3.6-8 8v56zm504-486H120c-4.4 0-8 3.6-8 8v56c0 4.4 3.6 8 8 8h784c4.4 0 8-3.6 8-8v-56c0-4.4-3.6-8-8-8zm0 632H120c-4.4 0-8 3.6-8 8v56c0 4.4 3.6 8 8 8h784c4.4 0 8-3.6 8-8v-56c0-4.4-3.6-8-8-8zM115.4 518.9L271.7 642c5.8 4.6 14.4.5 14.4-6.9V388.9c0-7.4-8.5-11.5-14.4-6.9L115.4 505.1a8.74 8.74 0 0 0 0 13.8z"/>
+    </svg>
+  </symbol>
+  <symbol id="svg-menu" viewBox="0 0 24 24">
+    <title>Menu</title>
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor"
+      stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather-menu">
+      <line x1="3" y1="12" x2="21" y2="12"></line>
+      <line x1="3" y1="6" x2="21" y2="6"></line>
+      <line x1="3" y1="18" x2="21" y2="18"></line>
+    </svg>
+  </symbol>
+  <symbol id="svg-arrow-right" viewBox="0 0 24 24">
+    <title>Expand</title>
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor"
+      stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather-chevron-right">
+      <polyline points="9 18 15 12 9 6"></polyline>
+    </svg>
+  </symbol>
+  <symbol id="svg-sun" viewBox="0 0 24 24">
+    <title>Light mode</title>
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor"
+      stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" class="feather-sun">
+      <circle cx="12" cy="12" r="5"></circle>
+      <line x1="12" y1="1" x2="12" y2="3"></line>
+      <line x1="12" y1="21" x2="12" y2="23"></line>
+      <line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line>
+      <line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line>
+      <line x1="1" y1="12" x2="3" y2="12"></line>
+      <line x1="21" y1="12" x2="23" y2="12"></line>
+      <line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line>
+      <line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line>
+    </svg>
+  </symbol>
+  <symbol id="svg-moon" viewBox="0 0 24 24">
+    <title>Dark mode</title>
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor"
+      stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" class="icon-tabler-moon">
+      <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+      <path d="M12 3c.132 0 .263 0 .393 0a7.5 7.5 0 0 0 7.92 12.446a9 9 0 1 1 -8.313 -12.454z" />
+    </svg>
+  </symbol>
+  <symbol id="svg-sun-half" viewBox="0 0 24 24">
+    <title>Auto light/dark mode</title>
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor"
+      stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" class="icon-tabler-shadow">
+      <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
+      <circle cx="12" cy="12" r="9" />
+      <path d="M13 12h5" />
+      <path d="M13 15h4" />
+      <path d="M13 18h1" />
+      <path d="M13 9h4" />
+      <path d="M13 6h1" />
+    </svg>
+  </symbol>
+</svg>
+
+<input type="checkbox" class="sidebar-toggle" name="__navigation" id="__navigation">
+<input type="checkbox" class="sidebar-toggle" name="__toc" id="__toc">
+<label class="overlay sidebar-overlay" for="__navigation">
+  <div class="visually-hidden">Hide navigation sidebar</div>
+</label>
+<label class="overlay toc-overlay" for="__toc">
+  <div class="visually-hidden">Hide table of contents sidebar</div>
+</label>
+
+
+
+<div class="page">
+  <header class="mobile-header">
+    <div class="header-left">
+      <label class="nav-overlay-icon" for="__navigation">
+        <div class="visually-hidden">Toggle site navigation sidebar</div>
+        <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
+      </label>
+    </div>
+    <div class="header-center">
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
+    </div>
+    <div class="header-right">
+      <div class="theme-toggle-container theme-toggle-header">
+        <button class="theme-toggle">
+          <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
+          <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
+          <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
+          <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
+        </button>
+      </div>
+      <label class="toc-overlay-icon toc-header-icon no-toc" for="__toc">
+        <div class="visually-hidden">Toggle table of contents sidebar</div>
+        <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
+      </label>
+    </div>
+  </header>
+  <aside class="sidebar-drawer">
+    <div class="sidebar-container">
+      
+      <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
+  
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
+  
+</a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
+  <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
+  <input type="hidden" name="check_keywords" value="yes">
+  <input type="hidden" name="area" value="default">
+</form>
+<div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
+  <ul>
+<li class="toctree-l1"><a class="reference internal" href="../../overview.html">OSXPhotos</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../tutorial.html">OSXPhotos Tutorial</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../cli.html">OSXPhotos Command Line Interface (CLI)</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../template_help.html">OSXPhotos Template System</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../package_overview.html">OSXPhotos Python Package Overview</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../reference.html">OSXPhotos Python Reference</a></li>
+</ul>
 
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
-          
+</div>
+</div>
 
-          <div class="body" role="main">
-            
-  <h1>Source code for osxphotos.exifinfo</h1><div class="highlight"><pre>
+      </div>
+      
+    </div>
+  </aside>
+  <div class="main">
+    <div class="content">
+      <div class="article-container">
+        <a href="#" class="back-to-top muted-link">
+          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+            <path d="M13 20h-2V8l-5.5 5.5-1.42-1.42L12 4.16l7.92 7.92-1.42 1.42L13 8v12z"></path>
+          </svg>
+          <span>Back to top</span>
+        </a>
+        <div class="content-icon-container">
+          <div class="theme-toggle-container theme-toggle-content">
+            <button class="theme-toggle">
+              <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
+              <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
+              <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
+              <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
+            </button>
+          </div>
+          <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
+            <div class="visually-hidden">Toggle table of contents sidebar</div>
+            <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
+          </label>
+        </div>
+        <article role="main">
+          <h1>Source code for osxphotos.exifinfo</h1><div class="highlight"><pre>
 <span></span><span class="sd">&quot;&quot;&quot; ExifInfo class to expose EXIF info from the library &quot;&quot;&quot;</span>
 
 <span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">dataclass</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;ExifInfo&quot;</span><span class="p">]</span>
 
 
@@ -58,76 +222,51 @@
     <span class="n">longitude</span><span class="p">:</span> <span class="nb">float</span>
     <span class="n">shutter_speed</span><span class="p">:</span> <span class="nb">float</span>
     <span class="n">camera_make</span><span class="p">:</span> <span class="nb">str</span>
     <span class="n">camera_model</span><span class="p">:</span> <span class="nb">str</span>
     <span class="n">codec</span><span class="p">:</span> <span class="nb">str</span>
     <span class="n">lens_model</span><span class="p">:</span> <span class="nb">str</span></div>
 </pre></div>
-
-          </div>
+        </article>
+      </div>
+      <footer>
+        
+        <div class="related-pages">
+          
           
         </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="../../index.html">osxphotos</a></h1>
-
-
-
-
-
-
-
-
-<h3>Navigation</h3>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="../../overview.html">osxphotos</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../tutorial.html">Tutorial</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../cli.html">osxphotos command line interface (CLI)</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../reference.html">osxphotos package</a></li>
-</ul>
-
-<div class="relations">
-<h3>Related Topics</h3>
-<ul>
-  <li><a href="../../index.html">Documentation overview</a><ul>
-  <li><a href="../index.html">Module code</a><ul>
-  </ul></li>
-  </ul></li>
-</ul>
-</div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="../../search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
-      <input type="submit" value="Go" />
-    </form>
-    </div>
-</div>
-<script>$('#searchbox').show(0);</script>
-
-
-
-
-
-
-
-
+        <div class="bottom-of-page">
+          <div class="left-details">
+            <div class="copyright">
+                Copyright &#169; 2021, Rhet Turnbull
+            </div>
+            Made with <a href="https://www.sphinx-doc.org/">Sphinx</a> and <a class="muted-link" href="https://pradyunsg.me">@pradyunsg</a>'s
+            
+            <a href="https://github.com/pradyunsg/furo">Furo</a>
+            
+          </div>
+          <div class="right-details">
+            <div class="icons">
+              
+            </div>
+          </div>
         </div>
-      </div>
-      <div class="clearer"></div>
+        
+      </footer>
     </div>
-    <div class="footer">
-      &copy;2021, Rhet Turnbull.
+    <aside class="toc-drawer no-toc">
       
-      |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
-    </div>
-
-    
-
-    
-  </body>
+      
+    </aside>
+  </div>
+</div><script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
+    <script src="../../_static/jquery.js"></script>
+    <script src="../../_static/underscore.js"></script>
+    <script src="../../_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="../../_static/doctools.js"></script>
+    <script src="../../_static/sphinx_highlight.js"></script>
+    <script src="../../_static/scripts/furo.js"></script>
+    <script src="../../_static/clipboard.min.js"></script>
+    <script src="../../_static/copybutton.js"></script>
+    </body>
 </html>
```

##### html2text {}

```diff
@@ -1,14 +1,44 @@
 
 
 
 
 
 
 
+
+
+
+
+
+           ⁰ ⁰
+Hide navigation sidebar
+
+Hide table of contents sidebar
+Toggle site navigation sidebar
+
+osxphotos_0.61.0_documentation
+Toggle Light / Dark / Auto color theme
+
+Toggle table of contents sidebar
+
+
+osxphotos_0.61.0_documentation
+[q                   ]
+    * OSXPhotos
+    * OSXPhotos_Tutorial
+    * OSXPhotos_Command_Line_Interface_(CLI)
+    * OSXPhotos_Template_System
+    * OSXPhotos_Python_Package_Overview
+    * OSXPhotos_Python_Reference
+___Back_to_top
+Toggle Light / Dark / Auto color theme
+
+Toggle table of contents sidebar
+
 ****** Source code for osxphotos.exifinfo ******
 """ ExifInfo class to expose EXIF info from the library """
 
 from dataclasses import dataclass
 
 __all__ = ["ExifInfo"]
 
@@ -32,19 +62,10 @@
     latitude: float
     longitude: float
     shutter_speed: float
     camera_make: str
     camera_model: str
     codec: str
     lens_model: str
-****** osxphotos ******
-**** Navigation ****
-    * osxphotos
-    * Tutorial
-    * osxphotos_command_line_interface_(CLI)
-    * osxphotos_package
-**** Related Topics ****
-    * Documentation_overview
-          o Module_code
-**** Quick search ****
-[q                   ] [Go]
-©2021, Rhet Turnbull. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+Copyright © 2021, Rhet Turnbull
+Made with Sphinx and @pradyunsg's Furo
+
```

#### docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb._photosdb_process_comments - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.photosdb._photosdb_process_comments - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.9 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -255,15 +255,15 @@
 <span class="kn">from</span> <span class="nn">..phototemplate</span> <span class="kn">import</span> <span class="n">RenderOptions</span>
 <span class="kn">from</span> <span class="nn">..platform</span> <span class="kn">import</span> <span class="n">get_macos_version</span><span class="p">,</span> <span class="n">is_macos</span>
 <span class="kn">from</span> <span class="nn">..queryoptions</span> <span class="kn">import</span> <span class="n">QueryOptions</span>
 <span class="kn">from</span> <span class="nn">..rich_utils</span> <span class="kn">import</span> <span class="n">add_rich_markup_tag</span>
 <span class="kn">from</span> <span class="nn">..sqlite_utils</span> <span class="kn">import</span> <span class="n">sqlite_db_is_locked</span><span class="p">,</span> <span class="n">sqlite_open_ro</span>
 <span class="kn">from</span> <span class="nn">..unicode</span> <span class="kn">import</span> <span class="n">normalize_unicode</span>
 <span class="kn">from</span> <span class="nn">..utils</span> <span class="kn">import</span> <span class="n">_check_file_exists</span><span class="p">,</span> <span class="n">get_last_library_path</span><span class="p">,</span> <span class="n">noop</span>
-<span class="kn">from</span> <span class="nn">.photosdb_utils</span> <span class="kn">import</span> <span class="n">get_db_model_version</span><span class="p">,</span> <span class="n">get_db_version</span>
+<span class="kn">from</span> <span class="nn">.photosdb_utils</span> <span class="kn">import</span> <span class="n">get_photos_version_from_model</span><span class="p">,</span> <span class="n">get_db_version</span><span class="p">,</span> <span class="n">get_model_version</span>
 
 <span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
     <span class="kn">import</span> <span class="nn">photoscript</span>
 
 <span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;osxphotos&quot;</span><span class="p">)</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;PhotosDB&quot;</span><span class="p">]</span>
@@ -519,44 +519,46 @@
         <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Processing database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filepath</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="c1"># if database is exclusively locked, make a copy of it and use the copy</span>
         <span class="c1"># Photos maintains an exclusive lock on the database file while Photos is open</span>
         <span class="c1"># photoanalysisd sometimes maintains this lock even after Photos is closed</span>
         <span class="c1"># In those cases, make a temp copy of the file for sqlite3 to read</span>
         <span class="k">if</span> <span class="n">sqlite_db_is_locked</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile</span><span class="p">):</span>
-            <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database locked, creating temporary copy.&quot;</span><span class="p">)</span>
+            <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Database locked, creating temporary copy.&quot;</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_copy_db_file</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile</span><span class="p">)</span>
 
         <span class="c1"># _db_version is set from photos.db</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">=</span> <span class="n">get_db_version</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span><span class="p">)</span>
         <span class="c1"># _photos_version is set from Photos.sqlite which only exists for Photos 5+</span>
         <span class="n">db_ver_int</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db_version</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">db_ver_int</span> <span class="o">&lt;</span> <span class="mi">3000</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_photos_ver</span> <span class="o">=</span> <span class="mi">2</span>
         <span class="k">elif</span> <span class="n">db_ver_int</span> <span class="o">&lt;</span> <span class="mi">4000</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_photos_ver</span> <span class="o">=</span> <span class="mi">3</span>
         <span class="k">elif</span> <span class="n">db_ver_int</span> <span class="o">&lt;</span> <span class="mi">5000</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_photos_ver</span> <span class="o">=</span> <span class="mi">4</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_photos_ver</span> <span class="o">=</span> <span class="mi">5</span>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_model_ver</span> <span class="o">=</span> <span class="mi">0</span>  <span class="c1"># only set for Photos 5+</span>
+
         <span class="c1"># If Photos &gt;= 5, actual data isn&#39;t in photos.db but in Photos.sqlite</span>
         <span class="k">if</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db_version</span><span class="p">)</span> <span class="o">&gt;</span> <span class="nb">int</span><span class="p">(</span><span class="n">_PHOTOS_4_VERSION</span><span class="p">):</span>
             <span class="n">dbpath</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span>
             <span class="n">dbfile</span> <span class="o">=</span> <span class="n">dbpath</span> <span class="o">/</span> <span class="s2">&quot;Photos.sqlite&quot;</span>
             <span class="k">if</span> <span class="ow">not</span> <span class="n">_check_file_exists</span><span class="p">(</span><span class="n">dbfile</span><span class="p">):</span>
                 <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;dbfile </span><span class="si">{</span><span class="n">dbfile</span><span class="si">}</span><span class="s2"> does not exist&quot;</span><span class="p">,</span> <span class="n">dbfile</span><span class="p">)</span>
-            <span class="k">else</span><span class="p">:</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span> <span class="o">=</span> <span class="n">dbfile</span>
-                <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Processing database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filepath</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-                <span class="c1"># if database is exclusively locked, make a copy of it and use the copy</span>
-                <span class="k">if</span> <span class="n">sqlite_db_is_locked</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span><span class="p">):</span>
-                    <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database locked, creating temporary copy.&quot;</span><span class="p">)</span>
-                    <span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_copy_db_file</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span> <span class="o">=</span> <span class="n">dbfile</span>
+            <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Processing database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filepath</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <span class="c1"># if database is exclusively locked, make a copy of it and use the copy</span>
+            <span class="k">if</span> <span class="n">sqlite_db_is_locked</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span><span class="p">):</span>
+                <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Database locked, creating temporary copy.&quot;</span><span class="p">)</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_copy_db_file</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span><span class="p">)</span>
             <span class="c1"># set the photos version to actual value based on Photos.sqlite</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_photos_ver</span> <span class="o">=</span> <span class="n">get_db_model_version</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_photos_ver</span> <span class="o">=</span> <span class="n">get_photos_version_from_model</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_model_ver</span> <span class="o">=</span> <span class="n">get_model_version</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_tmp_db</span><span class="p">)</span>
 
             <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;_dbfile = </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile</span><span class="si">}</span><span class="s2">, _dbfile_actual = </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbfile_actual</span><span class="si">}</span><span class="s2">&quot;</span>
             <span class="p">)</span>
 
         <span class="n">library_path</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">dirname</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">abspath</span><span class="p">(</span><span class="n">dbfile</span><span class="p">))</span>
         <span class="p">(</span><span class="n">library_path</span><span class="p">,</span> <span class="n">_</span><span class="p">)</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">library_path</span><span class="p">)</span>  <span class="c1"># drop /database from path</span>
@@ -1428,15 +1430,15 @@
 
             <span class="c1"># fingerprint</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;masterFingerprint&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">45</span><span class="p">]</span>
 
             <span class="c1"># photos 5+ only, for shared photos</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;cloudownerhashedpersonid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
 
-            <span class="c1"># photos 8+ only, shared moments</span>
+            <span class="c1"># photos 7+ only, shared moments</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;moment_share&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
 
             <span class="c1"># compute signatures for finding possible duplicates</span>
             <span class="n">signature</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_duplicate_signature</span><span class="p">(</span><span class="n">uuid</span><span class="p">)</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_db_signatures</span><span class="p">[</span><span class="n">signature</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">uuid</span><span class="p">)</span>
             <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
@@ -2197,15 +2199,15 @@
         <span class="c1"># 37   ZGENERICASSET.ZADJUSTMENTTIMESTAMP -- when was photo edited?</span>
         <span class="c1"># 38   ZGENERICASSET.ZVISIBILITYSTATE -- 0 if visible, 2 if not (e.g. a burst image)</span>
         <span class="c1"># 39   ZGENERICASSET.ZTRASHEDDATE -- date item placed in the trash or null if not in trash</span>
         <span class="c1"># 40   ZGENERICASSET.ZSAVEDASSETTYPE -- how item imported</span>
         <span class="c1"># 41   ZGENERICASSET.ZADDEDDATE -- date item added to the library</span>
         <span class="c1"># 42   ZGENERICASSET.Z_PK -- primary key</span>
         <span class="c1"># 43   ZGENERICASSET.ZCLOUDOWNERHASHEDPERSONID -- used to look up owner name (for shared photos)</span>
-        <span class="c1"># 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 8+)</span>
+        <span class="c1"># 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 5+; in Photos 7+ these are in the scopes/momentshared folder)</span>
 
         <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">c</span><span class="p">:</span>
             <span class="n">uuid</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
             <span class="n">info</span> <span class="o">=</span> <span class="p">{}</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;_uuid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">uuid</span>  <span class="c1"># stored here for easier debugging</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;modelID&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;masterUuid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
@@ -2719,15 +2721,15 @@
         <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Processing comments and likes for shared photos.&quot;</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_process_comments</span><span class="p">()</span>
 
         <span class="c1"># process moments</span>
         <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Processing moments.&quot;</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_process_moments</span><span class="p">()</span>
 
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&gt;=</span> <span class="mi">8</span><span class="p">:</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&gt;=</span> <span class="mi">7</span><span class="p">:</span>
             <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Processing syndication info.&quot;</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_process_syndicationinfo</span><span class="p">()</span>
 
         <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Done processing details from Photos library.&quot;</span><span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">_process_moments</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Process data from ZMOMENT table&quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -96,15 +96,16 @@
 from ..phototemplate import RenderOptions
 from ..platform import get_macos_version, is_macos
 from ..queryoptions import QueryOptions
 from ..rich_utils import add_rich_markup_tag
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
 from ..unicode import normalize_unicode
 from ..utils import _check_file_exists, get_last_library_path, noop
-from .photosdb_utils import get_db_model_version, get_db_version
+from .photosdb_utils import get_photos_version_from_model, get_db_version,
+get_model_version
 
 if is_macos:
     import photoscript
 
 logger = logging.getLogger("osxphotos")
 
 __all__ = ["PhotosDB"]
@@ -398,15 +399,15 @@
         # if database is exclusively locked, make a copy of it and use the copy
         # Photos maintains an exclusive lock on the database file while Photos
 is open
         # photoanalysisd sometimes maintains this lock even after Photos is
 closed
         # In those cases, make a temp copy of the file for sqlite3 to read
         if sqlite_db_is_locked(self._dbfile):
-            verbose(f"Database locked, creating temporary copy.")
+            verbose("Database locked, creating temporary copy.")
             self._tmp_db = self._copy_db_file(self._dbfile)
 
         # _db_version is set from photos.db
         self._db_version = get_db_version(self._tmp_db)
         # _photos_version is set from Photos.sqlite which only exists for
 Photos 5+
         db_ver_int = int(self._db_version)
@@ -414,32 +415,34 @@
             self._photos_ver = 2
         elif db_ver_int < 4000:
             self._photos_ver = 3
         elif db_ver_int < 5000:
             self._photos_ver = 4
         else:
             self._photos_ver = 5
+        self._model_ver = 0  # only set for Photos 5+
+
         # If Photos >= 5, actual data isn't in photos.db but in Photos.sqlite
         if int(self._db_version) > int(_PHOTOS_4_VERSION):
             dbpath = pathlib.Path(self._dbfile).parent
             dbfile = dbpath / "Photos.sqlite"
             if not _check_file_exists(dbfile):
                 raise FileNotFoundError(f"dbfile {dbfile} does not exist",
 dbfile)
-            else:
-                self._dbfile_actual = self._tmp_db = dbfile
-                verbose(f"Processing database {self._filepath
+            self._dbfile_actual = self._tmp_db = dbfile
+            verbose(f"Processing database {self._filepath
 (self._dbfile_actual)}")
-                # if database is exclusively locked, make a copy of it and use
-the copy
-                if sqlite_db_is_locked(self._dbfile_actual):
-                    verbose(f"Database locked, creating temporary copy.")
-                    self._tmp_db = self._copy_db_file(self._dbfile_actual)
+            # if database is exclusively locked, make a copy of it and use the
+copy
+            if sqlite_db_is_locked(self._dbfile_actual):
+                verbose("Database locked, creating temporary copy.")
+                self._tmp_db = self._copy_db_file(self._dbfile_actual)
             # set the photos version to actual value based on Photos.sqlite
-            self._photos_ver = get_db_model_version(self._tmp_db)
+            self._photos_ver = get_photos_version_from_model(self._tmp_db)
+            self._model_ver = get_model_version(self._tmp_db)
 
             logger.debug(
                 f"_dbfile = {self._dbfile}, _dbfile_actual =
 {self._dbfile_actual}"
             )
 
         library_path = os.path.dirname(os.path.abspath(dbfile))
@@ -1370,15 +1373,15 @@
 
             # fingerprint
             self._dbphotos[uuid]["masterFingerprint"] = row[45]
 
             # photos 5+ only, for shared photos
             self._dbphotos[uuid]["cloudownerhashedpersonid"] = None
 
-            # photos 8+ only, shared moments
+            # photos 7+ only, shared moments
             self._dbphotos[uuid]["moment_share"] = None
 
             # compute signatures for finding possible duplicates
             signature = self._duplicate_signature(uuid)
             try:
                 self._db_signatures[signature].append(uuid)
             except KeyError:
@@ -2186,15 +2189,16 @@
         # 39   ZGENERICASSET.ZTRASHEDDATE -- date item placed in the trash or
 null if not in trash
         # 40   ZGENERICASSET.ZSAVEDASSETTYPE -- how item imported
         # 41   ZGENERICASSET.ZADDEDDATE -- date item added to the library
         # 42   ZGENERICASSET.Z_PK -- primary key
         # 43   ZGENERICASSET.ZCLOUDOWNERHASHEDPERSONID -- used to look up owner
 name (for shared photos)
-        # 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 8+)
+        # 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 5+;
+in Photos 7+ these are in the scopes/momentshared folder)
 
         for row in c:
             uuid = row[0]
             info = {}
             info["_uuid"] = uuid  # stored here for easier debugging
             info["modelID"] = None
             info["masterUuid"] = None
@@ -2746,15 +2750,15 @@
         verbose("Processing comments and likes for shared photos.")
         self._process_comments()
 
         # process moments
         verbose("Processing moments.")
         self._process_moments()
 
-        if self.photos_version >= 8:
+        if self.photos_version >= 7:
             verbose("Processing syndication info.")
             self._process_syndicationinfo()
 
         verbose("Done processing details from Photos library.")
 
     def _process_moments(self):
         """Process data from ZMOMENT table"""
```

#### docs/_modules/osxphotos/photosalbum.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosalbum - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.photosalbum - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/placeinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.placeinfo - osxphotos 0.60.7 documentation</title>
+        <title>osxphotos.placeinfo - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/momentinfo.html

```diff
@@ -1,17 +1,17 @@
 <!doctype html>
-<html class="no-js">
+<html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
-    <meta name="generator" content="sphinx-4.4.0, furo 2022.04.07"/>
-        <title>osxphotos.momentinfo - osxphotos 0.48.3 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
+        <title>osxphotos.momentinfo - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=68f4518137b9aefe99b631505a2064c3c42c9852" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
 <style>
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.48.3 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,29 +142,29 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.48.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul>
 <li class="toctree-l1"><a class="reference internal" href="../../overview.html">OSXPhotos</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../tutorial.html">OSXPhotos Tutorial</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../cli.html">OSXPhotos Command Line Interface (CLI)</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../template_help.html">OSXPhotos Template System</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../package_overview.html">OSXPhotos Python Package Overview</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../reference.html">OSXPhotos python API</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../reference.html">OSXPhotos Python Reference</a></li>
 </ul>
 
 </div>
 </div>
 
       </div>
       
@@ -175,114 +175,115 @@
       <div class="article-container">
         <a href="#" class="back-to-top muted-link">
           <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
             <path d="M13 20h-2V8l-5.5 5.5-1.42-1.42L12 4.16l7.92 7.92-1.42 1.42L13 8v12z"></path>
           </svg>
           <span>Back to top</span>
         </a>
-        <div class="content-icon-container"><div class="theme-toggle-container theme-toggle-content">
+        <div class="content-icon-container">
+          <div class="theme-toggle-container theme-toggle-content">
             <button class="theme-toggle">
               <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
               <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
               <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
               <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
             </button>
           </div>
           <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
           <h1>Source code for osxphotos.momentinfo</h1><div class="highlight"><pre>
-<span></span><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">"MomentInfo"</span><span class="p">]</span>
-<span class="sd">"""MomentInfo class with details about photo moments."""</span>
+<span></span><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;MomentInfo&quot;</span><span class="p">]</span>
+<span class="sd">&quot;&quot;&quot;MomentInfo class with details about photo moments.&quot;&quot;&quot;</span>
 
 
 <div class="viewcode-block" id="MomentInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.MomentInfo">[docs]</a><span class="k">class</span> <span class="nc">MomentInfo</span><span class="p">:</span>
-    <span class="sd">"""Info about a photo moment"""</span>
+    <span class="sd">&quot;&quot;&quot;Info about a photo moment&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">db</span><span class="p">,</span> <span class="n">moment_pk</span><span class="p">):</span>
-        <span class="sd">"""Initialize with a moment PK; returns None if PK not found."""</span>
+        <span class="sd">&quot;&quot;&quot;Initialize with a moment PK; returns None if PK not found.&quot;&quot;&quot;</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_db</span> <span class="o">=</span> <span class="n">db</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_pk</span> <span class="o">=</span> <span class="n">moment_pk</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_moment_pk</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">moment_pk</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">"No moment with PK </span><span class="si">{</span><span class="n">moment_pk</span><span class="si">}</span><span class="s2">"</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No moment with PK </span><span class="si">{</span><span class="n">moment_pk</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">pk</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Primary key of the moment."""</span>
+        <span class="sd">&quot;&quot;&quot;Primary key of the moment.&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pk</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">location</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Location of the moment."""</span>
-        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"latitude"</span><span class="p">),</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"longitude"</span><span class="p">))</span>
+        <span class="sd">&quot;&quot;&quot;Location of the moment.&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;latitude&quot;</span><span class="p">),</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;longitude&quot;</span><span class="p">))</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">title</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Title of the moment."""</span>
-        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"title"</span><span class="p">)</span>
+        <span class="sd">&quot;&quot;&quot;Title of the moment.&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;title&quot;</span><span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">subtitle</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Subtitle of the moment."""</span>
-        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"subtitle"</span><span class="p">)</span>
+        <span class="sd">&quot;&quot;&quot;Subtitle of the moment.&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;subtitle&quot;</span><span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">start_date</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Start date of the moment."""</span>
-        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"startDate"</span><span class="p">)</span>
+        <span class="sd">&quot;&quot;&quot;Start date of the moment.&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;startDate&quot;</span><span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">end_date</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Stop date of the moment."""</span>
-        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"endDate"</span><span class="p">)</span>
+        <span class="sd">&quot;&quot;&quot;Stop date of the moment.&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;endDate&quot;</span><span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">date</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Date of the moment."""</span>
-        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"representativeDate"</span><span class="p">)</span>
+        <span class="sd">&quot;&quot;&quot;Date of the moment.&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;representativeDate&quot;</span><span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">modification_date</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Modification date of the moment."""</span>
-        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"modificationDate"</span><span class="p">)</span>
+        <span class="sd">&quot;&quot;&quot;Modification date of the moment.&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;modificationDate&quot;</span><span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">photos</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""All photos in this moment"""</span>
+        <span class="sd">&quot;&quot;&quot;All photos in this moment&quot;&quot;&quot;</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_photos</span>
         <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
             <span class="n">photo_uuids</span> <span class="o">=</span> <span class="p">[</span>
                 <span class="n">uuid</span>
                 <span class="k">for</span> <span class="n">uuid</span><span class="p">,</span> <span class="n">photo</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_dbphotos</span><span class="o">.</span><span class="n">items</span><span class="p">()</span>
-                <span class="k">if</span> <span class="n">photo</span><span class="p">[</span><span class="s2">"momentID"</span><span class="p">]</span> <span class="o">==</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pk</span>
+                <span class="k">if</span> <span class="n">photo</span><span class="p">[</span><span class="s2">&quot;momentID&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pk</span>
             <span class="p">]</span>
 
             <span class="bp">self</span><span class="o">.</span><span class="n">_photos</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_by_uuid</span><span class="p">(</span><span class="n">photo_uuids</span><span class="p">)</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_photos</span>
 
 <div class="viewcode-block" id="MomentInfo.asdict"><a class="viewcode-back" href="../../reference.html#osxphotos.MomentInfo.asdict">[docs]</a>    <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">"""Returns all moment info as dictionary"""</span>
+        <span class="sd">&quot;&quot;&quot;Returns all moment info as dictionary&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="p">{</span>
-            <span class="s2">"pk"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">pk</span><span class="p">,</span>
-            <span class="s2">"location"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">location</span><span class="p">,</span>
-            <span class="s2">"title"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">,</span>
-            <span class="s2">"subtitle"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">subtitle</span><span class="p">,</span>
-            <span class="s2">"start_date"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_date</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-            <span class="s2">"end_date"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">end_date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">end_date</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-            <span class="s2">"date"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">date</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-            <span class="s2">"modification_date"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">modification_date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span>
+            <span class="s2">&quot;pk&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">pk</span><span class="p">,</span>
+            <span class="s2">&quot;location&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">location</span><span class="p">,</span>
+            <span class="s2">&quot;title&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">,</span>
+            <span class="s2">&quot;subtitle&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">subtitle</span><span class="p">,</span>
+            <span class="s2">&quot;start_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_date</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+            <span class="s2">&quot;end_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">end_date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">end_date</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+            <span class="s2">&quot;date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">date</span> <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
+            <span class="s2">&quot;modification_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">modification_date</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">modification_date</span>
             <span class="k">else</span> <span class="kc">None</span><span class="p">,</span>
-            <span class="s2">"photos"</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">photos</span><span class="p">,</span>
+            <span class="s2">&quot;photos&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">photos</span><span class="p">,</span>
         <span class="p">}</span></div></div>
 </pre></div>
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
@@ -313,13 +314,15 @@
       
       
     </aside>
   </div>
 </div><script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/jquery.js"></script>
     <script src="../../_static/underscore.js"></script>
+    <script src="../../_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="../../_static/doctools.js"></script>
+    <script src="../../_static/sphinx_highlight.js"></script>
     <script src="../../_static/scripts/furo.js"></script>
     <script src="../../_static/clipboard.min.js"></script>
     <script src="../../_static/copybutton.js"></script>
     </body>
 </html>
```

##### html2text {}

```diff
@@ -12,28 +12,28 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.48.3_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.48.3_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
-    * OSXPhotos_python_API
+    * OSXPhotos_Python_Reference
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 ****** Source code for osxphotos.momentinfo ******
 __all__ = ["MomentInfo"]
```

#### docs/_modules/osxphotos/albuminfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.albuminfo - osxphotos 0.59.2 documentation</title>
+        <title>osxphotos.albuminfo - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/exiftool.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.exiftool - osxphotos 0.59.1 documentation</title>
+        <title>osxphotos.exiftool - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.59.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.1_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.1_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/debug.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.debug - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.debug - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/queryoptions.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.queryoptions - osxphotos 0.60.9 documentation</title>
+        <title>osxphotos.queryoptions - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/personinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.personinfo - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.personinfo - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -330,15 +330,15 @@
             <span class="k">else</span> <span class="kc">False</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="fm">__ne__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">):</span>
         <span class="k">return</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="fm">__eq__</span><span class="p">(</span><span class="n">other</span><span class="p">)</span></div>
 
 
-<span class="k">class</span> <span class="nc">FaceInfo</span><span class="p">:</span>
+<div class="viewcode-block" id="FaceInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.FaceInfo">[docs]</a><span class="k">class</span> <span class="nc">FaceInfo</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;Info about a face in the Photos library&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">db</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">pk</span><span class="o">=</span><span class="kc">None</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Creates a new FaceInfo instance</span>
 
 <span class="sd">        Arguments:</span>
 <span class="sd">            db: instance of PhotosDB object</span>
@@ -468,38 +468,38 @@
             <span class="n">h</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">size_pixels</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">width</span>
             <span class="n">w</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">size_pixels</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">height</span>
             <span class="n">x</span> <span class="o">=</span> <span class="n">x</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">size_pixels</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">width</span> <span class="o">/</span> <span class="mi">2</span>
             <span class="n">y</span> <span class="o">=</span> <span class="n">y</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">size_pixels</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span><span class="o">.</span><span class="n">height</span> <span class="o">/</span> <span class="mi">2</span>
 
         <span class="k">return</span> <span class="n">MPRI_Reg_Rect</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">h</span><span class="p">,</span> <span class="n">w</span><span class="p">)</span>
 
-    <span class="k">def</span> <span class="nf">face_rect</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+<div class="viewcode-block" id="FaceInfo.face_rect"><a class="viewcode-back" href="../../reference.html#osxphotos.FaceInfo.face_rect">[docs]</a>    <span class="k">def</span> <span class="nf">face_rect</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Get face rectangle coordinates for current version of the associated image</span>
 <span class="sd">            If image has been edited, rectangle applies to edited version, otherwise original version</span>
 <span class="sd">            Coordinates in format and reference frame used by PIL</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">            list [(x0, x1), (y0, y1)] of coordinates in reference frame used by PIL</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">photo</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">photo</span>
         <span class="n">size_reference</span> <span class="o">=</span> <span class="n">photo</span><span class="o">.</span><span class="n">width</span> <span class="k">if</span> <span class="n">photo</span><span class="o">.</span><span class="n">width</span> <span class="o">&gt;</span> <span class="n">photo</span><span class="o">.</span><span class="n">height</span> <span class="k">else</span> <span class="n">photo</span><span class="o">.</span><span class="n">height</span>
         <span class="n">radius</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">/</span> <span class="mi">2</span><span class="p">)</span> <span class="o">*</span> <span class="n">size_reference</span>
         <span class="n">x</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_make_point</span><span class="p">((</span><span class="bp">self</span><span class="o">.</span><span class="n">center_x</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">center_y</span><span class="p">))</span>
         <span class="n">x0</span><span class="p">,</span> <span class="n">y0</span> <span class="o">=</span> <span class="n">x</span> <span class="o">-</span> <span class="n">radius</span><span class="p">,</span> <span class="n">y</span> <span class="o">-</span> <span class="n">radius</span>
         <span class="n">x1</span><span class="p">,</span> <span class="n">y1</span> <span class="o">=</span> <span class="n">x</span> <span class="o">+</span> <span class="n">radius</span><span class="p">,</span> <span class="n">y</span> <span class="o">+</span> <span class="n">radius</span>
-        <span class="k">return</span> <span class="p">[(</span><span class="n">x0</span><span class="p">,</span> <span class="n">y0</span><span class="p">),</span> <span class="p">(</span><span class="n">x1</span><span class="p">,</span> <span class="n">y1</span><span class="p">)]</span>
+        <span class="k">return</span> <span class="p">[(</span><span class="n">x0</span><span class="p">,</span> <span class="n">y0</span><span class="p">),</span> <span class="p">(</span><span class="n">x1</span><span class="p">,</span> <span class="n">y1</span><span class="p">)]</span></div>
 
-    <span class="k">def</span> <span class="nf">roll_pitch_yaw</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+<div class="viewcode-block" id="FaceInfo.roll_pitch_yaw"><a class="viewcode-back" href="../../reference.html#osxphotos.FaceInfo.roll_pitch_yaw">[docs]</a>    <span class="k">def</span> <span class="nf">roll_pitch_yaw</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Roll, pitch, yaw of face in radians as tuple&quot;&quot;&quot;</span>
         <span class="n">info</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span>
         <span class="n">roll</span> <span class="o">=</span> <span class="mi">0</span> <span class="k">if</span> <span class="n">info</span><span class="p">[</span><span class="s2">&quot;roll&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="kc">None</span> <span class="k">else</span> <span class="n">info</span><span class="p">[</span><span class="s2">&quot;roll&quot;</span><span class="p">]</span>
         <span class="n">pitch</span> <span class="o">=</span> <span class="mi">0</span> <span class="k">if</span> <span class="n">info</span><span class="p">[</span><span class="s2">&quot;pitch&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="kc">None</span> <span class="k">else</span> <span class="n">info</span><span class="p">[</span><span class="s2">&quot;pitch&quot;</span><span class="p">]</span>
         <span class="n">yaw</span> <span class="o">=</span> <span class="mi">0</span> <span class="k">if</span> <span class="n">info</span><span class="p">[</span><span class="s2">&quot;yaw&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="kc">None</span> <span class="k">else</span> <span class="n">info</span><span class="p">[</span><span class="s2">&quot;yaw&quot;</span><span class="p">]</span>
 
-        <span class="k">return</span> <span class="p">(</span><span class="n">roll</span><span class="p">,</span> <span class="n">pitch</span><span class="p">,</span> <span class="n">yaw</span><span class="p">)</span>
+        <span class="k">return</span> <span class="p">(</span><span class="n">roll</span><span class="p">,</span> <span class="n">pitch</span><span class="p">,</span> <span class="n">yaw</span><span class="p">)</span></div>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">roll</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Return roll angle in radians of the face region&quot;&quot;&quot;</span>
         <span class="n">roll</span><span class="p">,</span> <span class="n">_</span><span class="p">,</span> <span class="n">_</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">roll_pitch_yaw</span><span class="p">()</span>
         <span class="k">return</span> <span class="n">roll</span>
 
@@ -594,15 +594,15 @@
         <span class="c1"># rotate about center</span>
         <span class="n">xmid</span><span class="p">,</span> <span class="n">ymid</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">center</span>
         <span class="n">roll</span><span class="p">,</span> <span class="n">_</span><span class="p">,</span> <span class="n">_</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">roll_pitch_yaw</span><span class="p">()</span>
         <span class="n">xr</span><span class="p">,</span> <span class="n">yr</span> <span class="o">=</span> <span class="n">rotate_image_point</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">xmid</span><span class="p">,</span> <span class="n">ymid</span><span class="p">,</span> <span class="n">roll</span><span class="p">)</span>
 
         <span class="k">return</span> <span class="p">(</span><span class="nb">int</span><span class="p">(</span><span class="n">xr</span><span class="p">),</span> <span class="nb">int</span><span class="p">(</span><span class="n">yr</span><span class="p">))</span>
 
-    <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+<div class="viewcode-block" id="FaceInfo.asdict"><a class="viewcode-back" href="../../reference.html#osxphotos.FaceInfo.asdict">[docs]</a>    <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns dict representation of class instance&quot;&quot;&quot;</span>
         <span class="n">roll</span><span class="p">,</span> <span class="n">pitch</span><span class="p">,</span> <span class="n">yaw</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">roll_pitch_yaw</span><span class="p">()</span>
         <span class="k">return</span> <span class="p">{</span>
             <span class="s2">&quot;_pk&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">_pk</span><span class="p">,</span>
             <span class="s2">&quot;uuid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">,</span>
             <span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">name</span><span class="p">,</span>
             <span class="s2">&quot;asset_uuid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">asset_uuid</span><span class="p">,</span>
@@ -629,19 +629,19 @@
             <span class="s2">&quot;facial_hair_type&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">facial_hair_type</span><span class="p">,</span>
             <span class="s2">&quot;gender_type&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">gender_type</span><span class="p">,</span>
             <span class="s2">&quot;glasses_type&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">glasses_type</span><span class="p">,</span>
             <span class="s2">&quot;hair_color_type&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">hair_color_type</span><span class="p">,</span>
             <span class="s2">&quot;intrash&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">intrash</span><span class="p">,</span>
             <span class="s2">&quot;lip_makeup_type&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">lip_makeup_type</span><span class="p">,</span>
             <span class="s2">&quot;smile_type&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">smile_type</span><span class="p">,</span>
-        <span class="p">}</span>
+        <span class="p">}</span></div>
 
-    <span class="k">def</span> <span class="nf">json</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+<div class="viewcode-block" id="FaceInfo.json"><a class="viewcode-back" href="../../reference.html#osxphotos.FaceInfo.json">[docs]</a>    <span class="k">def</span> <span class="nf">json</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Return JSON representation of FaceInfo instance&quot;&quot;&quot;</span>
-        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">())</span>
+        <span class="k">return</span> <span class="n">json</span><span class="o">.</span><span class="n">dumps</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">())</span></div>
 
     <span class="k">def</span> <span class="fm">__str__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;FaceInfo(uuid=</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">, center_x=</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">center_x</span><span class="si">}</span><span class="s2">, center_y = </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">center_y</span><span class="si">}</span><span class="s2">, size=</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="si">}</span><span class="s2">, person=</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">, asset_uuid=</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">asset_uuid</span><span class="si">}</span><span class="s2">)&quot;</span>
 
     <span class="k">def</span> <span class="fm">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;FaceInfo(db=</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="si">}</span><span class="s2">, pk=</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_pk</span><span class="si">}</span><span class="s2">)&quot;</span>
 
@@ -650,15 +650,15 @@
             <span class="k">return</span> <span class="kc">False</span>
 
         <span class="k">return</span> <span class="nb">all</span><span class="p">(</span>
             <span class="nb">getattr</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">field</span><span class="p">)</span> <span class="o">==</span> <span class="nb">getattr</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">field</span><span class="p">)</span> <span class="k">for</span> <span class="n">field</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;_db&quot;</span><span class="p">,</span> <span class="s2">&quot;_pk&quot;</span><span class="p">]</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="fm">__ne__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">):</span>
-        <span class="k">return</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="fm">__eq__</span><span class="p">(</span><span class="n">other</span><span class="p">)</span>
+        <span class="k">return</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="fm">__eq__</span><span class="p">(</span><span class="n">other</span><span class="p">)</span></div>
 
 
 <span class="k">def</span> <span class="nf">rotate_image_point</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">xmid</span><span class="p">,</span> <span class="n">ymid</span><span class="p">,</span> <span class="n">angle</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;rotate image point about xm, ym by angle in radians</span>
 
 <span class="sd">    Arguments:</span>
 <span class="sd">        x: x coordinate of point to rotate</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -180,15 +180,15 @@
         )
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
 
 
-class FaceInfo:
+[docs]class FaceInfo:
     """Info about a face in the Photos library"""
 
     def __init__(self, db=None, pk=None):
         """Creates a new FaceInfo instance
 
         Arguments:
             db: instance of PhotosDB object
@@ -323,15 +323,15 @@
             h = self.size_pixels / self.photo.width
             w = self.size_pixels / self.photo.height
             x = x - self.size_pixels / self.photo.width / 2
             y = y - self.size_pixels / self.photo.height / 2
 
         return MPRI_Reg_Rect(x, y, h, w)
 
-    def face_rect(self):
+[docs]    def face_rect(self):
         """Get face rectangle coordinates for current version of the associated
 image
             If image has been edited, rectangle applies to edited version,
 otherwise original version
             Coordinates in format and reference frame used by PIL
 
         Returns:
@@ -343,23 +343,25 @@
 photo.height
         radius = (self.size / 2) * size_reference
         x, y = self._make_point((self.center_x, self.center_y))
         x0, y0 = x - radius, y - radius
         x1, y1 = x + radius, y + radius
         return [(x0, y0), (x1, y1)]
 
-    def roll_pitch_yaw(self):
+
+[docs]    def roll_pitch_yaw(self):
         """Roll, pitch, yaw of face in radians as tuple"""
         info = self._info
         roll = 0 if info["roll"] is None else info["roll"]
         pitch = 0 if info["pitch"] is None else info["pitch"]
         yaw = 0 if info["yaw"] is None else info["yaw"]
 
         return (roll, pitch, yaw)
 
+
     @property
     def roll(self):
         """Return roll angle in radians of the face region"""
         roll, _, _ = self.roll_pitch_yaw()
         return roll
 
     @property
@@ -458,15 +460,15 @@
         # rotate about center
         xmid, ymid = self.center
         roll, _, _ = self.roll_pitch_yaw()
         xr, yr = rotate_image_point(x, y, xmid, ymid, roll)
 
         return (int(xr), int(yr))
 
-    def asdict(self):
+[docs]    def asdict(self):
         """Returns dict representation of class instance"""
         roll, pitch, yaw = self.roll_pitch_yaw()
         return {
             "_pk": self._pk,
             "uuid": self.uuid,
             "name": self.name,
             "asset_uuid": self.asset_uuid,
@@ -495,18 +497,20 @@
             "glasses_type": self.glasses_type,
             "hair_color_type": self.hair_color_type,
             "intrash": self.intrash,
             "lip_makeup_type": self.lip_makeup_type,
             "smile_type": self.smile_type,
         }
 
-    def json(self):
+
+[docs]    def json(self):
         """Return JSON representation of FaceInfo instance"""
         return json.dumps(self.asdict())
 
+
     def __str__(self):
         return f"FaceInfo(uuid={self.uuid}, center_x={self.center_x}, center_y
 = {self.center_y}, size={self.size}, person={self.name}, asset_uuid=
 {self.asset_uuid})"
 
     def __repr__(self):
         return f"FaceInfo(db={self._db}, pk={self._pk})"
@@ -520,14 +524,15 @@
 "_pk"]
         )
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
 
+
 def rotate_image_point(x, y, xmid, ymid, angle):
     """rotate image point about xm, ym by angle in radians
 
     Arguments:
         x: x coordinate of point to rotate
         y: y coordinate of point to rotate
         xmid: x coordinate of center point to rotate about
```

#### docs/_modules/osxphotos/_constants.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos._constants - osxphotos 0.60.8 documentation</title>
+        <title>osxphotos._constants - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -245,14 +245,17 @@
 <span class="c1"># Ranges for model version by Photos version</span>
 <span class="n">_PHOTOS_5_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">13000</span><span class="p">,</span> <span class="mi">13999</span><span class="p">]</span>
 <span class="n">_PHOTOS_6_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">14000</span><span class="p">,</span> <span class="mi">14999</span><span class="p">]</span>
 <span class="n">_PHOTOS_7_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">15000</span><span class="p">,</span> <span class="mi">15999</span><span class="p">]</span>  <span class="c1"># Dev preview: 15134, 12.1: 15331</span>
 <span class="n">_PHOTOS_8_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">16000</span><span class="p">,</span> <span class="mi">16999</span><span class="p">]</span>  <span class="c1"># Ventura dev preview: 16119</span>
 <span class="n">_PHOTOS_9_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">17000</span><span class="p">,</span> <span class="mi">17999</span><span class="p">]</span>  <span class="c1"># Sonoma dev preview: 17120</span>
 
+<span class="c1"># the preview versions of 12.0.0 had a difference schema for syndication info so need to check model version before processing</span>
+<span class="n">_PHOTOS_SYNDICATION_MODEL_VERSION</span> <span class="o">=</span> <span class="mi">15323</span> <span class="c1"># 12.0.1</span>
+
 <span class="c1"># some table names differ between Photos 5 and later versions</span>
 <span class="n">_DB_TABLE_NAMES</span> <span class="o">=</span> <span class="p">{</span>
     <span class="mi">5</span><span class="p">:</span> <span class="p">{</span>
         <span class="s2">&quot;ASSET&quot;</span><span class="p">:</span> <span class="s2">&quot;ZGENERICASSET&quot;</span><span class="p">,</span>
         <span class="s2">&quot;KEYWORD_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_1KEYWORDS.Z_37KEYWORDS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_34ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_SORT_ORDER&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_FOK_34ASSETS&quot;</span><span class="p">,</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.8_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -88,14 +88,18 @@
 # Ranges for model version by Photos version
 _PHOTOS_5_MODEL_VERSION = [13000, 13999]
 _PHOTOS_6_MODEL_VERSION = [14000, 14999]
 _PHOTOS_7_MODEL_VERSION = [15000, 15999]  # Dev preview: 15134, 12.1: 15331
 _PHOTOS_8_MODEL_VERSION = [16000, 16999]  # Ventura dev preview: 16119
 _PHOTOS_9_MODEL_VERSION = [17000, 17999]  # Sonoma dev preview: 17120
 
+# the preview versions of 12.0.0 had a difference schema for syndication info
+so need to check model version before processing
+_PHOTOS_SYNDICATION_MODEL_VERSION = 15323 # 12.0.1
+
 # some table names differ between Photos 5 and later versions
 _DB_TABLE_NAMES = {
     5: {
         "ASSET": "ZGENERICASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_37KEYWORDS",
         "ALBUM_JOIN": "Z_26ASSETS.Z_34ASSETS",
         "ALBUM_SORT_ORDER": "Z_26ASSETS.Z_FOK_34ASSETS",
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.9'
+     - The osxphotos version, e.g. '0.61.0'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.9',
+    VERSION: '0.61.0',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.9 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1939,14 +1939,20 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-sidecar-drop-ext">
 <span class="sig-name descname"><span class="pre">--sidecar-drop-ext</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-sidecar-drop-ext" title="Permalink to this definition">#</a></dt>
 <dd><p>Drop the photo’s extension when naming sidecar files. By default, sidecar files are named in format ‘photo_filename.photo_ext.sidecar_ext’, e.g. ‘IMG_1234.JPG.xmp’. Use ‘–sidecar-drop-ext’ to ignore the photo extension. Resulting sidecar files will have name in format ‘IMG_1234.xmp’. Warning: this may result in sidecar filename collisions if there are files of different types but the same name in the output directory, e.g. ‘IMG_1234.JPG’ and ‘IMG_1234.MOV’.</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-sidecar-template">
+<span class="sig-name descname"><span class="pre">--sidecar-template</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;MAKO_TEMPLATE_FILE</span> <span class="pre">SIDECAR_FILENAME_TEMPLATE</span> <span class="pre">WRITE_SKIPPED</span> <span class="pre">STRIP_WHITESPACE</span> <span class="pre">STRIP_LINES&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-export-sidecar-template" title="Permalink to this definition">#</a></dt>
+<dd><p>Create a custom sidecar file for each photo exported with user provided Mako template (MAKO_TEMPLATE_FILE). MAKO_TEMPLATE_FILE must be a valid Mako template (see <a class="reference external" href="https://www.makotemplates.org/">https://www.makotemplates.org/</a>). The template will passed the following variables: photo (PhotoInfo object for the photo being exported), sidecar_path (pathlib.Path object for the path to the sidecar being written), and photo_path (pathlib.Path object for the path to the exported photo. SIDECAR_FILENAME_TEMPLATE must be a valid template string (see Templating System in help) which will be rendered to generate the filename of the sidecar file. The <cite>{filepath}</cite> template variable may be used in the SIDECAR_FILENAME_TEMPLATE to refer to the filename of the photo being exported. WRITE_SKIPPED is a boolean value (true/false, yes/no, 1/0 are all valid values) and indicates whether or not write the sidecar file even if the photo is skipped during export. If WRITE_SKIPPED is false, the sidecar file will not be written if the photo is skipped during export. If WRITE_SKIPPED is true, the sidecar file will be written even if the photo is skipped during export. STRIP_WHITESPACE and STRIP_LINES are boolean values (true/false, yes/no, 1/0 are all valid values) and indicate whether or not to strip whitespace and blank lines from the resulting sidecar file. For example, to create a sidecar file with extension .xmp using a template file named ‘sidecar.mako’ and write a sidecar for skipped photos and strip blank lines but not whitespace: <cite>–sidecar-template sidecar.mako ‘{filepath}.xmp’ yes no yes</cite>. To do the same but to drop the photo extension from the sidecar filename: <cite>–sidecar-template sidecar.mako ‘{filepath.parent}/{filepath.stem}.xmp’ yes no yes –sidecar-drop-ext</cite>. For an example Mako file see <a class="reference external" href="https://raw.githubusercontent.com/RhetTbull/osxphotos/main/examples/custom_sidecar.mako">https://raw.githubusercontent.com/RhetTbull/osxphotos/main/examples/custom_sidecar.mako</a></p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-exiftool">
 <span class="sig-name descname"><span class="pre">--exiftool</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-exiftool" title="Permalink to this definition">#</a></dt>
 <dd><p>Use exiftool to write metadata directly to exported photos. To use this option, exiftool must be installed and in the path.  exiftool may be installed from <a class="reference external" href="https://exiftool.org/">https://exiftool.org/</a>.  Cannot be used with –export-as-hardlink.  Writes the following metadata: EXIF:ImageDescription, XMP:Description (see also –description-template); XMP:Title; XMP:TagsList, IPTC:Keywords, XMP:Subject (see also –keyword-template, –person-keyword, –album-keyword); XMP:PersonInImage; EXIF:GPSLatitudeRef; EXIF:GPSLongitudeRef; EXIF:GPSLatitude; EXIF:GPSLongitude; EXIF:GPSPosition; EXIF:DateTimeOriginal; EXIF:OffsetTimeOriginal; EXIF:ModifyDate (see –ignore-date-modified); IPTC:DateCreated; IPTC:TimeCreated; (video files only): QuickTime:CreationDate; QuickTime:CreateDate; QuickTime:ModifyDate (see also –ignore-date-modified); QuickTime:GPSCoordinates; UserData:GPSCoordinates.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-exiftool-path">
@@ -4927,59 +4933,54 @@
 <dd><p>Run COMMAND if there is a new version of osxphotos available.</p>
 </dd></dl>
 
 </section>
 </section>
 <div class="highlight-text notranslate"><div class="highlight"><pre><span></span>Usage: python -m osxphotos [OPTIONS] COMMAND [ARGS]...
 
-  osxphotos: query and export your Photos library
+  osxphotos: the multi-tool for your Photos library
 
 Options:
-  --db PHOTOS_LIBRARY_PATH  Specify Photos database path. Path to Photos
-                            library/database can be specified using either
-                            --db or directly as PHOTOS_LIBRARY positional
-                            argument. If neither --db or PHOTOS_LIBRARY
-                            provided, will attempt to find the library to use
-                            in the following order: 1. last opened library, 2.
-                            system library, 3. ~/Pictures/Photos
-                            Library.photoslibrary
-  --json                    Print output in JSON format.
-  -v, --version             Show the version and exit.
-  -h, --help                Show this message and exit.
+  -v, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
 
 Commands:
-  about      Print information about osxphotos including license.
-  albums     Print out albums found in the Photos library.
-  diff       Compare two Photos databases and print out differences
-  docs       Open osxphotos documentation in your browser.
-  dump       Print list of all photos &amp; associated info from the Photos...
-  exiftool   Run exiftool on previously exported files to update metadata.
-  export     Export photos from the Photos database.
-  exportdb   Utilities for working with the osxphotos export database
-  help       Print help; for help on commands: help &lt;command&gt;.
-  import     Import photos and videos into Photos.
-  info       Print out descriptive info of the Photos library database.
-  inspect    Interactively inspect photos selected in Photos.
-  install    Install Python packages into the same environment as osxphotos
-  keywords   Print out keywords found in the Photos library.
-  labels     Print out image classification labels found in the Photos...
-  list       Print list of Photos libraries found on the system.
-  orphans    Find orphaned photos in a Photos library
-  persons    Print out persons (faces) found in the Photos library.
-  places     Print out places found in the Photos library.
-  query      Query the Photos database using 1 or more search options; if...
-  repl       Run interactive osxphotos REPL shell (useful for debugging,...
-  run        Run a python file using same environment as osxphotos.
-  snap       Create snapshot of Photos database to use with diff command
-  theme      Manage osxphotos color themes.
-  timewarp   Adjust date/time/timezone of photos in Apple Photos.
-  tutorial   Display osxphotos tutorial.
-  uninstall  Uninstall Python packages from the osxphotos environment
-  uuid       Print out unique IDs (UUID) of photos selected in Photos
-  version    Check for new version of osxphotos.
+  about          Print information about osxphotos including license.
+  add-locations  Add missing location data to photos in Photos.app using...
+  albums         Print out albums found in the Photos library.
+  batch-edit     Batch edit photo metadata such as title, description,...
+  diff           Compare two Photos databases and print out differences
+  docs           Open osxphotos documentation in your browser.
+  dump           Print list of all photos &amp; associated info from the...
+  exiftool       Run exiftool on previously exported files to update...
+  export         Export photos from the Photos database.
+  exportdb       Utilities for working with the osxphotos export database
+  help           Print help; for help on commands: help &lt;command&gt;.
+  import         Import photos and videos into Photos.
+  info           Print out descriptive info of the Photos library database.
+  inspect        Interactively inspect photos selected in Photos.
+  install        Install Python packages into the same environment as...
+  keywords       Print out keywords found in the Photos library.
+  labels         Print out image classification labels found in the...
+  list           Print list of Photos libraries found on the system.
+  orphans        Find orphaned photos in a Photos library
+  persons        Print out persons (faces) found in the Photos library.
+  places         Print out places found in the Photos library.
+  query          Query the Photos database using 1 or more search...
+  repl           Run interactive osxphotos REPL shell (useful for...
+  run            Run a python file using same environment as osxphotos.
+  show           Show photo, album, or folder in Photos from UUID_OR_NAME
+  snap           Create snapshot of Photos database to use with diff command
+  sync           Sync metadata and albums between Photos libraries.
+  theme          Manage osxphotos color themes.
+  timewarp       Adjust date/time/timezone of photos in Apple Photos.
+  tutorial       Display osxphotos tutorial.
+  uninstall      Uninstall Python packages from the osxphotos environment
+  uuid           Print out unique IDs (UUID) of photos selected in Photos
+  version        Check for new version of osxphotos.
 </pre></div>
 </div>
 </section>
 
         </article>
       </div>
       <footer>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1002,14 +1002,43 @@
       sidecar files are named in format
       âphoto_filename.photo_ext.sidecar_extâ, e.g. âIMG_1234.JPG.xmpâ.
       Use ââsidecar-drop-extâ to ignore the photo extension. Resulting
       sidecar files will have name in format âIMG_1234.xmpâ. Warning: this
       may result in sidecar filename collisions if there are files of different
       types but the same name in the output directory, e.g. âIMG_1234.JPGâ
       and âIMG_1234.MOVâ.
+  --sidecar-template <MAKO_TEMPLATE_FILE SIDECAR_FILENAME_TEMPLATE
+  WRITE_SKIPPED STRIP_WHITESPACE STRIP_LINES>#
+      Create a custom sidecar file for each photo exported with user provided
+      Mako template (MAKO_TEMPLATE_FILE). MAKO_TEMPLATE_FILE must be a valid
+      Mako template (see https://www.makotemplates.org/). The template will
+      passed the following variables: photo (PhotoInfo object for the photo
+      being exported), sidecar_path (pathlib.Path object for the path to the
+      sidecar being written), and photo_path (pathlib.Path object for the path
+      to the exported photo. SIDECAR_FILENAME_TEMPLATE must be a valid template
+      string (see Templating System in help) which will be rendered to generate
+      the filename of the sidecar file. The{filepath}template variable may be
+      used in the SIDECAR_FILENAME_TEMPLATE to refer to the filename of the
+      photo being exported. WRITE_SKIPPED is a boolean value (true/false, yes/
+      no, 1/0 are all valid values) and indicates whether or not write the
+      sidecar file even if the photo is skipped during export. If WRITE_SKIPPED
+      is false, the sidecar file will not be written if the photo is skipped
+      during export. If WRITE_SKIPPED is true, the sidecar file will be written
+      even if the photo is skipped during export. STRIP_WHITESPACE and
+      STRIP_LINES are boolean values (true/false, yes/no, 1/0 are all valid
+      values) and indicate whether or not to strip whitespace and blank lines
+      from the resulting sidecar file. For example, to create a sidecar file
+      with extension .xmp using a template file named âsidecar.makoâ and
+      write a sidecar for skipped photos and strip blank lines but not
+      whitespace:âsidecar-template sidecar.mako â{filepath}.xmpâ yes no
+      yes. To do the same but to drop the photo extension from the sidecar
+      filename:âsidecar-template sidecar.mako â{filepath.parent}/
+      {filepath.stem}.xmpâ yes no yes âsidecar-drop-ext. For an example
+      Mako file see https://raw.githubusercontent.com/RhetTbull/osxphotos/main/
+      examples/custom_sidecar.mako
   --exiftool#
       Use exiftool to write metadata directly to exported photos. To use this
       option, exiftool must be installed and in the path. exiftool may be
       installed from https://exiftool.org/. Cannot be used with âexport-as-
       hardlink. Writes the following metadata: EXIF:ImageDescription, XMP:
       Description (see also âdescription-template); XMP:Title; XMP:TagsList,
       IPTC:Keywords, XMP:Subject (see also âkeyword-template, âperson-
@@ -2734,59 +2763,54 @@
 osxphotos version [OPTIONS]
 Options
   --run <COMMAND>#
       Run COMMAND if there is a new version of osxphotos available.
 
 Usage: python -m osxphotos [OPTIONS] COMMAND [ARGS]...
 
-  osxphotos: query and export your Photos library
+  osxphotos: the multi-tool for your Photos library
 
 Options:
-  --db PHOTOS_LIBRARY_PATH  Specify Photos database path. Path to Photos
-                            library/database can be specified using either
-                            --db or directly as PHOTOS_LIBRARY positional
-                            argument. If neither --db or PHOTOS_LIBRARY
-                            provided, will attempt to find the library to use
-                            in the following order: 1. last opened library, 2.
-                            system library, 3. ~/Pictures/Photos
-                            Library.photoslibrary
-  --json                    Print output in JSON format.
-  -v, --version             Show the version and exit.
-  -h, --help                Show this message and exit.
+  -v, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
 
 Commands:
-  about      Print information about osxphotos including license.
-  albums     Print out albums found in the Photos library.
-  diff       Compare two Photos databases and print out differences
-  docs       Open osxphotos documentation in your browser.
-  dump       Print list of all photos & associated info from the Photos...
-  exiftool   Run exiftool on previously exported files to update metadata.
-  export     Export photos from the Photos database.
-  exportdb   Utilities for working with the osxphotos export database
-  help       Print help; for help on commands: help <command>.
-  import     Import photos and videos into Photos.
-  info       Print out descriptive info of the Photos library database.
-  inspect    Interactively inspect photos selected in Photos.
-  install    Install Python packages into the same environment as osxphotos
-  keywords   Print out keywords found in the Photos library.
-  labels     Print out image classification labels found in the Photos...
-  list       Print list of Photos libraries found on the system.
-  orphans    Find orphaned photos in a Photos library
-  persons    Print out persons (faces) found in the Photos library.
-  places     Print out places found in the Photos library.
-  query      Query the Photos database using 1 or more search options; if...
-  repl       Run interactive osxphotos REPL shell (useful for debugging,...
-  run        Run a python file using same environment as osxphotos.
-  snap       Create snapshot of Photos database to use with diff command
-  theme      Manage osxphotos color themes.
-  timewarp   Adjust date/time/timezone of photos in Apple Photos.
-  tutorial   Display osxphotos tutorial.
-  uninstall  Uninstall Python packages from the osxphotos environment
-  uuid       Print out unique IDs (UUID) of photos selected in Photos
-  version    Check for new version of osxphotos.
+  about          Print information about osxphotos including license.
+  add-locations  Add missing location data to photos in Photos.app using...
+  albums         Print out albums found in the Photos library.
+  batch-edit     Batch edit photo metadata such as title, description,...
+  diff           Compare two Photos databases and print out differences
+  docs           Open osxphotos documentation in your browser.
+  dump           Print list of all photos & associated info from the...
+  exiftool       Run exiftool on previously exported files to update...
+  export         Export photos from the Photos database.
+  exportdb       Utilities for working with the osxphotos export database
+  help           Print help; for help on commands: help <command>.
+  import         Import photos and videos into Photos.
+  info           Print out descriptive info of the Photos library database.
+  inspect        Interactively inspect photos selected in Photos.
+  install        Install Python packages into the same environment as...
+  keywords       Print out keywords found in the Photos library.
+  labels         Print out image classification labels found in the...
+  list           Print list of Photos libraries found on the system.
+  orphans        Find orphaned photos in a Photos library
+  persons        Print out persons (faces) found in the Photos library.
+  places         Print out places found in the Photos library.
+  query          Query the Photos database using 1 or more search...
+  repl           Run interactive osxphotos REPL shell (useful for...
+  run            Run a python file using same environment as osxphotos.
+  show           Show photo, album, or folder in Photos from UUID_OR_NAME
+  snap           Create snapshot of Photos database to use with diff command
+  sync           Sync metadata and albums between Photos libraries.
+  theme          Manage osxphotos color themes.
+  timewarp       Adjust date/time/timezone of photos in Apple Photos.
+  tutorial       Display osxphotos tutorial.
+  uninstall      Uninstall Python packages from the osxphotos environment
+  uuid           Print out unique IDs (UUID) of photos selected in Photos
+  version        Check for new version of osxphotos.
 
 Next
 OSXPhotos_Template_System
 
 Previous
 OSXPhotos_Tutorial
 Copyright © 2021, Rhet Turnbull
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.9 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.61.0 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -2293,14 +2293,21 @@
     --sidecar-drop-ext
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-export-sidecar-drop-ext">osxphotos-export command line option</a>
 </li>
         </ul></li>
         <li>
+    --sidecar-template
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-export-sidecar-template">osxphotos-export command line option</a>
+</li>
+        </ul></li>
+        <li>
     --skip-bursts
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-bursts">osxphotos-export command line option</a>
 </li>
         </ul></li>
         <li>
@@ -4470,14 +4477,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-shared-moment">--shared-moment</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-sidecar">--sidecar</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-sidecar-drop-ext">--sidecar-drop-ext</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-sidecar-template">--sidecar-template</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-bursts">--skip-bursts</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-edited">--skip-edited</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-live">--skip-live</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-original-if-edited">--skip-original-if-edited</a>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -41,908 +41,908 @@
 | S | T | U | V | W | Y
 
 ***** Symbols *****
     * --add-exported-to-album
           o osxphotos-export_command
             line_option
     * --add-missing-to-album
-          o osxphotos-export_command
-            line_option                     * --not-hidden
-    * --add-skipped-to-album                      o osxphotos-add-locations
+          o osxphotos-export_command        * --not-hidden
+            line_option                           o osxphotos-add-locations
+    * --add-skipped-to-album                        command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+    * --add-to-album                              o osxphotos-query_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-timewarp_command              option
+            line_option                           o osxphotos-sync_command_line
+    * --added-after                                 option
+          o osxphotos-add-locations         * --not-in-album
+            command_line_option                   o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-    * --add-to-album                                line_option
-          o osxphotos-query_command               o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-timewarp_command            o osxphotos-repl_command_line
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --added-before                                option
+          o osxphotos-add-locations         * --not-incloud
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --added-in-last                               option
+          o osxphotos-add-locations         * --not-live
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --album                                       option
+          o osxphotos-add-locations         * --not-missing
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-repl_command_line             option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-sync_command_line             option
+            option                          * --not-panorama
+    * --album-keyword                             o osxphotos-add-locations
+          o osxphotos-exiftool_command              command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-query_command
+    * --alt-copy                                    line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
-    * --added-after                               o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --not-in-album
+    * --append                                    o osxphotos-sync_command_line
+          o osxphotos-exiftool_command              option
+            line_option                     * --not-portrait
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
+          o osxphotos-exportdb_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --added-before                              o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --not-incloud
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
+          o osxphotos-import_command              o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
-            option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --added-in-last                             o osxphotos-sync_command_line
+    * --burst                                     o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-live
+            command_line_option             * --not-reference
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --album                                     o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --not-missing
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-import_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-query_command
+    * --check-signatures                          o osxphotos-sync_command_line
+          o osxphotos-exportdb_command              option
+            line_option                     * --not-saved-to-library
+    * --check-templates                           o osxphotos-add-locations
+          o osxphotos-import_command                command_line_option
+            line_option                           o osxphotos-export_command
+    * --cleanup                                     line_option
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-    * --album-keyword                       * --not-panorama
-          o osxphotos-exiftool_command            o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+    * --clear-location                            o osxphotos-repl_command_line
+          o osxphotos-import_command                option
+            line_option                           o osxphotos-sync_command_line
+    * --clear-metadata                              option
+          o osxphotos-import_command        * --not-screenshot
+            line_option                           o osxphotos-add-locations
+    * --clone                                       command_line_option
+          o osxphotos-theme_command               o osxphotos-export_command
             line_option                             line_option
-    * --alt-copy                                  o osxphotos-query_command
-          o osxphotos-export_command                line_option
+    * --cloudasset                                o osxphotos-query_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
+            line_option                     * --not-selfie
+          o osxphotos-repl_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --compare-exif                              o osxphotos-query_command
+          o osxphotos-timewarp_command              line_option
             line_option                           o osxphotos-repl_command_line
-    * --append                                      option
-          o osxphotos-exiftool_command            o osxphotos-sync_command_line
+    * --config                                      option
+          o osxphotos-theme_command               o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-export_command        * --not-portrait
-            line_option                           o osxphotos-add-locations
-          o osxphotos-exportdb_command              command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-import_command                line_option
+    * --config-only                         * --not-shared
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+    * --convert-to-jpeg                           o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --burst                                       option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * --not-reference
-            line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --check-signatures                            option
-          o osxphotos-exportdb_command            o osxphotos-sync_command_line
+    * --count                                       line_option
+          o osxphotos-query_command               o osxphotos-repl_command_line
             line_option                             option
-    * --check-templates                     * --not-saved-to-library
-          o osxphotos-import_command              o osxphotos-add-locations
+    * --current-name                        * --not-shared-moment
+          o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-    * --cleanup                                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
+    * --date                                      o osxphotos-export_command
+          o osxphotos-timewarp_command              line_option
             line_option                           o osxphotos-query_command
-    * --clear-location                              line_option
-          o osxphotos-import_command              o osxphotos-repl_command_line
+    * --date-added                                  line_option
+          o osxphotos-timewarp_command            o osxphotos-repl_command_line
             line_option                             option
-    * --clear-metadata                            o osxphotos-sync_command_line
-          o osxphotos-import_command                option
-            line_option                     * --not-screenshot
-    * --clone                                     o osxphotos-add-locations
-          o osxphotos-theme_command                 command_line_option
+    * --date-added-from-photo                     o osxphotos-sync_command_line
+          o osxphotos-timewarp_command              option
+            line_option                     * --not-slow-mo
+    * --date-delta                                o osxphotos-add-locations
+          o osxphotos-timewarp_command              command_line_option
             line_option                           o osxphotos-export_command
-    * --cloudasset                                  line_option
-          o osxphotos-add-locations               o osxphotos-query_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
+    * --db                                          line_option
+          o osxphotos-albums_command              o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-batch-edit                  o osxphotos-repl_command_line
+            command_line_option                     option
+          o osxphotos-diff_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-dump_command_line     * --not-syndicated
+            option                                o osxphotos-add-locations
+          o osxphotos-exiftool_command              command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-info_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-inspect_command               option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-keywords_command              option
+            line_option                     * --not-time-lapse
+          o osxphotos-labels_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-orphans_command             o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-persons_command             o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-places_command              o osxphotos-repl_command_line
             line_option                             option
           o osxphotos-query_command               o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-repl_command_line     * --not-selfie
+          o osxphotos-repl_command_line     * --only-movies
             option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
+          o osxphotos-show_command_line             command_line_option
             option                                o osxphotos-export_command
-    * --compare-exif                                line_option
-          o osxphotos-timewarp_command            o osxphotos-query_command
-            line_option                             line_option
-    * --config                                    o osxphotos-repl_command_line
-          o osxphotos-theme_command                 option
-            line_option                           o osxphotos-sync_command_line
-    * --config-only                                 option
-          o osxphotos-export_command        * --not-shared
-            line_option                           o osxphotos-add-locations
-    * --convert-to-jpeg                             command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-    * --count                                     o osxphotos-query_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-repl_command_line
-    * --current-name                                option
-          o osxphotos-export_command        * --not-shared-moment
-            line_option                           o osxphotos-add-locations
-    * --date                                        command_line_option
-          o osxphotos-timewarp_command            o osxphotos-export_command
-            line_option                             line_option
-    * --date-added                                o osxphotos-query_command
-          o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-repl_command_line
-    * --date-added-from-photo                       option
-          o osxphotos-timewarp_command            o osxphotos-sync_command_line
+          o osxphotos-snap_command_line             line_option
+            option                                o osxphotos-query_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-repl_command_line
+    * --db-config                                   option
+          o osxphotos-exiftool_command            o osxphotos-sync_command_line
             line_option                             option
-    * --date-delta                          * --not-slow-mo
-          o osxphotos-timewarp_command            o osxphotos-add-locations
+    * --default                             * --only-new
+          o osxphotos-theme_command               o osxphotos-export_command
+            line_option                             line_option
+    * --delete                              * --only-photos
+          o osxphotos-theme_command               o osxphotos-add-locations
             line_option                             command_line_option
-    * --db                                        o osxphotos-export_command
-          o osxphotos-albums_command                line_option
+    * --delete-file                               o osxphotos-export_command
+          o osxphotos-exportdb_command              line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option                   o osxphotos-repl_command_line
-          o osxphotos-diff_command_line             option
-            option                                o osxphotos-sync_command_line
+    * --delete-uuid                                 line_option
+          o osxphotos-exportdb_command            o osxphotos-repl_command_line
+            line_option                             option
+    * --deleted                                   o osxphotos-sync_command_line
           o osxphotos-dump_command_line             option
-            option                          * --not-syndicated
-          o osxphotos-exiftool_command            o osxphotos-add-locations
-            line_option                             command_line_option
+            option                          * --original-suffix
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-info_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-inspect_command             o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-keywords_command            o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-labels_command        * --not-time-lapse
-            line_option                           o osxphotos-add-locations
-          o osxphotos-orphans_command               command_line_option
+          o osxphotos-query_command         * --overwrite
             line_option                           o osxphotos-export_command
-          o osxphotos-persons_command               line_option
+          o osxphotos-repl_command_line             line_option
+            option                          * --panorama
+    * --deleted-only                              o osxphotos-add-locations
+          o osxphotos-dump_command_line             command_line_option
+            option                                o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-places_command                line_option
+          o osxphotos-query_command                 line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
-            option                          * --only-movies
-          o osxphotos-show_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-snap_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                o osxphotos-sync_command_line
+    * --description                                 option
+          o osxphotos-add-locations         * --parse-date
+            command_line_option                   o osxphotos-import_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * --person
+          o osxphotos-import_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
-    * --db-config                                 o osxphotos-repl_command_line
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --description-template                      o osxphotos-sync_command_line
           o osxphotos-exiftool_command              option
-            line_option                           o osxphotos-sync_command_line
-    * --default                                     option
-          o osxphotos-theme_command         * --only-new
-            line_option                           o osxphotos-export_command
-    * --delete                                      line_option
-          o osxphotos-theme_command         * --only-photos
-            line_option                           o osxphotos-add-locations
-    * --delete-file                                 command_line_option
-          o osxphotos-exportdb_command            o osxphotos-export_command
+            line_option                     * --person-keyword
+          o osxphotos-export_command              o osxphotos-exiftool_command
             line_option                             line_option
-    * --delete-uuid                               o osxphotos-query_command
-          o osxphotos-exportdb_command              line_option
-            line_option                           o osxphotos-repl_command_line
-    * --deleted                                     option
-          o osxphotos-dump_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-export_command        * --original-suffix
+    * --detect-text                               o osxphotos-export_command
+          o osxphotos-inspect_command               line_option
+            line_option                     * --place
+    * --directory                                 o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --overwrite
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-    * --deleted-only                        * --panorama
-          o osxphotos-dump_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-query_command
+    * --download-missing                            line_option
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --description                               o osxphotos-sync_command_line
+    * --dry-run                                   o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --parse-date
-          o osxphotos-batch-edit                  o osxphotos-import_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-timewarp_command
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-batch-edit                    option
+            command_line_option             * --plain
+          o osxphotos-exiftool_command            o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-import_command        * --person
+          o osxphotos-export_command        * --portrait
             line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
+          o osxphotos-exportdb_command              command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --description-template                        option
-          o osxphotos-exiftool_command            o osxphotos-sync_command_line
+            option                                o osxphotos-query_command
+    * --dup-check                                   line_option
+          o osxphotos-import_command              o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-export_command        * --person-keyword
-            line_option                           o osxphotos-exiftool_command
-    * --detect-text                                 line_option
-          o osxphotos-inspect_command             o osxphotos-export_command
-            line_option                             line_option
-    * --directory                           * --place
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-    * --download-missing                          o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --dry-run                                     line_option
-          o osxphotos-add-locations               o osxphotos-repl_command_line
-            command_line_option                     option
-          o osxphotos-batch-edit                  o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-exiftool_command      * --plain
-            line_option                           o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
-            line_option                     * --portrait
-          o osxphotos-exportdb_command            o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-sync_command_line           o osxphotos-export_command
-            option                                  line_option
-    * --dup-check                                 o osxphotos-query_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-repl_command_line
-    * --duplicate                                   option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * --post-command
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --post-function
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-    * --edit                                * --preview
-          o osxphotos-theme_command               o osxphotos-export_command
-            line_option                             line_option
-    * --edited                                    o osxphotos-theme_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --preview-if-missing
+    * --duplicate                                 o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --post-command
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --preview-suffix
+          o osxphotos-query_command         * --post-function
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
-            option                          * --print
-          o osxphotos-sync_command_line           o osxphotos-dump_command_line
-            option                                  option
-    * --edited-suffix                             o osxphotos-export_command
+            option                                o osxphotos-import_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --preview
+    * --edit                                      o osxphotos-export_command
+          o osxphotos-theme_command                 line_option
+            line_option                           o osxphotos-theme_command
+    * --edited                                      line_option
+          o osxphotos-add-locations         * --preview-if-missing
+            command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --emacs                                       line_option
-          o osxphotos-repl_command_line     * --pull-exif
-            option                                o osxphotos-timewarp_command
-    * --errors                                      line_option
-          o osxphotos-exportdb_command      * --push-exif
-            line_option                           o osxphotos-timewarp_command
-    * --exif                                        line_option
-          o osxphotos-add-locations         * --query-eval
-            command_line_option                   o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-sync_command_line
-    * --exiftool                                    option
-          o osxphotos-export_command        * --query-function
-            line_option                           o osxphotos-add-locations
-          o osxphotos-import_command                command_line_option
-            line_option                           o osxphotos-export_command
-    * --exiftool-merge-keywords                     line_option
-          o osxphotos-exiftool_command            o osxphotos-query_command
+            line_option                     * --preview-suffix
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
-            line_option                             option
-    * --exiftool-merge-persons                    o osxphotos-sync_command_line
-          o osxphotos-exiftool_command              option
-            line_option                     * --quiet
+          o osxphotos-repl_command_line     * --print
+            option                                o osxphotos-dump_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-export_command
+    * --edited-suffix                               line_option
           o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-    * --exiftool-option                     * --ramdb
-          o osxphotos-exiftool_command            o osxphotos-export_command
+    * --emacs                               * --pull-exif
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+    * --errors                              * --push-exif
+          o osxphotos-exportdb_command            o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-export_command        * --raw-output
-            line_option                           o osxphotos-diff_command_line
-    * --exiftool-path                               option
-          o osxphotos-exiftool_command      * --regex
-            line_option                           o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-timewarp_command              line_option
+    * --exif                                * --query-eval
+          o osxphotos-add-locations               o osxphotos-add-locations
+            command_line_option                     command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --exiftool                            * --query-function
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-import_command              o osxphotos-export_command
+            line_option                             line_option
+    * --exiftool-merge-keywords                   o osxphotos-query_command
+          o osxphotos-exiftool_command              line_option
             line_option                           o osxphotos-repl_command_line
-    * --export                                      option
-          o osxphotos-orphans_command             o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+    * --exiftool-merge-persons                      option
+          o osxphotos-exiftool_command      * --quiet
+            line_option                           o osxphotos-query_command
+          o osxphotos-export_command                line_option
+            line_option                     * --ramdb
+    * --exiftool-option                           o osxphotos-export_command
+          o osxphotos-exiftool_command              line_option
+            line_option                     * --raw-output
+          o osxphotos-export_command              o osxphotos-diff_command_line
             line_option                             option
-          o osxphotos-sync_command_line     * --relative-to
-            option                                o osxphotos-import_command
-    * --export-aae                                  line_option
-          o osxphotos-export_command        * --replace-keywords
-            line_option                           o osxphotos-batch-edit
-    * --export-as-hardlink                          command_line_option
-          o osxphotos-export_command              o osxphotos-exiftool_command
+    * --exiftool-path                       * --regex
+          o osxphotos-exiftool_command            o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --export-by-date                            o osxphotos-export_command
+          o osxphotos-import_command              o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-timewarp_command            o osxphotos-repl_command_line
+            line_option                             option
+    * --export                                    o osxphotos-sync_command_line
+          o osxphotos-orphans_command               option
+            line_option                     * --relative-to
+          o osxphotos-sync_command_line           o osxphotos-import_command
+            option                                  line_option
+    * --export-aae                          * --replace-keywords
+          o osxphotos-export_command              o osxphotos-batch-edit
+            line_option                             command_line_option
+    * --export-as-hardlink                        o osxphotos-exiftool_command
           o osxphotos-export_command                line_option
-            line_option                     * --report
-    * --export-dir                                o osxphotos-exiftool_command
-          o osxphotos-exportdb_command              line_option
             line_option                           o osxphotos-export_command
-    * --exportdb                                    line_option
-          o osxphotos-exiftool_command            o osxphotos-exportdb_command
-            line_option                             line_option
-          o osxphotos-export_command              o osxphotos-import_command
+    * --export-by-date                              line_option
+          o osxphotos-export_command        * --report
+            line_option                           o osxphotos-exiftool_command
+    * --export-dir                                  line_option
+          o osxphotos-exportdb_command            o osxphotos-export_command
             line_option                             line_option
-    * --external-edit                             o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --resume
-          o osxphotos-export_command              o osxphotos-import_command
+    * --exportdb                                  o osxphotos-exportdb_command
+          o osxphotos-exiftool_command              line_option
+            line_option                           o osxphotos-import_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-sync_command_line
+    * --external-edit                               option
+          o osxphotos-add-locations         * --resume
+            command_line_option                   o osxphotos-import_command
+          o osxphotos-export_command                line_option
+            line_option                     * --retry
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --retry
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --run
-          o osxphotos-sync_command_line           o osxphotos-version_command
+          o osxphotos-repl_command_line     * --run
+            option                                o osxphotos-version_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --save-config
+    * --favorite                                  o osxphotos-exiftool_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-exportdb_command
+          o osxphotos-query_command                 line_option
+            line_option                     * --saved-to-library
+          o osxphotos-repl_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-sync_command_line           o osxphotos-export_command
             option                                  line_option
-    * --favorite                            * --save-config
-          o osxphotos-add-locations               o osxphotos-exiftool_command
-            command_line_option                     line_option
+    * --favorite-rating                           o osxphotos-query_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-repl_command_line
+    * --field                                       option
+          o osxphotos-dump_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-query_command         * --screenshot
+            line_option                           o osxphotos-add-locations
+    * --filename                                    command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-exportdb_command
+          o osxphotos-uuid_command_line           o osxphotos-query_command
+            option                                  line_option
+    * --finder-tag-keywords                       o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+    * --finder-tag-template                         option
+          o osxphotos-export_command        * --selected
+            line_option                           o osxphotos-add-locations
+    * --folder                                      command_line_option
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --saved-to-library
+          o osxphotos-query_command               o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-repl_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-sync_command_line     * --selfie
             option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
-            option                                o osxphotos-export_command
-    * --favorite-rating                             line_option
-          o osxphotos-export_command              o osxphotos-query_command
+    * --force                                       command_line_option
+          o osxphotos-timewarp_command            o osxphotos-export_command
             line_option                             line_option
-    * --field                                     o osxphotos-repl_command_line
-          o osxphotos-dump_command_line             option
-            option                                o osxphotos-sync_command_line
+    * --force-update                              o osxphotos-query_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-repl_command_line
+    * --from-date                                   option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * --set
+            line_option                           o osxphotos-sync_command_line
           o osxphotos-query_command                 option
-            line_option                     * --screenshot
-    * --filename                                  o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-uuid_command_line             line_option
-            option                                o osxphotos-query_command
-    * --finder-tag-keywords                         line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
-            line_option                             option
-    * --finder-tag-template                       o osxphotos-sync_command_line
+            line_option                     * --shared
+          o osxphotos-repl_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --from-time                                 o osxphotos-query_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-repl_command_line
           o osxphotos-export_command                option
-            line_option                     * --selected
-    * --folder                                    o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
+            line_option                     * --shared-moment
+          o osxphotos-query_command               o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                  line_option
+    * --function                                  o osxphotos-repl_command_line
+          o osxphotos-timewarp_command              option
+            line_option                           o osxphotos-sync_command_line
+    * --glob                                        option
+          o osxphotos-import_command        * --sidecar
+            line_option                           o osxphotos-export_command
+    * --has-comment                                 line_option
+          o osxphotos-add-locations         * --sidecar-drop-ext
             command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
-            option                          * --selfie
-    * --force                                     o osxphotos-add-locations
-          o osxphotos-timewarp_command              command_line_option
-            line_option                           o osxphotos-export_command
-    * --force-update                                line_option
-          o osxphotos-export_command              o osxphotos-query_command
+            line_option                     * --sidecar-template
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-    * --from-date                                 o osxphotos-repl_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --set
-          o osxphotos-query_command               o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-repl_command_line     * --shared
-            option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
-            option                                o osxphotos-export_command
-    * --from-time                                   line_option
-          o osxphotos-add-locations               o osxphotos-query_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-query_command         * --shared-moment
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
+          o osxphotos-repl_command_line     * --skip-bursts
             option                                o osxphotos-export_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-query_command
-    * --function                                    line_option
-          o osxphotos-timewarp_command            o osxphotos-repl_command_line
-            line_option                             option
-    * --glob                                      o osxphotos-sync_command_line
-          o osxphotos-import_command                option
-            line_option                     * --sidecar
-    * --has-comment                               o osxphotos-export_command
+            option                          * --skip-edited
+    * --has-likes                                 o osxphotos-export_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * --sidecar-drop-ext
+            command_line_option             * --skip-live
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --skip-bursts
+          o osxphotos-query_command         * --skip-original-if-edited
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
-            option                          * --skip-edited
+            option                          * --skip-raw
           o osxphotos-sync_command_line           o osxphotos-export_command
             option                                  line_option
-    * --has-likes                           * --skip-live
+    * --has-raw                             * --skip-uuid
           o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-export_command        * --skip-original-if-edited
+          o osxphotos-export_command        * --skip-uuid-from-file
             line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
-            line_option                     * --skip-raw
-          o osxphotos-repl_command_line           o osxphotos-export_command
+            line_option                     * --slow-mo
+          o osxphotos-repl_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --hdr                                       o osxphotos-query_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
+            line_option                     * --split-folder
+          o osxphotos-repl_command_line           o osxphotos-import_command
             option                                  line_option
-          o osxphotos-sync_command_line     * --skip-uuid
+          o osxphotos-sync_command_line     * --sql
+            option                                o osxphotos-exportdb_command
+    * --help                                        line_option
+          o osxphotos-run_command_line      * --strip
             option                                o osxphotos-export_command
-    * --has-raw                                     line_option
-          o osxphotos-add-locations         * --skip-uuid-from-file
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                     * --slow-mo
+    * --hidden                                      line_option
+          o osxphotos-add-locations         * --style
+            command_line_option                   o osxphotos-diff_command_line
+          o osxphotos-export_command                option
+            line_option                     * --syndicated
           o osxphotos-query_command               o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-query_command
             option                                  line_option
-    * --hdr                                       o osxphotos-repl_command_line
+    * --ignore-case                               o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
             command_line_option                   o osxphotos-sync_command_line
           o osxphotos-export_command                option
-            line_option                     * --split-folder
-          o osxphotos-query_command               o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-repl_command_line     * --sql
-            option                                o osxphotos-exportdb_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --strip
-    * --help                                      o osxphotos-export_command
-          o osxphotos-run_command_line              line_option
-            option                          * --style
-    * --hidden                                    o osxphotos-diff_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --syndicated
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --ignore-case                               o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --template
-          o osxphotos-export_command              o osxphotos-inspect_command
+            line_option                     * --template
+          o osxphotos-query_command               o osxphotos-inspect_command
             line_option                             line_option
-          o osxphotos-query_command         * --theme
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-batch-edit
+          o osxphotos-repl_command_line     * --theme
+            option                                o osxphotos-add-locations
           o osxphotos-sync_command_line             command_line_option
-            option                                o osxphotos-exiftool_command
-    * --ignore-date-modified                        line_option
-          o osxphotos-exiftool_command            o osxphotos-export_command
+            option                                o osxphotos-batch-edit
+    * --ignore-date-modified                        command_line_option
+          o osxphotos-exiftool_command            o osxphotos-exiftool_command
             line_option                             line_option
-          o osxphotos-export_command              o osxphotos-exportdb_command
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --ignore-signature                          o osxphotos-import_command
+    * --ignore-signature                          o osxphotos-exportdb_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-inspect_command
+            line_option                           o osxphotos-import_command
     * --import                                      line_option
-          o osxphotos-sync_command_line           o osxphotos-orphans_command
+          o osxphotos-sync_command_line           o osxphotos-inspect_command
             option                                  line_option
-    * --in-album                                  o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
+    * --in-album                                  o osxphotos-orphans_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-query_command                 line_option
             line_option                     * --time
-          o osxphotos-query_command               o osxphotos-timewarp_command
-            line_option                             line_option
-          o osxphotos-repl_command_line     * --time-delta
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * --time-delta
             option                                o osxphotos-timewarp_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --time-lapse
-    * --incloud                                   o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
+    * --incloud                                     line_option
+          o osxphotos-add-locations         * --time-lapse
+            command_line_option                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-sync_command_line
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
           o osxphotos-sync_command_line             option
-            option                          * --timestamp
-    * --info                                      o osxphotos-add-locations
-          o osxphotos-exportdb_command              command_line_option
-            line_option                           o osxphotos-batch-edit
+            option                                o osxphotos-sync_command_line
+    * --info                                        option
+          o osxphotos-exportdb_command      * --timestamp
+            line_option                           o osxphotos-add-locations
     * --inspect                                     command_line_option
-          o osxphotos-timewarp_command            o osxphotos-diff_command_line
-            line_option                             option
-    * --is-reference                              o osxphotos-exiftool_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-export_command
+          o osxphotos-timewarp_command            o osxphotos-batch-edit
+            line_option                             command_line_option
+    * --is-reference                              o osxphotos-diff_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-exiftool_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-exportdb_command
+            line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-import_command
+            line_option                           o osxphotos-exportdb_command
           o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-orphans_command
+            option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-sync_command_line
-    * --jpeg-ext                                    option
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option, [1]
-    * --jpeg-quality                        * --timezone
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option
-    * --json                                * --title
-          o osxphotos-albums_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-dump_command_line           o osxphotos-batch-edit
+            option                                o osxphotos-orphans_command
+    * --jpeg-ext                                    line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+    * --jpeg-quality                              o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option, [1]
+            line_option                     * --timezone
+    * --json                                      o osxphotos-timewarp_command
+          o osxphotos-albums_command                line_option
+            line_option                     * --title
+          o osxphotos-dump_command_line           o osxphotos-add-locations
             option                                  command_line_option
-          o osxphotos-info_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-keywords_command            o osxphotos-import_command
+          o osxphotos-info_command_line           o osxphotos-batch-edit
+            option                                  command_line_option
+          o osxphotos-keywords_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-labels_command              o osxphotos-query_command
+          o osxphotos-labels_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-list_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-persons_command             o osxphotos-sync_command_line
+          o osxphotos-list_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-persons_command             o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-places_command        * --tmpdir
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --to-date
-    * --keep                                      o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
+          o osxphotos-places_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * --tmpdir
             line_option                           o osxphotos-export_command
-    * --keyword                                     line_option
-          o osxphotos-add-locations               o osxphotos-query_command
+    * --keep                                        line_option
+          o osxphotos-export_command        * --to-date
+            line_option                           o osxphotos-add-locations
+    * --keyword                                     command_line_option
+          o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-batch-edit                  o osxphotos-repl_command_line
-            command_line_option                     option
-          o osxphotos-export_command              o osxphotos-sync_command_line
+          o osxphotos-batch-edit                  o osxphotos-query_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-import_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-import_command        * --to-time
+          o osxphotos-query_command         * --to-time
             line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
+          o osxphotos-repl_command_line             command_line_option
+            option                                o osxphotos-export_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --keyword-template                            option
-          o osxphotos-exiftool_command            o osxphotos-sync_command_line
+            option                                o osxphotos-query_command
+    * --keyword-template                            line_option
+          o osxphotos-exiftool_command            o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-export_command        * --touch-file
-            line_option                           o osxphotos-export_command
-    * --label                                       line_option
-          o osxphotos-add-locations               o osxphotos-exportdb_command
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+    * --label                               * --touch-file
+          o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-export_command        * --undo
+          o osxphotos-export_command              o osxphotos-exportdb_command
+            line_option                             line_option
+          o osxphotos-query_command         * --undo
             line_option                           o osxphotos-batch-edit
-          o osxphotos-query_command                 command_line_option
-            line_option                     * --unmatched
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
+          o osxphotos-repl_command_line             command_line_option
+            option                          * --unmatched
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
             option                                  option
-          o osxphotos-sync_command_line     * --update
-            option                                o osxphotos-export_command
-    * --last-errors                                 line_option
-          o osxphotos-exportdb_command      * --update-errors
-            line_option                           o osxphotos-export_command
-    * --last-run                                    line_option
-          o osxphotos-exportdb_command      * --update-signatures
-            line_option                           o osxphotos-exportdb_command
-    * --library                                     line_option
-          o osxphotos-albums_command        * --upgrade
-            line_option                           o osxphotos-install_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option             * --use-file-time
-          o osxphotos-diff_command_line           o osxphotos-timewarp_command
+    * --last-errors                         * --update
+          o osxphotos-exportdb_command            o osxphotos-export_command
+            line_option                             line_option
+    * --last-run                            * --update-errors
+          o osxphotos-exportdb_command            o osxphotos-export_command
+            line_option                             line_option
+    * --library                             * --update-signatures
+          o osxphotos-albums_command              o osxphotos-exportdb_command
+            line_option                             line_option
+          o osxphotos-batch-edit            * --upgrade
+            command_line_option                   o osxphotos-install_command
+          o osxphotos-diff_command_line             line_option
+            option                          * --use-file-time
+          o osxphotos-dump_command_line           o osxphotos-timewarp_command
             option                                  line_option
-          o osxphotos-dump_command_line     * --use-photokit
-            option                                o osxphotos-export_command
-          o osxphotos-exiftool_command              line_option
+          o osxphotos-exiftool_command      * --use-photokit
+            line_option                           o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                     * --use-photos-export
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-info_command_line     * --uti
-            option                                o osxphotos-add-locations
-          o osxphotos-inspect_command               command_line_option
+          o osxphotos-info_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-inspect_command       * --uti
+            line_option                           o osxphotos-add-locations
+          o osxphotos-keywords_command              command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-keywords_command              line_option
-            line_option                           o osxphotos-query_command
           o osxphotos-labels_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-orphans_command               line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-orphans_command               option
-            line_option                           o osxphotos-sync_command_line
           o osxphotos-persons_command               option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-places_command                option
             line_option                     * --uuid
-          o osxphotos-places_command              o osxphotos-add-locations
+          o osxphotos-query_command               o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-show_command_line           o osxphotos-query_command
             option                                  line_option
-          o osxphotos-show_command_line           o osxphotos-repl_command_line
+          o osxphotos-snap_command_line           o osxphotos-repl_command_line
             option                                  option
-          o osxphotos-snap_command_line           o osxphotos-sync_command_line
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
             option                                  option
-          o osxphotos-sync_command_line     * --uuid-files
-            option                                o osxphotos-exportdb_command
-          o osxphotos-timewarp_command              line_option
-            line_option                     * --uuid-from-file
-    * --limit                                     o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-    * --list                                        line_option
-          o osxphotos-theme_command               o osxphotos-query_command
+          o osxphotos-timewarp_command      * --uuid-files
+            line_option                           o osxphotos-exportdb_command
+    * --limit                                       line_option
+          o osxphotos-export_command        * --uuid-from-file
+            line_option                           o osxphotos-add-locations
+    * --list                                        command_line_option
+          o osxphotos-theme_command               o osxphotos-export_command
             line_option                             line_option
-    * --live                                      o osxphotos-repl_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
+    * --live                                      o osxphotos-query_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-repl_command_line
           o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
             line_option                     * --uuid-info
-          o osxphotos-query_command               o osxphotos-exportdb_command
-            line_option                             line_option
-          o osxphotos-repl_command_line     * --vacuum
+          o osxphotos-repl_command_line           o osxphotos-exportdb_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * --vacuum
             option                                o osxphotos-exportdb_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --verbose
-    * --load-config                               o osxphotos-add-locations
-          o osxphotos-exiftool_command              command_line_option
-            line_option                           o osxphotos-batch-edit
+    * --load-config                                 line_option
+          o osxphotos-exiftool_command      * --verbose
+            line_option                           o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-diff_command_line
-    * --location                                    option
-          o osxphotos-add-locations               o osxphotos-exiftool_command
-            command_line_option                     line_option
-          o osxphotos-batch-edit                  o osxphotos-export_command
+            line_option                           o osxphotos-batch-edit
+    * --location                                    command_line_option
+          o osxphotos-add-locations               o osxphotos-diff_command_line
+            command_line_option                     option
+          o osxphotos-batch-edit                  o osxphotos-exiftool_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-exportdb_command
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-import_command              o osxphotos-import_command
+          o osxphotos-import_command              o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-orphans_command
+          o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line           o osxphotos-orphans_command
             option                                  line_option
-    * --match-time                          * --version
-          o osxphotos-timewarp_command            o osxphotos_command_line
-            line_option                             option
-    * --max-size                                  o osxphotos-exportdb_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --walk
-          o osxphotos-export_command              o osxphotos-import_command
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --match-time                                o osxphotos-timewarp_command
+          o osxphotos-timewarp_command              line_option
+            line_option                     * --version
+    * --max-size                                  o osxphotos_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-exportdb_command
+          o osxphotos-export_command                line_option
+            line_option                     * --walk
+          o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-query_command         * --window
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
+          o osxphotos-repl_command_line     * --window
+            option                                o osxphotos-add-locations
+          o osxphotos-sync_command_line             command_line_option
             option                          * --xattr-template
-          o osxphotos-sync_command_line           o osxphotos-export_command
-            option                                  line_option
-    * --merge                               * --year
-          o osxphotos-sync_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --merge-keywords                            o osxphotos-export_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-query_command
+    * --merge                                     o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --year
+    * --merge-keywords                            o osxphotos-add-locations
+          o osxphotos-import_command                command_line_option
+            line_option                           o osxphotos-export_command
     * --migrate                                     line_option
-          o osxphotos-exportdb_command            o osxphotos-repl_command_line
-            line_option                             option
-    * --migrate-photos-library                    o osxphotos-sync_command_line
+          o osxphotos-exportdb_command            o osxphotos-query_command
+            line_option                             line_option
+    * --migrate-photos-library                    o osxphotos-repl_command_line
           o osxphotos-exportdb_command              option
-            line_option                     * --yes
-    * --min-size                                  o osxphotos-uninstall_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -A
-          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                           o osxphotos-sync_command_line
+    * --min-size                                    option
+          o osxphotos-add-locations         * --yes
+            command_line_option                   o osxphotos-uninstall_command
+          o osxphotos-export_command                line_option
+            line_option                     * -A
+          o osxphotos-query_command               o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-query_command         * -a
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-timewarp_command
+          o osxphotos-repl_command_line     * -a
+            option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
-            option                          * -C
-    * --missing                                   o osxphotos-import_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -c
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option
-          o osxphotos-query_command         * -D
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
             option                                o osxphotos-timewarp_command
+    * --missing                                     line_option
+          o osxphotos-add-locations         * -C
+            command_line_option                   o osxphotos-import_command
+          o osxphotos-export_command                line_option
+            line_option                     * -c
+          o osxphotos-query_command               o osxphotos-timewarp_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * -D
+            option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
-            option                          * -d
-    * --name                                      o osxphotos-import_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-timewarp_command
+            option                                o osxphotos-timewarp_command
+    * --name                                        line_option
+          o osxphotos-add-locations         * -d
+            command_line_option                   o osxphotos-import_command
           o osxphotos-export_command                line_option
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-query_command                 line_option
             line_option                     * -e
-          o osxphotos-query_command               o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line           o osxphotos-import_command
             option                                  line_option
-    * --no-comment                          * -F
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -f
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --no-comment                                o osxphotos-timewarp_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -F
+          o osxphotos-export_command              o osxphotos-timewarp_command
+            line_option                             line_option
+          o osxphotos-query_command         * -f
             line_option                           o osxphotos-dump_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
+          o osxphotos-repl_command_line             option
+            option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-timewarp_command
+            option                                o osxphotos-query_command
     * --no-description                              line_option
-          o osxphotos-add-locations               o osxphotos-uuid_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * -g
+          o osxphotos-add-locations               o osxphotos-timewarp_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-uuid_command_line
+            line_option                             option
+          o osxphotos-query_command         * -g
             line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                     * -h
-          o osxphotos-repl_command_line           o osxphotos-run_command_line
+          o osxphotos-repl_command_line             line_option
+            option                          * -h
+          o osxphotos-sync_command_line           o osxphotos-run_command_line
             option                                  option
-          o osxphotos-sync_command_line     * -i
-            option                                o osxphotos-add-locations
-    * --no-keyword                                  command_line_option
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-query_command
+    * --no-keyword                          * -i
+          o osxphotos-add-locations               o osxphotos-add-locations
+            command_line_option                     command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
+          o osxphotos-query_command               o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
             option                                  option, [1]
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
-            option                                  line_option
-    * --no-likes                            * -k
-          o osxphotos-add-locations               o osxphotos-import_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -L
+    * --no-likes                                  o osxphotos-timewarp_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -k
+          o osxphotos-export_command              o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-query_command         * -L
             line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-timewarp_command
           o osxphotos-repl_command_line             line_option
-            option                          * -l
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-    * --no-location                         * -M
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -m
-            line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-repl_command_line             option
             option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
-            option                          * -P
-    * --no-place                                  o osxphotos-import_command
+            option                          * -l
+    * --no-location                               o osxphotos-import_command
           o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-timewarp_command
+            command_line_option             * -M
+          o osxphotos-export_command              o osxphotos-timewarp_command
+            line_option                             line_option
+          o osxphotos-query_command         * -m
+            line_option                           o osxphotos-import_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-timewarp_command
+    * --no-place                                    line_option
+          o osxphotos-add-locations         * -P
+            command_line_option                   o osxphotos-import_command
           o osxphotos-export_command                line_option
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-query_command                 line_option
             line_option                     * -p
-          o osxphotos-query_command               o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line           o osxphotos-import_command
             option                                  line_option
-          o osxphotos-sync_command_line     * -R
-            option                                o osxphotos-import_command
-    * --no-progress                                 line_option
-          o osxphotos-export_command              o osxphotos-sync_command_line
+          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+    * --no-progress                         * -R
+          o osxphotos-export_command              o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-import_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-import_command        * -r
-            line_option                           o osxphotos-diff_command_line
-    * --no-title                                    option
-          o osxphotos-add-locations               o osxphotos-import_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -s
+    * --no-title                            * -r
+          o osxphotos-add-locations               o osxphotos-diff_command_line
+            command_line_option                     option
+          o osxphotos-export_command              o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-query_command         * -s
             line_option                           o osxphotos-diff_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-sync_command_line             option
             option                          * -T
-          o osxphotos-sync_command_line           o osxphotos-inspect_command
-            option                                  line_option
-    * --not-burst                                 o osxphotos-timewarp_command
+    * --not-burst                                 o osxphotos-inspect_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * -t
-          o osxphotos-export_command              o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-inspect_command
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * -t
+          o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line           o osxphotos-inspect_command
             option                                  line_option
-          o osxphotos-sync_command_line     * -U
-            option                                o osxphotos-install_command
-    * --not-cloudasset                              line_option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * -V
+          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+    * --not-cloudasset                      * -U
+          o osxphotos-add-locations               o osxphotos-install_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * -V
             line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-batch-edit
           o osxphotos-repl_command_line             command_line_option
+            option                                o osxphotos-batch-edit
+          o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-diff_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-exiftool_command
-    * --not-edited                                  line_option
-          o osxphotos-add-locations               o osxphotos-export_command
+    * --not-edited                                  option
+          o osxphotos-add-locations               o osxphotos-exiftool_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-exportdb_command
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-import_command
+          o osxphotos-query_command               o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-orphans_command
+          o osxphotos-repl_command_line           o osxphotos-import_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-    * --not-favorite                              o osxphotos-timewarp_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -v
-          o osxphotos-export_command              o osxphotos_command_line
+          o osxphotos-sync_command_line           o osxphotos-orphans_command
+            option                                  line_option
+    * --not-favorite                              o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * -v
+          o osxphotos-query_command               o osxphotos_command_line
             line_option                             option
-          o osxphotos-query_command         * -w
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
+          o osxphotos-repl_command_line     * -w
+            option                                o osxphotos-add-locations
+          o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                          * -y
-    * --not-hdr                                   o osxphotos-uninstall_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -z
-          o osxphotos-export_command              o osxphotos-timewarp_command
+    * --not-hdr                                     line_option
+          o osxphotos-add-locations         * -y
+            command_line_option                   o osxphotos-uninstall_command
+          o osxphotos-export_command                line_option
+            line_option                     * -z
+          o osxphotos-query_command               o osxphotos-timewarp_command
             line_option                             line_option
-          o osxphotos-query_command
-            line_option
           o osxphotos-repl_command_line
             option
           o osxphotos-sync_command_line
             option
 
 ***** A *****
     * activities_(osxphotos.SearchInfo
@@ -1603,130 +1603,131 @@
           o --screenshot                          o --not-in-album
           o --selected                            o --not-incloud
           o --selfie                              o --not-live
           o --shared                              o --not-missing
           o --shared-moment                       o --not-panorama
           o --sidecar                             o --not-portrait
           o --sidecar-drop-ext                    o --not-reference
-          o --skip-bursts                         o --not-saved-to-library
-          o --skip-edited                         o --not-screenshot
-          o --skip-live                           o --not-selfie
-          o --skip-original-if-edited             o --not-shared-moment
-          o --skip-raw                            o --not-slow-mo
-          o --skip-uuid                           o --not-syndicated
-          o --skip-uuid-from-file                 o --not-time-lapse
-          o --slow-mo                             o --only-movies
-          o --strip                               o --only-photos
-          o --syndicated                          o --panorama
-          o --theme                               o --person
-          o --time-lapse                          o --place
-          o --timestamp                           o --portrait
-          o --title                               o --query-eval
-          o --tmpdir                              o --query-function
-          o --to-date                             o --regex
-          o --to-time                             o --report
-          o --touch-file                          o --saved-to-library
-          o --update                              o --screenshot
-          o --update-errors                       o --selected
-          o --use-photokit                        o --selfie
-          o --use-photos-export                   o --set
-          o --uti                                 o --shared-moment
-          o --uuid                                o --slow-mo
-          o --uuid-from-file                      o --syndicated
-          o --verbose                             o --theme
-          o --xattr-template                      o --time-lapse
-          o --year                                o --timestamp
-          o -i                                    o --title
-          o -V                                    o --to-date
-          o DEST                                  o --to-time
-          o PHOTOS_LIBRARY                        o --unmatched
-    * osxphotos-exportdb command line             o --uti
-      option                                      o --uuid
-          o --append                              o --uuid-from-file
-          o --check-signatures                    o --verbose
-          o --delete-file                         o --year
-          o --delete-uuid                         o -A
-          o --dry-run                             o -e
-          o --errors                              o -i, [1]
-          o --export-dir                          o -m
-          o --info                                o -R
-          o --last-errors                         o -s
-          o --last-run                            o -U
-          o --migrate                             o -V
-          o --migrate-photos-library        * osxphotos-theme command line
-          o --report                          option
-          o --save-config                         o --clone
-          o --sql                                 o --config
-          o --theme                               o --default
-          o --timestamp                           o --delete
-          o --touch-file                          o --edit
-          o --update-signatures                   o --list
-          o --uuid-files                          o --preview
-          o --uuid-info                     * osxphotos-timewarp command line
-          o --vacuum                          option
-          o --verbose                             o --add-to-album
-          o --version                             o --compare-exif
-          o -V                                    o --date
-          o EXPORT_DATABASE                       o --date-added
-    * osxphotos-help command line                 o --date-added-from-photo
-      option                                      o --date-delta
-          o SUBTOPIC                              o --exiftool-path
-          o TOPIC                                 o --force
-    * osxphotos-import command line               o --function
-      option                                      o --inspect
-          o --album                               o --library
-          o --append                              o --match-time
-          o --check-templates                     o --parse-date
-          o --clear-location                      o --plain
-          o --clear-metadata                      o --pull-exif
-          o --description                         o --push-exif
-          o --dup-check                           o --theme
-          o --exiftool                            o --time
-          o --exiftool-path                       o --time-delta
-          o --glob                                o --timestamp, [1]
-          o --keyword                             o --timezone
-          o --location                            o --use-file-time
-          o --merge-keywords                      o --verbose
-          o --no-progress                         o -a
-          o --parse-date                          o -c
-          o --post-function                       o -d
-          o --relative-to                         o -D
-          o --report                              o -e
-          o --resume                              o -F
-          o --split-folder                        o -f
-          o --theme                               o -i
-          o --timestamp                           o -L
-          o --title                               o -M
-          o --verbose                             o -m
-          o --walk                                o -p
-          o -a                                    o -P
-          o -C                                    o -t
-          o -d                                    o -T
-          o -D                                    o -V
-          o -e                                    o -z
-          o -f                              * osxphotos-tutorial command line
-          o -g                                option
-          o -k                                    o WIDTH
-          o -l                              * osxphotos-uninstall command line
-          o -L                                option
-          o -m                                    o --yes
-          o -P                                    o -y
-          o -p                                    o PACKAGES
-          o -r                              * osxphotos-uuid command line
-          o -R                                option
-          o -t                                    o --filename
-          o -V                                    o -f
-          o -w                              * osxphotos-version command line
-          o FILES                             option
-    * osxphotos-info command line                 o --run
-      option                                * overwrite_
-          o --db                              (osxphotos.ExportOptions
-          o --json                            attribute)
-          o --library                       * owner_(osxphotos.PhotoInfo
-          o PHOTOS_LIBRARY                    property)
+          o --sidecar-template                    o --not-saved-to-library
+          o --skip-bursts                         o --not-screenshot
+          o --skip-edited                         o --not-selfie
+          o --skip-live                           o --not-shared-moment
+          o --skip-original-if-edited             o --not-slow-mo
+          o --skip-raw                            o --not-syndicated
+          o --skip-uuid                           o --not-time-lapse
+          o --skip-uuid-from-file                 o --only-movies
+          o --slow-mo                             o --only-photos
+          o --strip                               o --panorama
+          o --syndicated                          o --person
+          o --theme                               o --place
+          o --time-lapse                          o --portrait
+          o --timestamp                           o --query-eval
+          o --title                               o --query-function
+          o --tmpdir                              o --regex
+          o --to-date                             o --report
+          o --to-time                             o --saved-to-library
+          o --touch-file                          o --screenshot
+          o --update                              o --selected
+          o --update-errors                       o --selfie
+          o --use-photokit                        o --set
+          o --use-photos-export                   o --shared-moment
+          o --uti                                 o --slow-mo
+          o --uuid                                o --syndicated
+          o --uuid-from-file                      o --theme
+          o --verbose                             o --time-lapse
+          o --xattr-template                      o --timestamp
+          o --year                                o --title
+          o -i                                    o --to-date
+          o -V                                    o --to-time
+          o DEST                                  o --unmatched
+          o PHOTOS_LIBRARY                        o --uti
+    * osxphotos-exportdb command line             o --uuid
+      option                                      o --uuid-from-file
+          o --append                              o --verbose
+          o --check-signatures                    o --year
+          o --delete-file                         o -A
+          o --delete-uuid                         o -e
+          o --dry-run                             o -i, [1]
+          o --errors                              o -m
+          o --export-dir                          o -R
+          o --info                                o -s
+          o --last-errors                         o -U
+          o --last-run                            o -V
+          o --migrate                       * osxphotos-theme command line
+          o --migrate-photos-library          option
+          o --report                              o --clone
+          o --save-config                         o --config
+          o --sql                                 o --default
+          o --theme                               o --delete
+          o --timestamp                           o --edit
+          o --touch-file                          o --list
+          o --update-signatures                   o --preview
+          o --uuid-files                    * osxphotos-timewarp command line
+          o --uuid-info                       option
+          o --vacuum                              o --add-to-album
+          o --verbose                             o --compare-exif
+          o --version                             o --date
+          o -V                                    o --date-added
+          o EXPORT_DATABASE                       o --date-added-from-photo
+    * osxphotos-help command line                 o --date-delta
+      option                                      o --exiftool-path
+          o SUBTOPIC                              o --force
+          o TOPIC                                 o --function
+    * osxphotos-import command line               o --inspect
+      option                                      o --library
+          o --album                               o --match-time
+          o --append                              o --parse-date
+          o --check-templates                     o --plain
+          o --clear-location                      o --pull-exif
+          o --clear-metadata                      o --push-exif
+          o --description                         o --theme
+          o --dup-check                           o --time
+          o --exiftool                            o --time-delta
+          o --exiftool-path                       o --timestamp, [1]
+          o --glob                                o --timezone
+          o --keyword                             o --use-file-time
+          o --location                            o --verbose
+          o --merge-keywords                      o -a
+          o --no-progress                         o -c
+          o --parse-date                          o -d
+          o --post-function                       o -D
+          o --relative-to                         o -e
+          o --report                              o -F
+          o --resume                              o -f
+          o --split-folder                        o -i
+          o --theme                               o -L
+          o --timestamp                           o -M
+          o --title                               o -m
+          o --verbose                             o -p
+          o --walk                                o -P
+          o -a                                    o -t
+          o -C                                    o -T
+          o -d                                    o -V
+          o -D                                    o -z
+          o -e                              * osxphotos-tutorial command line
+          o -f                                option
+          o -g                                    o WIDTH
+          o -k                              * osxphotos-uninstall command line
+          o -l                                option
+          o -L                                    o --yes
+          o -m                                    o -y
+          o -P                                    o PACKAGES
+          o -p                              * osxphotos-uuid command line
+          o -r                                option
+          o -R                                    o --filename
+          o -t                                    o -f
+          o -V                              * osxphotos-version command line
+          o -w                                option
+          o FILES                                 o --run
+    * osxphotos-info command line           * overwrite_
+      option                                  (osxphotos.ExportOptions
+          o --db                              attribute)
+          o --json                          * owner_(osxphotos.PhotoInfo
+          o --library                         property)
+          o PHOTOS_LIBRARY
 
 ***** P *****
     * PACKAGES                              * photos()_(osxphotos.PhotosDB
           o osxphotos-install_command         method)
             line_option                     * photos_by_uuid()_
           o osxphotos-uninstall_command       (osxphotos.PhotosDB_method)
             line_option                     * PHOTOS_LIBRARY
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.9 documentation</title>
+        <title>osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -744,14 +744,15 @@
 osxphotos-export.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-export-screenshot -
 osxphotos-export.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selected -
 osxphotos-export.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selfie -
 osxphotos-export.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-export-shared -
 osxphotos-export.--shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-export-shared-moment -
 osxphotos-export.--sidecar std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar -
 osxphotos-export.--sidecar-drop-ext std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar-drop-ext -
+osxphotos-export.--sidecar-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar-template -
 osxphotos-export.--skip-bursts std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-bursts -
 osxphotos-export.--skip-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-edited -
 osxphotos-export.--skip-live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-live -
 osxphotos-export.--skip-original-if-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-original-if-edited -
 osxphotos-export.--skip-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-raw -
 osxphotos-export.--skip-uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid -
 osxphotos-export.--skip-uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid-from-file -
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.9 documentation</title>
+        <title>OSXPhotos - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.9 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.9 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.61.0 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.9 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1051,15 +1051,15 @@
 <dd><p>Return bit flags representing options that affect export</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ExportResults">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ExportResults</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">converted_to_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_directories</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_files</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif_updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_warning</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metadata_changed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">new</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">aae_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_touch</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">touched</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportResults"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportResults" title="Permalink to this definition">#</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ExportResults</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">converted_to_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_directories</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_files</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif_updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_error</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exiftool_warning</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exported_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metadata_changed</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">new</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">aae_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_exiftool_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_json_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_xmp_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_user_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sidecar_user_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">skipped_album</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_touch</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">touched</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">updated</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_skipped</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">xattr_written</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportResults"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportResults" title="Permalink to this definition">#</a></dt>
 <dd><p>Results class which holds export results for export</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.ExportResults.all_files">
 <span class="sig-name descname"><span class="pre">all_files</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></span><a class="reference internal" href="_modules/osxphotos/photoexporter.html#ExportResults.all_files"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ExportResults.all_files" title="Permalink to this definition">#</a></dt>
 <dd><p>return all filenames contained in results</p>
 </dd></dl>
 
@@ -2185,16 +2185,16 @@
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.saved_to_library">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">saved_to_library</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PhotoInfo.saved_to_library" title="Permalink to this definition">#</a></dt>
 <dd><p>Return True if syndicated photo has been saved to library;
 returns False if photo is not syndicated or has not been saved to the library.
-Returns None if not Photos 8+.
-Syndicated photos are photos that appear in “Shared with you” album; Photos 8+ only.</p>
+Returns None if not Photos 7+.
+Syndicated photos are photos that appear in “Shared with you” album; Photos 7+ only.</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.score">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">score</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.score" title="Permalink to this definition">#</a></dt>
 <dd><p>Computed score information for a photo</p>
 <dl class="field-list simple">
@@ -2236,29 +2236,29 @@
 <dd><p>returns True if photos is in a shared iCloud album otherwise false
 Only valid on Photos 5; returns None on older versions</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.shared_moment">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">shared_moment</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">bool</span></em><a class="headerlink" href="#osxphotos.PhotoInfo.shared_moment" title="Permalink to this definition">#</a></dt>
-<dd><p>Returns True if photo is part of a shared moment otherwise False</p>
+<dd><p>Returns True if photo is part of a shared moment otherwise False (Photos 7+ only)</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.slow_mo">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">slow_mo</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.slow_mo" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is a slow motion video, otherwise False</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.syndicated">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">syndicated</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PhotoInfo.syndicated" title="Permalink to this definition">#</a></dt>
 <dd><p>Return true if photo was shared via syndication (e.g. via Messages, etc.);
 these are photos that appear in “Shared with you” album.
-Photos 8+ only; returns None if not Photos 8+.</p>
+Photos 7+ only; returns None if not Photos 7+.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.tables">
 <span class="sig-name descname"><span class="pre">tables</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">PhotoTables</span></span></span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.tables"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.tables" title="Permalink to this definition">#</a></dt>
 <dd><p>Return PhotoTables object to provide access database tables associated with this photo (Photos 5+)</p>
 </dd></dl>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -445,15 +445,16 @@
   classosxphotos.ExportResults(converted_to_jpeg=None,
   deleted_directories=None, deleted_files=None, error=None, exif_updated=None,
   exiftool_error=None, exiftool_warning=None, exported=None,
   exported_album=None, metadata_changed=None, missing=None, missing_album=None,
   new=None, aae_written=None, sidecar_exiftool_skipped=None,
   sidecar_exiftool_written=None, sidecar_json_skipped=None,
   sidecar_json_written=None, sidecar_xmp_skipped=None,
-  sidecar_xmp_written=None, skipped=None, skipped_album=None, to_touch=None,
+  sidecar_xmp_written=None, sidecar_user_written=None,
+  sidecar_user_skipped=None, skipped=None, skipped_album=None, to_touch=None,
   touched=None, updated=None, xattr_skipped=None, xattr_written=None)[source]#
       Results class which holds export results for export
         all_files() &#x2192; List[str][source]#
             return all filenames contained in results
         propertyattributes: List[str]#
             Return list of attributes tracked by ExportResults
         propertydatetime: str#
@@ -1032,16 +1033,16 @@
                   tuple of list of rendered strings and list of unmatched
                   template values
               Return type:
                   ([rendered_strings], [unmatched])
         propertysaved_to_library: bool | None#
             Return True if syndicated photo has been saved to library; returns
             False if photo is not syndicated or has not been saved to the
-            library. Returns None if not Photos 8+. Syndicated photos are
-            photos that appear in âShared with youâ album; Photos 8+ only.
+            library. Returns None if not Photos 7+. Syndicated photos are
+            photos that appear in âShared with youâ album; Photos 7+ only.
         propertyscore#
             Computed score information for a photo
               Returns:
                   ScoreInfo instance
         propertyscreenshot#
             Returns True if photo is an HDR photo, otherwise False
         propertysearch_info#
@@ -1054,20 +1055,21 @@
             Returns True if photo is a selfie (front facing camera), otherwise
             False
         propertyshared#
             returns True if photos is in a shared iCloud album otherwise false
             Only valid on Photos 5; returns None on older versions
         propertyshared_moment: bool#
             Returns True if photo is part of a shared moment otherwise False
+            (Photos 7+ only)
         propertyslow_mo#
             Returns True if photo is a slow motion video, otherwise False
         propertysyndicated: bool | None#
             Return true if photo was shared via syndication (e.g. via Messages,
             etc.); these are photos that appear in âShared with youâ album.
-            Photos 8+ only; returns None if not Photos 8+.
+            Photos 7+ only; returns None if not Photos 7+.
         tables() &#x2192; PhotoTables[source]#
             Return PhotoTables object to provide access database tables
             associated with this photo (Photos 5+)
         propertytime_lapse#
             Returns True if photo is a time lapse video, otherwise False
         propertytitle#
             name / title of picture
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.9 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.61.0 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -1,276 +1,154 @@
 Search.setIndex({
     "docnames": ["cli", "index", "overview", "package_overview", "reference", "template_help", "tutorial"],
     "filenames": ["cli.rst", "index.rst", "overview.rst", "package_overview.rst", "reference.rst", "template_help.rst", "tutorial.rst"],
     "titles": ["OSXPhotos Command Line Interface (CLI)", "Welcome to OSXPhotos\u2019s documentation!", "OSXPhotos", "OSXPhotos Python Package Overview", "OSXPhotos Python Reference", "OSXPhotos Template System", "OSXPhotos Tutorial"],
     "terms": {
+        "multi": [0, 4, 5, 6],
+        "tool": [0, 6],
         "your": [0, 1, 2, 3, 5],
         "photo": [0, 1, 2, 3, 4, 5],
         "librari": [0, 1, 2, 3, 4],
         "option": [0, 1, 2, 3, 4, 5],
         "arg": [0, 2, 4],
-        "db": [0, 2, 3, 4, 5, 6],
-        "photos_library_path": 0,
-        "specifi": [0, 1, 2, 3, 4, 5],
-        "databas": [0, 2, 3, 4, 5, 6],
-        "path": [0, 1, 2, 3, 4, 5, 6],
-        "can": [0, 2, 3, 4, 5, 6],
-        "us": [0, 1, 2, 4, 5, 6],
-        "either": [0, 2, 4, 5, 6],
-        "directli": [0, 2, 6],
-        "photos_librari": [0, 2],
-        "posit": [0, 2],
-        "argument": [0, 2, 3, 4, 5, 6],
-        "If": [0, 2, 3, 4, 5, 6],
-        "neither": [0, 2, 4],
-        "provid": [0, 2, 4, 5, 6],
-        "attempt": [0, 2, 4, 6],
-        "find": [0, 2, 3, 4, 5, 6],
-        "follow": [0, 2, 3, 4, 5, 6],
-        "order": [0, 2, 4, 5],
-        "1": [0, 2, 4, 5, 6],
-        "last": [0, 2, 3, 4, 6],
-        "open": [0, 2, 3, 5, 6],
-        "2": [0, 2, 3, 4, 5],
-        "system": [0, 1, 4, 6],
-        "3": [0, 2, 3, 5, 6],
-        "pictur": [0, 2, 3, 4, 6],
-        "photoslibrari": [0, 2, 3, 6],
-        "json": [0, 1, 2, 4, 6],
-        "print": [0, 2, 3, 4, 6],
-        "output": [0, 2, 4, 5, 6],
-        "format": [0, 2, 4, 5, 6],
         "v": [0, 2],
-        "show": [1, 2, 3, 4, 6],
         "exit": [0, 2, 3, 4],
+        "print": [0, 2, 3, 4, 6],
         "inform": [0, 2, 3, 4, 5, 6],
         "includ": [0, 2, 3, 4, 5, 6],
         "licens": [0, 2],
-        "out": [0, 2, 6],
+        "miss": [0, 1, 3, 4],
+        "data": [0, 4, 5, 6],
+        "app": [0, 2, 4, 6],
+        "us": [0, 1, 2, 4, 5, 6],
+        "nearest": 0,
+        "neighbor": 0,
+        "thi": [0, 2, 3, 4, 5, 6],
+        "search": [0, 1, 2, 4, 6],
+        "ar": [0, 3, 4, 5, 6],
+        "look": [0, 2, 4, 6],
+        "within": [0, 5],
+        "given": [0, 4],
+        "window": [0, 4],
+        "time": [0, 2, 4, 5, 6],
+        "contain": [0, 3, 4, 5, 6],
+        "If": [0, 2, 3, 4, 5, 6],
+        "i": [0, 1, 3, 4, 5, 6],
         "found": [0, 2, 3, 4, 5, 6],
-        "": [0, 2, 4, 5, 6],
-        "compar": [0, 2, 4],
-        "two": [0, 2, 6],
-        "differ": [0, 2, 4, 6],
-        "To": [0, 2, 4, 5, 6],
+        "updat": [0, 1, 4, 5],
+        "For": [0, 4, 5, 6],
+        "exampl": [0, 1, 2, 4, 5],
         "you": [0, 2, 3, 4, 5, 6],
-        "ll": [0, 6],
-        "need": [0, 3, 4, 5, 6],
-        "sqldiff": 0,
-        "via": [0, 4, 6],
-        "homebrew": [0, 2],
-        "http": [0, 2, 4, 5, 6],
-        "brew": [0, 2],
-        "sh": [0, 2],
-        "alreadi": [0, 4, 6],
-        "when": [0, 4, 5, 6],
-        "current": [0, 4, 5, 6],
-        "most": [0, 6],
-        "recent": [0, 4],
-        "snapshot": [0, 2],
-        "osxphotos_snapshot": 0,
-        "directori": [0, 1, 3, 4, 5],
-        "just": [0, 3, 5, 6],
-        "db2": 0,
-        "both": [0, 2, 5, 6],
-        "see": [0, 4, 5, 6],
+        "took": [0, 3],
+        "pictur": [0, 2, 3, 4, 6],
+        "iphon": [0, 5, 6],
         "also": [0, 2, 3, 4, 5, 6],
-        "environ": [0, 2, 3],
-        "variabl": [0, 3, 4, 5],
-        "i": [0, 1, 3, 4, 5, 6],
-        "set": [0, 4, 5, 6],
-        "privat": 0,
-        "tmp": [0, 4],
-        "work": [0, 2, 4, 5, 6],
-        "onli": [0, 1, 2, 4, 5],
-        "sinc": [0, 6],
-        "catalina": [0, 5],
-        "10": [0, 2, 3, 5],
-        "15": [0, 2, 5],
-        "newer": 0,
-        "r": [0, 5],
-        "raw": [0, 4, 6],
-        "don": [0, 4, 6],
+        "camera": [0, 1, 4, 5],
+        "doesn": [0, 4, 6],
         "t": [0, 4, 5, 6],
-        "syntax": [0, 5, 6],
-        "highlight": 0,
-        "style": [0, 6],
-        "mai": [0, 3, 4, 5, 6],
-        "ani": [0, 2, 3, 4, 5, 6],
-        "valid": [0, 3, 4, 5, 6],
-        "pygment": 0,
-        "org": [0, 4, 5, 6],
-        "default": [0, 3, 4, 5, 6],
-        "monokai": 0,
-        "verbos": [0, 1, 4, 6],
-        "document": [0, 2, 4, 5],
-        "browser": [0, 2],
-        "all": [0, 1, 2, 3, 4, 5],
-        "associ": [0, 2, 4, 5, 6],
-        "from": [0, 1, 2, 3, 4, 5],
-        "delet": [0, 1, 4],
-        "folder": [0, 1, 3, 4, 5, 6],
-        "f": [0, 3, 4, 5],
-        "field": [0, 4, 5, 6],
-        "templat": [0, 1, 3, 4, 6],
-        "custom": [0, 3, 5, 6],
-        "name": [0, 1, 2, 3, 4, 5, 6],
-        "valu": [0, 4, 5, 6],
-        "repeat": [0, 6],
-        "multipl": [0, 5, 6],
-        "For": [0, 4, 5, 6],
-        "exampl": [0, 1, 2, 4, 5],
-        "titl": [0, 1, 3, 4, 5, 6],
-        "original_nam": [0, 5, 6],
-        "render": [0, 1, 4, 5, 6],
-        "string": [0, 4, 5, 6],
-        "each": [0, 4, 5, 6],
-        "stdout": 0,
-        "an": [0, 1, 3, 4, 5],
-        "thi": [0, 2, 3, 4, 5, 6],
-        "creat": [0, 1, 2, 3, 4, 5],
-        "report": [0, 1],
-        "etc": [0, 2, 4, 5, 6],
-        "regular": [0, 4, 5, 6],
-        "suppress": 0,
-        "ar": [0, 3, 4, 5, 6],
-        "previous": [0, 4, 6],
-        "file": [0, 1, 2, 3, 4, 5],
-        "updat": [0, 1, 4, 5],
-        "metadata": [0, 1, 2, 4, 5],
-        "did": [0, 6],
-        "now": [0, 2, 6],
-        "want": [0, 3, 4, 5, 6],
-        "do": [0, 2, 3, 4, 5, 6],
-        "so": [0, 4, 5, 6],
-        "simpli": [0, 6],
-        "re": [0, 4, 5, 6],
-        "becaus": [0, 6],
-        "detect": [0, 3, 4, 5],
         "have": [0, 3, 4, 5, 6],
-        "futur": [0, 5, 6],
-        "correctli": 0,
-        "unnecessarili": 0,
-        "export_directori": 0,
-        "config": [0, 4, 6],
-        "load": [0, 1, 3],
-        "configur": [0, 6],
-        "match": [0, 4, 5, 6],
-        "other": [0, 4, 5, 6],
-        "conjunct": [0, 6],
-        "thei": [0, 4, 6],
-        "overrid": [0, 5],
-        "correspond": [0, 4],
-        "config_fil": 0,
-        "written": [0, 4, 5, 6],
-        "save": [0, 1, 4],
-        "toml": [0, 6],
-        "exiftool_path": [0, 4],
-        "look": [0, 2, 4, 6],
-        "flag": [0, 4],
-        "pass": [0, 3, 4, 5, 6],
-        "m": [0, 4, 5],
-        "ignor": [0, 4, 6],
-        "minor": 0,
-        "warn": [0, 4],
-        "would": [0, 4, 5, 6],
-        "exiftool_pod": 0,
-        "html": 0,
-        "full": [0, 4, 5, 6],
-        "more": [0, 2, 3, 4, 5, 6],
-        "than": [0, 3, 4, 5, 6],
-        "one": [0, 4, 5, 6],
-        "e": [0, 2, 3, 4, 5, 6],
-        "g": [0, 2, 3, 4, 5, 6],
-        "merg": [0, 4, 6],
-        "origin": [0, 2, 3, 4, 5, 6],
-        "sidecar": [0, 1, 4],
-        "date": [0, 1, 2, 3, 4, 5],
-        "modifi": [0, 4, 5, 6],
-        "modif": [0, 4, 5, 6],
-        "exif": [0, 1, 3, 4, 5],
-        "modifyd": [0, 4],
-        "datetimeorigin": [0, 4],
-        "consist": 0,
-        "how": [0, 4, 5, 6],
-        "handl": [0, 6],
-        "tag": [0, 2, 4, 5, 6],
-        "imag": [0, 1, 2, 4, 5],
-        "form": [0, 4, 5, 6],
-        "same": [0, 2, 3, 4, 5, 6],
-        "add": [1, 4, 5, 6],
-        "contain": [0, 3, 4, 5, 6],
+        "can": [0, 2, 3, 4, 5, 6],
+        "taken": [0, 4, 6],
+        "from": [0, 1, 2, 3, 4, 5],
+        "those": [0, 3, 4, 6],
+        "mani": [0, 6],
         "could": [0, 3, 4, 5, 6],
-        "folder_album": [0, 4, 5, 6],
-        "year": [0, 1, 4, 5, 6],
-        "replac": [0, 4, 5, 6],
-        "below": [0, 4],
-        "By": [0, 6],
-        "exist": [0, 3, 4, 6],
-        "instead": [0, 4, 5, 6],
+        "some": [0, 4, 5, 6],
+        "manual": [0, 6],
+        "again": [0, 6],
+        "remain": 0,
+        "specifi": [0, 1, 2, 3, 4, 5],
+        "subset": [0, 4, 6],
+        "select": [0, 1, 2, 3, 4, 6],
+        "onli": [0, 1, 2, 4, 5],
         "ad": [0, 4, 5, 6],
-        "addit": [0, 3, 4, 5, 6],
-        "descript": [0, 1, 2, 3, 4, 5, 6],
-        "append": [0, 4, 5, 6],
-        "todai": [0, 5],
-        "descr": [0, 5, 6],
-        "locat": [1, 4, 6],
-        "report_fil": 0,
-        "write": [0, 4, 6],
-        "were": [0, 4, 6],
+        "after": [0, 4, 5, 6],
+        "2020": [0, 5, 6],
+        "01": [0, 3, 6],
+        "jan": 0,
+        "1": [0, 2, 4, 5, 6],
+        "etc": [0, 2, 4, 5, 6],
+        "all": [0, 1, 2, 3, 4, 5],
+        "2": [0, 2, 3, 4, 5],
+        "hour": [0, 5],
+        "hr": 0,
+        "verbos": [0, 1, 4, 6],
         "The": [0, 2, 3, 4, 5, 6],
-        "extens": [0, 4, 6],
-        "filenam": [0, 1, 3, 4, 5],
-        "determin": [0, 4, 6],
-        "csv": [0, 6],
-        "sqlite": [0, 3, 6],
-        "export_": 0,
-        "data": [0, 4, 5, 6],
-        "overwrit": [0, 1, 4],
-        "timestamp": 0,
-        "time": [0, 2, 4, 5, 6],
-        "stamp": 0,
+        "assum": [0, 4, 5],
+        "alreadi": [0, 4, 6],
+        "correct": [0, 4, 6],
+        "date": [0, 1, 2, 3, 4, 5],
+        "both": [0, 2, 5, 6],
+        "see": [0, 4, 5, 6],
+        "more": [0, 2, 3, 4, 5, 6],
+        "w": [0, 4],
+        "default": [0, 3, 4, 5, 6],
+        "format": [0, 2, 4, 5, 6],
+        "one": [0, 4, 5, 6],
+        "hh": 0,
+        "mm": [0, 5, 6],
+        "ss": 0,
+        "d": [0, 5],
+        "dai": [0, 5, 6],
+        "h": [0, 2, 4, 5],
+        "m": [0, 4, 5],
+        "minut": [0, 5, 6],
+        "min": [0, 5],
+        "": [0, 2, 4, 5, 6],
+        "second": [0, 3, 4, 5],
+        "sec": [0, 5],
+        "where": [0, 4, 5, 6],
         "dry": [0, 1, 4],
-        "mode": [0, 4, 6],
+        "don": [0, 4, 6],
         "actual": [0, 1, 4, 5],
-        "signatur": [0, 4, 6],
-        "color": [0, 1, 2],
-        "dark": [0, 6],
-        "light": 0,
-        "mono": 0,
-        "plain": [0, 6],
-        "depend": [0, 4, 5],
-        "requir": [0, 2, 4, 5, 6],
-        "dest": [0, 4],
-        "search": [0, 1, 2, 4, 6],
+        "just": [0, 3, 5, 6],
+        "what": [0, 1, 4, 5, 6],
+        "would": [0, 4, 5, 6],
+        "done": [0, 3, 4, 6],
+        "most": [0, 6],
+        "output": [0, 2, 4, 5, 6],
+        "mai": [0, 3, 4, 5, 6],
+        "multipl": [0, 5, 6],
+        "timestamp": 0,
+        "stamp": 0,
+        "than": [0, 3, 4, 5, 6],
         "treat": [0, 4, 5, 6],
-        "AND": [0, 4],
-        "edit": [1, 2, 3, 4, 5],
-        "live": [0, 1, 4, 5, 6],
-        "movi": [0, 1, 4, 6],
-        "burst": [0, 1, 4, 5],
-        "skip": [0, 3, 4, 6],
-        "behavior": [0, 4],
-        "progress": 0,
-        "displai": [0, 2, 4, 5],
-        "bar": [0, 3, 5],
-        "dure": [0, 1, 4],
         "OR": [0, 4],
+        "e": [0, 2, 3, 4, 5, 6],
+        "g": [0, 2, 3, 4, 5, 6],
+        "find": [0, 2, 3, 4, 5, 6],
+        "match": [0, 4, 5, 6],
+        "ani": [0, 2, 3, 4, 5, 6],
+        "folder": [0, 1, 3, 4, 5, 6],
+        "an": [0, 1, 3, 4, 5],
         "top": [0, 4, 6],
         "level": [0, 4, 6],
         "doe": [0, 3, 4, 5, 6],
         "subfold": [0, 1, 4, 5],
+        "name": [0, 1, 2, 3, 4, 5, 6],
+        "filenam": [0, 1, 3, 4, 5],
+        "thei": [0, 4, 6],
+        "repeat": [0, 6],
+        "file": [0, 1, 2, 3, 4, 5],
+        "load": [0, 1, 3],
         "singl": [0, 4, 5, 6],
         "per": 0,
         "preced": [0, 5, 6],
+        "ignor": [0, 4, 6],
+        "read": [0, 2, 4, 6],
+        "stdin": 0,
+        "titl": [0, 1, 3, 4, 5, 6],
+        "descript": [0, 1, 2, 3, 4, 5, 6],
         "desc": 0,
         "revers": [0, 4, 5, 6],
         "geoloc": [0, 4, 5, 6],
+        "associ": [0, 2, 4, 5, 6],
         "gp": [0, 6],
         "coordin": [0, 4, 6],
+        "imag": [0, 1, 2, 4, 5],
         "classif": [0, 2, 6],
         "5": [0, 2, 3, 4, 5],
         "uti": [0, 1, 4],
         "whose": 0,
         "uniform": [0, 4],
         "type": [0, 2, 3, 4, 5, 6],
         "identifi": [0, 4, 5, 6],
@@ -280,193 +158,384 @@
         "extern": [0, 1, 4, 5],
         "editor": [0, 4],
         "favorit": [0, 1, 4, 5, 6],
         "mark": [0, 4, 5, 6],
         "hidden": [0, 1, 4, 6],
         "share": [0, 1, 3, 4, 5, 6],
         "icloud": [0, 4, 6],
-        "taken": [0, 4, 6],
+        "burst": [0, 1, 4, 5],
+        "were": [0, 4, 6],
         "part": [0, 4, 5, 6],
+        "live": [0, 1, 4, 5, 6],
         "appl": [0, 2, 4, 5, 6],
         "portrait": [0, 1, 4, 5, 6],
+        "mode": [0, 4, 6],
         "screenshot": [0, 1, 4, 5, 6],
         "slow": [0, 4, 5, 6],
         "mo": [0, 4],
         "motion": [0, 4],
         "video": [0, 4, 5, 6],
         "laps": [0, 4],
         "hdr": [0, 1, 4, 5],
         "high": 0,
         "dynam": 0,
         "rang": [0, 4, 6],
         "selfi": [0, 1, 4, 5],
         "front": [0, 4],
         "face": [0, 2, 3, 4, 5, 6],
-        "camera": [0, 1, 4, 5],
         "panorama": [0, 1, 4, 5],
         "ha": [0, 3, 4, 5, 6],
+        "raw": [0, 4, 6],
         "jpeg": [0, 1, 4, 5],
+        "movi": [0, 1, 4, 6],
         "from_dat": [0, 1, 4],
         "item": [0, 4],
         "start": [0, 3, 4, 5, 6],
         "2000": 0,
-        "01": [0, 3, 6],
         "12t12": 0,
         "00": 0,
         "2001": 0,
         "07": [0, 3, 5],
         "12": [0, 2, 3],
         "31": [0, 6],
         "iso": [0, 4, 5],
         "8601": 0,
         "without": [0, 4, 5, 6],
         "timezon": [0, 2, 4],
         "to_dat": [0, 1, 4],
         "end": [0, 4, 5],
         "from_tim": [0, 4],
-        "dai": [0, 5, 6],
         "to_tim": [0, 4],
+        "year": [0, 1, 4, 5, 6],
         "specif": [0, 2, 4, 6],
         "2022": [0, 3],
         "befor": [0, 4, 5, 6],
-        "after": [0, 4, 5, 6],
         "librai": 0,
+        "last": [0, 2, 3, 4, 6],
         "time_delta": 0,
-        "where": [0, 4, 5, 6],
+        "string": [0, 4, 5, 6],
         "like": [0, 1, 3, 4, 5, 6],
-        "hr": 0,
         "1d": 0,
         "week": [0, 5, 6],
         "2week": 0,
         "month": [0, 1, 4, 5, 6],
         "7d": 0,
         "equival": 0,
-        "assum": [0, 4, 5],
         "30": 0,
         "365": 0,
         "common": [0, 6],
         "english": 0,
         "abbrevi": [0, 4, 5],
         "accept": 0,
-        "d": [0, 5],
-        "min": [0, 5],
-        "minut": [0, 5, 6],
         "comment": [0, 1, 3, 4, 5, 6],
         "refer": [0, 1, 5, 6],
         "referenc": [0, 4, 5],
         "copi": [0, 1, 3, 4, 6],
         "manag": [0, 2, 4, 6],
         "duplic": [0, 1, 3, 4, 5],
         "possibl": [0, 4, 6],
+        "compar": [0, 2, 4],
+        "signatur": [0, 4, 6],
         "evalu": [0, 3, 4, 5, 6],
+        "creat": [0, 1, 2, 3, 4, 5],
         "size": [0, 4, 5, 6],
         "height": [0, 1, 4],
         "width": [0, 1, 4],
         "statu": [0, 4],
         "byte": [0, 4],
         "nor": 0,
         "hash": [0, 4],
         "should": [0, 2, 4, 5, 6],
-        "within": [0, 5],
+        "origin": [0, 2, 3, 4, 5, 6],
+        "when": [0, 4, 5, 6],
         "integ": [0, 5],
         "si": 0,
         "nist": 0,
         "unit": [0, 5],
+        "follow": [0, 2, 3, 4, 5, 6],
+        "valid": [0, 3, 4, 5, 6],
         "1048576": 0,
         "048576mb": 0,
         "mib": 0,
         "max": 0,
+        "disk": [0, 1, 4],
+        "present": [0, 5],
+        "cloudasset": [0, 1, 4],
+        "incloud": [0, 1, 4],
+        "synch": [0, 4, 6],
+        "syndic": [0, 1, 4],
+        "via": [0, 4, 6],
+        "messag": [0, 2, 4],
+        "save": [0, 1, 4],
+        "moment": [0, 3, 4, 5],
         "regex": [0, 1, 4, 6],
+        "templat": [0, 1, 3, 4, 6],
+        "regular": [0, 4, 5, 6],
         "express": [0, 4, 5, 6],
         "begin": [0, 5],
         "beach": [0, 5],
-        "select": [0, 1, 2, 3, 4, 6],
+        "differ": [0, 2, 4, 6],
+        "argument": [0, 2, 3, 4, 5, 6],
         "filter": [0, 3, 4, 5, 6],
+        "current": [0, 4, 5, 6],
+        "exif": [0, 1, 3, 4, 5],
         "exif_tag": 0,
+        "valu": [0, 4, 5, 6],
+        "exist": [0, 3, 4, 6],
         "adob": 0,
         "photoshop": 0,
         "softwar": 0,
         "shot": 0,
         "canon": [0, 4],
         "make": [0, 3, 5, 6],
+        "tag": [0, 2, 4, 5, 6],
         "group": [0, 4, 5],
+        "To": [0, 2, 4, 5, 6],
         "must": [0, 4, 5, 6],
+        "path": [0, 1, 2, 3, 4, 5, 6],
         "eval": 0,
         "criteria": [0, 4, 6],
         "context": [0, 4],
         "python": [0, 1, 2, 5],
         "comprehens": [0, 6],
         "repres": [0, 4, 5],
         "photoinfo": [0, 1, 3, 4, 5],
         "object": [0, 3, 4, 5],
         "return": [0, 3, 4, 5],
+        "http": [0, 2, 4, 5, 6],
         "rhettbul": [0, 5],
         "github": [0, 5],
         "io": [0, 5],
+        "addit": [0, 3, 4, 5, 6],
+        "document": [0, 2, 4, 5],
         "class": [0, 3, 4, 5],
         "function": [0, 1, 3, 4, 5],
         "py": [0, 4, 5],
         "ve": [0, 4],
+        "want": [0, 3, 4, 5, 6],
         "call": [0, 2, 4, 5, 6],
+        "pass": [0, 3, 4, 5, 6],
         "expect": [0, 6],
+        "other": [0, 4, 5, 6],
         "com": [0, 4, 5],
         "blob": [0, 5],
         "master": [0, 5],
         "query_funct": 0,
-        "miss": [0, 1, 3, 4],
-        "download": [0, 4, 6],
+        "how": [0, 4, 5, 6],
+        "color": [0, 1, 2],
+        "dark": [0, 6],
+        "light": 0,
+        "mono": 0,
+        "plain": [0, 6],
+        "depend": [0, 4, 5],
+        "system": [0, 1, 4, 6],
+        "set": [0, 4, 5, 6],
+        "out": [0, 2, 6],
+        "photos_librari": [0, 2],
+        "db": [0, 2, 3, 4, 5, 6],
+        "photos_library_path": 0,
+        "provid": [0, 2, 4, 5, 6],
+        "attempt": [0, 2, 4, 6],
+        "order": [0, 2, 4, 5],
+        "open": [0, 2, 3, 5, 6],
+        "3": [0, 2, 3, 5, 6],
+        "photoslibrari": [0, 2, 3, 6],
+        "json": [0, 1, 2, 4, 6],
+        "metadata": [0, 1, 2, 4, 5],
+        "oper": [0, 1, 5, 6],
+        "california": 0,
+        "vacat": [0, 4, 5, 6],
+        "2023": 0,
+        "dd": [0, 5, 6],
+        "counter": [0, 5],
+        "03d": 0,
+        "famili": 0,
+        "travel": [0, 5, 6],
+        "02": [0, 5, 6],
+        "20": 0,
+        "001": 0,
+        "so": [0, 4, 5, 6],
+        "template_help": 0,
+        "html": 0,
+        "title_templ": 0,
+        "description_templ": [0, 1, 4],
+        "keyword_templ": [0, 1, 4],
+        "replac": [0, 4, 5, 6],
+        "latitud": [0, 4],
+        "longitud": [0, 4],
+        "pair": [0, 4, 5, 6],
+        "number": [0, 5, 6],
+        "90": 0,
+        "180": 0,
+        "chang": [0, 4, 5, 6],
+        "anyth": [0, 6],
+        "undo": 0,
+        "restor": 0,
+        "wa": [0, 4, 5, 6],
+        "prior": [0, 4],
+        "combin": [0, 5, 6],
+        "databas": [0, 2, 3, 4, 5, 6],
+        "either": [0, 2, 4, 5, 6],
+        "directli": [0, 2, 6],
+        "posit": [0, 2],
+        "neither": [0, 2, 4],
+        "two": [0, 2, 6],
+        "ll": [0, 6],
+        "need": [0, 3, 4, 5, 6],
+        "sqldiff": 0,
+        "homebrew": [0, 2],
+        "brew": [0, 2],
+        "sh": [0, 2],
+        "recent": [0, 4],
+        "snapshot": [0, 2],
+        "osxphotos_snapshot": 0,
+        "directori": [0, 1, 3, 4, 5],
+        "db2": 0,
+        "environ": [0, 2, 3],
+        "variabl": [0, 3, 4, 5],
+        "privat": 0,
+        "tmp": [0, 4],
+        "work": [0, 2, 4, 5, 6],
+        "sinc": [0, 6],
+        "catalina": [0, 5],
+        "10": [0, 2, 3, 5],
+        "15": [0, 2, 5],
+        "newer": 0,
+        "r": [0, 5],
+        "syntax": [0, 5, 6],
+        "highlight": 0,
+        "style": [0, 6],
+        "pygment": 0,
+        "org": [0, 4, 5, 6],
+        "monokai": 0,
+        "browser": [0, 2],
+        "note": [0, 4, 5, 6],
+        "deprec": 0,
+        "remov": [0, 1, 4, 5],
+        "futur": [0, 5, 6],
+        "releas": 0,
+        "instead": [0, 4, 5, 6],
+        "delet": [0, 1, 4],
+        "f": [0, 3, 4, 5],
+        "field": [0, 4, 5, 6],
+        "custom": [0, 3, 5, 6],
+        "original_nam": [0, 5, 6],
+        "render": [0, 1, 4, 5, 6],
+        "each": [0, 4, 5, 6],
+        "stdout": 0,
+        "report": [0, 1],
+        "suppress": 0,
+        "previous": [0, 4, 6],
+        "did": [0, 6],
+        "now": [0, 2, 6],
+        "do": [0, 2, 3, 4, 5, 6],
+        "simpli": [0, 6],
+        "re": [0, 4, 5, 6],
+        "becaus": [0, 6],
+        "detect": [0, 3, 4, 5],
+        "correctli": 0,
+        "unnecessarili": 0,
+        "export_directori": 0,
+        "config": [0, 4, 6],
+        "configur": [0, 6],
+        "conjunct": [0, 6],
+        "overrid": [0, 5],
+        "correspond": [0, 4],
+        "config_fil": 0,
+        "written": [0, 4, 5, 6],
+        "toml": [0, 6],
+        "exiftool_path": [0, 4],
+        "flag": [0, 4],
+        "minor": 0,
+        "warn": [0, 4],
+        "exiftool_pod": 0,
+        "full": [0, 4, 5, 6],
+        "merg": [0, 4, 6],
+        "sidecar": [0, 1, 4],
+        "modifi": [0, 4, 5, 6],
+        "modif": [0, 4, 5, 6],
+        "modifyd": [0, 4],
+        "datetimeorigin": [0, 4],
+        "consist": 0,
+        "handl": [0, 6],
+        "form": [0, 4, 5, 6],
+        "same": [0, 2, 3, 4, 5, 6],
+        "folder_album": [0, 4, 5, 6],
+        "below": [0, 4],
+        "By": [0, 6],
+        "append": [0, 4, 5, 6],
+        "todai": [0, 5],
+        "descr": [0, 5, 6],
+        "report_fil": 0,
+        "write": [0, 4, 6],
+        "extens": [0, 4, 6],
+        "determin": [0, 4, 6],
+        "csv": [0, 6],
+        "sqlite": [0, 3, 6],
+        "export_": 0,
+        "overwrit": [0, 1, 4],
+        "requir": [0, 2, 4, 5, 6],
+        "dest": [0, 4],
+        "AND": [0, 4],
+        "john": [0, 3],
+        "jane": 0,
+        "skip": [0, 3, 4, 6],
+        "behavior": [0, 4],
+        "progress": 0,
+        "displai": [0, 2, 4, 5],
+        "bar": [0, 3, 5],
+        "dure": [0, 1, 4],
         "new": [0, 2, 4, 6],
         "forc": [0, 4, 6],
-        "note": [0, 4, 5, 6],
         "unlik": [0, 5, 6],
-        "chang": [0, 4, 5, 6],
         "even": [0, 4, 6],
         "otherwis": [0, 3, 4, 5, 6],
         "trigger": [0, 4],
+        "error": [0, 4, 6],
+        "produc": [0, 4, 6],
+        "due": 0,
+        "bad": 0,
+        "successfulli": 0,
+        "gener": [0, 4, 6],
         "process": [0, 1, 3, 4, 5],
         "In": [0, 4, 5, 6],
         "normal": [0, 4, 6],
         "which": [0, 3, 4, 5, 6],
         "went": 0,
         "whether": 0,
-        "wa": [0, 4, 5, 6],
         "haven": 0,
         "limit": [0, 5, 6],
         "test": [0, 2, 3, 4, 6],
         "increment": [0, 1, 4, 5],
         "hardlink": [0, 1, 4],
         "them": [0, 4, 6],
         "cannot": [0, 4, 5],
         "embed": [0, 6],
         "apf": 0,
         "volum": [0, 6],
         "clone": 0,
         "give": 0,
-        "mani": [0, 6],
         "advantag": 0,
         "touch": [0, 4, 6],
         "caution": [0, 4],
         "collis": 0,
         "happen": [0, 5],
         "retri": [0, 6],
         "automat": [0, 5, 6],
         "up": [0, 4, 6],
-        "error": [0, 4, 6],
         "occur": [0, 4, 5],
         "network": [0, 4, 6],
         "drive": [0, 4, 6],
         "experi": 0,
         "intermitt": 0,
         "organ": [0, 6],
         "2019": [0, 6],
-        "20": 0,
         "photonam": [0, 6],
         "jpg": [0, 3, 4, 5, 6],
         "compon": 0,
-        "pair": [0, 4, 5, 6],
         "preview": [0, 1, 4, 5, 6],
         "renam": [0, 1, 4, 5, 6],
         "upon": [0, 4, 6],
         "had": [0, 6],
         "convert": [0, 1, 4, 5],
         "non": [0, 4, 6],
         "heic": 0,
@@ -480,34 +549,42 @@
         "machin": [0, 2, 4, 5, 6],
         "jpeg_qual": [0, 1, 4],
         "0": [0, 2, 3, 4, 5, 6],
         "A": [0, 5, 6],
         "best": [0, 4, 6],
         "maximum": [0, 4],
         "compress": [0, 4],
-        "gener": [0, 4, 6],
         "lower": [0, 4, 5, 6],
         "resolut": 0,
         "quickli": [0, 6],
         "suffix": [0, 4, 6],
         "photoname_preview": 0,
         "_low_r": 0,
         "photoname_low_r": 0,
         "_preview": [0, 4],
-        "multi": [0, 4, 5, 6],
         "permit": 0,
+        "download": [0, 4, 6],
         "implement": [0, 4, 5, 6],
         "applescript": [0, 4, 6],
         "interact": [0, 2, 3, 4],
-        "disk": [0, 1, 4],
         "internet": 0,
         "connect": [0, 1, 4, 6],
         "obvious": 0,
-        "synch": [0, 4, 6],
         "primari": [0, 4, 5],
+        "aae": [0, 4],
+        "adjust": [0, 1, 2, 4, 5, 6],
+        "detail": [0, 3, 4, 6],
+        "made": [0, 5],
+        "result": [0, 3, 4, 5, 6],
+        "back": [0, 4, 5, 6],
+        "succesfulli": 0,
+        "img_": 0,
+        "edited_vers": [0, 5],
+        "id": [0, 2, 4, 5],
+        "04d": 0,
         "xmp": [0, 4, 6],
         "digikam": [0, 6],
         "lightroom": [0, 6],
         "subject": [0, 4],
         "personinimag": [0, 4],
         "created": [0, 4],
         "gpslongitud": [0, 4],
@@ -518,16 +595,42 @@
         "j": [0, 4],
         "compat": [0, 6],
         "drop": [0, 4, 6],
         "photo_filenam": 0,
         "photo_ext": 0,
         "sidecar_ext": [0, 6],
         "img_1234": [0, 4, 6],
-        "result": [0, 3, 4, 5, 6],
         "mov": [0, 4],
+        "mako_template_fil": 0,
+        "sidecar_filename_templ": 0,
+        "write_skip": 0,
+        "strip_whitespac": 0,
+        "strip_lin": 0,
+        "user": [0, 1, 3, 4, 5],
+        "mako": 0,
+        "www": 0,
+        "makotempl": 0,
+        "being": [0, 4, 5, 6],
+        "sidecar_path": 0,
+        "pathlib": [0, 3, 4],
+        "photo_path": 0,
+        "filepath": [0, 3, 4, 6],
+        "boolean": [0, 4, 5, 6],
+        "true": [0, 3, 4, 5, 6],
+        "fals": [0, 4, 5, 6],
+        "ye": 0,
+        "indic": [0, 5],
+        "strip": [0, 1, 4, 5, 6],
+        "whitespac": [0, 4, 5, 6],
+        "blank": [0, 6],
+        "parent": [0, 1, 4],
+        "stem": 0,
+        "githubusercont": 0,
+        "main": [0, 3],
+        "custom_sidecar": 0,
         "imagedescript": [0, 4],
         "tagslist": [0, 4],
         "iptc": [0, 4, 5],
         "gpslatituderef": [0, 4],
         "gpslongituderef": [0, 4],
         "gpslatitud": [0, 4],
         "gpsposit": [0, 4],
@@ -551,81 +654,72 @@
         "copyright": [0, 6],
         "creator": 0,
         "findercom": [0, 6],
         "headlin": [0, 6],
         "particip": 0,
         "project": [0, 4, 5],
         "starrat": 0,
-        "detail": [0, 3, 4, 6],
-        "strip": [0, 1, 4, 5, 6],
         "lead": [0, 4, 6],
         "trail": [0, 6],
-        "whitespac": [0, 4, 5, 6],
         "space": [0, 5, 6],
-        "remov": [0, 1, 4, 5],
         "photoname_edit": 0,
         "_bearbeiten": 0,
         "photoname_bearbeiten": 0,
         "_edit": [0, 6],
         "_origin": 0,
         "filename_origin": 0,
         "photokit": [0, 4, 6],
         "direct": [0, 5],
         "highli": 0,
         "experiment": [0, 6],
         "alpha": 0,
         "featur": [0, 3, 4, 5, 6],
         "iterm2": 0,
         "termin": [0, 2, 6],
-        "app": [0, 2, 4, 6],
         "faster": [0, 4, 6],
         "reliabl": 0,
         "cleanup": 0,
         "subsequ": 0,
         "own": [0, 3, 5, 6],
         "script": [0, 3],
         "Be": 0,
         "sure": [0, 3, 6],
-        "what": [0, 1, 4, 5, 6],
         "intend": [0, 4, 6],
         "first": [0, 4, 5, 6],
         "certain": [0, 1, 5],
         "keep": [0, 6],
         "keep_path": 0,
         "prevent": 0,
-        "being": [0, 4, 5, 6],
         "wild": 0,
         "card": [0, 4, 5],
         "txt": [0, 6],
         "keepm": 0,
         "absolut": [0, 4],
         "rel": 0,
         "destin": [0, 3, 4],
         "enclos": [0, 5],
         "quot": [0, 5, 6],
         "shell": [0, 2, 3, 5, 6],
         "expand": [0, 4, 5, 6],
         "wildcard": 0,
         "kept": 0,
-        "doesn": [0, 4, 6],
         "know": [0, 4],
         "well": [0, 2, 3, 4, 5, 6],
         "larg": [0, 6],
         "post": [0, 1, 3],
         "categori": [0, 6],
         "exif_upd": [0, 4],
         "converted_to_jpeg": [0, 4],
         "sidecar_json_written": [0, 4],
         "sidecar_json_skip": [0, 4],
         "sidecar_exiftool_written": [0, 4],
         "sidecar_exiftool_skip": [0, 4],
         "sidecar_xmp_written": [0, 4],
         "sidecar_xmp_skip": [0, 4],
         "echo": [0, 3, 6],
-        "filepath": [0, 3, 4, 6],
         "shell_quot": [0, 5, 6],
         "export_dir": [0, 1, 4, 6],
         "exportdb_fil": 0,
         "altern": [0, 6],
         "store": [0, 4, 6],
         "state": [0, 1, 4, 5, 6],
         "osxphotos_export": [0, 6],
@@ -637,196 +731,227 @@
         "lose": [0, 6],
         "program": [0, 6],
         "interrupt": [0, 6],
         "crash": [0, 6],
         "tmpdir": [0, 1, 4],
         "dir": [0, 3, 4],
         "temporari": [0, 3, 4],
-        "number": [0, 5, 6],
-        "some": [0, 4, 5, 6],
         "particularli": 0,
+        "alt": 0,
+        "method": [0, 4],
+        "attach": [0, 6],
+        "storag": [0, 4, 6],
+        "na": [0, 6],
+        "devic": [0, 6],
+        "problem": 0,
+        "smb": 0,
+        "support": [0, 1, 5],
+        "preserv": [0, 6],
+        "filesystem": [0, 4, 6],
         "allow": [0, 2, 4, 5, 6],
         "complex": [0, 5, 6],
         "later": [0, 5],
         "reus": 0,
         "lot": 0,
         "here": [0, 6],
         "util": [0, 2, 4],
         "export_databas": 0,
         "vacuum": 0,
         "defrag": 0,
         "check": [0, 2],
         "file_path": 0,
         "run_id": 0,
-        "done": [0, 3, 4, 6],
         "didn": 0,
-        "second": [0, 3, 4, 5],
-        "prior": [0, 4],
         "migrat": 0,
         "sql": [0, 4],
         "sql_statement": 0,
         "execut": [0, 1, 4, 5, 6],
         "against": [0, 4, 6],
-        "parent": [0, 1, 4],
+        "move": [0, 6],
+        "comput": [0, 3, 4],
         "topic": 0,
         "subtop": 0,
         "album_templ": 0,
-        "title_templ": 0,
-        "description_templ": [0, 1, 4],
         "k": 0,
-        "keyword_templ": [0, 1, 4],
         "overwritten": 0,
         "l": 0,
-        "latitud": [0, 4],
-        "longitud": [0, 4],
-        "90": 0,
         "north": 0,
         "equat": 0,
         "neg": 0,
         "south": 0,
-        "180": 0,
         "east": 0,
         "prime": 0,
         "meridian": 0,
         "west": 0,
+        "p": [0, 3],
+        "pars": 0,
+        "date_pattern": 0,
+        "strptime": 0,
+        "pattern": [0, 6],
+        "describ": [0, 6],
+        "zone": 0,
+        "local": [0, 4, 5, 6],
+        "yet": [0, 4, 5, 6],
+        "img_1234_2022_11_23_12_34_56": 0,
+        "11": [0, 5],
+        "23": [0, 5],
+        "34": 0,
+        "56": 0,
+        "y_": 0,
+        "m_": 0,
+        "d_": 0,
+        "h_": 0,
+        "_": [0, 5, 6],
+        "further": [0, 6],
+        "narrow": 0,
+        "img_xxxx_": 0,
         "c": [0, 5],
         "clear": 0,
         "third": 0,
         "parti": 0,
-        "tool": [0, 6],
-        "support": [0, 1, 5],
-        "p": [0, 3],
         "relative_to_path": 0,
-        "comput": [0, 3, 4],
         "dup": 0,
         "split": [0, 5],
         "split_fold": [0, 4],
         "hierarch": [0, 4, 6],
         "charact": [0, 3, 5, 6],
-        "w": [0, 4],
         "walk": 0,
         "recurs": 0,
         "through": [0, 2, 6],
         "glob": 0,
         "unix": 0,
-        "pattern": [0, 6],
         "resum": [0, 6],
         "previou": [0, 1, 4],
-        "user": [0, 1, 3, 4, 5],
         "rhet": 0,
-        "local": [0, 4, 5, 6],
         "osxphotos_import": 0,
         "cancel": 0,
-        "anyth": [0, 6],
         "verifi": [0, 3, 6],
-        "correct": [0, 4, 6],
         "As": [0, 6],
         "press": 0,
         "ctrl": 0,
         "modern": 0,
         "kitti": 0,
         "text": [0, 4, 5, 6],
         "packag": [0, 1, 2],
         "u": [0, 4, 5],
         "upgrad": 0,
         "latest": 0,
         "export_path": [0, 3],
-        "present": [0, 5],
-        "cloudasset": [0, 1, 4],
-        "incloud": [0, 1, 4],
+        "count": [0, 4, 5],
         "quiet": 0,
         "debug": [0, 2, 4],
         "prototyp": 0,
         "emac": 0,
         "launch": 0,
         "keybind": 0,
         "vi": 0,
         "bind": 0,
-        "made": [0, 5],
         "avail": [0, 4, 5, 6],
         "python_fil": 0,
-        "h": [0, 2, 4, 5],
-        "messag": [0, 2, 4],
+        "uuid_or_nam": 0,
+        "12345678": 0,
+        "1234": 0,
+        "123456789012": 0,
+        "my": [0, 5, 6],
+        "root": 0,
+        "higher": 0,
         "entir": [0, 4, 6],
         "defin": [0, 3, 4, 5, 6],
+        "between": [0, 4, 5, 6],
+        "anoth": [0, 5, 6],
+        "ident": 0,
+        "sourc": [0, 1, 4],
+        "consid": 0,
+        "fingerprint": [0, 1, 4],
+        "ipad": 0,
+        "usb": 0,
+        "cabl": 0,
+        "imaz": 0,
+        "pleas": 0,
+        "me": 0,
+        "issu": 0,
+        "887": 0,
+        "togeth": [0, 5, 6],
+        "On": [0, 4],
+        "computer1": 0,
+        "computer2": 0,
+        "export_fil": 0,
+        "recommend": [0, 2, 6],
+        "though": 0,
+        "import_path": 0,
+        "properti": [0, 4, 5],
+        "comma": [0, 5, 6],
+        "separ": [0, 4, 5, 6],
+        "except": [0, 4],
+        "unmatch": [0, 4],
+        "update_": 0,
         "new_them": 0,
-        "adjust": [0, 1, 2, 4, 5, 6],
-        "oper": [0, 1, 5, 6],
         "smart": [0, 6],
         "view": 0,
         "overview": [0, 1],
         "yyyi": 0,
-        "mm": [0, 5, 6],
-        "dd": [0, 5, 6],
         "delta": 0,
-        "hh": 0,
-        "ss": 0,
         "fff": 0,
-        "hour": [0, 5],
-        "sec": [0, 5],
         "z": 0,
         "offset": [0, 4],
         "utc": [0, 4],
         "hhmm": 0,
         "mean": [0, 4, 5],
         "somewhat": [0, 6],
         "counterintuit": 0,
         "gmt": 0,
-        "02": [0, 5, 6],
         "ahead": [0, 4],
         "13": [0, 4],
         "old": 0,
         "exhibit": 0,
-        "manual": [0, 6],
         "get": [0, 2, 3, 4, 5, 6],
-        "window": [0, 4],
+        "itself": [0, 5, 6],
+        "scan": 0,
+        "midnight": 0,
         "push": 0,
         "pull": 0,
         "It": [0, 4, 5, 6],
         "might": [0, 4, 6],
         "thusli": 0,
         "unless": [0, 4, 5],
         "naiv": [0, 4],
         "datetim": [0, 1, 4],
         "timewarp_function_exampl": 0,
         "That": [0, 6],
         "wrong": 0,
         "while": [0, 5, 6],
-        "preserv": [0, 6],
-        "between": [0, 4, 5, 6],
         "usual": [0, 6],
         "abl": [0, 2, 6],
-        "those": [0, 3, 4, 6],
-        "o": [2, 3, 4],
-        "output_fil": [],
         "rich": [0, 1, 4, 6],
         "bypass": 0,
         "confirm": 0,
         "prompt": 0,
         "y": [0, 4, 5],
-        "ye": 0,
         "ask": 0,
         "uniqu": [0, 2, 4, 5],
-        "id": [0, 2, 4, 5],
         "suitabl": [0, 5],
         "usag": [0, 1, 3, 5],
         "instal": [1, 3, 4, 5, 6],
         "command": [1, 3, 4, 5],
         "line": [1, 3, 5, 6],
         "tutori": [1, 2],
         "export": [1, 2, 3, 4, 5],
         "structur": 1,
+        "edit": [1, 2, 3, 4, 5],
         "keyword": [1, 2, 3, 4, 5],
         "run": [1, 2, 4, 5],
         "theme": [1, 2],
         "conclus": 1,
         "interfac": [1, 2, 3, 4, 6],
         "cli": [1, 2],
         "about": [1, 2, 3, 4, 6],
+        "add": [1, 4, 5, 6],
+        "locat": [1, 4, 6],
         "album": [1, 2, 3, 4, 5, 6],
+        "batch": 1,
         "diff": [1, 2],
         "doc": [1, 2, 4],
         "dump": [1, 2],
         "exiftool": [1, 3, 4, 5, 6],
         "exportdb": [1, 4, 6],
         "help": [1, 2, 3, 5, 6],
         "import": [1, 3, 4, 5, 6],
@@ -835,32 +960,33 @@
         "label": [1, 2, 3, 4, 5, 6],
         "list": [1, 2, 3, 4, 5, 6],
         "orphan": 1,
         "person": [1, 2, 3, 4, 5, 6],
         "place": [1, 2, 4, 5, 6],
         "queri": [1, 2, 3, 4, 6],
         "repl": [1, 2],
+        "show": [1, 2, 3, 4, 6],
         "snap": [1, 2],
+        "sync": 1,
         "timewarp": [1, 2],
         "uninstal": [1, 2, 3],
         "uuid": [1, 2, 3, 4, 5],
         "version": [1, 2, 3, 4, 5, 6],
         "substitut": [1, 4],
         "code": [1, 2, 4, 5],
-        "api": [],
         "albuminfo": [1, 3, 4],
+        "asdict": [1, 4],
         "folder_list": [1, 4],
         "folder_nam": [1, 4],
         "photo_index": [1, 4],
         "sort_ord": [1, 4],
         "albumsortord": [1, 4],
         "commentinfo": [1, 4],
         "exifinfo": [1, 4],
         "addvalu": [1, 4],
-        "asdict": [1, 4],
         "pid": [1, 4],
         "run_command": [1, 4],
         "setvalu": [1, 4],
         "close": [1, 4, 5],
         "create_file_record": [1, 4],
         "create_or_get_file_record": [1, 4],
         "delete_data_for_filepath": [1, 4],
@@ -893,25 +1019,38 @@
         "live_photo": [1, 4, 5],
         "merge_exif_keyword": [1, 4],
         "merge_exif_person": [1, 4],
         "preview_suffix": [1, 4],
         "raw_photo": [1, 4],
         "render_opt": [1, 4],
         "replace_keyword": [1, 4],
+        "export_aa": [1, 4],
         "sidecar_drop_ext": [1, 4],
         "timeout": [1, 4],
         "touch_fil": [1, 4],
+        "update_error": [1, 4],
         "use_albums_as_keyword": [1, 4],
         "use_persons_as_keyword": [1, 4],
         "use_photos_export": [1, 4],
         "use_photokit": [1, 4],
         "favorite_r": [1, 4],
         "bit_flag": [1, 4],
         "exportresult": [1, 3, 4],
         "all_fil": [1, 4],
+        "faceinfo": [1, 4],
+        "center": [1, 4],
+        "face_rect": [1, 4],
+        "mpri_reg_rect": [1, 4],
+        "mwg_rs_area": [1, 4],
+        "person_info": [1, 4],
+        "pitch": [1, 4],
+        "roll": [1, 4, 6],
+        "roll_pitch_yaw": [1, 4],
+        "size_pixel": [1, 4],
+        "yaw": [1, 4],
         "fileutilnoop": [1, 4],
         "file_sig": [1, 4],
         "rmdir": [1, 4],
         "unlink": [1, 4],
         "utim": [1, 4],
         "folderinfo": [1, 4],
         "album_info": [1, 4],
@@ -921,24 +1060,28 @@
         "end_dat": [1, 4],
         "modification_d": [1, 4],
         "pk": [1, 4],
         "start_dat": [1, 4],
         "subtitl": [1, 4],
         "personinfo": [1, 4],
         "face_info": [1, 4],
+        "feature_less": [1, 4],
         "photoexport": [1, 3, 4],
         "exiftool_json_sidecar": [1, 4],
         "write_exiftool_metadata_to_fil": [1, 4],
+        "adjustments_path": [1, 4],
         "burst_album_info": [1, 4],
         "burst_album": [1, 4],
         "burst_default_pick": [1, 4],
         "burst_kei": [1, 4],
         "burst_photo": [1, 4],
         "burst_select": [1, 4],
+        "cloud_guid": [1, 4],
         "cloud_metadata": [1, 4],
+        "cloud_owner_hashed_id": [1, 4],
         "date_ad": [1, 4],
         "date_modifi": [1, 4],
         "date_trash": [1, 4],
         "detected_text": [1, 4, 5],
         "exif_info": [1, 4],
         "external_edit": [1, 4],
         "has_raw": [1, 4],
@@ -962,21 +1105,22 @@
         "original_width": [1, 4],
         "owner": [1, 4],
         "path_deriv": [1, 4],
         "path_edit": [1, 3, 4],
         "path_edited_live_photo": [1, 4],
         "path_live_photo": [1, 4],
         "path_raw": [1, 4],
-        "person_info": [1, 4],
         "project_info": [1, 4],
         "raw_origin": [1, 4],
         "render_templ": [1, 4],
+        "saved_to_librari": [1, 4],
         "score": [1, 3, 4, 5],
         "search_info": [1, 4],
         "search_info_norm": [1, 4],
+        "shared_mo": [1, 4],
         "slow_mo": [1, 4, 5],
         "time_laps": [1, 4, 5],
         "tzoffset": [1, 4],
         "uti_edit": [1, 4],
         "uti_origin": [1, 4],
         "uti_raw": [1, 4],
         "visibl": [1, 4],
@@ -1010,15 +1154,20 @@
         "get_photo": [1, 3, 4],
         "keywords_as_dict": [1, 3, 4],
         "labels_as_dict": [1, 4],
         "labels_normalized_as_dict": [1, 4],
         "library_path": [1, 3, 4],
         "persons_as_dict": [1, 3, 4],
         "photos_by_uuid": [1, 4],
+        "photos_vers": [1, 4],
         "placeinfo": [1, 3, 4],
+        "address": [1, 4, 5],
+        "address_str": [1, 4],
+        "country_cod": [1, 4, 5],
+        "ishom": [1, 4],
         "projectinfo": [1, 4],
         "queryopt": [1, 3, 4],
         "added_aft": [1, 4],
         "added_befor": [1, 4],
         "added_in_last": [1, 4],
         "deleted_onli": [1, 4],
         "has_com": [1, 4],
@@ -1034,14 +1183,15 @@
         "no_lik": [1, 4],
         "no_loc": [1, 4],
         "no_keyword": [1, 4],
         "no_plac": [1, 4],
         "no_titl": [1, 4],
         "not_burst": [1, 4],
         "not_cloudasset": [1, 4],
+        "not_edit": [1, 4],
         "not_favorit": [1, 4],
         "not_hdr": [1, 4],
         "not_hidden": [1, 4],
         "not_in_album": [1, 4],
         "not_incloud": [1, 4],
         "not_liv": [1, 4],
         "not_miss": [1, 4],
@@ -1050,74 +1200,73 @@
         "not_refer": [1, 4],
         "not_screenshot": [1, 4],
         "not_selfi": [1, 4],
         "not_shar": [1, 4],
         "not_slow_mo": [1, 4],
         "not_time_laps": [1, 4],
         "query_ev": [1, 4],
+        "not_synd": [1, 4],
+        "not_saved_to_librari": [1, 4],
+        "not_shared_mo": [1, 4],
         "scoreinfo": [1, 3, 4],
         "searchinfo": [1, 3, 4, 5],
         "activ": [1, 4, 5],
         "bodies_of_wat": [1, 4],
         "citi": [1, 4, 5],
         "countri": [1, 4, 5, 6],
         "holidai": [1, 4, 5],
         "locality_nam": [1, 4],
         "media_typ": [1, 4, 5],
         "neighborhood": [1, 4],
         "place_nam": [1, 4],
         "season": [1, 4, 5],
         "state_abbrevi": [1, 4],
         "street": [1, 4, 5],
+        "text_found": [1, 4],
         "venue_typ": [1, 4, 5],
         "venu": [1, 4, 5],
         "is_debug": [1, 4],
         "set_debug": [1, 4],
         "index": [1, 4, 5],
         "modul": [1, 4],
         "page": 1,
         "abil": 2,
         "veri": [2, 6],
         "flexibl": [2, 6],
         "easili": [2, 6],
         "aka": 2,
+        "o": [2, 3, 4],
         "x": [2, 4, 5],
         "sierra": 2,
         "6": [2, 5],
         "monterei": [2, 5],
-        "read": [0, 2, 4, 6],
         "vice": 2,
         "versa": 2,
         "8": [2, 4],
-        "recommend": [0, 2, 6],
         "wai": [2, 6],
         "pipx": [2, 3],
         "easiest": 2,
         "applic": [2, 6],
         "accord": 2,
         "instruct": [2, 6],
         "Then": [2, 6],
         "command_nam": 2,
         "simpl": 3,
         "def": 3,
-        "main": 3,
         "album_nam": 3,
         "foo": [3, 5],
-        "john": [0, 3],
         "smith": 3,
         "alic": 3,
         "__name__": 3,
         "__main__": 3,
-        "pathlib": [3, 4],
         "sy": 3,
         "click": 3,
         "pathvalid": 3,
         "is_valid_filepath": 3,
         "sanitize_filepath": 3,
-        "true": [3, 4, 5, 6],
         "unfil": 3,
         "none": [3, 4],
         "default_album": 3,
         "expandus": 3,
         "els": [3, 4, 6],
         "invalid": [3, 4],
         "platform": 3,
@@ -1139,16 +1288,14 @@
         "32": 3,
         "29": 3,
         "47": 3,
         "lock": 3,
         "6000": 3,
         "session": [3, 4, 5],
         "aesthet": [3, 5],
-        "moment": [0, 3, 4, 5],
-        "took": [0, 3],
         "18": 3,
         "54": 3,
         "31581": 3,
         "77": 3,
         "instanc": [3, 4, 6],
         "len": [3, 5],
         "all_photo": 3,
@@ -1163,18 +1310,18 @@
         "explor": [3, 6],
         "objexplor": 3,
         "q": 3,
         "quit": [3, 6],
         "programmat": 3,
         "pip": 3,
         "likewis": 3,
-        "sourc": [0, 1, 4],
-        "properti": [0, 4, 5],
-        "sub": [4, 5],
+        "__init__": 4,
+        "dict": 4,
         "empti": [4, 5, 6],
+        "sub": [4, 5],
         "sort": [4, 5],
         "qualnam": 4,
         "boundari": 4,
         "str": [4, 5],
         "ismin": 4,
         "bool": 4,
         "flash_fir": 4,
@@ -1195,48 +1342,41 @@
         "camera_model": [4, 5],
         "codec": 4,
         "lens_model": [4, 5],
         "large_file_support": 4,
         "basic": [4, 6],
         "paramet": 4,
         "success": 4,
-        "fals": [4, 5, 6],
         "self": 4,
         "delai": 4,
         "until": 4,
         "caller": 4,
         "ensur": [4, 6],
         "liter": [4, 6],
         "appear": 4,
         "tag_group": 4,
         "dictionari": 4,
-        "dict": 4,
         "kei": [4, 5, 6],
         "no_fil": 4,
         "errror": 4,
         "dbfile": 4,
         "sqlite3": 4,
-        "union": 4,
         "exportrecord": 4,
         "record": 4,
-        "given": [0, 4],
         "retriev": [4, 6],
         "tupl": 4,
         "track": [4, 6],
-        "struct": [],
         "target": 4,
         "config_data": 4,
         "pickl": 4,
         "gzip": 4,
-        "storag": [0, 4, 6],
         "renderopt": 4,
         "120": 4,
         "callabl": 4,
         "conform": 4,
-        "method": [0, 4],
         "relat": 4,
         "fileutilabc": 4,
         "variou": [4, 6],
         "fail": 4,
         "markup": 4,
         "bit": 4,
         "sidecar_xmp": 4,
@@ -1247,32 +1387,61 @@
         "deleted_directori": 4,
         "deleted_fil": 4,
         "exiftool_error": 4,
         "exiftool_warn": 4,
         "exported_album": 4,
         "metadata_chang": 4,
         "missing_album": 4,
+        "aae_written": 4,
+        "sidecar_user_written": 4,
+        "sidecar_user_skip": 4,
         "skipped_album": 4,
         "to_touch": 4,
         "xattr_skip": 4,
         "xattr_written": 4,
         "hold": [4, 5, 6],
+        "represent": [4, 5],
+        "pil": 4,
+        "rectangl": 4,
+        "frame": 4,
+        "x0": 4,
+        "x1": 4,
+        "y0": 4,
+        "y1": 4,
+        "left": [4, 6],
+        "corner": 4,
+        "en": 4,
+        "win32": 4,
+        "wic": 4,
+        "peopl": 4,
+        "area": [4, 5],
+        "starea": 4,
+        "stackexchang": 4,
+        "question": [4, 5],
+        "106410": 4,
+        "angl": 4,
+        "radian": 4,
+        "pixel": 4,
+        "around": [4, 5],
+        "center_x": 4,
+        "center_i": 4,
+        "circl": 4,
+        "drawn": 4,
         "No": [4, 6],
         "op": 4,
-        "except": [0, 4],
         "cmp": 4,
         "cmp_file_sig": 4,
         "file_cmp": 4,
         "mock": 4,
         "classmethod": 4,
         "src_file": 4,
         "dest_fil": 4,
         "compression_qu": 4,
         "src": 4,
-        "norsrc": [],
+        "shutil": 4,
         "succeed": 4,
         "rais": 4,
         "oserror": 4,
         "typeerror": 4,
         "file1": 4,
         "stat": 4,
         "f1": 4,
@@ -1280,85 +1449,84 @@
         "link": 4,
         "dirpath": 4,
         "prefix": 4,
         "temporarydirectori": 4,
         "secur": 4,
         "rule": 4,
         "mkdtemp": 4,
-        "On": [0, 4],
         "complet": [4, 6],
         "destruct": 4,
         "newli": 4,
         "its": [4, 5, 6],
         "content": 4,
-        "filesystem": [0, 4, 6],
         "access": [4, 5, 6],
         "moment_pk": 4,
         "stop": [4, 5],
-        "represent": [4, 5],
-        "faceinfo": [1, 4],
         "highest": 4,
         "lowest": 4,
         "n": [4, 5, 6],
+        "4": [4, 5, 6],
+        "less": [4, 5, 6],
+        "7": [4, 5],
         "build": 4,
         "send": 4,
         "captionabstract": 4,
         "objectnam": 4,
         "digitalcreationd": 4,
         "cr2": 4,
         "incorrect": [4, 5],
         "exportdbinmemori": 4,
         "respect": 4,
         "purpos": [4, 6],
         "slower": 4,
         "adjustmentsinfo": 4,
+        "shallow": 4,
+        "intern": [4, 5, 6],
         "stack": 4,
+        "guid": 4,
         "zcloudmastermediametadata": 4,
         "creation": [4, 5, 6],
         "awar": 4,
         "asset": [4, 5, 6],
         "long": 4,
         "confidence_threshold": 4,
         "75": [4, 5],
         "confid": [4, 5],
         "threshold": [4, 5],
         "text_detection_confidence_threshold": 4,
         "fall": 4,
-        "back": [0, 4, 5, 6],
         "earlier": 4,
         "exiftoolcach": 4,
         "log": [4, 6],
         "silent": 4,
-        "boolean": [4, 5, 6],
         "outsid": 4,
-        "pixel": 4,
         "digest": 4,
         "cloud": [4, 6],
-        "yet": [0, 4, 5, 6],
         "asynchroun": 4,
         "immedi": [4, 6],
         "particular": 4,
         "notic": 4,
         "someth": [4, 6],
         "exact": 4,
         "mysteri": 4,
         "storat": 4,
         "still": [4, 6],
+        "indent": 4,
         "categor": [4, 5],
         "older": 4,
         "degre": 4,
         "belong": [4, 6],
         "mangl": 4,
         "files": 4,
         "deriv": 4,
         "largest": 4,
         "template_str": 4,
-        "unmatch": [0, 4],
         "rendered_str": 4,
-        "produc": [0, 4, 6],
+        "tabl": 4,
+        "photot": 4,
         "public": [4, 5],
         "visbl": 4,
         "enforc": 4,
         "valueerror": 4,
         "predic": [4, 5],
         "subfield": [4, 5],
         "field_arg": [4, 5],
@@ -1367,32 +1535,77 @@
         "media": [4, 5, 6],
         "attr": 4,
         "bool_val": 4,
         "lookup": [4, 6],
         "delim": [4, 5],
         "delimit": [4, 5],
         "path_sep": 4,
-        "separ": [0, 4, 5, 6],
         "model": [4, 5],
         "photoscript": 4,
         "_skip_searchinfo": 4,
         "extract": [4, 5],
-        "4": [4, 5, 6],
-        "count": [0, 4, 5],
         "descend": 4,
         "initi": 4,
         "liglob": 4,
-        "tabl": 4,
-        "statement": [4, 5, 6],
+        "param": 4,
         "cursor": 4,
+        "statement": [4, 5, 6],
         "wed": 4,
-        "vacat": [0, 4, 5, 6],
         "aren": 4,
         "regardless": 4,
         "suppli": 4,
+        "postaladdress": 4,
+        "namedtupl": 4,
+        "postal": [4, 5],
+        "postal_cod": [4, 5],
+        "sub_administrative_area": 4,
+        "sub_loc": 4,
+        "iso_country_cod": 4,
+        "gb": 4,
+        "home": [4, 6],
+        "algorithm": [4, 5, 6],
+        "shown": 4,
+        "placenam": 4,
+        "zero": [4, 5],
+        "ascend": 4,
+        "area_of_interest": [4, 5],
+        "gulf": 4,
+        "island": 4,
+        "nation": 4,
+        "seashor": 4,
+        "santa": 4,
+        "rosa": 4,
+        "knott": 4,
+        "berri": 4,
+        "farm": 4,
+        "With": [4, 6],
+        "body_of_wat": 4,
+        "clplacemark": 4,
+        "coreloc": 4,
+        "placemark": 4,
+        "state_provinc": [4, 5],
+        "administrativearea": 4,
+        "provinc": [4, 5],
+        "administr": 4,
+        "additional_city_info": 4,
+        "subloc": 4,
+        "ocean": 4,
+        "areasofinterest": 4,
+        "relev": 4,
+        "interest": [4, 5, 6],
+        "inland_wat": 4,
+        "inland": 4,
+        "water": 4,
+        "bodi": 4,
+        "geograph": 4,
+        "sub_throughfar": 4,
+        "street_address": 4,
+        "throughfar": 4,
+        "union": 4,
+        "reserv": 4,
         "calendar": [4, 5],
         "slideshow": [4, 5],
         "timedelta": 4,
         "iter": 4,
         "bitmath": 4,
         "minimum": 4,
         "overal": [4, 5],
@@ -1418,35 +1631,32 @@
         "sharply_focused_subject": 4,
         "tastefully_blur": 4,
         "well_chosen_subject": 4,
         "well_framed_subject": 4,
         "well_timed_shot": 4,
         "term": [4, 6],
         "learn": [4, 5, 6],
-        "bodi": 4,
-        "water": 4,
         "town": 4,
+        "safar": 4,
         "languag": 5,
         "simplest": 5,
         "template_field": 5,
         "resolv": 5,
         "pretext": 5,
         "condit": [5, 6],
         "bool_valu": 5,
         "posttext": 5,
         "white": 5,
         "sensit": 5,
         "tab": 5,
         "free": [5, 6],
-        "my": [0, 5, 6],
         "foobar": 5,
         "vertic": 5,
         "pipe": 5,
         "symbol": 5,
-        "combin": [0, 5, 6],
         "capit": 5,
         "paren": 5,
         "upper": 5,
         "titlecas": 5,
         "word": 5,
         "brace": [5, 6],
         "curli": [5, 6],
@@ -1454,174 +1664,161 @@
         "bracket": 5,
         "safe": 5,
         "function_nam": 5,
         "template_filt": 5,
         "value1": 5,
         "value2": 5,
         "autosplit": 5,
-        "comma": [0, 5, 6],
         "semicolon": 5,
         "chop": 5,
         "off": 5,
-        "travel": [0, 5, 6],
         "trave": 5,
         "beac": 5,
         "chomp": 5,
         "alu": 5,
         "ravel": 5,
         "b": 5,
         "rsort": 5,
         "uniq": 5,
         "similar": 5,
-        "togeth": [0, 5, 6],
         "abc": 5,
         "prepend": 5,
+        "tring": 5,
+        "bd": 5,
+        "cd": 5,
+        "da": 5,
+        "dc": 5,
         "slice": 5,
         "step": 5,
         "semant": 5,
         "sslice": 5,
-        "tring": 5,
         "abcd": 5,
         "bc": 5,
-        "bd": 5,
         "event": [5, 6],
         "point": 5,
         "album1": 5,
         "folder1": [5, 6],
         "folder1album1": 5,
-        "anoth": [0, 5, 6],
         "take": [5, 6],
         "negat": 5,
         "comparison": 5,
         "exactli": [5, 6],
         "partial": 5,
         "startswith": [5, 6],
         "endswith": 5,
-        "less": [4, 5, 6],
         "equal": 5,
         "greater": 5,
         "bare": 5,
         "unquot": 5,
         "phrase": 5,
-        "itself": [0, 5, 6],
         "beachdai": 5,
-        "7": [4, 5],
         "Not": 5,
         "imagenam": 5,
         "unmodifi": 5,
         "abov": [5, 6],
         "ishdr": 5,
         "nothdr": 5,
         "strftime": 5,
-        "_": [0, 5, 6],
         "februari": 5,
-        "2020": [0, 5, 6],
         "19": 5,
         "38": 5,
         "04": [5, 6],
         "190738": 5,
         "vid\u00e9o": 5,
         "vid\u00e9o_acc\u00e9l\u00e9r\u00e9": 5,
         "openbrac": 5,
         "closebrac": 5,
         "var": 5,
         "prohibit": 5,
-        "around": [4, 5],
         "kati": 5,
         "percent": 5,
         "sign": 5,
         "escap": 5,
         "photo_or_video": 5,
         "foto": 5,
         "value_if_tru": 5,
         "value_if_fals": 5,
-        "edited_vers": [0, 5],
         "03": 5,
         "22": 5,
         "digit": [5, 6],
         "yy": 5,
-        "zero": [4, 5],
         "pad": 5,
         "mon": 5,
         "dow": 5,
         "doi": 5,
         "julian": 5,
-        "23": [0, 5],
         "null": [5, 6],
-        "country_cod": [1, 4, 5],
-        "state_provinc": [4, 5],
-        "provinc": [4, 5],
-        "area_of_interest": [4, 5],
-        "area": [4, 5],
-        "interest": [4, 5, 6],
         "landmark": 5,
-        "address": [1, 4, 5],
-        "postal": [4, 5],
         "2007": 5,
         "18th": 5,
         "st": 5,
         "nw": 5,
         "washington": 5,
-        "dc": 5,
         "20009": 5,
-        "postal_cod": [4, 5],
         "summer": [5, 6],
-        "algorithm": [4, 5, 6],
-        "iphon": [0, 5, 6],
         "15mm": 5,
-        "intern": [4, 5, 6],
         "univers": 5,
         "128fb4c6": 5,
         "0b16": 5,
         "4e7d": 5,
         "9108": 5,
         "fb2e90da1546": 5,
         "shortuuid": 5,
         "shorter": 5,
         "jysxugp9ujetmcbbchxcmu": 5,
         "sequenti": 5,
         "05d": 5,
         "00001": 5,
         "00002": 5,
         "00003": 5,
+        "starting_valu": 5,
+        "caus": [5, 6],
+        "reset": 5,
+        "valuewhen": 5,
+        "reach": 5,
+        "byth": 5,
+        "thestop": 5,
+        "omit": 5,
+        "countfrom": 5,
+        "arbitrari": 5,
+        "namepreced": 5,
+        "period": [5, 6],
+        "stateand": 5,
         "album_seq": 5,
-        "indic": 5,
         "sequenc": 5,
         "seq": 5,
-        "starting_valu": 5,
         "00000": 5,
         "0001": 5,
         "folder_album_seq": 5,
         "questionmark": 5,
-        "question": [4, 5],
         "openparen": 5,
         "closeparen": 5,
         "openbracket": 5,
         "closebracket": 5,
         "newlin": [5, 6],
         "lf": 5,
         "feed": 5,
         "alia": 5,
         "cr": 5,
         "carriag": 5,
         "crlf": 5,
         "rn": 5,
         "osxphotos_vers": 5,
+        "61": 5,
         "osxphotos_cmd_lin": 5,
         "greet": 5,
         "album_project": 5,
         "folder_album_project": 5,
         "assign": [5, 6],
         "label_norm": 5,
         "christma": 5,
         "sport": 5,
         "restaur": 5,
         "knowledg": 5,
         "underli": 5,
-        "caus": [5, 6],
         "built": 5,
         "down": [5, 6],
         "cach": 5,
         "reprocess": 5,
         "colon": 5,
         "thing": [5, 6],
         "1f": 5,
@@ -1642,34 +1839,31 @@
         "sever": 6,
         "focu": 6,
         "probabl": 6,
         "thousand": 6,
         "isn": 6,
         "2021": 6,
         "21": 6,
-        "With": [4, 6],
         "2015": 6,
         "05": 6,
         "prefer": 6,
         "wide": 6,
         "throughout": 6,
         "worth": 6,
         "interpret": 6,
         "almost": 6,
         "known": 6,
         "Of": 6,
         "cours": 6,
         "underscor": 6,
-        "further": [0, 6],
         "under": 6,
         "often": 6,
         "dsc05678": 6,
         "dng": 6,
         "caption": 6,
-        "blank": 6,
         "logic": 6,
         "everi": 6,
         "crop": 6,
         "distinguish": 6,
         "img_1234_edit": 6,
         "april": 6,
         "img_1234_2021": 6,
@@ -1686,76 +1880,67 @@
         "optim": 6,
         "alwai": 6,
         "encount": 6,
         "commun": 6,
         "buggi": 6,
         "restart": 6,
         "There": 6,
-        "attach": [0, 6],
-        "na": [0, 6],
-        "devic": [0, 6],
         "unreli": 6,
         "flaki": 6,
         "decreas": 6,
         "dbpath": 6,
         "put": 6,
-        "home": [4, 6],
         "rememb": 6,
         "ram": 6,
         "much": 6,
         "offer": 6,
         "signific": 6,
         "boost": 6,
         "tremend": 6,
         "amount": 6,
         "nativ": 6,
         "capabl": 6,
         "howev": 6,
         "websit": 6,
-        "again": [0, 6],
         "classic": 6,
         "folder2": 6,
         "power": 6,
         "classifi": 6,
         "think": 6,
         "oppos": 6,
         "mykeyword": 6,
         "insert": 6,
         "never": 6,
         "desir": 6,
         "nolabel": 6,
         "carri": 6,
         "photopr": 6,
         "manner": 6,
-        "period": [5, 6],
         "backup": 6,
         "rather": 6,
         "won": 6,
         "dot": 6,
         "intent": 6,
         "workflow": 6,
         "involv": 6,
-        "move": [0, 6],
         "maintain": 6,
         "decid": 6,
         "excel": 6,
         "And": 6,
         "cover": 6,
         "50": 6,
         "better": 6,
         "understand": 6,
         "matter": 6,
-        "subset": [0, 4, 6],
         "certainli": 6,
         "insid": 6,
         "2018": 6,
         "28": 6,
         "worst": 6,
-        "9": [5, 6],
-        "describ": [0, 6],
+        "9": 6,
         "section": 6,
         "varieti": 6,
         "titlen": 6,
         "ndescript": 6,
         "advanc": 6,
         "explan": 6,
         "noth": 6,
@@ -1777,508 +1962,35 @@
         "bin": 6,
         "integr": 6,
         "concept": 6,
         "discuss": 6,
         "thank": 6,
         "philipp": 6,
         "contribut": 6,
-        "roll": [1, 4, 6],
         "basi": 6,
         "ot": 6,
         "rise": 6,
         "nevertheless": 6,
         "good": 6,
         "cut": 6,
         "pro": 6,
         "pick": 6,
-        "left": [4, 6],
         "chose": 6,
         "quik": 6,
         "spot": 6,
         "gopro": 6,
         "popul": 6,
         "enabl": 6,
         "desktop": 6,
         "legibl": 6,
         "suit": 6,
         "mere": 6,
         "spend": 6,
         "few": 6,
-        "kind": 6,
-        "alt": 0,
-        "problem": 0,
-        "smb": 0,
-        "pars": 0,
-        "date_pattern": 0,
-        "strptime": 0,
-        "zone": 0,
-        "img_1234_2022_11_23_12_34_56": 0,
-        "11": [0, 5],
-        "34": 0,
-        "56": 0,
-        "y_": 0,
-        "m_": 0,
-        "d_": 0,
-        "h_": 0,
-        "img_": 0,
-        "narrow": 0,
-        "img_xxxx_": 0,
-        "55": [],
-        "jane": 0,
-        "due": 0,
-        "bad": 0,
-        "successfulli": 0,
-        "update_error": [1, 4],
-        "ident": 0,
-        "consid": 0,
-        "fingerprint": [0, 1, 4],
-        "ipad": 0,
-        "usb": 0,
-        "cabl": 0,
-        "imaz": 0,
-        "pleas": 0,
-        "me": 0,
-        "issu": 0,
-        "887": 0,
-        "computer1": 0,
-        "computer2": 0,
-        "export_fil": 0,
-        "though": 0,
-        "import_path": 0,
-        "update_": 0,
-        "sync": 1,
-        "nearest": 0,
-        "neighbor": 0,
-        "remain": 0,
-        "jan": 0,
-        "photos_vers": [1, 4],
-        "text_found": [1, 4],
-        "safar": 4,
-        "feature_less": [1, 4],
-        "param": 4,
-        "not_edit": [1, 4],
-        "__init__": 4,
-        "counter": [0, 5],
-        "reset": 5,
-        "reach": 5,
-        "omit": 5,
-        "arbitrari": 5,
-        "valuewhen": 5,
-        "byth": 5,
-        "thestop": 5,
-        "countfrom": 5,
-        "namepreced": 5,
-        "stateand": 5,
-        "deprec": 0,
-        "releas": 0,
-        "57": [],
-        "stdin": 0,
-        "uuid_or_nam": 0,
-        "12345678": 0,
-        "1234": 0,
-        "123456789012": 0,
-        "higher": 0,
-        "helper": [],
-        "mirror": [],
-        "distribut": [],
-        "query_command": [],
-        "decor": [],
-        "turn": [],
-        "fledg": [],
-        "conveni": [],
-        "sampl": [],
-        "cli_example_1": [],
-        "quick": [],
-        "addition": [],
-        "incorpor": [],
-        "whatev": [],
-        "cli_example_2": [],
-        "__future__": [],
-        "annot": [],
-        "kwarg": [],
-        "docstr": [],
-        "vv": [],
-        "abort": [],
-        "exit_cod": [],
-        "echo_error": [],
-        "stderr": [],
-        "logger": [],
-        "kvstore": [],
-        "sqlitekvstor": [],
-        "textual": [],
-        "no_chang": [],
-        "num": [],
-        "tz": [],
-        "simpler": [],
-        "is_flag": [],
-        "palletsproject": [],
-        "persist": [],
-        "kv": [],
-        "continu": [],
-        "serial": [],
-        "isoformat": [],
-        "accordingli": [],
-        "emoji": [],
-        "stand": [],
-        "selection_command": [],
-        "filenotfounderror": [],
-        "held": [],
-        "switch": [],
-        "therefor": [],
-        "explicit": [],
-        "fulli": [],
-        "qualifi": [],
-        "resid": [],
-        "thousdand": [],
-        "libari": [],
-        "who": [],
-        "shouldn": [],
-        "birthdai": [],
-        "juan": [],
-        "rodriguez": [],
-        "maria": [],
-        "ski": [],
-        "trip": [],
-        "osmnio5sqfgztbj9wrydrb": [],
-        "complic": [],
-        "programmaticali": [],
-        "kid": [],
-        "photos1": [],
-        "photos2": [],
-        "photos3": [],
-        "gui": [],
-        "sai": [],
-        "386": [],
-        "474": [],
-        "25": [],
-        "002": [],
-        "609": [],
-        "similarli": [],
-        "625": [],
-        "151": [],
-        "25002": [],
-        "5609": [],
-        "19393": [],
-        "shared_movi": [],
-        "keyword_dict": [],
-        "ie": [],
-        "persons_dict": [],
-        "albums_dict": [],
-        "albums_shared_dict": [],
-        "peopl": 4,
-        "dog": [],
-        "easier": [],
-        "conn": [],
-        "zuuid": [],
-        "zgenericasset": [],
-        "zfavorit": [],
-        "fetchal": [],
-        "row": [],
-        "individu": [],
-        "presum": [],
-        "element": [],
-        "f19e06b8": [],
-        "a712": [],
-        "4b5c": [],
-        "907a": [],
-        "c007d37bda16_1_101_o": [],
-        "c007d37bda16_1_102_o": [],
-        "c007d37bda16_1_105_c": [],
-        "unadjustednonraw_mini_6": [],
-        "unadjustednonraw_thumb_6": [],
-        "y6oofykbr96spbs6xgwoqw_mini_1": [],
-        "decod": [],
-        "is_raw": [],
-        "upload": [],
-        "unmount": [],
-        "img_9851": [],
-        "img_9853": [],
-        "img_9852": [],
-        "img_9854": [],
-        "img_9855": [],
-        "unselect": [],
-        "technic": [],
-        "teturn": [],
-        "phone": [],
-        "recogn": [],
-        "ealier": [],
-        "lowercas": [],
-        "typic": [],
-        "At": [],
-        "get_exiftool_path": [],
-        "composit": [],
-        "9188916666667": [],
-        "138": [],
-        "596861111111": [],
-        "images": [],
-        "2754": [],
-        "2017": [],
-        "06": [],
-        "17": [],
-        "lensmak": [],
-        "lensmodel": [],
-        "elder": [],
-        "park": [],
-        "speed": [],
-        "reflect": [],
-        "practic": [],
-        "advers": [],
-        "behav": [],
-        "fast": [],
-        "identif": [],
-        "approach": [],
-        "robust": [],
-        "enough": [],
-        "menu": [],
-        "twice": [],
-        "reli": [],
-        "correl": [],
-        "across": [],
-        "happili": [],
-        "alreai": [],
-        "associt": [],
-        "stem": [],
-        "photo_nam": [],
-        "none_str": [],
-        "mtl": [],
-        "regard": [],
-        "engin": [],
-        "sep": [],
-        "expand_inplac": [],
-        "inplace_sep": [],
-        "sanit": [],
-        "dirnam": [],
-        "evalut": [],
-        "resembl": [],
-        "notabl": [],
-        "henc": [],
-        "why": [],
-        "famili": 0,
-        "_constant": [],
-        "vision": [],
-        "framework": [],
-        "circa": [],
-        "2013": [],
-        "macbook": [],
-        "memoiz": [],
-        "photosinfo": [],
-        "nikon_photo": [],
-        "nikon": [],
-        "earliest": [],
-        "albuminfold": [],
-        "subfolder2": [],
-        "illustr": [],
-        "subfolder1": [],
-        "bega": [],
-        "projcet_info": [],
-        "plugin": [],
-        "enum": [],
-        "unknown": [],
-        "newest_first": [],
-        "oldest_first": [],
-        "effect": [],
-        "children": [],
-        "0x10fcc0160": [],
-        "shown": 4,
-        "mayfair": [],
-        "shop": [],
-        "centr": [],
-        "victoria": [],
-        "canada": [],
-        "vancouv": [],
-        "island": 4,
-        "british": [],
-        "columbia": [],
-        "placenam": 4,
-        "namedtupl": 4,
-        "ascend": 4,
-        "gulf": 4,
-        "nation": 4,
-        "seashor": 4,
-        "santa": 4,
-        "rosa": 4,
-        "knott": 4,
-        "berri": 4,
-        "farm": 4,
-        "body_of_wat": 4,
-        "clplacemark": 4,
-        "reserv": 4,
-        "placemark": 4,
-        "administrativearea": 4,
-        "sub_administrative_area": 4,
-        "administr": 4,
-        "additional_city_info": 4,
-        "subloc": 4,
-        "ocean": 4,
-        "areasofinterest": 4,
-        "relev": 4,
-        "inland_wat": 4,
-        "inland": 4,
-        "geograph": 4,
-        "sub_throughfar": 4,
-        "street_address": 4,
-        "throughfar": 4,
-        "gb": 4,
-        "2038": [],
-        "postaladdress": 4,
-        "sub_loc": 4,
-        "iso_country_cod": 4,
-        "3700": [],
-        "wailea": [],
-        "alanui": [],
-        "dr": [],
-        "kihei": [],
-        "maui": [],
-        "hi": [],
-        "96753": [],
-        "expos": [],
-        "food": [],
-        "best_food_photo": [],
-        "lambda": [],
-        "municip": [],
-        "witht": [],
-        "photoo": [],
-        "thumbnail": [],
-        "shortcut": [],
-        "metdata": [],
-        "mwg": [],
-        "starea": 4,
-        "rectangl": 4,
-        "mpri": [],
-        "corner": 4,
-        "x0": 4,
-        "y0": 4,
-        "x1": 4,
-        "y1": 4,
-        "rectangular": [],
-        "frame": 4,
-        "pillow": [],
-        "pathedit": [],
-        "diamet": [],
-        "radian": 4,
-        "center_x": 4,
-        "center_i": 4,
-        "measur": [],
-        "source_width": [],
-        "source_height": [],
-        "has_smil": [],
-        "face_typ": [],
-        "age_typ": [],
-        "eye_makeup_typ": [],
-        "eye_st": [],
-        "facial_hair_typ": [],
-        "gender_typ": [],
-        "glasses_typ": [],
-        "hair_color_typ": [],
-        "lip_makeup_typ": [],
-        "smile_typ": [],
-        "adjus": [],
-        "plist": [],
-        "undecod": [],
-        "binari": [],
-        "bundl": [],
-        "format_id": [],
-        "base_vers": [],
-        "format_vers": [],
-        "adj_metadata": [],
-        "adj_orient": [],
-        "adj_format_vers": [],
-        "adj_version_info": [],
-        "extra": [],
-        "img_0001": [],
-        "img_001": [],
-        "latter": [],
-        "denot": [],
-        "icon": [],
-        "superimpos": [],
-        "simplifi": [],
-        "deal": [],
-        "struggl": [],
-        "suggest": [],
-        "all_raw": [],
-        "availab": [],
-        "exifdict": [],
-        "keyword1": [],
-        "keyword2": [],
-        "keyword3": [],
-        "largefilesupport": [],
-        "significantli": [],
-        "subprocess": [],
-        "stay_open": [],
-        "background": [],
-        "clean": [],
-        "singleton": [],
-        "tmpfile": [],
-        "avoid": [],
-        "unnecessari": [],
-        "osxmetadata": [],
-        "xarg": [],
-        "creation_d": [],
-        "ishom": [1, 4],
-        "address_str": [1, 4],
-        "display_nam": [],
-        "keyphoto": [],
-        "facecount": [],
-        "asset_uuid": [],
-        "mwg_rs_area": [1, 4],
-        "mpri_reg_rect": [1, 4],
-        "face_rect": [1, 4],
-        "center": [1, 4],
-        "size_pixel": [1, 4],
-        "roll_pitch_yaw": [1, 4],
-        "pitch": [1, 4],
-        "yaw": [1, 4],
-        "get_system_library_path": [],
-        "get_last_library_path": [],
-        "list_photo_librari": [],
-        "cloud_guid": [1, 4],
-        "cloud_owner_hashed_id": [1, 4],
-        "guid": 4,
-        "root": 0,
-        "california": 0,
-        "2023": 0,
-        "03d": 0,
-        "001": 0,
-        "template_help": 0,
-        "undo": 0,
-        "restor": 0,
-        "scan": 0,
-        "midnight": 0,
-        "batch": 1,
-        "58": [],
-        "cd": 5,
-        "da": 5,
-        "59": [],
-        "indent": 4,
-        "shallow": 4,
-        "shutil": 4,
-        "photot": 4,
-        "60": 5,
-        "syndic": [0, 1, 4],
-        "saved_to_librari": [1, 4],
-        "not_synd": [1, 4],
-        "not_saved_to_librari": [1, 4],
-        "pil": 4,
-        "en": 4,
-        "win32": 4,
-        "wic": 4,
-        "stackexchang": 4,
-        "106410": 4,
-        "angl": 4,
-        "circl": 4,
-        "drawn": 4,
-        "coreloc": 4,
-        "aae": [0, 4],
-        "succesfulli": 0,
-        "04d": 0,
-        "export_aa": [1, 4],
-        "adjustments_path": [1, 4],
-        "aae_written": 4,
-        "shared_mo": [1, 4],
-        "not_shared_mo": [1, 4]
+        "kind": 6
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "osxphotos"]
         ],
         "osxphotos": [
             [4, 1, 1, "", "AlbumInfo"],
@@ -3045,14 +2757,15 @@
             [0, 6, 1, "cmdoption-osxphotos-export-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-export-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-export-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-export-shared", "--shared"],
             [0, 6, 1, "cmdoption-osxphotos-export-shared-moment", "--shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-export-sidecar", "--sidecar"],
             [0, 6, 1, "cmdoption-osxphotos-export-sidecar-drop-ext", "--sidecar-drop-ext"],
+            [0, 6, 1, "cmdoption-osxphotos-export-sidecar-template", "--sidecar-template"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-bursts", "--skip-bursts"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-edited", "--skip-edited"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-live", "--skip-live"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-original-if-edited", "--skip-original-if-edited"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-raw", "--skip-raw"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-uuid", "--skip-uuid"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-uuid-from-file", "--skip-uuid-from-file"],
@@ -3618,15 +3331,19 @@
     "titleterms": {
         "osxphoto": [0, 1, 2, 3, 4, 5, 6],
         "command": [0, 2, 6],
         "line": [0, 2],
         "interfac": 0,
         "cli": [0, 3],
         "about": 0,
+        "add": 0,
+        "locat": 0,
         "album": 0,
+        "batch": 0,
+        "edit": [0, 6],
         "diff": 0,
         "doc": 0,
         "dump": 0,
         "exiftool": 0,
         "export": [0, 6],
         "exportdb": 0,
         "help": 0,
@@ -3639,15 +3356,17 @@
         "list": 0,
         "orphan": 0,
         "person": 0,
         "place": 0,
         "queri": 0,
         "repl": [0, 3],
         "run": [0, 3, 6],
+        "show": 0,
         "snap": 0,
+        "sync": 0,
         "theme": [0, 6],
         "timewarp": 0,
         "tutori": [0, 6],
         "uninstal": 0,
         "uuid": 0,
         "version": 0,
         "welcom": 1,
@@ -3663,25 +3382,24 @@
         "usag": 2,
         "python": [3, 4],
         "packag": 3,
         "overview": [3, 6],
         "exampl": [3, 6],
         "us": 3,
         "code": 3,
-        "api": [],
+        "refer": 4,
         "templat": 5,
         "substitut": 5,
         "your": 6,
         "photo": 6,
         "date": 6,
         "specifi": 6,
         "directori": 6,
         "structur": 6,
         "filenam": 6,
-        "edit": [0, 6],
         "librari": 6,
         "miss": 6,
         "extern": 6,
         "disk": 6,
         "metadata": 6,
         "remov": 6,
         "dure": 6,
@@ -3706,239 +3424,15 @@
         "post": 6,
         "process": 6,
         "an": 6,
         "from": 6,
         "actual": 6,
         "user": 6,
         "color": 6,
-        "conclus": 6,
-        "sync": 0,
-        "add": 0,
-        "locat": 0,
-        "show": 0,
-        "content": [],
-        "print": [],
-        "titl": [],
-        "build": [],
-        "simpl": [],
-        "tool": [],
-        "photosdb": [],
-        "read": [],
-        "databas": [],
-        "open": [],
-        "default": [],
-        "last": [],
-        "specif": [],
-        "A": [],
-        "name": [],
-        "photosdbphoto": [],
-        "none": [],
-        "true": [],
-        "movi": [],
-        "from_dat": [],
-        "to_dat": [],
-        "intrash": [],
-        "fals": [],
-        "getphoto": [],
-        "get_photo": [],
-        "photosdbqueri": [],
-        "queryopt": [],
-        "photoinfo": [],
-        "photosdbalbuminfo": [],
-        "album_info": [],
-        "albums_shar": [],
-        "import_info": [],
-        "project_info": [],
-        "moment_info": [],
-        "folder_info": [],
-        "folder": [],
-        "dbpersoninfo": [],
-        "person_info": [],
-        "keywords_as_dict": [],
-        "persons_as_dict": [],
-        "albums_as_dict": [],
-        "albums_shared_as_dict": [],
-        "labels_norm": [],
-        "labels_as_dict": [],
-        "labels_normalized_as_dict": [],
-        "library_path": [],
-        "db_path": [],
-        "db_version": [],
-        "photos_vers": [],
-        "get_db_connect": [],
-        "execut": [],
-        "sql": [],
-        "original_filenam": [],
-        "date_ad": [],
-        "date_modifi": [],
-        "descript": [],
-        "photopersoninfo": [],
-        "photofaceinfo": [],
-        "face_info": [],
-        "path": [],
-        "path_edit": [],
-        "path_deriv": [],
-        "path_raw": [],
-        "has_raw": [],
-        "israw": [],
-        "raw_origin": [],
-        "height": [],
-        "width": [],
-        "orient": [],
-        "original_height": [],
-        "original_width": [],
-        "original_orient": [],
-        "original_files": [],
-        "ismiss": [],
-        "hasadjust": [],
-        "adjust": [],
-        "external_edit": [],
-        "favorit": [],
-        "hidden": [],
-        "visibl": [],
-        "date_trash": [],
-        "share": [],
-        "owner": [],
-        "comment": [],
-        "like": [],
-        "isrefer": [],
-        "isphoto": [],
-        "ismovi": [],
-        "iscloudasset": [],
-        "incloud": [],
-        "uti": [],
-        "uti_origin": [],
-        "uti_edit": [],
-        "uti_raw": [],
-        "burst": [],
-        "burst_select": [],
-        "burst_kei": [],
-        "burst_default_pick": [],
-        "burst_photo": [],
-        "burst_album": [],
-        "burst_album_info": [],
-        "live_photo": [],
-        "path_live_photo": [],
-        "path_edited_live_photo": [],
-        "portrait": [],
-        "hdr": [],
-        "selfi": [],
-        "time_laps": [],
-        "panorama": [],
-        "slow_mo": [],
-        "photosearchinfo": [],
-        "search_info": [],
-        "normal": [],
-        "search_info_norm": [],
-        "exif_info": [],
-        "score": [],
-        "duplic": [],
-        "fingerprint": [],
-        "hexdigest": [],
-        "json": [],
-        "asdict": [],
-        "rendertempl": [],
-        "render_templ": [],
-        "template_str": [],
-        "detected_text_method": [],
-        "detected_text": [],
-        "confidence_threshold": [],
-        "text_detection_confidence_threshold": [],
-        "exifinfo": [],
-        "albuminfo": [],
-        "albumphoto": [],
-        "creation_d": [],
-        "start_dat": [],
-        "end_dat": [],
-        "folder_list": [],
-        "folder_nam": [],
-        "parent": [],
-        "importinfo": [],
-        "importphoto": [],
-        "projectinfo": [],
-        "projectphoto": [],
-        "momentinfo": [],
-        "pk": [],
-        "subtitl": [],
-        "modification_d": [],
-        "folderinfo": [],
-        "album_info_shar": [],
-        "subfold": [],
-        "sort_ord": [],
-        "photo_index": [],
-        "placeinfo": [],
-        "ishom": [],
-        "country_cod": [],
-        "address_str": [],
-        "address": [],
-        "scoreinfo": [],
-        "searchinfo": [],
-        "place_nam": [],
-        "street": [],
-        "neighborhood": [],
-        "locality_nam": [],
-        "citi": [],
-        "state": [],
-        "state_abbrevi": [],
-        "countri": [],
-        "month": [],
-        "year": [],
-        "bodies_of_wat": [],
-        "holidai": [],
-        "activ": [],
-        "season": [],
-        "venu": [],
-        "venue_typ": [],
-        "media_typ": [],
-        "personinfo": [],
-        "display_nam": [],
-        "keyphoto": [],
-        "facecount": [],
-        "personphoto": [],
-        "personfaceinfo": [],
-        "personfavorit": [],
-        "personsortord": [],
-        "faceinfo": [],
-        "asset_uuid": [],
-        "mwg_rs_area": [],
-        "mpri_reg_rect": [],
-        "face_rect": [],
-        "center": [],
-        "size_pixel": [],
-        "roll_pitch_yaw": [],
-        "roll": [],
-        "pitch": [],
-        "yaw": [],
-        "addit": [],
-        "properti": [],
-        "commentinfo": [],
-        "likeinfo": [],
-        "adjustmentsinfo": [],
-        "raw": [],
-        "relat": [],
-        "exiftoolexiftool": [],
-        "method": [],
-        "implement": [],
-        "note": [],
-        "photoexport": [],
-        "dest": [],
-        "exportopt": [],
-        "exportresult": [],
-        "textdetect": [],
-        "text": [],
-        "detect": [],
-        "util": [],
-        "function": [],
-        "get_system_library_path": [],
-        "get_last_library_path": [],
-        "list_photo_librari": [],
-        "refer": 4,
-        "auto": [],
-        "gener": [],
-        "batch": 0
+        "conclus": 6
     },
     "envversion": {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 8,
         "sphinx.domains.index": 1,
@@ -5122,14 +4616,17 @@
         ],
         "--sidecar": [
             [0, "cmdoption-osxphotos-export-sidecar"]
         ],
         "--sidecar-drop-ext": [
             [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
         ],
+        "--sidecar-template": [
+            [0, "cmdoption-osxphotos-export-sidecar-template"]
+        ],
         "--skip-bursts": [
             [0, "cmdoption-osxphotos-export-skip-bursts"]
         ],
         "--skip-edited": [
             [0, "cmdoption-osxphotos-export-skip-edited"]
         ],
         "--skip-live": [
@@ -5781,14 +5278,15 @@
             [0, "cmdoption-osxphotos-export-screenshot"],
             [0, "cmdoption-osxphotos-export-selected"],
             [0, "cmdoption-osxphotos-export-selfie"],
             [0, "cmdoption-osxphotos-export-shared"],
             [0, "cmdoption-osxphotos-export-shared-moment"],
             [0, "cmdoption-osxphotos-export-sidecar"],
             [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
+            [0, "cmdoption-osxphotos-export-sidecar-template"],
             [0, "cmdoption-osxphotos-export-skip-bursts"],
             [0, "cmdoption-osxphotos-export-skip-edited"],
             [0, "cmdoption-osxphotos-export-skip-live"],
             [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
             [0, "cmdoption-osxphotos-export-skip-raw"],
             [0, "cmdoption-osxphotos-export-skip-uuid"],
             [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.9 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.9’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.61.0’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.9â
+{osxphotos_version}            The osxphotos version, e.g. â0.61.0â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.9 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.61.0 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.61.0 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.61.0 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.9_documentation
+osxphotos_0.61.0_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.9/osxphotos/exif_datetime_updater.py` & `osxphotos-0.61.0/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/exifinfo.py` & `osxphotos-0.61.0/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/exiftool.py` & `osxphotos-0.61.0/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/exiftool_filetypes.json` & `osxphotos-0.61.0/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/export_db.py` & `osxphotos-0.61.0/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/export_db_utils.py` & `osxphotos-0.61.0/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/fileutil.py` & `osxphotos-0.61.0/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/frozen_photoinfo.py` & `osxphotos-0.61.0/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/imageconverter.py` & `osxphotos-0.61.0/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/momentinfo.py` & `osxphotos-0.61.0/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/path_utils.py` & `osxphotos-0.61.0/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/personinfo.py` & `osxphotos-0.61.0/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photodates.py` & `osxphotos-0.61.0/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photoexporter.py` & `osxphotos-0.61.0/osxphotos/photoexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,16 @@
         "aae_written",
         "sidecar_exiftool_skipped",
         "sidecar_exiftool_written",
         "sidecar_json_skipped",
         "sidecar_json_written",
         "sidecar_xmp_skipped",
         "sidecar_xmp_written",
+        "sidecar_user_written",
+        "sidecar_user_skipped",
         "skipped",
         "skipped_album",
         "to_touch",
         "touched",
         "updated",
         "xattr_skipped",
         "xattr_written",
@@ -317,14 +319,16 @@
         aae_written=None,
         sidecar_exiftool_skipped=None,
         sidecar_exiftool_written=None,
         sidecar_json_skipped=None,
         sidecar_json_written=None,
         sidecar_xmp_skipped=None,
         sidecar_xmp_written=None,
+        sidecar_user_written=None,
+        sidecar_user_skipped=None,
         skipped=None,
         skipped_album=None,
         to_touch=None,
         touched=None,
         updated=None,
         xattr_skipped=None,
         xattr_written=None,
@@ -357,14 +361,16 @@
             + self.aae_written
             + self.sidecar_json_written
             + self.sidecar_json_skipped
             + self.sidecar_exiftool_written
             + self.sidecar_exiftool_skipped
             + self.sidecar_xmp_written
             + self.sidecar_xmp_skipped
+            + self.sidecar_user_written
+            + self.sidecar_user_skipped
             + self.missing
         )
         files += [x[0] for x in self.exiftool_warning]
         files += [x[0] for x in self.exiftool_error]
         files += [x[0] for x in self.error]
 
         return list(set(files))
```

### Comparing `osxphotos-0.60.9/osxphotos/photoinfo.py` & `osxphotos-0.61.0/osxphotos/photoinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,19 @@
             self._path = photopath
             return photopath
 
     def _path_5(self):
         """Returns candidate path for original photo on Photos >= version 5"""
         if self._info["shared"]:
             return self._path_5_shared()
-        if self.shared_moment and self._path_shared_moment():
+        if (
+            self.shared_moment
+            and self._db.photos_version >= 7
+            and self._path_shared_moment()
+        ):
             # path for photos in shared moments if it's in the shared moment folder
             # the file may also be in the originals folder which the next check will catch
             # check shared_moment first as a photo can be both a shared moment and syndicated
             # and if so, will be in the shared moment folder
             return self._path_shared_moment()
         if self.syndicated and not self.saved_to_library:
             # path for "shared with you" syndicated photos that have not yet been saved to the library
@@ -218,31 +222,31 @@
             self._db._library_path,
             shared_path,
             self._info["directory"],
             filename,
         )
 
     def _path_syndication(self):
-        """Return path for syndicated photo on Photos >= version 8"""
-        # Photos 8+ stores syndicated photos in a separate directory
+        """Return path for syndicated photo on Photos >= version 7"""
+        # Photos 7+ stores syndicated photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID.ext
         # where X is first digit of UUID
         syndication_path = "scopes/syndication/originals"
         uuid_dir = self.uuid[0]
         path = os.path.join(
             self._db._library_path,
             syndication_path,
             uuid_dir,
             self.filename,
         )
         return path if os.path.isfile(path) else None
 
     def _path_shared_moment(self):
-        """Return path for shared moment photo on Photos >= version 8"""
-        # Photos 8+ stores shared moment photos in a separate directory
+        """Return path for shared moment photo on Photos >= version 7"""
+        # Photos 7+ stores shared moment photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID.ext
         # where X is first digit of UUID
         momentshared_path = "scopes/momentshared/originals"
         uuid_dir = self.uuid[0]
         path = os.path.join(
             self._db._library_path,
             momentshared_path,
@@ -367,15 +371,15 @@
             raise ValueError(f"Unknown type {type_}")
 
         return os.path.join(
             library, "resources", "media", "version", folder_id, nn_id, filename
         )
 
     def _path_edited_4(self) -> str | None:
-        """return path_edited for Photos <= 4; modified version of code in PhotoInfo to debug #859"""
+        """return path_edited for Photos <= 4; #859"""
 
         if not self._info["hasAdjustments"]:
             return None
 
         if edit_id := self._info["edit_resource_id"]:
             try:
                 photopath = self._get_predicted_path_edited_4()
@@ -472,15 +476,15 @@
 
     @property
     def path_raw(self):
         """absolute path of associated RAW image or None if there is not one"""
 
         # In Photos 5, raw is in same folder as original but with _4.ext
         # Unless "Copy Items to the Photos Library" is not checked
-        # then RAW image is not renamed but has same name is jpeg buth with raw extension
+        # then RAW image is not renamed but has same name is jpeg but with raw extension
         # Current implementation finds images with the correct raw UTI extension
         # in same folder as the original and with same stem as original in form: original_stem*.raw_ext
         # TODO: I don't like this -- would prefer a more deterministic approach but until I have more
         # data on how Photos stores and retrieves RAW images, this seems to be working
 
         if self._info["isMissing"] == 1:
             return None  # path would be meaningless until downloaded
@@ -927,15 +931,15 @@
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
             if self.shared:
                 return self._path_live_photo_shared_5()
-            if self.shared_moment:
+            if self.shared_moment and self._db.photos_version >= 7:
                 return self._path_live_shared_moment()
             if self.syndicated and not self.saved_to_library:
                 # syndicated ("Shared with you") photos not yet saved to library
                 return self._path_live_syndicated()
 
             filename = pathlib.Path(self.path)
             photopath = filename.parent.joinpath(f"{filename.stem}_3.mov")
@@ -991,32 +995,32 @@
                     # TODO: should this be a warning or debug?
                     photopath = None
         else:
             photopath = None
         return photopath
 
     def _path_live_syndicated(self):
-        """Return path for live syndicated photo on Photos >= version 8"""
-        # Photos 8+ stores live syndicated photos in a separate directory
+        """Return path for live syndicated photo on Photos >= version 7"""
+        # Photos 7+ stores live syndicated photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID_3.mov
         # where X is first digit of UUID
         syndication_path = "scopes/syndication/originals"
         uuid_dir = self.uuid[0]
         filename = f"{pathlib.Path(self.filename).stem}_3.mov"
         live_photo = os.path.join(
             self._db._library_path,
             syndication_path,
             uuid_dir,
             filename,
         )
         return live_photo if os.path.isfile(live_photo) else None
 
     def _path_live_shared_moment(self):
-        """Return path for live shared moment photo on Photos >= version 8"""
-        # Photos 8+ stores live shared moment photos in a separate directory
+        """Return path for live shared moment photo on Photos >= version 7"""
+        # Photos 7+ stores live shared moment photos in a separate directory
         # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID_3.mov
         # where X is first digit of UUID
         shared_moment_path = "scopes/momentshared/originals"
         uuid_dir = self.uuid[0]
         filename = f"{pathlib.Path(self.filename).stem}_3.mov"
         live_photo = os.path.join(
             self._db._library_path,
@@ -1032,15 +1036,15 @@
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
 
         if self.shared:
             return self._path_derivatives_5_shared()
 
         directory = self._uuid[0]  # first char of uuid
-        if self.shared_moment:
+        if self.shared_moment and self._db.photos_version >= 7:
             # shared moments
             derivative_path = "scopes/momentshared/resources/derivatives"
             thumb_path = (
                 f"{derivative_path}/masters/{directory}/{self.uuid}_4_5005_c.jpeg"
             )
         elif self.syndicated and not self.saved_to_library:
             # syndicated ("Shared with you") photos not yet saved to library
@@ -1394,45 +1398,45 @@
             self._search_info_normalized = SearchInfo(self, normalized=True)
             return self._search_info_normalized
 
     @cached_property
     def syndicated(self) -> bool | None:
         """Return true if photo was shared via syndication (e.g. via Messages, etc.);
         these are photos that appear in "Shared with you" album.
-        Photos 8+ only; returns None if not Photos 8+.
+        Photos 7+ only; returns None if not Photos 7+.
         """
-        if self._db.photos_version < 8:
+        if self._db.photos_version < 7:
             return None
 
         try:
             return (
                 self._db._db_syndication_uuid[self.uuid]["syndication_identifier"]
                 is not None
             )
         except KeyError:
             return False
 
     @cached_property
     def saved_to_library(self) -> bool | None:
         """Return True if syndicated photo has been saved to library;
         returns False if photo is not syndicated or has not been saved to the library.
-        Returns None if not Photos 8+.
-        Syndicated photos are photos that appear in "Shared with you" album; Photos 8+ only.
+        Returns None if not Photos 7+.
+        Syndicated photos are photos that appear in "Shared with you" album; Photos 7+ only.
         """
-        if self._db.photos_version < 8:
+        if self._db.photos_version < 7:
             return None
 
         try:
             return self._db._db_syndication_uuid[self.uuid]["syndication_history"] != 0
         except KeyError:
             return False
 
     @cached_property
     def shared_moment(self) -> bool:
-        """Returns True if photo is part of a shared moment otherwise False"""
+        """Returns True if photo is part of a shared moment otherwise False (Photos 7+ only)"""
         return bool(self._info["moment_share"])
 
     @property
     def labels(self):
         """returns list of labels applied to photo by Photos image categorization
         only valid on Photos 5, on older libraries returns empty list
         """
@@ -1929,14 +1933,18 @@
         exif_info = dataclasses.asdict(self.exif_info) if self.exif_info else {}
         face_info = [face.asdict() for face in self.face_info]
         folders = {album.title: album.folder_names for album in self.album_info}
         likes = [like.asdict() for like in self.likes]
         place = self.place.asdict() if self.place else {}
         score = dataclasses.asdict(self.score) if self.score else {}
 
+        # do not add any new properties to data_dict as this is used by export to determine
+        # if a photo needs to be re-exported and adding new properties may cause all photos
+        # to be re-exported
+        # see below `if not shallow:`
         dict_data = {
             "albums": self.albums,
             "burst": self.burst,
             "cloud_guid": self.cloud_guid,
             "cloud_owner_hashed_id": self.cloud_owner_hashed_id,
             "comments": comments,
             "date_added": self.date_added,
@@ -2003,14 +2011,15 @@
             "uti": self.uti,
             "uuid": self.uuid,
             "visible": self.visible,
             "width": self.width,
         }
 
         # non-shallow keys
+        # add any new properties here
         if not shallow:
             dict_data["album_info"] = [album.asdict() for album in self.album_info]
             dict_data["path_derivatives"] = self.path_derivatives
             dict_data["adjustments"] = (
                 self.adjustments.asdict() if self.adjustments else {}
             )
             dict_data["burst_album_info"] = [a.asdict() for a in self.burst_album_info]
@@ -2030,14 +2039,17 @@
                 self.search_info.asdict() if self.search_info else {}
             )
             dict_data["search_info_normalized"] = (
                 self.search_info_normalized.asdict()
                 if self.search_info_normalized
                 else {}
             )
+            dict_data["syndicated"] = self.syndicated
+            dict_data["saved_to_library"] = self.saved_to_library
+            dict_data["shared_moment"] = self.shared_moment
 
         return dict_data
 
     def json(self, indent: int | None = None, shallow: bool = True) -> str:
         """Return JSON representation
 
         Args:
```

### Comparing `osxphotos-0.60.9/osxphotos/photokit.py` & `osxphotos-0.61.0/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photosalbum.py` & `osxphotos-0.61.0/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photoscript_utils.py` & `osxphotos-0.61.0/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_syndicationinfo.py` & `osxphotos-0.61.0/osxphotos/photosdb/_photosdb_process_syndicationinfo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """ Methods for PhotosDB to process Syndication info (#1054) """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from .._constants import _DB_TABLE_NAMES
+from .._constants import _DB_TABLE_NAMES, _PHOTOS_SYNDICATION_MODEL_VERSION
 from ..sqlite_utils import sqlite_open_ro
 
 if TYPE_CHECKING:
     from osxphotos.photosdb import PhotosDB
 
 
 def _process_syndicationinfo(self: PhotosDB):
     """Process syndication information"""
 
     self._db_syndication_uuid = {}
 
-    if self.photos_version < 8:
+    if self.photos_version < 7:
         raise NotImplementedError(
             f"syndication info not implemented for this database version: {self.photos_version}"
         )
-    else:
-        _process_syndicationinfo_8(self)
 
+    if self._model_ver < _PHOTOS_SYNDICATION_MODEL_VERSION:
+        return
 
-def _process_syndicationinfo_8(photosdb: PhotosDB):
+    _process_syndicationinfo_7(self)
+
+
+def _process_syndicationinfo_7(photosdb: PhotosDB):
     """Process Syndication info for Photos 8.0 and later
 
     Args:
         photosdb: an OSXPhotosDB instance
     """
 
     db = photosdb._tmp_db
```

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/photosdb.py` & `osxphotos-0.61.0/osxphotos/photosdb/photosdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 from ..phototemplate import RenderOptions
 from ..platform import get_macos_version, is_macos
 from ..queryoptions import QueryOptions
 from ..rich_utils import add_rich_markup_tag
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
 from ..unicode import normalize_unicode
 from ..utils import _check_file_exists, get_last_library_path, noop
-from .photosdb_utils import get_db_model_version, get_db_version
+from .photosdb_utils import get_photos_version_from_model, get_db_version, get_model_version
 
 if is_macos:
     import photoscript
 
 logger = logging.getLogger("osxphotos")
 
 __all__ = ["PhotosDB"]
@@ -322,44 +322,46 @@
         verbose(f"Processing database {self._filepath(self._dbfile)}")
 
         # if database is exclusively locked, make a copy of it and use the copy
         # Photos maintains an exclusive lock on the database file while Photos is open
         # photoanalysisd sometimes maintains this lock even after Photos is closed
         # In those cases, make a temp copy of the file for sqlite3 to read
         if sqlite_db_is_locked(self._dbfile):
-            verbose(f"Database locked, creating temporary copy.")
+            verbose("Database locked, creating temporary copy.")
             self._tmp_db = self._copy_db_file(self._dbfile)
 
         # _db_version is set from photos.db
         self._db_version = get_db_version(self._tmp_db)
         # _photos_version is set from Photos.sqlite which only exists for Photos 5+
         db_ver_int = int(self._db_version)
         if db_ver_int < 3000:
             self._photos_ver = 2
         elif db_ver_int < 4000:
             self._photos_ver = 3
         elif db_ver_int < 5000:
             self._photos_ver = 4
         else:
             self._photos_ver = 5
+        self._model_ver = 0  # only set for Photos 5+
+
         # If Photos >= 5, actual data isn't in photos.db but in Photos.sqlite
         if int(self._db_version) > int(_PHOTOS_4_VERSION):
             dbpath = pathlib.Path(self._dbfile).parent
             dbfile = dbpath / "Photos.sqlite"
             if not _check_file_exists(dbfile):
                 raise FileNotFoundError(f"dbfile {dbfile} does not exist", dbfile)
-            else:
-                self._dbfile_actual = self._tmp_db = dbfile
-                verbose(f"Processing database {self._filepath(self._dbfile_actual)}")
-                # if database is exclusively locked, make a copy of it and use the copy
-                if sqlite_db_is_locked(self._dbfile_actual):
-                    verbose(f"Database locked, creating temporary copy.")
-                    self._tmp_db = self._copy_db_file(self._dbfile_actual)
+            self._dbfile_actual = self._tmp_db = dbfile
+            verbose(f"Processing database {self._filepath(self._dbfile_actual)}")
+            # if database is exclusively locked, make a copy of it and use the copy
+            if sqlite_db_is_locked(self._dbfile_actual):
+                verbose("Database locked, creating temporary copy.")
+                self._tmp_db = self._copy_db_file(self._dbfile_actual)
             # set the photos version to actual value based on Photos.sqlite
-            self._photos_ver = get_db_model_version(self._tmp_db)
+            self._photos_ver = get_photos_version_from_model(self._tmp_db)
+            self._model_ver = get_model_version(self._tmp_db)
 
             logger.debug(
                 f"_dbfile = {self._dbfile}, _dbfile_actual = {self._dbfile_actual}"
             )
 
         library_path = os.path.dirname(os.path.abspath(dbfile))
         (library_path, _) = os.path.split(library_path)  # drop /database from path
@@ -1231,15 +1233,15 @@
 
             # fingerprint
             self._dbphotos[uuid]["masterFingerprint"] = row[45]
 
             # photos 5+ only, for shared photos
             self._dbphotos[uuid]["cloudownerhashedpersonid"] = None
 
-            # photos 8+ only, shared moments
+            # photos 7+ only, shared moments
             self._dbphotos[uuid]["moment_share"] = None
 
             # compute signatures for finding possible duplicates
             signature = self._duplicate_signature(uuid)
             try:
                 self._db_signatures[signature].append(uuid)
             except KeyError:
@@ -2000,15 +2002,15 @@
         # 37   ZGENERICASSET.ZADJUSTMENTTIMESTAMP -- when was photo edited?
         # 38   ZGENERICASSET.ZVISIBILITYSTATE -- 0 if visible, 2 if not (e.g. a burst image)
         # 39   ZGENERICASSET.ZTRASHEDDATE -- date item placed in the trash or null if not in trash
         # 40   ZGENERICASSET.ZSAVEDASSETTYPE -- how item imported
         # 41   ZGENERICASSET.ZADDEDDATE -- date item added to the library
         # 42   ZGENERICASSET.Z_PK -- primary key
         # 43   ZGENERICASSET.ZCLOUDOWNERHASHEDPERSONID -- used to look up owner name (for shared photos)
-        # 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 8+)
+        # 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 5+; in Photos 7+ these are in the scopes/momentshared folder)
 
         for row in c:
             uuid = row[0]
             info = {}
             info["_uuid"] = uuid  # stored here for easier debugging
             info["modelID"] = None
             info["masterUuid"] = None
@@ -2522,15 +2524,15 @@
         verbose("Processing comments and likes for shared photos.")
         self._process_comments()
 
         # process moments
         verbose("Processing moments.")
         self._process_moments()
 
-        if self.photos_version >= 8:
+        if self.photos_version >= 7:
             verbose("Processing syndication info.")
             self._process_syndicationinfo()
 
         verbose("Done processing details from Photos library.")
 
     def _process_moments(self):
         """Process data from ZMOMENT table"""
```

### Comparing `osxphotos-0.60.9/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.61.0/osxphotos/photosdb/photosdb_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     _TESTED_DB_VERSIONS,
 )
 from ..sqlite_utils import sqlite_open_ro
 
 __all__ = [
     "get_db_version",
     "get_model_version",
-    "get_db_model_version",
+    "get_photos_version_from_model",
     "get_photos_library_version",
 ]
 
 
 def get_db_version(db_file):
     """Gets the Photos DB version from LiGlobals table
 
@@ -90,15 +90,15 @@
 
     conn.close()
 
     plist = plistlib.loads(results[1])
     return plist["PLModelVersion"]
 
 
-def get_db_model_version(db_file: str) -> int:
+def get_photos_version_from_model(db_file: str) -> int:
     """Returns Photos version based on model version found in db_file
 
     Args:
         db_file: path to Photos.sqlite file
 
     Returns: int of major Photos version number (e.g. 5 or 6).
     If unknown model version found, logs warning and returns most current Photos version.
```

### Comparing `osxphotos-0.60.9/osxphotos/phototables.py` & `osxphotos-0.61.0/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/phototemplate.cog.md` & `osxphotos-0.61.0/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/phototemplate.md` & `osxphotos-0.61.0/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/phototemplate.py` & `osxphotos-0.61.0/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/phototemplate.tx` & `osxphotos-0.61.0/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/phototz.py` & `osxphotos-0.61.0/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/placeinfo.py` & `osxphotos-0.61.0/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/platform.py` & `osxphotos-0.61.0/osxphotos/platform.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/pyrepl.py` & `osxphotos-0.61.0/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.61.0/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/query_builder.py` & `osxphotos-0.61.0/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/queryoptions.py` & `osxphotos-0.61.0/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/scoreinfo.py` & `osxphotos-0.61.0/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/searchinfo.py` & `osxphotos-0.61.0/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/sqlgrep.py` & `osxphotos-0.61.0/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/sqlite_utils.py` & `osxphotos-0.61.0/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/sqlitekvstore.py` & `osxphotos-0.61.0/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/template_counter.py` & `osxphotos-0.61.0/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.61.0/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.61.0/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/text_detection.py` & `osxphotos-0.61.0/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/timeutils.py` & `osxphotos-0.61.0/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/timezones.py` & `osxphotos-0.61.0/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/tutorial.md` & `osxphotos-0.61.0/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/unicode.py` & `osxphotos-0.61.0/osxphotos/unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/uti.py` & `osxphotos-0.61.0/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos/utils.py` & `osxphotos-0.61.0/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.61.0/osxphotos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.9
+Version: 0.61.0
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.9/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.61.0/osxphotos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 osxphotos/cli/places.py
 osxphotos/cli/print_photo_info.py
 osxphotos/cli/query.py
 osxphotos/cli/repl.py
 osxphotos/cli/report_writer.py
 osxphotos/cli/rich_progress.py
 osxphotos/cli/show_command.py
+osxphotos/cli/sidecar.py
 osxphotos/cli/snap_diff.py
 osxphotos/cli/sync.py
 osxphotos/cli/sync_results.py
 osxphotos/cli/theme.py
 osxphotos/cli/timewarp.py
 osxphotos/cli/tutorial.py
 osxphotos/cli/uuid.py
@@ -140,14 +141,15 @@
 tests/test_cli_add_to_album.py
 tests/test_cli_all_commands.py
 tests/test_cli_batch_edit.py
 tests/test_cli_dump.py
 tests/test_cli_exiftool.py
 tests/test_cli_export_cloud.py
 tests/test_cli_export_projects.py
+tests/test_cli_export_sidecar_template.py
 tests/test_cli_exportdb.py
 tests/test_cli_import.py
 tests/test_cli_orphans.py
 tests/test_cli_param_types.py
 tests/test_cli_sync.py
 tests/test_cli_timewarp.py
 tests/test_cli_utils.py
```

### Comparing `osxphotos-0.60.9/osxphotos.egg-info/requires.txt` & `osxphotos-0.61.0/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/setup.py` & `osxphotos-0.61.0/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_10_12_6.py` & `osxphotos-0.61.0/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.61.0/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.61.0/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.61.0/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_catalina_10_15_7.py` & `osxphotos-0.61.0/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli.py` & `osxphotos-0.61.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_add_locations.py` & `osxphotos-0.61.0/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_add_to_album.py` & `osxphotos-0.61.0/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_all_commands.py` & `osxphotos-0.61.0/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_batch_edit.py` & `osxphotos-0.61.0/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_dump.py` & `osxphotos-0.61.0/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_exiftool.py` & `osxphotos-0.61.0/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_export_cloud.py` & `osxphotos-0.61.0/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_export_projects.py` & `osxphotos-0.61.0/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_exportdb.py` & `osxphotos-0.61.0/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_import.py` & `osxphotos-0.61.0/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_orphans.py` & `osxphotos-0.61.0/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_param_types.py` & `osxphotos-0.61.0/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_sync.py` & `osxphotos-0.61.0/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_timewarp.py` & `osxphotos-0.61.0/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_utils.py` & `osxphotos-0.61.0/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cli_verbose.py` & `osxphotos-0.61.0/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_cloud_owner_catalina.py` & `osxphotos-0.61.0/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_comments.py` & `osxphotos-0.61.0/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_concurrent_export.py` & `osxphotos-0.61.0/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_configoptions.py` & `osxphotos-0.61.0/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_datetime_formatter.py` & `osxphotos-0.61.0/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_datetime_utils.py` & `osxphotos-0.61.0/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_debug.py` & `osxphotos-0.61.0/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_empty_library_4_0.py` & `osxphotos-0.61.0/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_exif_info.py` & `osxphotos-0.61.0/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_exiftool.py` & `osxphotos-0.61.0/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_exiftool_caching.py` & `osxphotos-0.61.0/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.61.0/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.61.0/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.61.0/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_export_db.py` & `osxphotos-0.61.0/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.61.0/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_exportresults.py` & `osxphotos-0.61.0/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_faceinfo.py` & `osxphotos-0.61.0/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_fileutil.py` & `osxphotos-0.61.0/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_highsierra.py` & `osxphotos-0.61.0/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_image_converter.py` & `osxphotos-0.61.0/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.61.0/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.61.0/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.61.0/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.61.0/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.61.0/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.61.0/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_monterey_12_0_1.py` & `osxphotos-0.61.0/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.61.0/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_movies_4_0.py` & `osxphotos-0.61.0/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_movies_5_0.py` & `osxphotos-0.61.0/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_path_utils.py` & `osxphotos-0.61.0/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_personinfo.py` & `osxphotos-0.61.0/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_photokit.py` & `osxphotos-0.61.0/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_photosalbum_unicode.py` & `osxphotos-0.61.0/tests/test_photosalbum_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_photosdb_utils.py` & `osxphotos-0.61.0/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_placeinfo.py` & `osxphotos-0.61.0/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.61.0/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.61.0/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_projects_catalina.py` & `osxphotos-0.61.0/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_projects_sierra.py` & `osxphotos-0.61.0/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_score_info.py` & `osxphotos-0.61.0/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_search_info_10_14_6.py` & `osxphotos-0.61.0/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_search_info_10_15_4.py` & `osxphotos-0.61.0/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_search_info_10_15_5.py` & `osxphotos-0.61.0/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_search_info_10_15_7.py` & `osxphotos-0.61.0/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.61.0/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_sidecar_xmp.py` & `osxphotos-0.61.0/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_sonoma_14_0_0.py` & `osxphotos-0.61.0/tests/test_sonoma_14_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.61.0/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.61.0/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.61.0/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_specials_sierra_10_12.py` & `osxphotos-0.61.0/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_sqlitekvstore.py` & `osxphotos-0.61.0/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_template.py` & `osxphotos-0.61.0/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_template_counter.py` & `osxphotos-0.61.0/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_template_today.py` & `osxphotos-0.61.0/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_unicode.py` & `osxphotos-0.61.0/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_uti.py` & `osxphotos-0.61.0/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_utils.py` & `osxphotos-0.61.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_ventura_13_0_0.py` & `osxphotos-0.61.0/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.9/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.61.0/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

