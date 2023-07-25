# Comparing `tmp/ytdl-sub-2023.7.25.post2.tar.gz` & `tmp/ytdl-sub-2023.7.25.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.25.post2.tar", last modified: Tue Jul 25 07:16:18 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.25.post3.tar", last modified: Tue Jul 25 07:38:50 2023, max compression
```

## Comparing `ytdl-sub-2023.7.25.post2.tar` & `ytdl-sub-2023.7.25.post3.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.413833 ytdl-sub-2023.7.25.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 07:15:55.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.429833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 07:38:50.326462 ytdl-sub-2023.7.25.post3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.298462 ytdl-sub-2023.7.25.post3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.302462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.302462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/downloader_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.310462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.310462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.318462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.318462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.302462 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.25.post2/LICENSE` & `ytdl-sub-2023.7.25.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/PKG-INFO` & `ytdl-sub-2023.7.25.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post2
+Version: 2023.7.25.post3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post2/README.md` & `ytdl-sub-2023.7.25.post3/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/pyproject.toml` & `ytdl-sub-2023.7.25.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/setup.cfg` & `ytdl-sub-2023.7.25.post3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
 from ytdl_sub.config.config_validator import ConfigValidator
 from ytdl_sub.config.preset_class_mappings import DownloadStrategyMapping
 from ytdl_sub.config.preset_class_mappings import PluginMapping
 from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import Overrides
+from ytdl_sub.config.preset_options import TOptionsValidator
 from ytdl_sub.config.preset_options import YTDLOptions
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
-from ytdl_sub.downloaders.base_downloader import BaseDownloaderValidator
+from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptionsT
 from ytdl_sub.prebuilt_presets import PREBUILT_PRESET_NAMES
 from ytdl_sub.prebuilt_presets import PUBLISHED_PRESET_NAMES
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.yaml import dump_yaml
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
@@ -81,15 +81,15 @@
         """
         Returns
         -------
         Plugin and PluginOptions zipped
         """
         return zip(self.plugin_types, self.plugin_options)
 
-    def get(self, plugin_type: Type[PluginOptionsT]) -> Optional[PluginOptionsT]:
+    def get(self, plugin_type: Type[TOptionsValidator]) -> Optional[TOptionsValidator]:
         """
         Parameters
         ----------
         plugin_type
             Fetch the plugin options for this type
 
         Returns
@@ -273,27 +273,27 @@
     def __validate_and_get_downloader(self, downloader_source: str) -> Type[BaseDownloader]:
         return self._validate_key(key=downloader_source, validator=DownloadStrategyValidator).get(
             downloader_source=downloader_source
         )
 
     def __validate_and_get_downloader_options(
         self, downloader_source: str, downloader: Type[BaseDownloader]
-    ) -> BaseDownloaderValidator:
+    ) -> DownloaderValidator:
         # Remove the download_strategy key before validating it against the downloader options
         # TODO: make this cleaner
         del self._dict[downloader_source]["download_strategy"]
         return self._validate_key(
             key=downloader_source, validator=downloader.downloader_options_type
         )
 
     def __validate_and_get_downloader_and_options(
         self,
-    ) -> Tuple[Type[BaseDownloader], BaseDownloaderValidator]:
+    ) -> Tuple[Type[BaseDownloader], DownloaderValidator]:
         downloader: Optional[Type[BaseDownloader]] = None
-        download_options: Optional[BaseDownloaderValidator] = None
+        download_options: Optional[DownloaderValidator] = None
         downloader_sources = DownloadStrategyMapping.sources()
 
         for key in self._keys:
             # skip if the key is not a download source
             if key not in downloader_sources:
                 continue
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import TypeVar
 
 from yt_dlp.utils import sanitize_filename
 
 from ytdl_sub.config.defaults import DEFAULT_DOWNLOAD_ARCHIVE_NAME
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.validators.file_path_validators import OverridesStringFormatterFilePathValidator
@@ -67,14 +68,17 @@
             Available source variables when running the plugin
         override_variables
             Available override variables when running the plugin
         """
         return None
 
 
+TOptionsValidator = TypeVar("TOptionsValidator", bound=OptionsValidator)
+
+
 class OptionsDictValidator(StrictDictValidator, OptionsValidator, ABC):
     pass
 
 
 # pylint: enable=no-self-use
 # pylint: enable=unused-argument
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 import abc
 from abc import ABC
 from typing import Generic
 from typing import Iterable
 from typing import List
 from typing import Type
-from typing import TypeVar
 
-from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.config.preset_options import Overrides
+from ytdl_sub.config.preset_options import TOptionsValidator
+from ytdl_sub.downloaders.downloader_validator import TDownloaderValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadArchiver
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
-BaseDownloaderValidator = OptionsDictValidator
-BaseDownloaderOptionsT = TypeVar("BaseDownloaderOptionsT", bound=BaseDownloaderValidator)
 
-
-class BaseDownloaderPlugin(Plugin[BaseDownloaderOptionsT], ABC):
+class BaseDownloaderPlugin(Plugin[TDownloaderValidator], ABC):
     """
     Plugins that get added automatically by using a downloader. Downloader options
     are the plugin options.
     """
 
     def __init__(
         self,
-        downloader_options: BaseDownloaderOptionsT,
+        downloader_options: TDownloaderValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
             # Downloader plugins use download options as their plugin options
             plugin_options=downloader_options,
             overrides=overrides,
             enhanced_download_archive=enhanced_download_archive,
         )
 
 
-class BaseDownloader(DownloadArchiver, Generic[BaseDownloaderOptionsT], ABC):
-    downloader_options_type: Type[BaseDownloaderOptionsT]
+class BaseDownloader(DownloadArchiver, Generic[TOptionsValidator], ABC):
+    downloader_options_type: Type[TOptionsValidator]
 
     def __init__(
         self,
-        download_options: BaseDownloaderOptionsT,
+        download_options: TOptionsValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
     ):
         super().__init__(enhanced_download_archive=enhanced_download_archive)
         self.download_options = download_options
@@ -63,15 +60,15 @@
     def download(self, entry: Entry) -> Entry:
         """The function to perform the download of all media entries"""
 
     # pylint: disable=unused-argument
     @classmethod
     def added_plugins(
         cls,
-        downloader_options: BaseDownloaderOptionsT,
+        downloader_options: TOptionsValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         overrides: Overrides,
     ) -> List[BaseDownloaderPlugin]:
         """Add these plugins from the Downloader to the subscription"""
         return []
 
     # pylint: enable=unused-argument
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import copy
 import json
 from pathlib import Path
 from typing import Dict
 from typing import Iterable
 from typing import List
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
-from ytdl_sub.downloaders.base_downloader import BaseDownloaderOptionsT
-from ytdl_sub.downloaders.base_downloader import BaseDownloaderValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import get_file_extension
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadMapping
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
-class InfoJsonDownloaderOptions(BaseDownloaderValidator):
+class InfoJsonDownloaderOptions(OptionsDictValidator):
     _optional_keys = {"no-op"}
 
 
 class InfoJsonDownloader(BaseDownloader[InfoJsonDownloaderOptions]):
     downloader_options_type = InfoJsonDownloaderOptions
 
     def __init__(
         self,
-        download_options: BaseDownloaderOptionsT,
+        download_options: InfoJsonDownloaderOptions,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
     ):
         super().__init__(
             download_options=download_options,
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import abc
 import contextlib
 import os
 from abc import ABC
 from pathlib import Path
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
@@ -11,17 +10,17 @@
 from typing import Set
 from typing import Tuple
 
 from yt_dlp.utils import RejectedVideoReached
 
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
-from ytdl_sub.downloaders.base_downloader import BaseDownloaderOptionsT
 from ytdl_sub.downloaders.base_downloader import BaseDownloaderPlugin
-from ytdl_sub.downloaders.base_downloader import BaseDownloaderValidator
+from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
+from ytdl_sub.downloaders.downloader_validator import TDownloaderValidator
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 from ytdl_sub.downloaders.url.validators import UrlThumbnailListValidator
 from ytdl_sub.downloaders.url.validators import UrlValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.downloaders.ytdlp import YTDLP
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.entry_parent import EntryParent
@@ -41,48 +40,14 @@
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.utils.thumbnail import download_and_convert_url_thumbnail
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 download_logger = Logger.get(name="downloader")
 
 
-class DownloaderValidator(BaseDownloaderValidator, ABC):
-    """
-    Placeholder class to define downloader options
-    """
-
-    @property
-    @abc.abstractmethod
-    def collection_validator(self) -> MultiUrlValidator:
-        """
-        Returns
-        -------
-        MultiUrlValidator
-            To determine how the entries are downloaded
-        """
-
-    def added_source_variables(self) -> List[str]:
-        """
-        Returns
-        -------
-        Added source variables on the collection
-        """
-        return self.collection_validator.added_source_variables()
-
-    def validate_with_variables(
-        self, source_variables: List[str], override_variables: Dict[str, str]
-    ) -> None:
-        """
-        Validates any source variables added by the collection
-        """
-        self.collection_validator.validate_with_variables(
-            source_variables=source_variables, override_variables=override_variables
-        )
-
-
 class URLDownloadState:
     def __init__(self, entries_total: int):
         self.entries_total = entries_total
         self.entries_downloaded = 0
 
 
 class UrlDownloaderThumbnailPlugin(BaseDownloaderPlugin):
@@ -217,24 +182,24 @@
         )
 
         entry.add_variables(variables_to_add=collection_url.variables.dict_with_format_strings)
 
         return entry
 
 
-class BaseUrlDownloader(BaseDownloader[BaseDownloaderOptionsT], ABC):
+class BaseUrlDownloader(BaseDownloader[TDownloaderValidator], ABC):
     """
     Class that interacts with ytdl to perform the download of metadata and content,
     and should translate that to list of Entry objects.
     """
 
     @classmethod
     def added_plugins(
         cls,
-        downloader_options: BaseDownloaderOptionsT,
+        downloader_options: TDownloaderValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         overrides: Overrides,
     ) -> List[Plugin]:
         """
         Adds
         1. URL thumbnail download plugin
         2. Collection variable plugin to add to each entry
@@ -260,15 +225,15 @@
            ytdl_options:
              ignoreerrors: True  # ignore errors like hidden videos, age restriction, etc
         """
         return {"ignoreerrors": True}
 
     def __init__(
         self,
-        download_options: BaseDownloaderOptionsT,
+        download_options: TDownloaderValidator,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
     ):
         """
         Parameters
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 from typing import List
 
+from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.downloaders.url.downloader import BaseUrlDownloader
-from ytdl_sub.downloaders.url.downloader import DownloaderValidator
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 
 
 class MultiUrlDownloadOptions(MultiUrlValidator, DownloaderValidator):
     """
     Downloads from multiple URLs. If an entry is returned from more than one URL, it will
     resolve to the bottom-most URL settings.
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.downloaders.url.downloader import BaseUrlDownloader
-from ytdl_sub.downloaders.url.downloader import DownloaderValidator
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 from ytdl_sub.downloaders.url.validators import UrlValidator
 
 
 class UrlDownloadOptions(UrlValidator, DownloaderValidator):
     """
     Downloads from a single URL supported by yt-dlp.
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from abc import ABC
 from typing import Dict
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
-from typing import TypeVar
 
-from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.config.preset_options import Overrides
+from ytdl_sub.config.preset_options import TOptionsValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadArchiver
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
@@ -39,31 +38,28 @@
         Returns
         -------
         True if the plugin should modify an entry after a potential split. False otherwise.
         """
         return self.modify_entry >= PluginPriority.MODIFY_ENTRY_AFTER_SPLIT
 
 
-PluginOptionsT = TypeVar("PluginOptionsT", bound=OptionsValidator)
-
-
-class Plugin(DownloadArchiver, Generic[PluginOptionsT], ABC):
+class Plugin(DownloadArchiver, Generic[TOptionsValidator], ABC):
     """
     Class to define the new plugin functionality
     """
 
-    plugin_options_type: Type[PluginOptionsT] = NotImplemented
+    plugin_options_type: Type[TOptionsValidator] = NotImplemented
     priority: PluginPriority = PluginPriority()
 
     # If the plugin creates multiple entries from a single entry
     is_split_plugin: bool = False
 
     def __init__(
         self,
-        plugin_options: PluginOptionsT,
+        plugin_options: TOptionsValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         DownloadArchiver.__init__(self=self, enhanced_download_archive=enhanced_download_archive)
         self.plugin_options = plugin_options
         self.overrides = overrides
         # TODO pass yaml snake case name in the class somewhere, and use it for the logger
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ytdl_sub.config.config_validator import ConfigOptions
 from ytdl_sub.config.preset import Preset
 from ytdl_sub.config.preset import PresetPlugins
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import YTDLOptions
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
-from ytdl_sub.downloaders.base_downloader import BaseDownloaderValidator
+from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
 class BaseSubscription(ABC):
     """
     Subscription classes are the 'controllers' that perform...
 
@@ -57,15 +57,15 @@
         Returns
         -------
         This subscription's downloader class
         """
         return self._preset_options.downloader
 
     @property
-    def downloader_options(self) -> BaseDownloaderValidator:
+    def downloader_options(self) -> DownloaderValidator:
         """
         Returns
         -------
         The download options for this subscription's downloader
         """
         return self._preset_options.downloader_options
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post2
+Version: 2023.7.25.post3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/ytdl_sub/config/config_validator.py
 src/ytdl_sub/config/defaults.py
 src/ytdl_sub/config/preset.py
 src/ytdl_sub/config/preset_class_mappings.py
 src/ytdl_sub/config/preset_options.py
 src/ytdl_sub/downloaders/__init__.py
 src/ytdl_sub/downloaders/base_downloader.py
+src/ytdl_sub/downloaders/downloader_validator.py
 src/ytdl_sub/downloaders/ytdl_options_builder.py
 src/ytdl_sub/downloaders/ytdlp.py
 src/ytdl_sub/downloaders/info_json/__init__.py
 src/ytdl_sub/downloaders/info_json/info_json_downloader.py
 src/ytdl_sub/downloaders/url/__init__.py
 src/ytdl_sub/downloaders/url/downloader.py
 src/ytdl_sub/downloaders/url/multi_url.py
```

