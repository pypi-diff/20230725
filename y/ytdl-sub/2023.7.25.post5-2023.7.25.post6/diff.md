# Comparing `tmp/ytdl-sub-2023.7.25.post5.tar.gz` & `tmp/ytdl-sub-2023.7.25.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.25.post5.tar", last modified: Tue Jul 25 19:39:16 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.25.post6.tar", last modified: Tue Jul 25 21:05:45 2023, max compression
```

## Comparing `ytdl-sub-2023.7.25.post5.tar` & `ytdl-sub-2023.7.25.post6.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.521696 ytdl-sub-2023.7.25.post5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.525696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 19:38:56.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.529696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.529696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.533696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.533696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.533696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url_source_options_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.537696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.537696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.541696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.545696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.545696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.545696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.549697 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.553696 ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 19:38:55.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:39:16.529696 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:39:16.000000 ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.752559 ytdl-sub-2023.7.25.post6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 21:05:45.752559 ytdl-sub-2023.7.25.post6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 21:05:45.756559 ytdl-sub-2023.7.25.post6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.716559 ytdl-sub-2023.7.25.post6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.720559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 21:05:21.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.724559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.728559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.728559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.728559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.732559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/multi_url_source_options_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.732559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.732559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.740559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.740559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.740559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.740559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.740559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.744559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.744559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15121 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.744559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.748559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.752559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.752559 ytdl-sub-2023.7.25.post6/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 21:05:20.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:05:45.724559 ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 21:05:45.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-25 21:05:45.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:05:45.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 21:05:45.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 21:05:45.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 21:05:45.000000 ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.25.post5/LICENSE` & `ytdl-sub-2023.7.25.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/PKG-INFO` & `ytdl-sub-2023.7.25.post6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post5
+Version: 2023.7.25.post6
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post5/README.md` & `ytdl-sub-2023.7.25.post6/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/pyproject.toml` & `ytdl-sub-2023.7.25.post6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/setup.cfg` & `ytdl-sub-2023.7.25.post6/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/plugin.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     MODIFY_ENTRY_AFTER_SPLIT = 10
 
     # if post_process is >= to this value, run after file_convert
     POST_PROCESS_AFTER_FILE_CONVERT = 10
 
     MODIFY_ENTRY_FIRST = 0
 
-    def __init__(self, modify_entry: int = 5, post_process: int = 5):
+    def __init__(
+        self, modify_entry_metadata: int = 5, modify_entry: int = 5, post_process: int = 5
+    ):
+        self.modify_entry_metadata = modify_entry_metadata
         self.modify_entry = modify_entry
         self.post_process = post_process
 
     @property
     def modify_entry_after_split(self) -> bool:
         """
         Returns
```

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import abc
 from abc import ABC
+from typing import Dict
 from typing import Generic
 from typing import Iterable
 from typing import List
+from typing import Optional
+from typing import Type
+from typing import final
 
 from ytdl_sub.config.plugin import BasePlugin
 from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import TOptionsValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
@@ -15,16 +19,26 @@
 
 class SourcePluginExtension(Plugin[TOptionsValidator], ABC):
     """
     Plugins that get added automatically by using a downloader. Downloader options
     are the plugin options.
     """
 
+    @final
+    def ytdl_options(self) -> Optional[Dict]:
+        """
+        SourcePluginExtensions are intended to run after downloading. ytdl_options at that point
+        are not needed.
+        """
+        return None
+
 
 class SourcePlugin(BasePlugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
+    plugin_extensions: List[Type[SourcePluginExtension]] = []
+
     def __init__(
         self,
         options: TOptionsValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
@@ -41,19 +55,18 @@
     def download_metadata(self) -> Iterable[Entry]:
         """Gathers metadata of all entries to download"""
 
     @abc.abstractmethod
     def download(self, entry: Entry) -> Entry:
         """The function to perform the download of all media entries"""
 
-    # pylint: disable=unused-argument
-    @classmethod
-    def added_plugins(
-        cls,
-        downloader_options: TOptionsValidator,
-        enhanced_download_archive: EnhancedDownloadArchive,
-        overrides: Overrides,
-    ) -> List[SourcePluginExtension]:
+    @final
+    def added_plugins(self) -> List[SourcePluginExtension]:
         """Add these plugins from the Downloader to the subscription"""
-        return []
-
-    # pylint: enable=unused-argument
+        return [
+            plugin_extension(
+                options=self.plugin_options,
+                overrides=self.overrides,
+                enhanced_download_archive=self._enhanced_download_archive,
+            )
+            for plugin_extension in self.plugin_extensions
+        ]
```

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
 from yt_dlp.utils import RejectedVideoReached
 
-from ytdl_sub.config.plugin import Plugin
+from ytdl_sub.config.plugin import PluginPriority
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.downloaders.source_plugin import SourcePlugin
 from ytdl_sub.downloaders.source_plugin import SourcePluginExtension
 from ytdl_sub.downloaders.url.multi_url_source_options_validator import (
     MultiUrlSourceOptionsValidator,
 )
 from ytdl_sub.downloaders.url.multi_url_source_options_validator import (
@@ -51,14 +51,16 @@
 class URLDownloadState:
     def __init__(self, entries_total: int):
         self.entries_total = entries_total
         self.entries_downloaded = 0
 
 
 class UrlDownloaderThumbnailPlugin(SourcePluginExtension):
+    priority = PluginPriority(modify_entry=0)
+
     def __init__(
         self,
         options: MultiUrlSourceOptionsValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
@@ -150,29 +152,31 @@
                 collection_url=self._collection_url_mapping[entry.kwargs(COLLECTION_URL)],
                 entry=entry,
             )
         return entry
 
 
 class UrlDownloaderCollectionVariablePlugin(SourcePluginExtension):
+    priority = PluginPriority(modify_entry_metadata=0)
+
     def __init__(
         self,
-        downloader_options: MultiUrlSourceOptionsValidator,
+        options: MultiUrlSourceOptionsValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
-            options=downloader_options,
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
 
     def modify_entry_metadata(self, entry: Entry) -> Optional[Entry]:
         """
         Add collection variables to the entry
         """
         # COLLECTION_URL is a recent variable that may not exist for old entries when updating.
@@ -192,38 +196,15 @@
 
 class BaseUrlDownloader(SourcePlugin[TMultiURLSourceOptionsValidator], ABC):
     """
     Class that interacts with ytdl to perform the download of metadata and content,
     and should translate that to list of Entry objects.
     """
 
-    @classmethod
-    def added_plugins(
-        cls,
-        downloader_options: TMultiURLSourceOptionsValidator,
-        enhanced_download_archive: EnhancedDownloadArchive,
-        overrides: Overrides,
-    ) -> List[Plugin]:
-        """
-        Adds
-        1. URL thumbnail download plugin
-        2. Collection variable plugin to add to each entry
-        """
-        return [
-            UrlDownloaderThumbnailPlugin(
-                options=downloader_options,
-                overrides=overrides,
-                enhanced_download_archive=enhanced_download_archive,
-            ),
-            UrlDownloaderCollectionVariablePlugin(
-                downloader_options=downloader_options,
-                overrides=overrides,
-                enhanced_download_archive=enhanced_download_archive,
-            ),
-        ]
+    plugin_extensions = [UrlDownloaderThumbnailPlugin, UrlDownloaderCollectionVariablePlugin]
 
     @classmethod
     def ytdl_option_defaults(cls) -> Dict:
         """
         .. code-block:: yaml
 
            ytdl_options:
```

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/multi_url_source_options_validator.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/multi_url_source_options_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,42 +170,33 @@
 
     def _initialize_plugins(self) -> List[Plugin]:
         """
         Returns
         -------
         List of plugins defined in the subscription, initialized and ready to use.
         """
-        # Always add plugins provided by the downloader
-        plugins: List[Plugin] = self.downloader_class.added_plugins(
-            downloader_options=self.downloader_options,
-            enhanced_download_archive=self._enhanced_download_archive,
-            overrides=self.overrides,
-        )
-
-        for plugin_type, plugin_options in self.plugins.zipped():
-            plugin = plugin_type(
+        return [
+            plugin_type(
                 options=plugin_options,
                 overrides=self.overrides,
                 enhanced_download_archive=self._enhanced_download_archive,
             )
-
-            plugins.append(plugin)
-
-        return plugins
+            for plugin_type, plugin_options in self.plugins.zipped()
+        ]
 
     @classmethod
     def _cleanup_entry_files(cls, entry: Entry):
         FileHandler.delete(entry.get_download_file_path())
         FileHandler.delete(entry.get_download_thumbnail_path())
         FileHandler.delete(entry.get_download_info_json_path())
 
     @classmethod
     def _preprocess_entry(cls, plugins: List[Plugin], entry: Entry) -> Optional[Entry]:
         maybe_entry: Optional[Entry] = entry
-        for plugin in plugins:
+        for plugin in sorted(plugins, key=lambda _plugin: _plugin.priority.modify_entry_metadata):
             if (maybe_entry := plugin.modify_entry_metadata(maybe_entry)) is None:
                 return None
 
         return maybe_entry
 
     def _post_process_entry(
         self, plugins: List[Plugin], dry_run: bool, entry: Entry, entry_metadata: FileMetadata
@@ -343,14 +334,16 @@
             options=self.downloader_options,
             enhanced_download_archive=self._enhanced_download_archive,
             download_ytdl_options=subscription_ytdl_options.download_builder(),
             metadata_ytdl_options=subscription_ytdl_options.metadata_builder(),
             overrides=self.overrides,
         )
 
+        plugins.extend(downloader.added_plugins())
+
         return self._process_subscription(
             plugins=plugins,
             downloader=downloader,
             dry_run=dry_run,
         )
 
     def update_with_info_json(self, dry_run: bool = False) -> FileHandlerTransactionLog:
@@ -361,14 +354,33 @@
         ----------
         dry_run
             If true, do not modify any video/audio files or move anything to the output directory.
         """
         self._enhanced_download_archive.reinitialize(dry_run=dry_run)
         plugins = self._initialize_plugins()
 
+        subscription_ytdl_options = SubscriptionYTDLOptions(
+            preset=self._preset_options,
+            plugins=plugins,
+            enhanced_download_archive=self._enhanced_download_archive,
+            working_directory=self.working_directory,
+            dry_run=dry_run,
+        )
+
+        # Re-add the original downloader class' plugins
+        plugins.extend(
+            self.downloader_class(
+                options=self.downloader_options,
+                enhanced_download_archive=self._enhanced_download_archive,
+                download_ytdl_options=subscription_ytdl_options.download_builder(),
+                metadata_ytdl_options=subscription_ytdl_options.metadata_builder(),
+                overrides=self.overrides,
+            ).added_plugins()
+        )
+
         downloader = InfoJsonDownloader(
             options=InfoJsonDownloaderOptions(name="no-op", value={}),
             enhanced_download_archive=self._enhanced_download_archive,
             download_ytdl_options=YTDLOptionsBuilder(),
             metadata_ytdl_options=YTDLOptionsBuilder(),
             overrides=self.overrides,
         )
```

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post5
+Version: 2023.7.25.post6
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post5/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.25.post6/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

