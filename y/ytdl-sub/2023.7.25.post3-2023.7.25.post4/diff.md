# Comparing `tmp/ytdl-sub-2023.7.25.post3.tar.gz` & `tmp/ytdl-sub-2023.7.25.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.25.post3.tar", last modified: Tue Jul 25 07:38:50 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.25.post4.tar", last modified: Tue Jul 25 19:13:26 2023, max compression
```

## Comparing `ytdl-sub-2023.7.25.post3.tar` & `ytdl-sub-2023.7.25.post4.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 07:38:50.326462 ytdl-sub-2023.7.25.post3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.298462 ytdl-sub-2023.7.25.post3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.302462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.302462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/downloader_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.306462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.310462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.310462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.314462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.318462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.318462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.322462 ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 07:38:22.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:38:50.302462 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 07:38:50.000000 ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.906962 ytdl-sub-2023.7.25.post4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.910962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.910962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/downloader_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.914962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20898 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.918962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.918962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.922962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.926962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.926962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.930962 ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 19:12:57.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:13:26.910962 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:13:26.000000 ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.25.post3/LICENSE` & `ytdl-sub-2023.7.25.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/PKG-INFO` & `ytdl-sub-2023.7.25.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post3
+Version: 2023.7.25.post4
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post3/README.md` & `ytdl-sub-2023.7.25.post4/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/pyproject.toml` & `ytdl-sub-2023.7.25.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/setup.cfg` & `ytdl-sub-2023.7.25.post4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 from mergedeep import mergedeep
 
 from ytdl_sub.config.config_validator import ConfigValidator
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_class_mappings import DownloadStrategyMapping
 from ytdl_sub.config.preset_class_mappings import PluginMapping
 from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import TOptionsValidator
 from ytdl_sub.config.preset_options import YTDLOptions
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.prebuilt_presets import PREBUILT_PRESET_NAMES
 from ytdl_sub.prebuilt_presets import PUBLISHED_PRESET_NAMES
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.yaml import dump_yaml
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Dict
 from typing import List
 from typing import Type
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.url.multi_url import MultiUrlDownloader
 from ytdl_sub.downloaders.url.url import UrlDownloader
 from ytdl_sub.plugins.audio_extract import AudioExtractPlugin
 from ytdl_sub.plugins.chapters import ChaptersPlugin
 from ytdl_sub.plugins.date_range import DateRangePlugin
 from ytdl_sub.plugins.embed_thumbnail import EmbedThumbnailPlugin
 from ytdl_sub.plugins.file_convert import FileConvertPlugin
 from ytdl_sub.plugins.internal.view import ViewPlugin
 from ytdl_sub.plugins.match_filters import MatchFiltersPlugin
 from ytdl_sub.plugins.music_tags import MusicTagsPlugin
 from ytdl_sub.plugins.nfo_tags import NfoTagsPlugin
 from ytdl_sub.plugins.output_directory_nfo_tags import OutputDirectoryNfoTagsPlugin
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.plugins.regex import RegexPlugin
 from ytdl_sub.plugins.split_by_chapters import SplitByChaptersPlugin
 from ytdl_sub.plugins.subtitles import SubtitlesPlugin
 from ytdl_sub.plugins.video_tags import VideoTagsPlugin
 
 
 class DownloadStrategyMapping:
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import abc
 from abc import ABC
 from typing import Generic
 from typing import Iterable
 from typing import List
 from typing import Type
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import TOptionsValidator
 from ytdl_sub.downloaders.downloader_validator import TDownloaderValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadArchiver
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
 class BaseDownloaderPlugin(Plugin[TDownloaderValidator], ABC):
     """
     Plugins that get added automatically by using a downloader. Downloader options
@@ -25,15 +25,15 @@
         self,
         downloader_options: TDownloaderValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         super().__init__(
             # Downloader plugins use download options as their plugin options
-            plugin_options=downloader_options,
+            options=downloader_options,
             overrides=overrides,
             enhanced_download_archive=enhanced_download_archive,
         )
 
 
 class BaseDownloader(DownloadArchiver, Generic[TOptionsValidator], ABC):
     downloader_options_type: Type[TOptionsValidator]
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/downloader_validator.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/downloader_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
 from yt_dlp.utils import RejectedVideoReached
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.base_downloader import BaseDownloaderPlugin
 from ytdl_sub.downloaders.downloader_validator import DownloaderValidator
 from ytdl_sub.downloaders.downloader_validator import TDownloaderValidator
 from ytdl_sub.downloaders.url.validators import MultiUrlValidator
 from ytdl_sub.downloaders.url.validators import UrlThumbnailListValidator
@@ -29,15 +30,14 @@
 from ytdl_sub.entries.variables.kwargs import DOWNLOAD_INDEX
 from ytdl_sub.entries.variables.kwargs import PLAYLIST_ENTRY
 from ytdl_sub.entries.variables.kwargs import REQUESTED_SUBTITLES
 from ytdl_sub.entries.variables.kwargs import SOURCE_ENTRY
 from ytdl_sub.entries.variables.kwargs import SPONSORBLOCK_CHAPTERS
 from ytdl_sub.entries.variables.kwargs import UPLOAD_DATE_INDEX
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_MATCH_FILTER_REJECT
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.thumbnail import ThumbnailTypes
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.utils.thumbnail import download_and_convert_url_thumbnail
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/audio_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os.path
 from typing import Any
 from typing import Dict
 from typing import Optional
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.exceptions import FileNotDownloadedException
 from ytdl_sub.validators.audo_codec_validator import AUDIO_CODEC_TYPES_EXTENSION_MAPPING
 from ytdl_sub.validators.audo_codec_validator import AudioTypeValidator
 from ytdl_sub.validators.validators import FloatValidator
 
 
 class AudioExtractOptions(OptionsDictValidator):
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/chapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import collections
 import re
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import COMMENTS
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_CUSTOM_CHAPTERS
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.chapters import Chapters
 from ytdl_sub.utils.ffmpeg import set_ffmpeg_metadata_chapters
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.validators.regex_validator import RegexListValidator
 from ytdl_sub.validators.string_select_validator import StringSelectValidator
 from ytdl_sub.validators.validators import BoolValidator
 from ytdl_sub.validators.validators import ListValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/date_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict
 from typing import Optional
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.datetime import to_date_range
 from ytdl_sub.validators.string_datetime import StringDatetimeValidator
 
 
 class DateRangeOptions(OptionsDictValidator):
     """
     Only download files uploaded within the specified date range.
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
 from typing import Optional
 
 import mediafile
 
+from ytdl_sub.config.plugin import Plugin
+from ytdl_sub.config.plugin import PluginPriority
 from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.validators.audo_codec_validator import AUDIO_CODEC_EXTS
 from ytdl_sub.validators.validators import BoolValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/file_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from typing import Any
 from typing import Dict
 from typing import Optional
 
+from ytdl_sub.config.plugin import Plugin
+from ytdl_sub.config.plugin import PluginPriority
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import EXT
-from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.exceptions import FileNotDownloadedException
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.validators.audo_codec_validator import FileTypeValidator
 from ytdl_sub.validators.string_formatter_validators import OverridesStringFormatterValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/internal/view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import copy
 from typing import Optional
 
+from ytdl_sub.config.plugin import Plugin
+from ytdl_sub.config.plugin import PluginPriority
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.output_directory_nfo_tags import OutputDirectoryNfoTagsOptions
-from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
 class ViewOptions(OptionsDictValidator):
     """
     INTERNAL PLUGIN. Do not expose in documentation
@@ -23,19 +22,23 @@
     plugin_options_type = ViewOptions
     priority: PluginPriority = PluginPriority(modify_entry=PluginPriority.MODIFY_ENTRY_AFTER_SPLIT)
 
     _MAX_LINE_WIDTH: int = 80
 
     def __init__(
         self,
-        plugin_options: OutputDirectoryNfoTagsOptions,
+        options: ViewOptions,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
-        super().__init__(plugin_options, overrides, enhanced_download_archive)
+        super().__init__(
+            options=options,
+            overrides=overrides,
+            enhanced_download_archive=enhanced_download_archive,
+        )
         self._first_entry: Optional[Entry] = None
 
     @classmethod
     def _truncate_value(cls, value: str) -> str:
         """No new lines and cut off after 80 characters"""
         value = " <newline> ".join(str(value).split("\n"))
         if len(value) > cls._MAX_LINE_WIDTH:
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/match_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from yt_dlp import match_filter_func
 
+from ytdl_sub.config.plugin import Plugin
+from ytdl_sub.config.plugin import PluginPriority
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_MATCH_FILTER_REJECT
-from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.validators import StringListValidator
 
 logger = Logger.get("match_filters")
 
 
 class MatchFiltersOptions(OptionsDictValidator):
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/music_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from collections import defaultdict
 from typing import Any
 from typing import Dict
 from typing import List
 
 import mediafile
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.validators.audo_codec_validator import AUDIO_CODEC_EXTS
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import ListFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from collections import defaultdict
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.xml import XmlElement
 from ytdl_sub.utils.xml import to_max_3_byte_utf8_dict
 from ytdl_sub.utils.xml import to_max_3_byte_utf8_string
 from ytdl_sub.utils.xml import to_xml
 from ytdl_sub.validators.file_path_validators import StringFormatterFileNameValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,19 +89,19 @@
 
 
 class OutputDirectoryNfoTagsPlugin(SharedNfoTagsPlugin):
     plugin_options_type = OutputDirectoryNfoTagsOptions
 
     def __init__(
         self,
-        plugin_options: OutputDirectoryNfoTagsOptions,
+        options: OutputDirectoryNfoTagsOptions,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
-        super().__init__(plugin_options, overrides, enhanced_download_archive)
+        super().__init__(options, overrides, enhanced_download_archive)
         self._last_entry: Optional[Entry] = None
 
     def post_process_entry(self, entry: Entry) -> None:
         """
         Tracks the last entry processed
         """
         self._last_entry = entry
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/config/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from abc import ABC
+from abc import abstractmethod
 from typing import Dict
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import TOptionsValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.file_handler import FileMetadata
-from ytdl_sub.utils.logger import Logger
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadArchiver
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
 class PluginPriority:
     """
     Defines priority for plugins, 0 is highest priority
@@ -38,61 +38,48 @@
         Returns
         -------
         True if the plugin should modify an entry after a potential split. False otherwise.
         """
         return self.modify_entry >= PluginPriority.MODIFY_ENTRY_AFTER_SPLIT
 
 
-class Plugin(DownloadArchiver, Generic[TOptionsValidator], ABC):
+# pylint: disable=no-self-use,unused-argument
+
+
+class BasePlugin(DownloadArchiver, Generic[TOptionsValidator], ABC):
     """
-    Class to define the new plugin functionality
+    Shared code amongst all SourcePlugins (downloaders) and Plugins (post-download modification)
     """
 
-    plugin_options_type: Type[TOptionsValidator] = NotImplemented
     priority: PluginPriority = PluginPriority()
-
-    # If the plugin creates multiple entries from a single entry
-    is_split_plugin: bool = False
+    plugin_options_type: Type[TOptionsValidator]
 
     def __init__(
         self,
-        plugin_options: TOptionsValidator,
+        options: TOptionsValidator,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         DownloadArchiver.__init__(self=self, enhanced_download_archive=enhanced_download_archive)
-        self.plugin_options = plugin_options
+        self.plugin_options = options
         self.overrides = overrides
-        # TODO pass yaml snake case name in the class somewhere, and use it for the logger
-        self._logger = Logger.get(self.__class__.__name__)
 
-    # pylint: disable=no-self-use,unused-argument
+
+class Plugin(BasePlugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
+    """
+    Class to define the new plugin functionality
+    """
+
     def ytdl_options(self) -> Optional[Dict]:
         """
         Returns
         -------
         ytdl options to enable/disable when downloading entries for this specific plugin
         """
 
-    def split(self, entry: Entry) -> List[Tuple[Entry, FileMetadata]]:
-        """
-        Very specialized function that takes an entry and creates multiple entries from it.
-        Should mark ``is_split_plugin`` on the plugin class.
-
-        Parameters
-        ----------
-        entry
-            Entry to create multiple entries from
-
-        Returns
-        -------
-        List of entries and metadata created from the source entry
-        """
-        return []
-
     def modify_entry_metadata(self, entry: Entry) -> Optional[Entry]:
         """
         After entry metadata has been gathered, perform preprocessing on the metadata
 
         Parameters
         ----------
         entry
@@ -131,13 +118,34 @@
 
         Returns
         -------
         Optional file metadata for the entry media file.
         """
         return None
 
-    # pylint: enable=no-self-use,unused-argument
-
     def post_process_subscription(self):
         """
         After all downloaded files have been post-processed, apply a subscription-wide post process
         """
+
+
+class SplitPlugin(Plugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
+    """
+    Plugin that splits entries into zero or more entries
+    """
+
+    @abstractmethod
+    def split(self, entry: Entry) -> List[Tuple[Entry, FileMetadata]]:
+        """
+        Very specialized function that takes an entry and creates multiple entries from it.
+        Should mark ``is_split_plugin`` on the plugin class.
+
+        Parameters
+        ----------
+        entry
+            Entry to create multiple entries from
+
+        Returns
+        -------
+        List of entries and metadata created from the source entry
+        """
+        return []
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from yt_dlp.utils import sanitize_filename
 
+from ytdl_sub.config.plugin import Plugin
+from ytdl_sub.config.plugin import PluginPriority
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_REGEX_SOURCE_VARS
-from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.exceptions import RegexNoMatchException
 from ytdl_sub.utils.exceptions import StringFormattingVariableNotFoundException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.regex_validator import RegexListValidator
 from ytdl_sub.validators.source_variable_validator import SourceVariableNameListValidator
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import ListFormatterValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from yt_dlp.utils import sanitize_filename
 
+from ytdl_sub.config.plugin import SplitPlugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import CHAPTERS
 from ytdl_sub.entries.variables.kwargs import SPLIT_BY_CHAPTERS_PARENT_ENTRY
 from ytdl_sub.entries.variables.kwargs import SPONSORBLOCK_CHAPTERS
 from ytdl_sub.entries.variables.kwargs import UID
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.chapters import Chapters
 from ytdl_sub.utils.chapters import Timestamp
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
@@ -97,17 +97,16 @@
         """
         Behavior to perform when no chapters are present. Supports "pass" (continue processing),
         "drop" (exclude it from output), and "error" (stop processing for everything).
         """
         return self._when_no_chapters
 
 
-class SplitByChaptersPlugin(Plugin[SplitByChaptersOptions]):
+class SplitByChaptersPlugin(SplitPlugin[SplitByChaptersOptions]):
     plugin_options_type = SplitByChaptersOptions
-    is_split_plugin = True
 
     def _create_split_entry(
         self, source_entry: Entry, title: str, idx: int, chapters: Chapters
     ) -> Tuple[Entry, FileMetadata]:
         """
         Runs ffmpeg to create the split video
         """
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/subtitles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Optional
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.subtitles import SUBTITLE_EXTENSIONS
 from ytdl_sub.validators.file_path_validators import StringFormatterFileNameValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.string_select_validator import StringSelectValidator
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/plugins/video_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 from typing import Any
 from typing import Dict
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.utils.ffmpeg import add_ffmpeg_metadata_key_values
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
 
 logger = Logger.get("video_tags")
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 import os
 import shutil
 from abc import ABC
 from pathlib import Path
 from typing import List
 from typing import Optional
 
+from ytdl_sub.config.plugin import Plugin
+from ytdl_sub.config.plugin import SplitPlugin
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.info_json.info_json_downloader import InfoJsonDownloader
 from ytdl_sub.downloaders.info_json.info_json_downloader import InfoJsonDownloaderOptions
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.subscriptions.base_subscription import BaseSubscription
 from ytdl_sub.subscriptions.subscription_ytdl_options import SubscriptionYTDLOptions
 from ytdl_sub.utils.datetime import to_date_range
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileHandlerTransactionLog
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 
 
-def _get_split_plugin(plugins: List[Plugin]) -> Optional[Plugin]:
-    split_plugins = [plugin for plugin in plugins if plugin.is_split_plugin]
+def _get_split_plugin(plugins: List[Plugin]) -> Optional[SplitPlugin]:
+    split_plugins = [plugin for plugin in plugins if isinstance(plugin, SplitPlugin)]
 
     if len(split_plugins) == 1:
         return split_plugins[0]
     if len(split_plugins) > 1:
         raise ValidationException("Can not use more than one split plugins at a time")
     return None
 
@@ -178,15 +179,15 @@
             downloader_options=self.downloader_options,
             enhanced_download_archive=self._enhanced_download_archive,
             overrides=self.overrides,
         )
 
         for plugin_type, plugin_options in self.plugins.zipped():
             plugin = plugin_type(
-                plugin_options=plugin_options,
+                options=plugin_options,
                 overrides=self.overrides,
                 enhanced_download_archive=self._enhanced_download_archive,
             )
 
             plugins.append(plugin)
 
         return plugins
@@ -239,15 +240,15 @@
             self._post_process_entry(
                 plugins=plugins, dry_run=dry_run, entry=entry_, entry_metadata=entry_metadata
             )
 
         self._cleanup_entry_files(entry)
 
     def _process_split_entry(
-        self, split_plugin: Plugin, plugins: List[Plugin], dry_run: bool, entry: Entry
+        self, split_plugin: SplitPlugin, plugins: List[Plugin], dry_run: bool, entry: Entry
     ) -> None:
         entry_: Optional[Entry] = entry
 
         plugins_pre_split = sorted(
             [plugin for plugin in plugins if not plugin.priority.modify_entry_after_split],
             key=lambda _plugin: _plugin.priority.modify_entry,
         )
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
+from ytdl_sub.config.plugin import Plugin
 from ytdl_sub.config.preset import Preset
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.plugins.audio_extract import AudioExtractPlugin
 from ytdl_sub.plugins.chapters import ChaptersPlugin
 from ytdl_sub.plugins.date_range import DateRangePlugin
 from ytdl_sub.plugins.file_convert import FileConvertPlugin
 from ytdl_sub.plugins.match_filters import MatchFiltersPlugin
-from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.plugins.subtitles import SubtitlesPlugin
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 PluginT = TypeVar("PluginT", bound=Plugin)
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post3
+Version: 2023.7.25.post4
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post3/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.25.post4/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/ytdl_sub/cli/download_args_parser.py
 src/ytdl_sub/cli/main.py
 src/ytdl_sub/cli/main_args_parser.py
 src/ytdl_sub/config/__init__.py
 src/ytdl_sub/config/config_file.py
 src/ytdl_sub/config/config_validator.py
 src/ytdl_sub/config/defaults.py
+src/ytdl_sub/config/plugin.py
 src/ytdl_sub/config/preset.py
 src/ytdl_sub/config/preset_class_mappings.py
 src/ytdl_sub/config/preset_options.py
 src/ytdl_sub/downloaders/__init__.py
 src/ytdl_sub/downloaders/base_downloader.py
 src/ytdl_sub/downloaders/downloader_validator.py
 src/ytdl_sub/downloaders/ytdl_options_builder.py
@@ -46,15 +47,14 @@
 src/ytdl_sub/plugins/date_range.py
 src/ytdl_sub/plugins/embed_thumbnail.py
 src/ytdl_sub/plugins/file_convert.py
 src/ytdl_sub/plugins/match_filters.py
 src/ytdl_sub/plugins/music_tags.py
 src/ytdl_sub/plugins/nfo_tags.py
 src/ytdl_sub/plugins/output_directory_nfo_tags.py
-src/ytdl_sub/plugins/plugin.py
 src/ytdl_sub/plugins/regex.py
 src/ytdl_sub/plugins/split_by_chapters.py
 src/ytdl_sub/plugins/subtitles.py
 src/ytdl_sub/plugins/video_tags.py
 src/ytdl_sub/plugins/internal/__init__.py
 src/ytdl_sub/plugins/internal/view.py
 src/ytdl_sub/prebuilt_presets/__init__.py
```

