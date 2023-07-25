# Comparing `tmp/ytdl-sub-2023.7.25.post4.tar.gz` & `tmp/ytdl-sub-2023.7.25.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.25.post4.tar", last modified: Tue Jul 25 19:13:26 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.25.post5.tar", last modified: Tue Jul 25 19:39:16 2023, max compression
```

## Comparing `ytdl-sub-2023.7.25.post4.tar` & `ytdl-sub-2023.7.25.post5.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.906962 ytdl-sub-2023.7.25.post4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.910962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.910962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/downloader_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.918962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.918962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.926962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.926962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.910962 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.521696 ytdl-sub-2023.7.25.post5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.525696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 19:38:56.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.529696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.529696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.533696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.533696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.533696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url_source_options_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.537696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.537696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.545696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.545696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.545696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.549697 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.529696 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.25.post4/LICENSE` & `ytdl-sub-2023.7.25.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/PKG-INFO` & `ytdl-sub-2023.7.25.post5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post4
+Version: 2023.7.25.post5
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post4/README.md` & `ytdl-sub-2023.7.25.post5/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/pyproject.toml` & `ytdl-sub-2023.7.25.post5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/setup.cfg` & `ytdl-sub-2023.7.25.post5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/plugin.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from ytdl_sub.config.preset_class_mappings import DownloadStrategyMapping
 from ytdl_sub.config.preset_class_mappings import PluginMapping
 from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import TOptionsValidator
 from ytdl_sub.config.preset_options import YTDLOptions
-from ytdl_sub.downloaders.base_downloader import BaseDownloader
-from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
+from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.prebuilt_presets import PREBUILT_PRESET_NAMES
 from ytdl_sub.prebuilt_presets import PUBLISHED_PRESET_NAMES
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.yaml import dump_yaml
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
@@ -117,15 +116,15 @@
     def __init__(self, name: str, value: Any):
         super().__init__(name=name, value=value)
         self.download_strategy_name = self._validate_key(
             key="download_strategy",
             validator=StringValidator,
         ).value
 
-    def get(self, downloader_source: str) -> Type[BaseDownloader]:
+    def get(self, downloader_source: str) -> Type[SourcePlugin]:
         """
         Parameters
         ----------
         downloader_source:
             Name of the download source
 
         Returns
@@ -209,15 +208,15 @@
             source_dict["download_strategy"] = download_strategy
 
         downloader = DownloadStrategyValidator(name=f"{name}.{source_name}", value=source_dict).get(
             downloader_source=source_name
         )
         del source_dict["download_strategy"]
 
-        downloader.downloader_options_type.partial_validate(
+        downloader.plugin_options_type.partial_validate(
             name=f"{name}.{source_name}", value=source_dict
         )
 
     @classmethod
     def preset_partial_validate(cls, config: ConfigValidator, name: str, value: Any) -> None:
         """
         Partially validates a preset. Used to ensure every preset in a ConfigFile looks sane.
@@ -266,34 +265,32 @@
                 validator=PluginMapping.get(plugin_name).plugin_options_type,
             )
 
     @property
     def _source_variables(self) -> List[str]:
         return Entry.source_variables()
 
-    def __validate_and_get_downloader(self, downloader_source: str) -> Type[BaseDownloader]:
+    def __validate_and_get_downloader(self, downloader_source: str) -> Type[SourcePlugin]:
         return self._validate_key(key=downloader_source, validator=DownloadStrategyValidator).get(
             downloader_source=downloader_source
         )
 
     def __validate_and_get_downloader_options(
-        self, downloader_source: str, downloader: Type[BaseDownloader]
-    ) -> DownloaderValidator:
+        self, downloader_source: str, downloader: Type[SourcePlugin]
+    ) -> OptionsValidator:
         # Remove the download_strategy key before validating it against the downloader options
         # TODO: make this cleaner
         del self._dict[downloader_source]["download_strategy"]
-        return self._validate_key(
-            key=downloader_source, validator=downloader.downloader_options_type
-        )
+        return self._validate_key(key=downloader_source, validator=downloader.plugin_options_type)
 
     def __validate_and_get_downloader_and_options(
         self,
-    ) -> Tuple[Type[BaseDownloader], DownloaderValidator]:
-        downloader: Optional[Type[BaseDownloader]] = None
-        download_options: Optional[DownloaderValidator] = None
+    ) -> Tuple[Type[SourcePlugin], OptionsValidator]:
+        downloader: Optional[Type[SourcePlugin]] = None
+        download_options: Optional[OptionsValidator] = None
         downloader_sources = DownloadStrategyMapping.sources()
 
         for key in self._keys:
             # skip if the key is not a download source
             if key not in downloader_sources:
                 continue
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict
 from typing import List
 from typing import Type
 
 from ytdl_sub.config.plugin import Plugin
-from ytdl_sub.downloaders.base_downloader import BaseDownloader
+from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.downloaders.url.multi_url import MultiUrlDownloader
 from ytdl_sub.downloaders.url.url import UrlDownloader
 from ytdl_sub.plugins.audio_extract import AudioExtractPlugin
 from ytdl_sub.plugins.chapters import ChaptersPlugin
 from ytdl_sub.plugins.date_range import DateRangePlugin
 from ytdl_sub.plugins.embed_thumbnail import EmbedThumbnailPlugin
 from ytdl_sub.plugins.file_convert import FileConvertPlugin
@@ -23,15 +23,15 @@
 
 
 class DownloadStrategyMapping:
     """
     Maps downloader strategies defined in the preset to its respective downloader class
     """
 
-    _MAPPING: Dict[str, Dict[str, Type[BaseDownloader]]] = {
+    _MAPPING: Dict[str, Dict[str, Type[SourcePlugin]]] = {
         "download": {
             "multi_url": MultiUrlDownloader,
             "url": UrlDownloader,
         },
     }
 
     @classmethod
@@ -78,15 +78,15 @@
             raise ValueError(
                 f"Tried to use download strategy '{download_strategy}' with source '{source}', "
                 f"which does not exist. Available download strategies: "
                 f"{', '.join(cls.source_download_strategies(source))}"
             )
 
     @classmethod
-    def get(cls, source: str, download_strategy: str) -> Type[BaseDownloader]:
+    def get(cls, source: str, download_strategy: str) -> Type[SourcePlugin]:
         """
         Parameters
         ----------
         source:
             The source (i.e. 'youtube', 'soundcloud') of the downloader
         download_strategy:
             The download strategy name
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,43 @@
 import abc
 from abc import ABC
 from typing import Generic
 from typing import Iterable
 from typing import List
-from typing import Type
 
+from ytdl_sub.config.plugin import BasePlugin
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import TOptionsValidator
-from ytdl_sub.downloaders.downloader_validator import TDownloaderValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadArchiver
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
-class BaseDownloaderPlugin(Plugin[TDownloaderValidator], ABC):
+class SourcePluginExtension(Plugin[TOptionsValidator], ABC):
     """
     Plugins that get added automatically by using a downloader. Downloader options
     are the plugin options.
     """
 
-    def __init__(
-        self,
-        downloader_options: TDownloaderValidator,
-        overrides: Overrides,
-        enhanced_download_archive: EnhancedDownloadArchive,
-    ):
-        super().__init__(
-            # Downloader plugins use download options as their plugin options
-            options=downloader_options,
-            overrides=overrides,
-            enhanced_download_archive=enhanced_download_archive,
-        )
-
-
-class BaseDownloader(DownloadArchiver, Generic[TOptionsValidator], ABC):
-    downloader_options_type: Type[TOptionsValidator]
 
+class SourcePlugin(BasePlugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
     def __init__(
         self,
-        download_options: TOptionsValidator,
+        options: TOptionsValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
     ):
-        super().__init__(enhanced_download_archive=enhanced_download_archive)
-        self.download_options = download_options
-        self.overrides = overrides
+        super().__init__(
+            options=options,
+            overrides=overrides,
+            enhanced_download_archive=enhanced_download_archive,
+        )
         self._download_ytdl_options_builder = download_ytdl_options
         self._metadata_ytdl_options_builder = metadata_ytdl_options
 
     @abc.abstractmethod
     def download_metadata(self) -> Iterable[Entry]:
         """Gathers metadata of all entries to download"""
 
@@ -63,12 +48,12 @@
     # pylint: disable=unused-argument
     @classmethod
     def added_plugins(
         cls,
         downloader_options: TOptionsValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         overrides: Overrides,
-    ) -> List[BaseDownloaderPlugin]:
+    ) -> List[SourcePluginExtension]:
         """Add these plugins from the Downloader to the subscription"""
         return []
 
     # pylint: enable=unused-argument
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/downloader_validator.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url_source_options_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 from typing import TypeVar
 
 from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 
 
-class DownloaderValidator(OptionsValidator, ABC):
+class MultiUrlSourceOptionsValidator(OptionsValidator, ABC):
     """
     Placeholder class to define downloader options
     """
 
     @property
     @abc.abstractmethod
     def collection_validator(self) -> MultiUrlValidator:
@@ -38,8 +38,10 @@
         Validates any source variables added by the collection
         """
         self.collection_validator.validate_with_variables(
             source_variables=source_variables, override_variables=override_variables
         )
 
 
-TDownloaderValidator = TypeVar("TDownloaderValidator", bound=DownloaderValidator)
+TMultiURLSourceOptionsValidator = TypeVar(
+    "TMultiURLSourceOptionsValidator", bound=MultiUrlSourceOptionsValidator
+)
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 from pathlib import Path
 from typing import Dict
 from typing import Iterable
 from typing import List
 
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.config.preset_options import Overrides
-from ytdl_sub.downloaders.base_downloader import BaseDownloader
+from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import get_file_extension
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadMapping
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
 class InfoJsonDownloaderOptions(OptionsDictValidator):
     _optional_keys = {"no-op"}
 
 
-class InfoJsonDownloader(BaseDownloader[InfoJsonDownloaderOptions]):
-    downloader_options_type = InfoJsonDownloaderOptions
+class InfoJsonDownloader(SourcePlugin[InfoJsonDownloaderOptions]):
+    plugin_options_type = InfoJsonDownloaderOptions
 
     def __init__(
         self,
-        download_options: InfoJsonDownloaderOptions,
+        options: InfoJsonDownloaderOptions,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
     ):
         super().__init__(
-            download_options=download_options,
+            options=options,
             enhanced_download_archive=enhanced_download_archive,
             download_ytdl_options=download_ytdl_options,
             metadata_ytdl_options=metadata_ytdl_options,
             overrides=overrides,
         )
         # Keep track of original file mappings for the 'mock' download
         self._original_entry_mappings = copy.deepcopy(
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 from typing import Set
 from typing import Tuple
 
 from yt_dlp.utils import RejectedVideoReached
 
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import Overrides
-from ytdl_sub.downloaders.base_downloader import BaseDownloader
-from ytdl_sub.downloaders.base_downloader import BaseDownloaderPlugin
-from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
-from ytdl_sub.downloaders.downloader_validator import TDownloaderValidator
+from ytdl_sub.downloaders.source_plugin import SourcePlugin
+from ytdl_sub.downloaders.source_plugin import SourcePluginExtension
+from ytdl_sub.downloaders.url.multi_url_source_options_validator import (
+    MultiUrlSourceOptionsValidator,
+)
+from ytdl_sub.downloaders.url.multi_url_source_options_validator import (
+    TMultiURLSourceOptionsValidator,
+)
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 from ytdl_sub.downloaders.url.validators import UrlThumbnailListValidator
 from ytdl_sub.downloaders.url.validators import UrlValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.downloaders.ytdlp import YTDLP
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.entry_parent import EntryParent
@@ -46,30 +50,30 @@
 
 class URLDownloadState:
     def __init__(self, entries_total: int):
         self.entries_total = entries_total
         self.entries_downloaded = 0
 
 
-class UrlDownloaderThumbnailPlugin(BaseDownloaderPlugin):
+class UrlDownloaderThumbnailPlugin(SourcePluginExtension):
     def __init__(
         self,
-        downloader_options: DownloaderValidator,
+        options: MultiUrlSourceOptionsValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
-            downloader_options=downloader_options,
+            options=options,
             overrides=overrides,
             enhanced_download_archive=enhanced_download_archive,
         )
         self._thumbnails_downloaded: Set[str] = set()
         self._collection_url_mapping: Dict[str, UrlValidator] = {
             self.overrides.apply_formatter(collection_url.url): collection_url
-            for collection_url in downloader_options.collection_validator.urls.list
+            for collection_url in options.collection_validator.urls.list
         }
 
     def _download_parent_thumbnails(
         self,
         thumbnail_list_info: UrlThumbnailListValidator,
         entry: Entry,
         parent: EntryParent,
@@ -145,23 +149,23 @@
             self._download_url_thumbnails(
                 collection_url=self._collection_url_mapping[entry.kwargs(COLLECTION_URL)],
                 entry=entry,
             )
         return entry
 
 
-class UrlDownloaderCollectionVariablePlugin(BaseDownloaderPlugin):
+class UrlDownloaderCollectionVariablePlugin(SourcePluginExtension):
     def __init__(
         self,
-        downloader_options: DownloaderValidator,
+        downloader_options: MultiUrlSourceOptionsValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
-            downloader_options=downloader_options,
+            options=downloader_options,
             overrides=overrides,
             enhanced_download_archive=enhanced_download_archive,
         )
         self._thumbnails_downloaded: Set[str] = set()
         self._collection_url_mapping: Dict[str, UrlValidator] = {
             self.overrides.apply_formatter(collection_url.url): collection_url
             for collection_url in downloader_options.collection_validator.urls.list
@@ -182,35 +186,35 @@
         )
 
         entry.add_variables(variables_to_add=collection_url.variables.dict_with_format_strings)
 
         return entry
 
 
-class BaseUrlDownloader(BaseDownloader[TDownloaderValidator], ABC):
+class BaseUrlDownloader(SourcePlugin[TMultiURLSourceOptionsValidator], ABC):
     """
     Class that interacts with ytdl to perform the download of metadata and content,
     and should translate that to list of Entry objects.
     """
 
     @classmethod
     def added_plugins(
         cls,
-        downloader_options: TDownloaderValidator,
+        downloader_options: TMultiURLSourceOptionsValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         overrides: Overrides,
     ) -> List[Plugin]:
         """
         Adds
         1. URL thumbnail download plugin
         2. Collection variable plugin to add to each entry
         """
         return [
             UrlDownloaderThumbnailPlugin(
-                downloader_options=downloader_options,
+                options=downloader_options,
                 overrides=overrides,
                 enhanced_download_archive=enhanced_download_archive,
             ),
             UrlDownloaderCollectionVariablePlugin(
                 downloader_options=downloader_options,
                 overrides=overrides,
                 enhanced_download_archive=enhanced_download_archive,
@@ -225,36 +229,36 @@
            ytdl_options:
              ignoreerrors: True  # ignore errors like hidden videos, age restriction, etc
         """
         return {"ignoreerrors": True}
 
     def __init__(
         self,
-        download_options: TDownloaderValidator,
+        options: TMultiURLSourceOptionsValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
     ):
         """
         Parameters
         ----------
-        download_options
+        options
             Options validator for this downloader
         enhanced_download_archive
             Download archive
         download_ytdl_options
             YTDL options builder for downloading media
         metadata_ytdl_options
             YTDL options builder for downloading metadata
         overrides
             Override variables
         """
         super().__init__(
-            download_options=download_options,
+            options=options,
             enhanced_download_archive=enhanced_download_archive,
             download_ytdl_options=download_ytdl_options,
             metadata_ytdl_options=metadata_ytdl_options,
             overrides=overrides,
         )
         self._downloaded_entries: Set[str] = set()
         self._url_state: Optional[URLDownloadState] = None
@@ -311,15 +315,15 @@
 
     def _mark_downloaded(self, entry: Entry) -> None:
         self._downloaded_entries.add(entry.ytdl_uid())
 
     @property
     def collection(self) -> MultiUrlValidator:
         """Return the download options collection"""
-        return self.download_options.collection_validator
+        return self.plugin_options.collection_validator
 
     @contextlib.contextmanager
     def _separate_download_archives(self, clear_info_json_files: bool = False):
         """
         Separate download archive writing between collection urls. This is so break_on_existing
         does not break when downloading from subset urls.
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Dict
 from typing import List
 
-from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.downloaders.url.downloader import BaseUrlDownloader
+from ytdl_sub.downloaders.url.multi_url_source_options_validator import (
+    MultiUrlSourceOptionsValidator,
+)
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 
 
-class MultiUrlDownloadOptions(MultiUrlValidator, DownloaderValidator):
+class MultiUrlDownloadOptions(MultiUrlValidator, MultiUrlSourceOptionsValidator):
     """
     Downloads from multiple URLs. If an entry is returned from more than one URL, it will
     resolve to the bottom-most URL settings.
 
     Usage:
 
     .. code-block:: yaml
@@ -61,8 +63,8 @@
             has_non_empty_url |= bool(url_validator.url.apply_formatter(override_variables))
 
         if not has_non_empty_url:
             raise self._validation_exception("Must contain at least one url that is non-empty")
 
 
 class MultiUrlDownloader(BaseUrlDownloader[MultiUrlDownloadOptions]):
-    downloader_options_type = MultiUrlDownloadOptions
+    plugin_options_type = MultiUrlDownloadOptions
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.downloaders.url.downloader import BaseUrlDownloader
+from ytdl_sub.downloaders.url.multi_url_source_options_validator import (
+    MultiUrlSourceOptionsValidator,
+)
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 from ytdl_sub.downloaders.url.validators import UrlValidator
 
 
-class UrlDownloadOptions(UrlValidator, DownloaderValidator):
+class UrlDownloadOptions(UrlValidator, MultiUrlSourceOptionsValidator):
     """
     Downloads from a single URL supported by yt-dlp.
 
     Usage:
 
     .. code-block:: yaml
 
@@ -33,8 +35,8 @@
         return MultiUrlValidator(
             name=self._name,
             value={"urls": [self._value]},
         )
 
 
 class UrlDownloader(BaseUrlDownloader[UrlDownloadOptions]):
-    downloader_options_type = UrlDownloadOptions
+    plugin_options_type = UrlDownloadOptions
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from abc import ABC
 from pathlib import Path
 from typing import Type
 
 from ytdl_sub.config.config_validator import ConfigOptions
 from ytdl_sub.config.preset import Preset
 from ytdl_sub.config.preset import PresetPlugins
+from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import YTDLOptions
-from ytdl_sub.downloaders.base_downloader import BaseDownloader
-from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
+from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
 class BaseSubscription(ABC):
     """
     Subscription classes are the 'controllers' that perform...
 
@@ -48,24 +48,24 @@
         self._enhanced_download_archive = EnhancedDownloadArchive(
             file_name=self.overrides.apply_formatter(self.output_options.download_archive_name),
             working_directory=self.working_directory,
             output_directory=self.output_directory,
         )
 
     @property
-    def downloader_class(self) -> Type[BaseDownloader]:
+    def downloader_class(self) -> Type[SourcePlugin]:
         """
         Returns
         -------
         This subscription's downloader class
         """
         return self._preset_options.downloader
 
     @property
-    def downloader_options(self) -> DownloaderValidator:
+    def downloader_options(self) -> OptionsValidator:
         """
         Returns
         -------
         The download options for this subscription's downloader
         """
         return self._preset_options.downloader_options
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from abc import ABC
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.plugin import SplitPlugin
-from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.info_json.info_json_downloader import InfoJsonDownloader
 from ytdl_sub.downloaders.info_json.info_json_downloader import InfoJsonDownloaderOptions
+from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.subscriptions.base_subscription import BaseSubscription
 from ytdl_sub.subscriptions.subscription_ytdl_options import SubscriptionYTDLOptions
 from ytdl_sub.utils.datetime import to_date_range
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.file_handler import FileHandler
@@ -287,15 +287,15 @@
                 self._cleanup_entry_files(split_entry)
 
         self._cleanup_entry_files(entry)
 
     def _process_subscription(
         self,
         plugins: List[Plugin],
-        downloader: BaseDownloader,
+        downloader: SourcePlugin,
         dry_run: bool,
     ) -> FileHandlerTransactionLog:
         with self._subscription_download_context_managers():
             for entry in downloader.download_metadata():
                 if (entry := self._preprocess_entry(plugins=plugins, entry=entry)) is None:
                     continue
 
@@ -336,15 +336,15 @@
             plugins=plugins,
             enhanced_download_archive=self._enhanced_download_archive,
             working_directory=self.working_directory,
             dry_run=dry_run,
         )
 
         downloader = self.downloader_class(
-            download_options=self.downloader_options,
+            options=self.downloader_options,
             enhanced_download_archive=self._enhanced_download_archive,
             download_ytdl_options=subscription_ytdl_options.download_builder(),
             metadata_ytdl_options=subscription_ytdl_options.metadata_builder(),
             overrides=self.overrides,
         )
 
         return self._process_subscription(
@@ -362,15 +362,15 @@
         dry_run
             If true, do not modify any video/audio files or move anything to the output directory.
         """
         self._enhanced_download_archive.reinitialize(dry_run=dry_run)
         plugins = self._initialize_plugins()
 
         downloader = InfoJsonDownloader(
-            download_options=InfoJsonDownloaderOptions(name="no-op", value={}),
+            options=InfoJsonDownloaderOptions(name="no-op", value={}),
             enhanced_download_archive=self._enhanced_download_archive,
             download_ytdl_options=YTDLOptionsBuilder(),
             metadata_ytdl_options=YTDLOptionsBuilder(),
             overrides=self.overrides,
         )
 
         return self._process_subscription(
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset import Preset
-from ytdl_sub.downloaders.base_downloader import BaseDownloader
+from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.plugins.audio_extract import AudioExtractPlugin
 from ytdl_sub.plugins.chapters import ChaptersPlugin
 from ytdl_sub.plugins.date_range import DateRangePlugin
 from ytdl_sub.plugins.file_convert import FileConvertPlugin
 from ytdl_sub.plugins.match_filters import MatchFiltersPlugin
 from ytdl_sub.plugins.subtitles import SubtitlesPlugin
@@ -39,15 +39,15 @@
     def _get_plugin(self, plugin_type: Type[PluginT]) -> Optional[PluginT]:
         for plugin in self._plugins:
             if isinstance(plugin, plugin_type):
                 return plugin
         return None
 
     @property
-    def _downloader(self) -> Type[BaseDownloader]:
+    def _downloader(self) -> Type[SourcePlugin]:
         return self._preset.downloader
 
     @property
     def _global_options(self) -> Dict:
         """
         Returns
         -------
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post4
+Version: 2023.7.25.post5
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 src/ytdl_sub/config/config_validator.py
 src/ytdl_sub/config/defaults.py
 src/ytdl_sub/config/plugin.py
 src/ytdl_sub/config/preset.py
 src/ytdl_sub/config/preset_class_mappings.py
 src/ytdl_sub/config/preset_options.py
 src/ytdl_sub/downloaders/__init__.py
-src/ytdl_sub/downloaders/base_downloader.py
-src/ytdl_sub/downloaders/downloader_validator.py
+src/ytdl_sub/downloaders/source_plugin.py
 src/ytdl_sub/downloaders/ytdl_options_builder.py
 src/ytdl_sub/downloaders/ytdlp.py
 src/ytdl_sub/downloaders/info_json/__init__.py
 src/ytdl_sub/downloaders/info_json/info_json_downloader.py
 src/ytdl_sub/downloaders/url/__init__.py
 src/ytdl_sub/downloaders/url/downloader.py
 src/ytdl_sub/downloaders/url/multi_url.py
+src/ytdl_sub/downloaders/url/multi_url_source_options_validator.py
 src/ytdl_sub/downloaders/url/url.py
 src/ytdl_sub/downloaders/url/validators.py
 src/ytdl_sub/entries/__init__.py
 src/ytdl_sub/entries/base_entry.py
 src/ytdl_sub/entries/entry.py
 src/ytdl_sub/entries/entry_parent.py
 src/ytdl_sub/entries/variables/__init__.py
```

