# Comparing `tmp/ytdl-sub-2023.7.25.post1.tar.gz` & `tmp/ytdl-sub-2023.7.25.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.25.post1.tar", last modified: Tue Jul 25 01:20:25 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.25.post2.tar", last modified: Tue Jul 25 07:16:18 2023, max compression
```

## Comparing `ytdl-sub-2023.7.25.post1.tar` & `ytdl-sub-2023.7.25.post2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:25.014762 ytdl-sub-2023.7.25.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 01:20:25.014762 ytdl-sub-2023.7.25.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 01:20:25.014762 ytdl-sub-2023.7.25.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.966758 ytdl-sub-2023.7.25.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.974759 ytdl-sub-2023.7.25.post1/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.978759 ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.982759 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.982759 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.982759 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.986760 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.986760 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.990760 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.994760 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.994760 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.994760 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.998761 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.998761 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.998761 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:25.002761 ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:25.002761 ytdl-sub-2023.7.25.post1/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:25.006761 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:25.010762 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:25.014762 ytdl-sub-2023.7.25.post1/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 01:19:55.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:20:24.978759 ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 01:20:24.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-25 01:20:24.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:20:24.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 01:20:24.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 01:20:24.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 01:20:24.000000 ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.413833 ytdl-sub-2023.7.25.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 07:15:55.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.421833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.425833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.429833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.433833 ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-25 07:15:54.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:16:18.417833 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 07:16:18.000000 ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.25.post1/LICENSE` & `ytdl-sub-2023.7.25.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/PKG-INFO` & `ytdl-sub-2023.7.25.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post1
+Version: 2023.7.25.post2
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post1/README.md` & `ytdl-sub-2023.7.25.post2/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/pyproject.toml` & `ytdl-sub-2023.7.25.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/setup.cfg` & `ytdl-sub-2023.7.25.post2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/music_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,17 @@
                 f"to audio using the audio_extract plugin."
             )
 
         # pylint: disable=protected-access
         if self.plugin_options._is_old_format:
             logger.warning(
                 "music_tags.tags is now deprecated. Place your tags directly under music_tags "
-                "instead. The old format will be removed in October of 2023."
+                "instead. The old format will be removed in October of 2023. See "
+                "https://ytdl-sub.readthedocs.io/en/latest/deprecation_notices.html#music-tags "
+                "for more details."
             )
         if self.plugin_options.embed_thumbnail:
             logger.warning(
                 "music_tags.embed_thumbnail is also deprecated. Use the dedicated "
                 "embed_thumbnail plugin instead. This will be removed in October of 2023."
             )
```

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/plugins/video_tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,17 @@
         """
         Tags the entry's audio file using values defined in the metadata options
         """
         # pylint: disable=protected-access
         if self.plugin_options._is_old_format:
             logger.warning(
                 "video_tags.tags is now deprecated. Place your tags directly under video_tags "
-                "instead. The old format will be removed in October of 2023."
+                "instead. The old format will be removed in October of 2023. See "
+                "https://ytdl-sub.readthedocs.io/en/latest/deprecation_notices.html#video-tags "
+                "for more details."
             )
 
         tags_to_write: Dict[str, str] = {}
         for tag_name, tag_formatter in self.plugin_options.tags.dict.items():
             tag_value = self.overrides.apply_formatter(formatter=tag_formatter, entry=entry)
             tags_to_write[tag_name] = tag_value
```

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.25.post1
+Version: 2023.7.25.post2
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.25.post1/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.25.post2/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

