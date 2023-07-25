# Comparing `tmp/pioreactor-23.6.7-py3-none-any.whl.zip` & `tmp/pioreactor-23.7.25rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,85 +1,85 @@
-Zip file size: 185139 bytes, number of entries: 83
--rw-r--r--  2.0 unx      117 b- defN 23-Jun-07 16:33 pioreactor/__init__.py
--rw-r--r--  2.0 unx     6834 b- defN 23-Jun-07 16:33 pioreactor/config.py
--rw-r--r--  2.0 unx      265 b- defN 23-Jun-07 16:33 pioreactor/error_codes.py
--rw-r--r--  2.0 unx      443 b- defN 23-Jun-07 16:33 pioreactor/exc.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jun-07 16:33 pioreactor/hardware.py
--rw-r--r--  2.0 unx     6614 b- defN 23-Jun-07 16:33 pioreactor/logging.py
--rw-r--r--  2.0 unx    14871 b- defN 23-Jun-07 16:33 pioreactor/mureq.py
--rw-r--r--  2.0 unx    12957 b- defN 23-Jun-07 16:33 pioreactor/pubsub.py
--rw-r--r--  2.0 unx     6400 b- defN 23-Jun-07 16:33 pioreactor/structs.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Jun-07 16:33 pioreactor/types.py
--rw-r--r--  2.0 unx     2152 b- defN 23-Jun-07 16:33 pioreactor/version.py
--rw-r--r--  2.0 unx     3654 b- defN 23-Jun-07 16:33 pioreactor/whoami.py
--rw-r--r--  2.0 unx      540 b- defN 23-Jun-07 16:33 pioreactor/actions/__init__.py
--rw-r--r--  2.0 unx     8743 b- defN 23-Jun-07 16:33 pioreactor/actions/led_intensity.py
--rw-r--r--  2.0 unx     7755 b- defN 23-Jun-07 16:33 pioreactor/actions/od_blank.py
--rw-r--r--  2.0 unx    20343 b- defN 23-Jun-07 16:33 pioreactor/actions/od_calibration.py
--rw-r--r--  2.0 unx    17612 b- defN 23-Jun-07 16:33 pioreactor/actions/pump.py
--rw-r--r--  2.0 unx    21362 b- defN 23-Jun-07 16:33 pioreactor/actions/pump_calibration.py
--rw-r--r--  2.0 unx    16662 b- defN 23-Jun-07 16:33 pioreactor/actions/self_test.py
--rw-r--r--  2.0 unx     5175 b- defN 23-Jun-07 16:33 pioreactor/actions/stirring_calibration.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/__init__.py
--rw-r--r--  2.0 unx     4744 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/backup_database.py
--rw-r--r--  2.0 unx     7151 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/experiment_profile.py
--rw-r--r--  2.0 unx     6426 b- defN 23-Jun-07 16:33 pioreactor/actions/leader/export_experiment_data.py
--rw-r--r--  2.0 unx      445 b- defN 23-Jun-07 16:33 pioreactor/automations/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/__init__.py
--rw-r--r--  2.0 unx    28416 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/base.py
--rw-r--r--  2.0 unx     1404 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/chemostat.py
--rw-r--r--  2.0 unx     1194 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/fed_batch.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/morbidostat.py
--rw-r--r--  2.0 unx     4880 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/pid_morbidostat.py
--rw-r--r--  2.0 unx      468 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/silent.py
--rw-r--r--  2.0 unx     2252 b- defN 23-Jun-07 16:33 pioreactor/automations/dosing/turbidostat.py
--rw-r--r--  2.0 unx      510 b- defN 23-Jun-07 16:33 pioreactor/automations/events/__init__.py
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-07 16:33 pioreactor/automations/led/__init__.py
--rw-r--r--  2.0 unx    11851 b- defN 23-Jun-07 16:33 pioreactor/automations/led/base.py
--rw-r--r--  2.0 unx     3136 b- defN 23-Jun-07 16:33 pioreactor/automations/led/light_dark_cycle.py
--rw-r--r--  2.0 unx      205 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/__init__.py
--rw-r--r--  2.0 unx     9722 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/base.py
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/constant_duty_cycle.py
--rw-r--r--  2.0 unx      517 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/only_record_temperature.py
--rw-r--r--  2.0 unx     4314 b- defN 23-Jun-07 16:33 pioreactor/automations/temperature/thermostat.py
--rw-r--r--  2.0 unx      715 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/__init__.py
--rw-r--r--  2.0 unx    42618 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/base.py
--rw-r--r--  2.0 unx     6854 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/dosing_control.py
--rw-r--r--  2.0 unx    20221 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/growth_rate_calculating.py
--rw-r--r--  2.0 unx     5488 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/led_control.py
--rw-r--r--  2.0 unx    24314 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/monitor.py
--rw-r--r--  2.0 unx    47033 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/od_reading.py
--rw-r--r--  2.0 unx    17577 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/stirring.py
--rw-r--r--  2.0 unx    25723 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/temperature_control.py
--rw-r--r--  2.0 unx      605 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/leader/__init__.py
--rw-r--r--  2.0 unx    16280 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
--rw-r--r--  2.0 unx     3829 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/leader/watchdog.py
--rw-r--r--  2.0 unx      609 b- defN 23-Jun-07 16:33 pioreactor/background_jobs/subjobs/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 16:33 pioreactor/cli/__init__.py
--rw-r--r--  2.0 unx    29779 b- defN 23-Jun-07 16:33 pioreactor/cli/pio.py
--rw-r--r--  2.0 unx    22314 b- defN 23-Jun-07 16:33 pioreactor/cli/pios.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 16:33 pioreactor/experiment_profiles/__init__.py
--rw-r--r--  2.0 unx      963 b- defN 23-Jun-07 16:33 pioreactor/experiment_profiles/profile_struct.py
--rw-r--r--  2.0 unx     3517 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/__init__.py
--rw-r--r--  2.0 unx     1316 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/install_plugin.py
--rw-r--r--  2.0 unx     1086 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/list_plugins.py
--rw-r--r--  2.0 unx     1605 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/uninstall_plugin.py
--rw-r--r--  2.0 unx      792 b- defN 23-Jun-07 16:33 pioreactor/plugin_management/utils.py
--rw-r--r--  2.0 unx    10951 b- defN 23-Jun-07 16:33 pioreactor/utils/__init__.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Jun-07 16:33 pioreactor/utils/adcs.py
--rw-r--r--  2.0 unx     1930 b- defN 23-Jun-07 16:33 pioreactor/utils/dacs.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jun-07 16:33 pioreactor/utils/gpio_helpers.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jun-07 16:33 pioreactor/utils/math_helpers.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Jun-07 16:33 pioreactor/utils/mock.py
--rw-r--r--  2.0 unx     3951 b- defN 23-Jun-07 16:33 pioreactor/utils/networking.py
--rw-r--r--  2.0 unx     7559 b- defN 23-Jun-07 16:33 pioreactor/utils/pwm.py
--rw-r--r--  2.0 unx     3393 b- defN 23-Jun-07 16:33 pioreactor/utils/rpi_bad_power.py
--rw-r--r--  2.0 unx     7749 b- defN 23-Jun-07 16:33 pioreactor/utils/sqlite_worker.py
--rw-r--r--  2.0 unx    15186 b- defN 23-Jun-07 16:33 pioreactor/utils/streaming_calculations.py
--rw-r--r--  2.0 unx     5614 b- defN 23-Jun-07 16:33 pioreactor/utils/timing.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     3893 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7656 b- defN 23-Jun-07 16:33 pioreactor-23.6.7.dist-info/RECORD
-83 files, 604752 bytes uncompressed, 172823 bytes compressed:  71.4%
+Zip file size: 187736 bytes, number of entries: 83
+-rw-r--r--  2.0 unx      117 b- defN 23-Jul-25 18:13 pioreactor/__init__.py
+-rw-r--r--  2.0 unx     6887 b- defN 23-Jul-25 18:13 pioreactor/config.py
+-rw-r--r--  2.0 unx      265 b- defN 23-Jul-25 18:13 pioreactor/error_codes.py
+-rw-r--r--  2.0 unx      443 b- defN 23-Jul-25 18:13 pioreactor/exc.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jul-25 18:13 pioreactor/hardware.py
+-rw-r--r--  2.0 unx     6618 b- defN 23-Jul-25 18:13 pioreactor/logging.py
+-rw-r--r--  2.0 unx    15510 b- defN 23-Jul-25 18:13 pioreactor/mureq.py
+-rw-r--r--  2.0 unx    12950 b- defN 23-Jul-25 18:13 pioreactor/pubsub.py
+-rw-r--r--  2.0 unx     6391 b- defN 23-Jul-25 18:13 pioreactor/structs.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jul-25 18:13 pioreactor/types.py
+-rw-r--r--  2.0 unx     2156 b- defN 23-Jul-25 18:13 pioreactor/version.py
+-rw-r--r--  2.0 unx     4458 b- defN 23-Jul-25 18:13 pioreactor/whoami.py
+-rw-r--r--  2.0 unx      540 b- defN 23-Jul-25 18:13 pioreactor/actions/__init__.py
+-rw-r--r--  2.0 unx     8743 b- defN 23-Jul-25 18:13 pioreactor/actions/led_intensity.py
+-rw-r--r--  2.0 unx     7755 b- defN 23-Jul-25 18:13 pioreactor/actions/od_blank.py
+-rw-r--r--  2.0 unx    21010 b- defN 23-Jul-25 18:13 pioreactor/actions/od_calibration.py
+-rw-r--r--  2.0 unx    17612 b- defN 23-Jul-25 18:13 pioreactor/actions/pump.py
+-rw-r--r--  2.0 unx    21362 b- defN 23-Jul-25 18:13 pioreactor/actions/pump_calibration.py
+-rw-r--r--  2.0 unx    17031 b- defN 23-Jul-25 18:13 pioreactor/actions/self_test.py
+-rw-r--r--  2.0 unx     5175 b- defN 23-Jul-25 18:13 pioreactor/actions/stirring_calibration.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/__init__.py
+-rw-r--r--  2.0 unx     4745 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/backup_database.py
+-rw-r--r--  2.0 unx     8717 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/experiment_profile.py
+-rw-r--r--  2.0 unx     6426 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/export_experiment_data.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Jul-25 18:13 pioreactor/automations/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/__init__.py
+-rw-r--r--  2.0 unx    28429 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/base.py
+-rw-r--r--  2.0 unx     1404 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/chemostat.py
+-rw-r--r--  2.0 unx     1194 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/fed_batch.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/morbidostat.py
+-rw-r--r--  2.0 unx     4880 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/pid_morbidostat.py
+-rw-r--r--  2.0 unx      468 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/silent.py
+-rw-r--r--  2.0 unx     2252 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/turbidostat.py
+-rw-r--r--  2.0 unx      510 b- defN 23-Jul-25 18:13 pioreactor/automations/events/__init__.py
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-25 18:13 pioreactor/automations/led/__init__.py
+-rw-r--r--  2.0 unx    11868 b- defN 23-Jul-25 18:13 pioreactor/automations/led/base.py
+-rw-r--r--  2.0 unx     3875 b- defN 23-Jul-25 18:13 pioreactor/automations/led/light_dark_cycle.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/__init__.py
+-rw-r--r--  2.0 unx     9722 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/base.py
+-rw-r--r--  2.0 unx      674 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/constant_duty_cycle.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/only_record_temperature.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/thermostat.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/__init__.py
+-rw-r--r--  2.0 unx    43584 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/base.py
+-rw-r--r--  2.0 unx     6851 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/dosing_control.py
+-rw-r--r--  2.0 unx    20247 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/growth_rate_calculating.py
+-rw-r--r--  2.0 unx     5485 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/led_control.py
+-rw-r--r--  2.0 unx    25386 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/monitor.py
+-rw-r--r--  2.0 unx    48495 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/od_reading.py
+-rw-r--r--  2.0 unx    17586 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/stirring.py
+-rw-r--r--  2.0 unx    24346 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/temperature_control.py
+-rw-r--r--  2.0 unx      605 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/leader/__init__.py
+-rw-r--r--  2.0 unx    16378 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
+-rw-r--r--  2.0 unx     4187 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/leader/watchdog.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/subjobs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 18:13 pioreactor/cli/__init__.py
+-rw-r--r--  2.0 unx    30358 b- defN 23-Jul-25 18:13 pioreactor/cli/pio.py
+-rw-r--r--  2.0 unx    24399 b- defN 23-Jul-25 18:13 pioreactor/cli/pios.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 18:13 pioreactor/experiment_profiles/__init__.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-25 18:13 pioreactor/experiment_profiles/profile_struct.py
+-rw-r--r--  2.0 unx     3716 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/__init__.py
+-rw-r--r--  2.0 unx     1316 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/install_plugin.py
+-rw-r--r--  2.0 unx     1086 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/list_plugins.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/uninstall_plugin.py
+-rw-r--r--  2.0 unx      792 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/utils.py
+-rw-r--r--  2.0 unx    10998 b- defN 23-Jul-25 18:13 pioreactor/utils/__init__.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jul-25 18:13 pioreactor/utils/adcs.py
+-rw-r--r--  2.0 unx     1930 b- defN 23-Jul-25 18:13 pioreactor/utils/dacs.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jul-25 18:13 pioreactor/utils/gpio_helpers.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jul-25 18:13 pioreactor/utils/math_helpers.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Jul-25 18:13 pioreactor/utils/mock.py
+-rw-r--r--  2.0 unx     3951 b- defN 23-Jul-25 18:13 pioreactor/utils/networking.py
+-rw-r--r--  2.0 unx     7559 b- defN 23-Jul-25 18:13 pioreactor/utils/pwm.py
+-rw-r--r--  2.0 unx     3393 b- defN 23-Jul-25 18:13 pioreactor/utils/rpi_bad_power.py
+-rw-r--r--  2.0 unx     7749 b- defN 23-Jul-25 18:13 pioreactor/utils/sqlite_worker.py
+-rw-r--r--  2.0 unx    17179 b- defN 23-Jul-25 18:13 pioreactor/utils/streaming_calculations.py
+-rw-r--r--  2.0 unx     5614 b- defN 23-Jul-25 18:13 pioreactor/utils/timing.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3778 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7681 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/RECORD
+83 files, 616953 bytes uncompressed, 175372 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -225,26 +225,26 @@
 
 Filename: pioreactor/utils/streaming_calculations.py
 Comment: 
 
 Filename: pioreactor/utils/timing.py
 Comment: 
 
-Filename: pioreactor-23.6.7.dist-info/LICENSE
+Filename: pioreactor-23.7.25rc0.dist-info/LICENSE
 Comment: 
 
-Filename: pioreactor-23.6.7.dist-info/METADATA
+Filename: pioreactor-23.7.25rc0.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor-23.6.7.dist-info/WHEEL
+Filename: pioreactor-23.7.25rc0.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor-23.6.7.dist-info/entry_points.txt
+Filename: pioreactor-23.7.25rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor-23.6.7.dist-info/top_level.txt
+Filename: pioreactor-23.7.25rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor-23.6.7.dist-info/RECORD
+Filename: pioreactor-23.7.25rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor/config.py

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import configparser
 import os
 from functools import cache
 
-from pioreactor.whoami import is_testing_env
-
 
 def __getattr__(attr):  # type: ignore
     """
     This dynamically creates the module level variables, so if
     we don't call them, they are never created, saving time - mostly in the CLI.
     """
     if attr == "leader_hostname":
@@ -119,14 +117,15 @@
         waste=3
         media=4
 
     and `od_config.photodiode_channel_reverse`
 
     """
     config = ConfigParserMod()
+    from pioreactor.whoami import is_testing_env
 
     if is_testing_env():
         global_config_path = os.environ.get("GLOBAL_CONFIG", "./config.dev.ini")
         local_config_path = os.environ.get("LOCAL_CONFIG", "")
     else:
         global_config_path = "/home/pioreactor/.pioreactor/config.ini"
         local_config_path = "/home/pioreactor/.pioreactor/unit_config.ini"
@@ -173,14 +172,16 @@
 
 @cache
 def get_leader_address() -> str:
     return get_config().get("cluster.topology", "leader_address", fallback="localhost")
 
 
 def check_firstboot_successful() -> bool:
+    from pioreactor.whoami import is_testing_env
+
     if is_testing_env():
         return True
     return os.path.isfile("/usr/local/bin/firstboot.sh.done")
 
 
 def get_active_workers_in_inventory() -> tuple[str, ...]:
     # note that this rehydrates conifg.ini from disk before checking.
```

## pioreactor/logging.py

```diff
@@ -111,18 +111,18 @@
         mqtt_msg = self.client.publish(
             self.topic, payload, qos=self.qos, retain=self.retain, **self.mqtt_kwargs
         )
 
         if (record.levelno == logging.ERROR) and config.getboolean(
             "data_sharing_with_pioreactor", "send_errors_to_Pioreactor", fallback=False
         ):
-            publish_to_pioreactor_cloud("reported_errors", data=payload)
+            publish_to_pioreactor_cloud("reported_errors", data_str=payload)
 
         # if Python exits too quickly, the last msg might never make it to the broker.
-        mqtt_msg.wait_for_publish(timeout=1)
+        mqtt_msg.wait_for_publish(timeout=2)
 
     def close(self) -> None:
         self.client.loop_stop()
         self.client.disconnect()
         super().close()
```

## pioreactor/mureq.py

```diff
@@ -11,27 +11,38 @@
 import contextlib
 import io
 import json as jsonlib
 import os.path
 import socket
 import ssl
 import urllib.parse
+from base64 import b64encode
 from http.client import HTTPConnection
 from http.client import HTTPException
 from http.client import HTTPMessage
+from http.client import HTTPResponse
 from http.client import HTTPSConnection
+from typing import Generator
 from typing import Optional
 
-__version__ = "0.1.0"
+from pioreactor.config import config
+
 
 DEFAULT_TIMEOUT = 15.0
 DEFAULT_UA = "Python/Pioreactor"
+DEFAULT_AUTH = f'Basic {config.get("ui_basic_auth", "api_key", fallback="")}'
+
+
+def basic_auth(username: str, password: str):
+    # get(..., headers={ 'Authorization' : f'Basic {basic_auth(username, password)}'})
+    token = b64encode(f"{username}:{password}".encode("utf-8")).decode("ascii")
+    return token
 
 
-def request(method, url, *, read_limit=None, **kwargs):
+def request(method, url, *, read_limit=None, **kwargs) -> Response:
     """request performs an HTTP request and reads the entire response body.
 
     :param str method: HTTP method to request (e.g. 'GET', 'POST')
     :param str url: URL to request
     :param read_limit: maximum number of bytes to read from the body, or None for no limit
     :type read_limit: int or None
     :param kwargs: optional arguments defined by yield_response
@@ -43,47 +54,47 @@
         try:
             body = response.read(read_limit)
         except HTTPException:
             raise
         except IOError as e:
             raise HTTPException(str(e)) from e
         return Response(
-            response.url,
+            response.url,  # type: ignore
             response.status,
             _prepare_incoming_headers(response.headers),
             body,
         )
 
 
-def get(url, **kwargs):
+def get(url, **kwargs) -> Response:
     """get performs an HTTP GET request."""
     return request("GET", url=url, **kwargs)
 
 
-def post(url, body: Optional[bytes] = None, **kwargs):
+def post(url, body: Optional[bytes] = None, **kwargs) -> Response:
     """post performs an HTTP POST request."""
     return request("POST", url=url, body=body, **kwargs)
 
 
-def head(url, **kwargs):
+def head(url, **kwargs) -> Response:
     """head performs an HTTP HEAD request."""
     return request("HEAD", url=url, **kwargs)
 
 
-def put(url, body: Optional[bytes] = None, **kwargs):
+def put(url, body: Optional[bytes] = None, **kwargs) -> Response:
     """put performs an HTTP PUT request."""
     return request("PUT", url=url, body=body, **kwargs)
 
 
-def patch(url, body: Optional[bytes] = None, **kwargs):
+def patch(url, body: Optional[bytes] = None, **kwargs) -> Response:
     """patch performs an HTTP PATCH request."""
     return request("PATCH", url=url, body=body, **kwargs)
 
 
-def delete(url, **kwargs):
+def delete(url, **kwargs) -> Response:
     """delete performs an HTTP DELETE request."""
     return request("DELETE", url=url, **kwargs)
 
 
 @contextlib.contextmanager
 def yield_response(
     method,
@@ -96,15 +107,15 @@
     body=None,
     form=None,
     json=None,
     verify=True,
     source_address=None,
     max_redirects=None,
     ssl_context=None,
-):
+) -> Generator[HTTPResponse, None, None]:
     """yield_response is a low-level API that exposes the actual
     http.client.HTTPResponse via a contextmanager.
 
     Note that unlike mureq.Response, http.client.HTTPResponse does not
     automatically canonicalize multiple appearances of the same header by
     joining them together with a comma delimiter. To retrieve canonicalized
     headers from the response, use response.getheader():
@@ -134,15 +145,15 @@
     :raises: HTTPException
     """
     method = method.upper()
     headers = _prepare_outgoing_headers(headers)
     enc_params = _prepare_params(params)
     body = _prepare_body(body, form, json, headers)
 
-    visited_urls = []
+    visited_urls: list[str] = []
 
     while max_redirects is None or len(visited_urls) <= max_redirects:
         url, conn, path = _prepare_request(
             method,
             url,
             enc_params=enc_params,
             timeout=timeout,
@@ -246,15 +257,15 @@
 class HTTPErrorStatus(HTTPException):
     """HTTPErrorStatus is raised by Response.raise_for_status() to indicate an
     HTTP error code (a 40x or a 50x). Note that a well-formed response with an
     error code does not result in an exception unless raise_for_status() is
     called explicitly.
     """
 
-    def __init__(self, status_code):
+    def __init__(self, status_code: int):
         self.status_code = status_code
 
     def __str__(self):
         return f"HTTP response returned error code {self.status_code:d}"
 
 
 # end public API, begin internal implementation details
@@ -333,14 +344,15 @@
             iterator = headers.items()
         else:
             iterator = iter(headers)
         for k, v in iterator:
             new_headers[k] = v
         headers = new_headers
     _setdefault_header(headers, "User-Agent", DEFAULT_UA)
+    _setdefault_header(headers, "Authorization", DEFAULT_AUTH)
     return headers
 
 
 # XXX join multi-headers together so that get(), __getitem__(),
 # etc. behave intuitively, then stuff them back in an HTTPMessage.
 def _prepare_incoming_headers(headers):
     headers_dict = {}
```

## pioreactor/pubsub.py

```diff
@@ -7,42 +7,38 @@
 import threading
 from enum import IntEnum
 from time import sleep
 from typing import Any
 from typing import Callable
 from typing import Optional
 
-from paho.mqtt.client import Client as PahoClient  # type: ignore
+from paho.mqtt.client import Client as PahoClient
 
 from pioreactor.config import leader_address
 from pioreactor.types import MQTTMessage
 
 
-class PIOREACTOR:
-    """
-    Use to construct MQTT paths like Pathlib in Python core.
+class MQTT_TOPIC:
+    def __init__(self, init: str):
+        self.body = init
 
-    > PIOREACTOR() / unit / experiment / "+" / "$state" / "set"
-    >> "pioreactor/test_unit/test_experiment/+/$state/set"
+    def __truediv__(self, other: str | MQTT_TOPIC) -> MQTT_TOPIC:
+        return MQTT_TOPIC(self.body + "/" + str(other))
 
-    BETA: may be deleted in the future.
+    def __str__(self) -> str:
+        return self.body
 
-    """
+    def __repr__(self) -> str:
+        return str(self)
 
-    def __init__(self, body="pioreactor"):
-        self.body = body
+    def __iter__(self):
+        return iter(str(self))
 
-    def __truediv__(self, other):
-        return PIOREACTOR(self.body + "/" + other)
 
-    def __str__(self):
-        return self.body
-
-    def __repr__(self):
-        return str(self)
+PIOREACTOR = MQTT_TOPIC("pioreactor")
 
 
 def add_hash_suffix(s: str) -> str:
     """Adds random 4-character hash to the end of a string.
 
     Args:
         s: The string to which the hash should be added.
@@ -89,15 +85,15 @@
     """
     Create a MQTT client and connect to a host.
     """
 
     def default_on_connect(client: Client, userdata, flags, rc: int, properties=None):
         if rc > 1:
             from pioreactor.logging import create_logger
-            from paho.mqtt.client import connack_string  # type: ignore
+            from paho.mqtt.client import connack_string
 
             logger = create_logger("pubsub.create_client", to_mqtt=False)
             logger.error(f"Connection failed with error code {rc=}: {connack_string(rc)}")
 
     client = Client(
         client_id=add_hash_suffix(client_id) if client_id else "",
         clean_session=clean_session,
@@ -135,15 +131,15 @@
 
     return client
 
 
 def publish(
     topic: str, message, hostname: str = leader_address, retries: int = 10, **mqtt_kwargs
 ) -> None:
-    from paho.mqtt import publish as mqtt_publish  # type: ignore
+    from paho.mqtt import publish as mqtt_publish
     import socket
 
     for retry_count in range(retries):
         try:
             mqtt_publish.single(
                 topic,
                 payload=message,
@@ -360,15 +356,15 @@
         self.unit = unit
         self.experiment = experiment
         # create a bucket for the logs
         self.bucket: list[dict] = []
         # subscribe to the logs
         self.client: Client = subscribe_and_callback(
             self._collect_logs_into_bucket,
-            str(PIOREACTOR() / self.unit / self.experiment / "logs" / "app"),
+            str(PIOREACTOR / self.unit / self.experiment / "logs" / "app"),
         )
 
     def _collect_logs_into_bucket(self, message):
         from json import loads
 
         # load the message
         log = loads(message.payload)
@@ -382,37 +378,43 @@
     def __exit__(self, *args):
         # stop listening for messages
         self.client.loop_stop()
         # disconnect from the broker
         self.client.disconnect()
 
 
-def publish_to_pioreactor_cloud(endpoint: str, data=None, json=None) -> None:
+def publish_to_pioreactor_cloud(
+    endpoint: str, data_dict: Optional[dict] = None, data_str: Optional[str] = None
+) -> None:
     """
     Parameters
     ------------
     endpoint: the function to send to the data to
-    data: (optional) Dictionary, list of tuples, bytes, or file-like object to send in the body.
-    json: (optional) json data to send in the body.
+    json: (optional) data to send in the body.
 
     """
     from pioreactor.mureq import post
     from pioreactor.whoami import get_hashed_serial_number, is_testing_env
     from pioreactor.utils.timing import current_utc_timestamp
+    from json import dumps
+
+    assert (data_dict is not None) or (data_str is not None)
 
     if is_testing_env():
         return
 
-    if json is not None:
-        json["hashed_serial_number"] = get_hashed_serial_number()
-        json["timestamp"] = current_utc_timestamp()
+    if data_dict is not None:
+        data_dict["hashed_serial_number"] = get_hashed_serial_number()
+        data_dict["timestamp"] = current_utc_timestamp()
+        body = dumps(data_dict).encode("utf-8")
+    elif data_str is not None:
+        body = data_str.encode("utf-8")
 
     headers = {"Content-type": "application/json", "Accept": "text/plain"}
     try:
         post(
             f"https://cloud.pioreactor.com/{endpoint}",
-            data=data,
-            json=json,
+            body=body,
             headers=headers,
         )
     except Exception:
         pass
```

## pioreactor/structs.py

```diff
@@ -230,15 +230,15 @@
     maximum_od600: float
     minimum_od600: float
     minimum_voltage: float
     maximum_voltage: float
     curve_type: str
     curve_data_: list[float]
     voltages: list[float]
-    inferred_od600s: list[float]
+    od600s: list[float]
     ir_led_intensity: float
     pd_channel: pt.PdChannel
 
 
 class OD45Calibration(ODCalibration, tag="od_45"):
     pass
```

## pioreactor/version.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
 
 # Append "dev" if a dev version
 # Append "rc0" if a rc version
-__version__ = "23.6.7"
+__version__ = "23.7.25rc0"
 
 
 def _get_hardware_version() -> tuple[int, int] | tuple[int, int, str]:
     if os.environ.get("HARDWARE") is not None:
         # ex: > HARDWARE=1.1 pio ...
         return int(os.environ["HARDWARE"].split(".")[0]), int(os.environ["HARDWARE"].split(".")[1])
```

## pioreactor/whoami.py

```diff
@@ -5,15 +5,14 @@
 import sys
 import time
 from functools import cache
 from hashlib import md5
 
 from msgspec.json import decode
 
-from pioreactor.mureq import get
 from pioreactor.structs import ExperimentMetadata
 from pioreactor.version import serial_number
 
 UNIVERSAL_IDENTIFIER = "$broadcast"
 UNIVERSAL_EXPERIMENT = "$experiment"
 NO_EXPERIMENT = "$no_experiment_present"
 
@@ -25,36 +24,60 @@
 
 @cache
 def get_latest_experiment_name() -> str:
     return _get_latest_experiment_name()
 
 
 def _get_latest_experiment_name() -> str:
+    from pioreactor.logging import create_logger
+    from pioreactor import mureq
+
     if os.environ.get("EXPERIMENT") is not None:
         return os.environ["EXPERIMENT"]
     elif is_testing_env():
         return "_testing_experiment"
 
     from pioreactor.config import leader_address
 
     retries = 10
+    exit_reason = ""
+
     for attempt in range(retries):
         try:
-            result = get(f"http://{leader_address}/api/experiments/latest")
+            result = mureq.get(f"http://{leader_address}/api/experiments/latest")
             result.raise_for_status()
             return decode(result.body, type=ExperimentMetadata).experiment
+        except mureq.HTTPErrorStatus as e:
+            if e.status_code == 401:
+                # auth error, something is wrong
+                exit_reason = "auth"
+                break
+        except mureq.HTTPException:
+            exit_reason = "connection_refused"
         except Exception:
-            time.sleep(0.5 * attempt)
-
-    from pioreactor.logging import create_logger
+            # some other error? Keep trying
+            pass
+        time.sleep(0.5 * attempt)
+    else:
+        exit_reason = "timeout"
 
     logger = create_logger("pioreactor", experiment=UNIVERSAL_EXPERIMENT, to_mqtt=False)
-    logger.warning(
-        f"No experiment found. Check http://{leader_address}/api/experiments/latest for an experiment."
-    )
+
+    if exit_reason == "auth":
+        logger.warning(
+            f"Error in authentication to UI. Check http://{leader_address} and config.ini for api_key."
+        )
+    elif exit_reason == "timeout":
+        logger.warning(
+            f"Not able to access experiments in UI. Check http://{leader_address}/api/experiments/latest"
+        )
+    elif exit_reason == "connection_refused":
+        logger.warning(
+            f"Not able to access experiments in UI. Check http://{leader_address} is online and check network."
+        )
     return NO_EXPERIMENT
 
 
 @cache
 def is_testing_env() -> bool:
     return ("pytest" in sys.modules) or (os.environ.get("TESTING") is not None)
```

## pioreactor/actions/od_calibration.py

```diff
@@ -13,14 +13,15 @@
 from msgspec.json import decode
 from msgspec.json import encode
 
 from pioreactor import structs
 from pioreactor import types as pt
 from pioreactor.background_jobs.od_reading import start_od_reading
 from pioreactor.background_jobs.stirring import start_stirring as stirring
+from pioreactor.background_jobs.stirring import Stirrer
 from pioreactor.config import config
 from pioreactor.config import leader_address
 from pioreactor.mureq import patch
 from pioreactor.mureq import put
 from pioreactor.utils import is_pio_job_running
 from pioreactor.utils import local_persistant_storage
 from pioreactor.utils import publish_ready_to_disconnected_state
@@ -34,18 +35,19 @@
     import logging
 
     logging.disable(logging.WARNING)
 
     click.clear()
     click.echo(
         """This routine will calibrate the current Pioreactor to (offline) OD600 readings. You'll need:
-    1. A Pioreactor
-    2. At least 10mL of a culture with density the most you'll ever observe, and its OD600 measurement
-    3. Micro-pipette
+    1. The Pioreactor you wish to calibrate (the one you are using)
+    2. At least 10mL of a culture with density the most you'll ever observe, and its OD600 measurement.
+    3. A micro-pipette
     4. Accurate 10mL measurement tool
+    5. Sterile media, amount to be determined shortly.
 """
     )
 
 
 def get_metadata_from_user():
     from math import log2
 
@@ -61,24 +63,24 @@
             elif name == "current":
                 click.echo("Name cannot be `current`.")
                 continue
             else:
                 break
 
     initial_od600 = click.prompt(
-        "Provide the OD600 measurement of your initial culture",
+        "Provide the OD600 measurement of your initial, high density, culture",
         type=click.FloatRange(min=0.01, clamp=False),
     )
 
     minimum_od600 = click.prompt(
-        "Provide the minimum OD600 measurement you want to calibrate to",
+        "Provide the minimum OD600 measurement you wish to calibrate to",
         type=click.FloatRange(min=0, max=initial_od600, clamp=False),
     )
 
-    while minimum_od600 == initial_od600:
+    while minimum_od600 >= initial_od600:
         minimum_od600 = click.prompt(
             "The minimum OD600 measurement must be less than the initial OD600 culture measurement",
             type=click.FloatRange(min=0, max=initial_od600, clamp=False),
         )
 
     if minimum_od600 == 0:
         minimum_od600 = 0.01
@@ -87,15 +89,19 @@
         "Provide the volume to be added to your vial each iteration (default = 1 mL)",
         default=1,
         type=click.FloatRange(min=0.01, max=10, clamp=False),
     )
 
     number_of_points = int(log2(initial_od600 / minimum_od600) * (10 / dilution_amount))
 
-    click.echo(f"This will require about {number_of_points} measurements.")
+    click.echo(f"This will require {number_of_points} data points.")
+    click.echo(
+        f"You will need at least {number_of_points * dilution_amount + 10}mL of media available."
+    )
+    click.confirm("Continue?", abort=True, default=True)
 
     if "REF" not in config["od_config.photodiode_channel_reverse"]:
         raise ValueError("REF required for OD calibration.")
         # technically it's not required? we just need a specific PD channel to calibrate from.
 
     ref_channel = config["od_config.photodiode_channel_reverse"]["REF"]
     signal_channel = "1" if ref_channel == "2" else "2"
@@ -131,15 +137,21 @@
         experiment=get_latest_testing_experiment_name(),
     )
     st.block_until_rpm_is_close_to_target(abs_tolerance=120)
     return st
 
 
 def plot_data(
-    x, y, title, x_min=None, x_max=None, interpolation_curve=None, highlight_recent_point=True
+    x,
+    y,
+    title,
+    x_min=None,
+    x_max=None,
+    interpolation_curve=None,
+    highlight_recent_point=True,
 ):
     import plotext as plt  # type: ignore
 
     plt.clf()
 
     plt.scatter(x, y, marker="hd")
 
@@ -155,15 +167,19 @@
         plt.plot_size(145, 42)
 
     plt.xlim(x_min, x_max)
     plt.show()
 
 
 def start_recording_and_diluting(
-    initial_od600: float, minimum_od600: float, dilution_amount: float, signal_channel
+    st: Stirrer,
+    initial_od600: float,
+    minimum_od600: float,
+    dilution_amount: float,
+    signal_channel,
 ):
     inferred_od600 = initial_od600
     voltages = []
     inferred_od600s = []
     current_volume_in_vial = initial_volume_in_vial = 10.0
     n_samples = int((20 - initial_volume_in_vial) / dilution_amount)
     click.echo("Starting OD recordings.")
@@ -185,17 +201,17 @@
 
         for _ in range(4):
             # warm up
             od_reader.record_from_adc()
 
         while inferred_od600 > minimum_od600:
             if inferred_od600 < initial_od600 and click.confirm(
-                "Do you want to enter a new OD600 value for the current density?"
+                "Do you want to enter an updated OD600 value for the current density?"
             ):
-                inferred_od600 = click.prompt("New measured OD600", type=float)
+                inferred_od600 = click.prompt("Updated OD600", type=float)
 
             inferred_od600s.append(inferred_od600)
 
             voltages.append(get_voltage_from_adc())
 
             for i in range(n_samples):
                 click.clear()
@@ -207,15 +223,15 @@
                     x_max=initial_od600,
                 )
                 click.echo()
                 click.secho(
                     f"Test {i+1} of {n_samples} [{'#' * (i+1) }{' ' * (n_samples - i - 1)}]",
                     fg="green",
                 )
-                click.echo(f"Add {dilution_amount}ml of DI water to vial.")
+                click.echo(f"Add {dilution_amount}ml of media to vial.")
 
                 while not click.confirm("Continue?", default=True):
                     pass
 
                 current_volume_in_vial = current_volume_in_vial + dilution_amount
 
                 for i in range(4):
@@ -242,23 +258,26 @@
                 plot_data(
                     inferred_od600s,
                     voltages,
                     title="OD Calibration (ongoing)",
                     x_min=minimum_od600,
                     x_max=initial_od600,
                 )
+                st.set_state("sleeping")
                 click.echo()
                 click.echo(click.style("Stop❗", fg="red"))
                 click.echo("Carefully remove vial.")
                 click.echo("(Optional: take new OD600 reading with external instrument.)")
                 click.echo("Reduce volume in vial back to 10ml.")
                 click.echo("Confirm vial outside is dry and clean. Place back into Pioreactor.")
                 while not click.confirm("Continue?", default=True):
                     pass
                 current_volume_in_vial = initial_volume_in_vial
+                st.set_state("ready")
+                st.block_until_rpm_is_close_to_target(abs_tolerance=120)
                 sleep(1.0)
 
         click.clear()
         plot_data(
             inferred_od600s,
             voltages,
             title="OD Calibration (ongoing)",
@@ -295,15 +314,18 @@
         click.echo("Unable to fit.")
         coefs = np.zeros(degree).tolist()
 
     return coefs, "poly"
 
 
 def show_results_and_confirm_with_user(
-    curve_data: list[float], curve_type: str, voltages: list[float], inferred_od600s: list[float]
+    curve_data: list[float],
+    curve_type: str,
+    voltages: list[float],
+    inferred_od600s: list[float],
 ) -> tuple[bool, int]:
     click.clear()
 
     curve_callable = curve_to_callable(curve_type, curve_data)
 
     plot_data(
         inferred_od600s,
@@ -336,15 +358,15 @@
         raise click.Abort()
 
 
 def save_results(
     curve_data_: list[float],
     curve_type: str,
     voltages: list[float],
-    inferred_od600s: list[float],
+    od600s: list[float],
     angle,
     name: str,
     maximum_od600: float,
     minimum_od600: float,
     signal_channel: pt.PdChannel,
     unit: str,
 ) -> structs.ODCalibration:
@@ -367,15 +389,15 @@
         maximum_od600=maximum_od600,
         minimum_od600=0,
         minimum_voltage=min(voltages),
         maximum_voltage=max(voltages),
         curve_data_=curve_data_,
         curve_type=curve_type,
         voltages=voltages,
-        inferred_od600s=inferred_od600s,
+        od600s=od600s,
         ir_led_intensity=float(config["od_config"]["ir_led_intensity"]),
         pd_channel=signal_channel,
     )
 
     with local_persistant_storage("od_calibrations") as cache:
         cache[name] = encode(data_blob)
 
@@ -400,17 +422,17 @@
             minimum_od600,
             dilution_amount,
             angle,
             signal_channel,
         ) = get_metadata_from_user()
         setup_HDC_instructions()
 
-        with start_stirring():
+        with start_stirring() as st:
             inferred_od600s, voltages = start_recording_and_diluting(
-                initial_od600, minimum_od600, dilution_amount, signal_channel
+                st, initial_od600, minimum_od600, dilution_amount, signal_channel
             )
 
         degree = 4
         while True:
             curve_data_, curve_type = calculate_curve_of_best_fit(voltages, inferred_od600s, degree)
             okay_with_result, degree = show_results_and_confirm_with_user(
                 curve_data_, curve_type, voltages, inferred_od600s
@@ -476,15 +498,15 @@
 
 
 def display(name: str | None) -> None:
     from pprint import pprint
 
     def display_from_calibration_blob(data_blob) -> None:
         voltages = data_blob["voltages"]
-        ods = data_blob["inferred_od600s"]
+        ods = data_blob["od600s"]
         name, angle = data_blob["name"], data_blob["angle"]
         click.echo()
         click.echo(click.style(f"Calibration `{name}`", underline=True, bold=True))
         plot_data(
             ods,
             voltages,
             title=f"`{name}`, calibration of {angle}°",
@@ -538,33 +560,38 @@
     return success
 
 
 def change_current(name: str) -> None:
     try:
         with local_persistant_storage("od_calibrations") as all_calibrations:
             new_calibration = decode(
-                all_calibrations[name], type=structs.subclass_union(structs.ODCalibration)
+                all_calibrations[name],
+                type=structs.subclass_union(structs.ODCalibration),
             )
 
         angle = new_calibration.angle
         with local_persistant_storage("current_od_calibration") as current_calibrations:
             if angle in current_calibrations:
                 old_calibration = decode(
-                    current_calibrations[angle], type=structs.subclass_union(structs.ODCalibration)
+                    current_calibrations[angle],
+                    type=structs.subclass_union(structs.ODCalibration),
                 )
             else:
                 old_calibration = None
 
             current_calibrations[angle] = encode(new_calibration)
 
-        res = patch(
-            f"http://{leader_address}/api/calibrations/{get_unit_name()}/{new_calibration.type}/{new_calibration.name}",
-            json={"current": 1},
-        )
-        if not res.ok:
+        try:
+            res = patch(
+                f"http://{leader_address}/api/calibrations/{get_unit_name()}/{new_calibration.type}/{new_calibration.name}",
+                json={"current": 1},
+            )
+            if not res.ok:
+                raise Exception
+        except Exception:
             click.echo("Could not update in database on leader ❌")
 
         if old_calibration:
             click.echo(f"Replaced {old_calibration.name} with {new_calibration.name}   ✅")
         else:
             click.echo(f"Set {new_calibration.name} to current calibration  ✅")
```

## pioreactor/actions/self_test.py

```diff
@@ -20,14 +20,15 @@
 
 from pioreactor.actions.led_intensity import ALL_LED_CHANNELS
 from pioreactor.actions.led_intensity import change_leds_intensities_temporarily
 from pioreactor.actions.led_intensity import led_intensity
 from pioreactor.background_jobs import stirring
 from pioreactor.background_jobs.od_reading import ADCReader
 from pioreactor.background_jobs.od_reading import ALL_PD_CHANNELS
+from pioreactor.background_jobs.od_reading import average_over_pd_channel_to_voltages
 from pioreactor.background_jobs.od_reading import IR_keyword
 from pioreactor.background_jobs.od_reading import REF_keyword
 from pioreactor.background_jobs.od_reading import start_od_reading
 from pioreactor.background_jobs.temperature_control import TemperatureController
 from pioreactor.config import config
 from pioreactor.hardware import is_HAT_present
 from pioreactor.hardware import is_heating_pcb_present
@@ -53,55 +54,61 @@
 def test_pioreactor_HAT_present(client: Client, logger: Logger, unit: str, experiment: str) -> None:
     assert is_HAT_present()
 
 
 def test_REF_is_in_correct_position(
     client: Client, logger: Logger, unit: str, experiment: str
 ) -> None:
-    # this _also_ uses stirring to increase the variance in the non-REF, so...
+    # this _also_ uses stirring to increase the variance in the non-REF.
+    # The idea is to trigger stirring on and off and the REF should not see a change in signal / variance, but the other PD should.
     from statistics import variance
 
+    reference_channel = cast(PdChannel, config["od_config.photodiode_channel_reverse"][REF_keyword])
+    signal_channel = ["1", "2"][int(reference_channel == "1")]
+
     signal1 = []
     signal2 = []
 
     with stirring.start_stirring(
-        target_rpm=450, unit=unit, experiment=experiment
-    ), start_od_reading(
+        target_rpm=1250,
+        unit=unit,
+        experiment=experiment,
+    ) as st, start_od_reading(
         od_angle_channel1="90",
         od_angle_channel2="90",
         interval=1.15,
         unit=unit,
         fake_data=is_testing_env(),
         experiment=experiment,
         use_calibration=False,
     ) as od_stream:
-        for i, reading in enumerate(od_stream):
+        st.block_until_rpm_is_close_to_target(abs_tolerance=150)
+
+        for i, reading in enumerate(od_stream, start=1):
             signal1.append(reading.ods["1"].od)
             signal2.append(reading.ods["2"].od)
 
+            if i % 5 == 0 and i % 2 == 0:
+                st.set_state("ready")
+            elif i % 5 == 0:
+                st.set_state("sleeping")
+
             if i == 25:
                 break
 
     norm_variance_per_channel = {
         "1": variance(signal1) / trimmed_mean(signal1) ** 2,
         "2": variance(signal2) / trimmed_mean(signal2) ** 2,
     }
 
-    ref_channel = config["od_config.photodiode_channel_reverse"][REF_keyword]
-
-    THRESHOLD = 1.0
-    if ref_channel == "1":
-        assert (
-            THRESHOLD * norm_variance_per_channel["1"] < norm_variance_per_channel["2"]
-        ), f"{ref_channel=}, {norm_variance_per_channel=}"
-
-    elif ref_channel == "2":
-        assert (
-            THRESHOLD * norm_variance_per_channel["2"] < norm_variance_per_channel["1"]
-        ), f"{ref_channel=}, {norm_variance_per_channel=}"
+    THRESHOLD = 6.0
+    assert (
+        THRESHOLD * norm_variance_per_channel[reference_channel]
+        < norm_variance_per_channel[signal_channel]
+    ), f"{reference_channel=}, {norm_variance_per_channel=}"
 
 
 def test_all_positive_correlations_between_pds_and_leds(
     client, logger: Logger, unit: str, experiment: str
 ) -> None:
     """
     This tests that there is a positive correlation between the IR LED channel, and the photodiodes
@@ -143,21 +150,21 @@
                 unit=unit,
                 experiment=current_experiment_name,
                 verbose=False,
                 source_of_event="self_test",
             )
 
             # record from ADC, we'll average them
-            readings1 = adc_reader.take_reading()
-            readings2 = adc_reader.take_reading()
+            avg_reading = average_over_pd_channel_to_voltages(
+                adc_reader.take_reading(), adc_reader.take_reading()
+            )
 
             # Add to accumulating list
             for pd_channel in ALL_PD_CHANNELS:
-                reading = 0.5 * (readings1[pd_channel] + readings2[pd_channel])
-                varying_intensity_results[pd_channel].append(reading)
+                varying_intensity_results[pd_channel].append(avg_reading[pd_channel])
 
         # compute the linear correlation between the intensities and observed PD measurements
         for pd_channel in ALL_PD_CHANNELS:
             measured_correlation = round(
                 correlation(INTENSITIES, varying_intensity_results[pd_channel]), 2
             )
             results[(led_channel, pd_channel)] = measured_correlation
@@ -258,15 +265,15 @@
         experiment=current_experiment_name,
         verbose=False,
     ):
         readings = adc_reader.take_reading()
 
     assert (
         0.05 < readings[reference_channel] < 0.256
-    ), f"Recorded {readings[reference_channel]} in REF, should ideally be between 0.05 and 0.256."
+    ), f"Recorded {readings[reference_channel]} in REF, should ideally be between 0.05 and 0.256. Current IR LED: {ir_intensity}%."
 
 
 def test_detect_heating_pcb(client: Client, logger: Logger, unit: str, experiment: str) -> None:
     assert is_heating_pcb_present()
 
 
 def test_positive_correlation_between_temperature_and_heating(
```

## pioreactor/actions/leader/backup_database.py

```diff
@@ -49,21 +49,22 @@
     experiment = UNIVERSAL_EXPERIMENT
 
     with publish_ready_to_disconnected_state(unit, experiment, "backup_database"):
         logger = create_logger(
             "backup_database", experiment=experiment, unit=unit, to_mqtt=False
         )  # the backup would take so long that the mqtt client would disconnect. We also don't want to write to the db.
 
+        logger.debug(f"Starting backup of database to {output_file}")
+
         if not force and count_writes_occurring(unit) >= 2:
             logger.debug("Too many writes to proceed with backup. Exiting.")
             return
 
         current_time = current_utc_timestamp()
         page_size = 50
-        logger.debug(f"Starting backup of database to {output_file}")
 
         con = sqlite3.connect(config.get("storage", "database"))
         bck = sqlite3.connect(output_file)
 
         with bck:
             # why 50? A larger sqlite3 database we used had 164510 pages.
             # pages=5 took 4m
```

## pioreactor/actions/leader/experiment_profile.py

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from threading import Timer
 from typing import Callable
 
 import click
+import pkg_resources
 from msgspec.json import encode
 from msgspec.yaml import decode
 
 from pioreactor.config import leader_address
-from pioreactor.experiment_profiles.profile_struct import Profile
+from pioreactor.experiment_profiles import profile_struct as struct
 from pioreactor.logging import create_logger
 from pioreactor.mureq import put
 from pioreactor.pubsub import publish
 from pioreactor.utils import publish_ready_to_disconnected_state
 from pioreactor.whoami import get_latest_experiment_name
 from pioreactor.whoami import get_unit_name
 from pioreactor.whoami import UNIVERSAL_IDENTIFIER
@@ -95,42 +96,83 @@
     return _update
 
 
 def hours_to_seconds(hours: float) -> float:
     return hours * 60 * 60
 
 
-def load_and_verify_profile_file(profile_filename: str) -> Profile:
+def load_and_verify_profile_file(profile_filename: str) -> struct.Profile:
     with open(profile_filename) as f:
-        return decode(f.read(), type=Profile)
+        return decode(f.read(), type=struct.Profile)
 
 
 def publish_labels_to_ui(labels_map: dict[str, str]) -> None:
     try:
         for unit_name, label in labels_map.items():
             put(
                 f"http://{leader_address}/api/unit_labels/current",
                 encode({"unit": unit_name, "label": label}),
                 headers={"Content-Type": "application/json"},
             )
     except Exception:
         pass
 
 
+def get_installed_packages() -> dict[str, str]:
+    """Return a dictionary of installed packages and their versions"""
+    installed_packages = {d.project_name: d.version for d in pkg_resources.working_set}
+    return installed_packages
+
+
+def check_plugins(plugins: list[struct.Plugin]) -> None:
+    """Check if the specified packages with versions are installed"""
+    installed_packages = get_installed_packages()
+    not_installed = []
+
+    for plugin in plugins:
+        name = plugin.name
+        version = plugin.version
+        if name in installed_packages:
+            if version.startswith(">="):
+                # Version constraint is '>='
+                if installed_packages[name] < version[2:]:
+                    not_installed.append(plugin)
+            if version.startswith("<="):
+                # Version constraint is '<='
+                if installed_packages[name] > version[2:]:
+                    not_installed.append(plugin)
+            else:
+                # No version constraint, exact version match required
+                if installed_packages[name] != version:
+                    not_installed.append(plugin)
+        else:
+            not_installed.append(plugin)
+
+    if not_installed:
+        raise ImportError(f"Missing packages {not_installed}")
+
+
 def execute_experiment_profile(profile_filename: str, dry_run: bool = False) -> None:
     unit = get_unit_name()
     experiment = get_latest_experiment_name()
     logger = create_logger("experiment_profile")
     with publish_ready_to_disconnected_state(unit, experiment, "experiment_profile") as state:
         profile = load_and_verify_profile_file(profile_filename)
 
         logger.notice(  # type: ignore
             f"Starting profile {profile.experiment_profile_name}, sourced from {profile_filename}."
         )
 
+        try:
+            check_plugins(profile.plugins)
+        except Exception as e:
+            logger.debug(e, exc_info=True)
+            logger.error(e)
+            raise e
+
         labels_to_units = {v: k for k, v in profile.labels.items()}
         publish_labels_to_ui(profile.labels)
 
         timers = []
 
         # process common jobs
         for job in profile.common:
@@ -172,17 +214,17 @@
             while any((timer.is_alive() for timer in timers)) and not state.exit_event.wait(10):
                 pass
         finally:
             if state.exit_event.is_set():
                 # ended early
                 for timer in timers:
                     timer.cancel()
-                logger.debug("Finished execution early. Exiting.")
+                logger.info(f"Exiting profile {profile.experiment_profile_name} early.")
             else:
-                logger.debug("Finished execution. Exiting.")
+                logger.info(f"Finished at commands in profile {profile.experiment_profile_name}.")
 
 
 @click.group(name="experiment_profile")
 def click_experiment_profile():
     pass
```

## pioreactor/automations/dosing/base.py

```diff
@@ -460,15 +460,15 @@
                 )
                 briefer_pause()
 
         return volumes_moved
 
     @property
     def most_stale_time(self) -> datetime:
-        return min(self.latest_normalized_od_at, self.latest_growth_rate_at)
+        return min(self.latest_normalized_od_at, self.latest_growth_rate_at, self.latest_od_at)
 
     @property
     def latest_growth_rate(self) -> float:
         # check if None
         if self._latest_growth_rate is None:
             # this should really only happen on the initialization.
             self.logger.debug("Waiting for OD and growth rate data to arrive")
@@ -510,17 +510,17 @@
         if self._latest_od is None:
             # this should really only happen on the initialization.
             self.logger.debug("Waiting for OD and growth rate data to arrive")
             if not is_pio_job_running("od_reading"):
                 raise exc.JobRequiredError("`od_reading` should be Ready.")
 
         # check most stale time
-        if (current_utc_datetime() - self.most_stale_time).seconds > 5 * 60:
+        if (current_utc_datetime() - self.latest_od_at).seconds > 5 * 60:
             raise exc.JobRequiredError(
-                f"readings are too stale (over 5 minutes old) - is `od_reading` running?. Last reading occurred at {self.most_stale_time}."
+                f"readings are too stale (over 5 minutes old) - is `od_reading` running?. Last reading occurred at {self.latest_od_at}."
             )
 
         assert self._latest_od is not None
         return self._latest_od
 
     ########## Private & internal methods
```

## pioreactor/automations/led/base.py

```diff
@@ -170,15 +170,15 @@
     def execute(self) -> Optional[events.AutomationEvent]:
         pass
 
     @property
     def most_stale_time(self) -> datetime:
         return min(self.latest_normalized_od_at, self.latest_growth_rate_at)
 
-    def set_led_intensity(self, channel: pt.LedChannel, intensity: float) -> bool:
+    def set_led_intensity(self, channel: pt.LedChannel, intensity: pt.LedIntensityValue) -> bool:
         """
         This first checks the lock on the LED channel, and will wait a few seconds for it to clear,
         and error out if it waits too long.
 
         Parameters
         ------------
 
@@ -258,15 +258,15 @@
         self._latest_settings_ended_at = current_utc_datetime()
         self._send_details_to_mqtt()
 
         with suppress(AttributeError):
             self.run_thread.join()
 
         led_intensity(
-            {channel: 0 for channel in self.edited_channels},
+            {channel: 0.0 for channel in self.edited_channels},
             unit=self.unit,
             experiment=self.experiment,
             source_of_event=f"{self.job_name}:{self.automation_name}",
         )
 
     def __setattr__(self, name, value) -> None:
         super(LEDAutomationJob, self).__setattr__(name, value)
```

## pioreactor/automations/led/light_dark_cycle.py

```diff
@@ -1,88 +1,109 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+from typing import Optional
+
 from pioreactor.automations import events
 from pioreactor.automations.led.base import LEDAutomationJob
 from pioreactor.types import LedChannel
 
 
 class LightDarkCycle(LEDAutomationJob):
     """
-    Follows as h light / h dark cycle. Starts light ON.
+    Follows as min light / min dark cycle. Starts light ON.
     """
 
     automation_name: str = "light_dark_cycle"
     published_settings = {
         "duration": {
             "datatype": "float",
             "settable": False,
             "unit": "min",
         },
         "light_intensity": {"datatype": "float", "settable": True, "unit": "%"},
-        "light_duration_hours": {"datatype": "integer", "settable": True, "unit": "h"},
-        "dark_duration_hours": {"datatype": "integer", "settable": True, "unit": "h"},
+        "light_duration_minutes": {"datatype": "integer", "settable": True, "unit": "min"},
+        "dark_duration_minutes": {"datatype": "integer", "settable": True, "unit": "min"},
     }
 
     def __init__(
         self,
         light_intensity: float | str,
-        light_duration_hours: int | str,
-        dark_duration_hours: int | str,
+        light_duration_minutes: int | str,
+        dark_duration_minutes: int | str,
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.hours_online: int = -1
+        self.minutes_online: int = -1
         self.light_active: bool = False
         self.channels: list[LedChannel] = ["D", "C"]
         self.set_light_intensity(light_intensity)
-        self.light_duration_hours = float(light_duration_hours)
-        self.dark_duration_hours = float(dark_duration_hours)
-
-    def execute(self) -> events.AutomationEvent:
-        self.hours_online += 1
-        return self.trigger_leds(self.hours_online)
-
-    def trigger_leds(self, hours: int) -> events.AutomationEvent:
-        cycle_duration = self.light_duration_hours + self.dark_duration_hours
+        self.light_duration_minutes = float(light_duration_minutes)
+        self.dark_duration_minutes = float(dark_duration_minutes)
 
-        if ((hours % cycle_duration) < self.light_duration_hours) and (not self.light_active):
+    def execute(self) -> Optional[events.AutomationEvent]:
+        # runs every minute
+        self.minutes_online += 1
+        return self.trigger_leds(self.minutes_online)
+
+    def trigger_leds(self, minutes: int) -> Optional[events.AutomationEvent]:
+        """
+        Changes the LED state based on the current minute in the cycle.
+
+        The light and dark periods are calculated as multiples of 60 minutes, forming a cycle.
+        Based on where in this cycle the current minute falls, the light is either turned ON or OFF.
+
+        Args:
+            minutes: The current minute of the cycle.
+
+        Returns:
+            An instance of AutomationEvent, indicating that LEDs' status might have changed.
+            Returns None if the LEDs' state didn't change.
+        """
+        cycle_duration_min = int(self.light_duration_minutes + self.dark_duration_minutes)
+
+        if ((minutes % cycle_duration_min) < (self.light_duration_minutes)) and (
+            not self.light_active
+        ):
             self.light_active = True
 
             for channel in self.channels:
                 self.set_led_intensity(channel, self.light_intensity)
 
-            return events.ChangedLedIntensity(f"{hours}h: turned on LEDs.")
+            return events.ChangedLedIntensity(f"{minutes:.1f}min: turned on LEDs.")
 
-        elif ((hours % cycle_duration) >= self.light_duration_hours) and (self.light_active):
+        elif ((minutes % cycle_duration_min) >= (self.light_duration_minutes)) and (
+            self.light_active
+        ):
             self.light_active = False
             for channel in self.channels:
                 self.set_led_intensity(channel, 0)
-            return events.ChangedLedIntensity(f"{hours}h: turned off LEDs.")
+            return events.ChangedLedIntensity(f"{minutes:.1f}min: turned off LEDs.")
 
         else:
-            return events.NoEvent(f"{hours}h: no change.")
+            return None
 
-    def set_dark_duration_hours(self, hours: int):
-        self.dark_duration_hours = hours
+    # minutes setters
+    def set_dark_duration_minutes(self, minutes: int):
+        self.dark_duration_minutes = minutes
 
-        self.trigger_leds(self.hours_online)
+        self.trigger_leds(self.minutes_online)
 
-    def set_light_duration_hours(self, hours: int):
-        self.light_duration_hours = hours
+    def set_light_duration_minutes(self, minutes: int):
+        self.light_duration_minutes = minutes
 
-        self.trigger_leds(self.hours_online)
+        self.trigger_leds(self.minutes_online)
 
     def set_light_intensity(self, intensity: float | str):
         # this is the settr of light_intensity attribute, eg. called when updated over MQTT
         self.light_intensity = float(intensity)
         if self.light_active:
             # update now!
             for channel in self.channels:
                 self.set_led_intensity(channel, self.light_intensity)
         else:
             pass
 
     def set_duration(self, duration: float) -> None:
-        if duration != 60:
-            self.logger.warning("Duration should be set to 60.")
+        if duration != 1:
+            self.logger.warning("Duration should be set to 1.")
         super().set_duration(duration)
```

## pioreactor/automations/temperature/thermostat.py

```diff
@@ -29,33 +29,29 @@
             Ki=config.getfloat("temperature_automation.thermostat", "Ki"),
             Kd=config.getfloat("temperature_automation.thermostat", "Kd"),
             setpoint=self.target_temperature,
             unit=self.unit,
             experiment=self.experiment,
             job_name=self.job_name,
             target_name="temperature",
+            output_limits=(-25, 25),  # avoid whiplashing
         )
 
     def execute(self) -> UpdatedHeaterDC:
         while not hasattr(self, "pid"):
             # sometimes when initializing, this execute can run before the subclasses __init__ is resolved.
             pass
 
         assert self.latest_temperature is not None
         output = self.pid.update(
             self.latest_temperature, dt=1
         )  # 1 represents an arbitrary unit of time. The PID values will scale such that 1 makes sense.
         self.update_heater_with_delta(output)
         self.logger.debug(f"PID output = {output}")
 
-        if (self.target_temperature - self.latest_temperature > 0) and self.heater_duty_cycle >= 98:
-            self.logger.warning(
-                f"Target temperature {self.target_temperature} unlikely to be able to be achieved. Try raising the ambient temperature."
-            )
-
         return UpdatedHeaterDC(
             f"delta_dc={output}",
             data={
                 "current_dc": self.heater_duty_cycle,
                 "delta_dc": output,
             },
         )
```

## pioreactor/background_jobs/base.py

```diff
@@ -16,14 +16,15 @@
 from pioreactor import types as pt
 from pioreactor.config import config
 from pioreactor.config import leader_address
 from pioreactor.config import leader_hostname
 from pioreactor.logging import create_logger
 from pioreactor.pubsub import Client
 from pioreactor.pubsub import create_client
+from pioreactor.pubsub import MQTT_TOPIC
 from pioreactor.pubsub import QOS
 from pioreactor.pubsub import subscribe
 from pioreactor.utils import append_signal_handlers
 from pioreactor.utils import is_pio_job_running
 from pioreactor.utils import local_intermittent_storage
 from pioreactor.utils.timing import current_utc_timestamp
 from pioreactor.utils.timing import RepeatedTimer
@@ -126,14 +127,26 @@
                           │            │                   │
                           │  sleeping  ├───────────────────┘
                           │            │
                           └────────────┘
 
     https://asciiflow.com/#/share/eJzNVEsKgzAQvYrM2lW7Uc%2BSjehQAmksmoIi3qJ4kC7F0%2FQkTS0tRE0crYuGWWSEeZ95wRpkfEaI5FUIH0RcYQ4R1AxKBlEYhD6DSt8OwVHfFJZKNww8wnnc%2BsViTBKhjOYzRqHYXm2nKURWqBdT2xFsGDrnDYytzLsioEzVjr5sQ7b2GoOyNWOGWCbn2pzewizaR0bmyCab%2BAJyyRVJ0PBSvBzjtFphQE%2BlvEgyKTFRmBrU%2B3rZIzXL%2B3Kn1t4dqXn2M6Cafqbu%2FxxicYHUSBZpHC0VoBCIFy5PP%2F9TV%2Bgkb87BBg00T7Hk%2FaY%3D)
 
+    states-mermaid-diagram
+        init --> ready
+        init --> lost
+        ready --> lost
+        ready --> disconnected
+        ready --> sleeping
+        sleeping --> ready
+        sleeping --> lost
+        sleeping --> disconnected
+        disconnected --> lost
+
+
     1. The job starts in `init`,
         - we publish `published_settings`: a list of variables that will be sent to the broker on initialization and retained.
         - we set up how to disconnect
         - the subclass runs their __init__ method
     2. The job moves to `ready`, and can be paused by entering `sleeping`.
     3. We catch key interrupts and kill signals from the underlying machine, and set the state to `disconnected`.
     4. If the job exits otherwise (kill -9, power loss, bug), the state is `lost`, and a last-will saying so is broadcast.
@@ -297,15 +310,44 @@
 
         # this should happen _after_ pub clients are set up
         self.start_general_passive_listeners()
 
         # next thing that run is the subclasses __init__
 
     def __post__init__(self) -> None:
-        # this function is called AFTER the subclass' __init__ finishes
+        """
+        This function is called AFTER the subclass' __init__ finishes successfully
+
+        Typical sequence (doesn't represent not calling stack, but "blocks of code" run)
+
+        P.__init__() # check for duplicate job
+        C.__init__() # risk of job failing here
+        P.__post__init__()  # write metadata to disk
+        P.on_init_to_ready()  # default noop - can be overwritten in sub.
+        P.ready()
+        C.on_ready()
+        """
+
+        with local_intermittent_storage(f"job_metadata_{self.job_name}") as cache:
+            # we set the "lock" in ready as then we know the __init__ finished successfully. Previously,
+            # __init__ might fail, and not clean up pio_job_* correctly.
+            # the catch is that there is a window where two jobs can be started, see growth_rate_calculating.
+            # sol for authors: move the long-running parts to the on_init_to_ready function.
+            cache["started_at"] = current_utc_timestamp()
+            cache["is_running"] = "1"
+            cache["source"] = self._source
+            cache["experiment"] = self.experiment
+            cache["unit"] = self.unit
+            cache["leader_hostname"] = leader_hostname
+            cache["pid"] = getpid()
+            cache["ended_at"] = ""  # populated later
+
+        with local_intermittent_storage("pio_jobs_running") as cache:
+            cache[self.job_name] = getpid()
+
         self.set_state(self.READY)
 
     def start_passive_listeners(self) -> None:
         # overwrite this to in subclasses to subscribe to topics in MQTT
         # using this handles reconnects correctly.
         pass
 
@@ -379,15 +421,15 @@
             payload = dumps(payload)
 
         self.pub_client.publish(topic, payload=payload, **kwargs)
 
     def subscribe_and_callback(
         self,
         callback: t.Callable[[pt.MQTTMessage], None],
-        subscriptions: list[str] | str,
+        subscriptions: list[str | MQTT_TOPIC] | str | MQTT_TOPIC,
         allow_retained: bool = True,
         qos: int = QOS.AT_MOST_ONCE,
     ) -> None:
         """
         Parameters
         -------------
         callback: callable
@@ -417,20 +459,28 @@
 
         assert callable(
             callback
         ), "callback should be callable - do you need to change the order of arguments?"
 
         subscriptions = [subscriptions] if isinstance(subscriptions, str) else subscriptions
 
-        for sub in subscriptions:
-            self.sub_client.message_callback_add(sub, wrap_callback(callback))
-            self.sub_client.subscribe(sub, qos=qos)
+        for topic in subscriptions:
+            self.sub_client.message_callback_add(str(topic), wrap_callback(callback))
+            self.sub_client.subscribe(str(topic), qos=qos)
         return
 
     def set_state(self, new_state: pt.JobState) -> None:
+        """
+        The preferred way to change states is to use this function (instead of self.state = state). Note:
+
+         - no-op if in the same state
+         - will call the transition callback
+
+        """
+
         if new_state not in {self.INIT, self.READY, self.DISCONNECTED, self.SLEEPING, self.LOST}:
             self.logger.error(f"saw {new_state}: not a valid state")
             return
 
         if new_state == self.state:
             return
 
@@ -671,30 +721,14 @@
             self.clean_up()
             raise e
 
         self._log_state(self.state)
 
     def ready(self) -> None:
         self.state = self.READY
-        with local_intermittent_storage(f"job_metadata_{self.job_name}") as cache:
-            # we set the "lock" in ready as then we know the __init__ finished successfully. Previously,
-            # __init__ might fail, and not clean up pio_job_* correctly.
-            # the catch is that there is a window where two jobs can be started, see growth_rate_calculating.
-            # sol for authors: move the long-running parts to the on_init_to_ready function.
-            cache["started_at"] = current_utc_timestamp()
-            cache["is_running"] = "1"
-            cache["source"] = self._source
-            cache["experiment"] = self.experiment
-            cache["unit"] = self.unit
-            cache["leader_hostname"] = leader_hostname
-            cache["pid"] = getpid()
-            cache["ended_at"] = ""  # populated later
-
-        with local_intermittent_storage("pio_jobs_running") as cache:
-            cache[self.job_name] = getpid()
 
         try:
             self.on_ready()
         except Exception as e:
             self.logger.error(e)
             self.logger.debug("Error in on_ready:")
             self.logger.debug(e, exc_info=True)
@@ -930,15 +964,15 @@
 
 class BackgroundJobContrib(_BackgroundJob):
     """
     Plugin jobs should inherit from this class.
     """
 
     def __init__(self, experiment: str, unit: str, plugin_name: str) -> None:
-        super().__init__(experiment=experiment, unit=unit, source="app")
+        super().__init__(experiment=experiment, unit=unit, source=plugin_name)
 
 
 class BackgroundJobWithDodging(_BackgroundJob):
     """
     This utility class allows for a change in behaviour when an OD reading is about to taken. Example: shutting
     off a air-bubbler, or shutting off a pump or valve, with appropriate delay between.
```

## pioreactor/background_jobs/dosing_control.py

```diff
@@ -159,17 +159,17 @@
 
 @click.command(
     name="dosing_control",
     context_settings=dict(ignore_unknown_options=True, allow_extra_args=True),
 )
 @click.option(
     "--automation-name",
-    default="silent",
     help="set the automation of the system: turbidostat, morbidostat, silent, etc.",
     show_default=True,
+    required=True,
 )
 @click.option(
     "--duration",
     default=60,
     type=float,
     help="Time, in minutes, between every monitor check",
 )
```

## pioreactor/background_jobs/growth_rate_calculating.py

```diff
@@ -235,14 +235,15 @@
 
     def _compute_and_cache_od_statistics(
         self,
     ) -> tuple[dict[pt.PdChannel, float], dict[pt.PdChannel, float]]:
         means, variances = od_statistics(
             self._yield_od_readings_from_mqtt(),
             action_name="od_normalization",
+            n_samples=35,
             unit=self.unit,
             experiment=self.experiment,
             logger=self.logger,
         )
         self.logger.info("Completed OD normalization metrics.")
 
         with local_persistant_storage("od_normalization_mean") as cache:
```

## pioreactor/background_jobs/led_control.py

```diff
@@ -118,17 +118,17 @@
 
 @click.command(
     name="led_control",
     context_settings=dict(ignore_unknown_options=True, allow_extra_args=True),
 )
 @click.option(
     "--automation-name",
-    default="silent",
     help="set the automation of the system: silent, etc.",
     show_default=True,
+    required=True,
 )
 @click.option("--duration", default=60.0, help="Time, in minutes, between every monitor check")
 @click.option(
     "--skip-first-run",
     type=click.IntRange(min=0, max=1),
     help="Normally algo will run immediately. Set this flag to wait <duration>min before executing.",
 )
```

## pioreactor/background_jobs/monitor.py

```diff
@@ -221,31 +221,51 @@
                 )
                 status = result.stdout.strip()
 
                 # Check if the output is okay
                 if status == "failed" or status == "inactive":
                     self.logger.error("lighttpd is not running. Check `systemctl status lighttpd`.")
                     self.flicker_led_with_error_code(error_codes.WEBSERVER_OFFLINE)
-
                 elif status == "activating":
                     # try again
                     pass
-
                 elif status == "active":
                     # okay
                     break
-
                 else:
                     raise ValueError(status)
-
         except Exception as e:
             self.logger.debug(f"Error checking lighttpd status: {e}", exc_info=True)
             self.logger.error(f"Error checking lighttpd status: {e}")
 
         try:
+            while True:
+                # Run the command 'systemctl is-active huey' and capture the output
+                result = subprocess.run(
+                    ["systemctl", "is-active", "huey"], capture_output=True, text=True
+                )
+                status = result.stdout.strip()
+
+                # Check if the output is okay
+                if status == "failed" or status == "inactive":
+                    self.logger.error("huey is not running. Check `systemctl status huey`.")
+                    self.flicker_led_with_error_code(error_codes.WEBSERVER_OFFLINE)
+                elif status == "activating":
+                    # try again
+                    pass
+                elif status == "active":
+                    # okay
+                    break
+                else:
+                    raise ValueError(status)
+        except Exception as e:
+            self.logger.debug(f"Error checking huey status: {e}", exc_info=True)
+            self.logger.error(f"Error checking huey status: {e}")
+
+        try:
             # can we ping ourselves? should have a response
             res = get("http://localhost")
             res.raise_for_status()
         except Exception as e:
             self.logger.debug(f"Error pinging UI: {e}", exc_info=True)
             self.logger.error(f"Error pinging UI: {e}")
             self.flicker_led_with_error_code(error_codes.WEBSERVER_OFFLINE)
@@ -391,30 +411,32 @@
         self.button_down = False
 
     def rpi_is_having_power_problems(self) -> tuple[bool, float]:
         from pioreactor.utils.rpi_bad_power import new_under_voltage
         from pioreactor.hardware import voltage_in_aux
 
         voltage_read = voltage_in_aux(precision=0.05)
-        if voltage_read <= 4.9:
+        if voltage_read <= 4.80:
             return (True, voltage_read)
 
         under_voltage = new_under_voltage()
         if under_voltage is None:
             # not supported on system
             return (False, voltage_read)
         elif under_voltage.get():
             return (True, voltage_read)
         else:
             return (False, voltage_read)
 
     def check_for_power_problems(self) -> None:
         is_rpi_having_power_probems, voltage = self.rpi_is_having_power_problems()
-        self.logger.debug(f"PWM power supply at ~{voltage:.1f}V.")
-        self.voltage_on_pwm_rail = Voltage(voltage=voltage, timestamp=current_utc_datetime())
+        self.logger.debug(f"PWM power supply at ~{voltage:.2f}V.")
+        self.voltage_on_pwm_rail = Voltage(
+            voltage=round(voltage, 2), timestamp=current_utc_datetime()
+        )
         if is_rpi_having_power_probems:
             self.logger.warning(
                 f"Low-voltage detected on rail. PWM power supply at {voltage:.1f}V. Suggestion: use a better power supply or an AUX power. See docs at: https://docs.pioreactor.com/user-guide/external-power"
             )
             self.flicker_led_with_error_code(error_codes.VOLTAGE_PROBLEM)
         else:
             self.logger.debug("Power status okay.")
@@ -429,24 +451,24 @@
             # TODO: add documentation to clear disk space.
             self.logger.warning(f"Disk space at {disk_usage_percent}%.")
             self.flicker_led_with_error_code(error_codes.DISK_IS_ALMOST_FULL)
 
         cpu_usage_percent = round(
             (psutil.cpu_percent() + psutil.cpu_percent() + psutil.cpu_percent()) / 3
         )  # this is a noisy process, and we average it over a small window.
-        if cpu_usage_percent <= 75:
+        if cpu_usage_percent <= 85:
             self.logger.debug(f"CPU usage at {cpu_usage_percent}%.")
         else:
             # TODO: add documentation
             self.logger.warning(f"CPU usage at {cpu_usage_percent}%.")
 
         memory_usage_percent = 100 - round(
             100 * psutil.virtual_memory().available / psutil.virtual_memory().total
         )
-        if memory_usage_percent <= 60:
+        if memory_usage_percent <= 75:
             self.logger.debug(f"Memory usage at {memory_usage_percent}%.")
         else:
             # TODO: add documentation
             self.logger.warning(f"Memory usage at {memory_usage_percent}%.")
 
         cpu_temperature_celcius = round(utils.get_cpu_temperature())
         if cpu_temperature_celcius <= 70:
```

## pioreactor/background_jobs/od_reading.py

```diff
@@ -59,15 +59,15 @@
 │   │                                                          │  │                        │  │                        │   │
 │   │ ┌──────────────┐   ┌──────────────┐    ┌───────────────┐ │  │  ┌─────────────────┐   │  │  ┌─────────────────┐   │   │
 │   │ │              ├───►              ├────►               │ │  │  │                 │   │  │  │                 │   │   │
 │   │ │              │   │              │    │               │ │  │  │                 │   │  │  │                 │   │   │
 │   │ │ samples from ├───►   ADC offset ├────►      sin      ├─┼──┼──►  IR output      ├───┼──┼──►  Transform via  ├───┼───┼───►
 │   │ │     ADC      │   │    removed   │    │   regression  │ │  │  │  compensation   │   │  │  │  calibration    │   │   │
 │   │ │              ├───►              ├────►               │ │  │  │                 │   │  │  │  curve          │   │   │
-│   │ └──────────────┘   └──────────────┘    └───────────────┘ │  │  └─────────────────┘   │  │  │                 │   │   │
+│   │ └──────────────┘   └──────────────┘    └───────────────┘ │  │  └─────────────────┘   │  │  │  (or no-op)     │   │   │
 │   │                                                          │  │                        │  │  └─────────────────┘   │   │
 │   │                                                          │  │                        │  │                        │   │
 │   └──────────────────────────────────────────────────────────┘  └────────────────────────┘  └────────────────────────┘   │
 │                                                                                                                          │
 │                                                                                                                          │
 └──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┘
 
@@ -116,26 +116,42 @@
 VALID_PD_ANGLES: list[pt.PdAngle] = ["45", "90", "135", "180"]
 PdChannelToVoltage = dict[pt.PdChannel, pt.Voltage]
 
 REF_keyword = "REF"
 IR_keyword = "IR"
 
 
+def average_over_pd_channel_to_voltages(*pd_channel_to_voltages: PdChannelToVoltage):
+    running_count = 0
+    summed_pd_channel_to_voltage: PdChannelToVoltage = {}
+    for pd_channel_to_voltage in pd_channel_to_voltages:
+        for channel, voltage in pd_channel_to_voltage.items():
+            summed_pd_channel_to_voltage[channel] = (
+                summed_pd_channel_to_voltage.get(channel, 0) + voltage
+            )
+        running_count += 1
+
+    return {
+        channel: voltage / running_count
+        for channel, voltage in summed_pd_channel_to_voltage.items()
+    }
+
+
 class ADCReader(LoggerMixin):
     _logger_name = "adc_reader"
     _setup_complete = False
 
     def __init__(
         self,
         channels: list[pt.PdChannel],
         fake_data: bool = False,
         interval: Optional[float] = 1.0,
         dynamic_gain: bool = True,
-        penalizer: float = 525.0,
-        oversampling_count: int = 28,
+        penalizer: float = 700.0,
+        oversampling_count: int = 30,
     ) -> None:
         super().__init__()
         self.fake_data = fake_data
         self.dynamic_gain = dynamic_gain
         self.max_signal_moving_average = ExponentialMovingAverage(alpha=0.05)
         self.channels: list[pt.PdChannel] = channels
         self.batched_readings: PdChannelToVoltage = {}
@@ -415,15 +431,15 @@
                             )
 
                     sleep(
                         max(
                             0,
                             -time_sampling_took_to_run()  # the time_sampling_took_to_run() reduces the variance by accounting for the duration of each sampling.
                             + 0.85 / (oversampling_count - 1)
-                            + 0.0015
+                            + 0.0012
                             * (
                                 (counter * 0.618034) % 1
                             ),  # this is to artificially jitter the samples, so that we observe less aliasing. That constant is phi.
                         )
                     )
 
             batched_estimates_: PdChannelToVoltage = {}
@@ -621,15 +637,25 @@
         self.logger.debug("Not using any calibration.")
 
 
 class CachedCalibrationTransformer(CalibrationTransformer):
     def __init__(self, channel_angle_map: dict[pt.PdChannel, pt.PdAngle]) -> None:
         super().__init__()
 
-        self.models: dict[pt.PdChannel, Callable] = {}
+        try:
+            self.models = self.get_models_from_disk(channel_angle_map)
+        except Exception as e:
+            self.logger.debug(e, exc_info=True)
+            self.logger.error("Unable to load calibration models", exc_info=True)
+            raise e
+
+    def get_models_from_disk(
+        self, channel_angle_map: dict[pt.PdChannel, pt.PdAngle]
+    ) -> dict[pt.PdChannel, Callable]:
+        models: dict[pt.PdChannel, Callable] = {}
 
         with local_persistant_storage("current_od_calibration") as c:
             for channel, angle in channel_angle_map.items():
                 if angle in c:
                     calibration_data = decode(c[angle], type=structs.AnyODCalibration)  # type: ignore
                     name = calibration_data.name
 
@@ -642,27 +668,28 @@
                         raise exc.CalibrationError(msg)
                     # confirm that PD channel is the same as when calibration was performed
                     elif calibration_data.pd_channel != channel:
                         msg = f"The calibration `{name}` was calibrated with a different PD channel ({calibration_data.pd_channel} vs current: {channel})."
                         self.logger.error(msg)
                         raise exc.CalibrationError(msg)
                     else:
-                        self.models[channel] = self._hydrate_model(calibration_data)
+                        models[channel] = self._hydrate_model(calibration_data)
                         self.logger.debug(f"Using calibration `{name}` for channel {channel}")
 
                     # confirm that PD channel is the same as when calibration was performed
                     if calibration_data.pd_channel != channel:
                         msg = f"The calibration `{name}` was calibrated with a different PD channel ({calibration_data.pd_channel} vs current: {channel})."
                         self.logger.error(msg)
                         raise exc.CalibrationError(msg)
 
                 else:
                     self.logger.debug(
                         f"No calibration available for channel {channel}, angle {angle}, skipping."
                     )
+        return models
 
     def _hydrate_model(self, calibration_data: structs.ODCalibration) -> Callable[[float], float]:
         if calibration_data.curve_type == "poly":
             """
             Finds the smallest root in the range [minOD, maxOD] calibrated against.
 
             Note: if the calibration curve is non-monotonic, ie. has a maximum not on the boundary of the range,
@@ -787,14 +814,19 @@
         self.first_od_obs_time: Optional[float] = None
         self._set_for_iterating = threading.Event()
 
         self.ir_channel: pt.LedChannel = self._get_ir_led_channel_from_configuration()
         self.ir_led_intensity: pt.LedIntensityValue = config.getfloat(
             "od_config", "ir_led_intensity"
         )
+        if self.ir_led_intensity > 90:
+            self.logger.warning(
+                f"The value for the IR LED, {self.ir_led_intensity}%, is very high. We suggest a value 90% or less to avoid damaging the LED."
+            )
+
         self.non_ir_led_channels: list[pt.LedChannel] = [
             ch for ch in led_utils.ALL_LED_CHANNELS if ch != self.ir_channel
         ]
 
         if not hardware.is_HAT_present():
             self.logger.error("Pioreactor HAT must be present.")
             self.clean_up()
@@ -805,32 +837,36 @@
         )
 
         self.pre_read_callbacks: list[Callable] = self._prepare_pre_callbacks()
         self.post_read_callbacks: list[Callable] = self._prepare_post_callbacks()
 
         # setup the ADC by turning off all LEDs.
         with led_utils.change_leds_intensities_temporarily(
-            self.ir_led_on_and_rest_off_state,
+            {ch: 0.0 for ch in led_utils.ALL_LED_CHANNELS},
             unit=self.unit,
             experiment=self.experiment,
             source_of_event=self.job_name,
             pubsub_client=self.pub_client,
             verbose=False,
         ):
             with led_utils.lock_leds_temporarily(self.non_ir_led_channels):
                 # IR led is on
-                sleep(0.1)
-
+                self.start_ir_led()
+                sleep(0.10)
                 self.adc_reader.setup_adc()  # determine best gain, max-signal, etc.
 
+                # IR led is off so we can set blanks
                 self.stop_ir_led()
-                sleep(0.15)
+                sleep(0.10)
 
-                blank_reading = self.adc_reader.take_reading()
-                self.adc_reader.set_offsets(blank_reading)  # determine offset
+                avg_blank_reading = average_over_pd_channel_to_voltages(
+                    self.adc_reader.take_reading(),
+                    self.adc_reader.take_reading(),
+                )
+                self.adc_reader.set_offsets(avg_blank_reading)  # set dark offset
 
                 # clear the history in adc_reader, so that we don't blank readings in later inference.
                 self.adc_reader.clear_batched_readings()
 
         if (self.interval is not None) and self.interval > 0:
             if self.interval <= 1.0:
                 self.logger.warning(
@@ -1129,15 +1165,15 @@
         ir_led_reference_tracker = PhotodiodeIrLedReferenceTrackerStaticInit(
             ir_led_reference_channel,
         )
         channels.append(ir_led_reference_channel)
     else:
         ir_led_reference_tracker = NullIrLedReferenceTracker()  # type: ignore
 
-    # use OD600 calibration?
+    # use an OD calibration?
     if use_calibration:
         calibration_transformer = CachedCalibrationTransformer(channel_angle_map)
     else:
         calibration_transformer = NullCalibrationTransformer()  # type: ignore
 
     return ODReader(
         channel_angle_map,
```

## pioreactor/background_jobs/stirring.py

```diff
@@ -349,15 +349,15 @@
     def poll(self, poll_for_seconds: float) -> Optional[structs.MeasuredRPM]:
         """
         Returns an MeasuredRPM, or None if not measuring RPM.
         """
         if self.rpm_calculator is None:
             return None
 
-        recent_rpm = self.rpm_calculator(poll_for_seconds)
+        recent_rpm = round(self.rpm_calculator(poll_for_seconds), 1)
 
         self._measured_rpm = recent_rpm
         self.measured_rpm = structs.MeasuredRPM(
             timestamp=current_utc_datetime(), measured_rpm=self._measured_rpm
         )
 
         if recent_rpm == 0 and self.state == self.READY and not is_testing_env():
@@ -455,15 +455,15 @@
         return True
 
 
 def start_stirring(
     target_rpm: float,
     unit: Optional[str] = None,
     experiment: Optional[str] = None,
-    use_rpm: bool = False,
+    use_rpm: bool = True,
 ) -> Stirrer:
     unit = unit or get_unit_name()
     experiment = experiment or get_latest_experiment_name()
 
     if use_rpm:
         rpm_calculator = RpmFromFrequency()
     else:
```

## pioreactor/background_jobs/temperature_control.py

```diff
@@ -57,26 +57,23 @@
     the following:
 
         {
             "temperature": <float>,
             "timestamp": <ISO 8601 timestamp>
         }
 
-    If you have your own thermo-couple, you can publish to this topic, with the same schema
-    and all should just work™️. Set `using_third_party_thermocouple` to True in the class creation, too.
-
-
     Parameters
     ------------
-    using_third_party_thermocouple: bool
-        True if supplying an external thermometer that will publish to MQTT.
+
     """
 
-    MAX_TEMP_TO_REDUCE_HEATING = 61.5  # ~PLA glass transition temp
-    MAX_TEMP_TO_DISABLE_HEATING = 63.5
+    MAX_TEMP_TO_REDUCE_HEATING = (
+        63.0  # ~PLA glass transition temp, and I've gone safely above this an it's not a problem.
+    )
+    MAX_TEMP_TO_DISABLE_HEATING = 65.0  # probably okay, but can't stay here for too long
     MAX_TEMP_TO_SHUTDOWN = 66.0
 
     INFERENCE_SAMPLES_EVERY_T_SECONDS: float = 5.0
     INFERENCE_N_SAMPLES: int = 29
     INFERENCE_EVERY_N_SECONDS: float = 225.0
     inference_total_time: float = INFERENCE_SAMPLES_EVERY_T_SECONDS * INFERENCE_N_SAMPLES
     # PWM is on for (INFERENCE_EVERY_N_SECONDS - inference_total_time) seconds
@@ -94,16 +91,14 @@
     }
 
     def __init__(
         self,
         automation_name: str,
         unit: str,
         experiment: str,
-        eval_and_publish_immediately: bool = True,
-        using_third_party_thermocouple: bool = False,
         **kwargs,
     ) -> None:
         super().__init__(unit=unit, experiment=experiment)
 
         if not hardware.is_HAT_present():
             self.logger.error("Pioreactor HAT must be present.")
             self.clean_up()
@@ -115,33 +110,31 @@
             raise exc.HardwareNotFoundError("Heating PCB must be attached to Pioreactor HAT")
 
         if whoami.is_testing_env():
             from pioreactor.utils.mock import MockTMP1075 as TMP1075
         else:
             from TMP1075 import TMP1075  # type: ignore
 
-        self.using_third_party_thermocouple = using_third_party_thermocouple
+        self.heater_duty_cycle = 0.0
         self.pwm = self.setup_pwm()
-        self.update_heater(0)
 
-        if not self.using_third_party_thermocouple:
-            self.tmp_driver = TMP1075(address=hardware.TEMP)
-            self.read_external_temperature_timer = RepeatedTimer(
-                53,
-                self.read_external_temperature,
-                run_immediately=False,
-            ).start()
-
-            self.publish_temperature_timer = RepeatedTimer(
-                int(self.INFERENCE_EVERY_N_SECONDS),
-                self.infer_temperature,
-                run_after=self.INFERENCE_EVERY_N_SECONDS
-                - self.inference_total_time,  # This gives an automation a "full" PWM cycle to be on before an inference starts.
-                run_immediately=True,
-            ).start()
+        self.heating_pcb_tmp_driver = TMP1075(address=hardware.TEMP)
+        self.read_external_temperature_timer = RepeatedTimer(
+            53,
+            self.read_external_temperature,
+            run_immediately=False,
+        ).start()
+
+        self.publish_temperature_timer = RepeatedTimer(
+            int(self.INFERENCE_EVERY_N_SECONDS),
+            self.infer_temperature,
+            run_after=self.INFERENCE_EVERY_N_SECONDS
+            - self.inference_total_time,  # This gives an automation a "full" PWM cycle to be on before an inference starts.
+            run_immediately=True,
+        ).start()
 
         try:
             automation_class = self.available_automations[automation_name]
         except KeyError:
             raise KeyError(
                 f"Unable to find automation {automation_name}. Available automations are {list(self.available_automations.keys())}"
             )
@@ -158,25 +151,24 @@
         except Exception as e:
             self.logger.error(e)
             self.logger.debug(e, exc_info=True)
             self.clean_up()
             raise e
         self.automation_name = self.automation.automation_name
 
-        if not self.using_third_party_thermocouple:
-            if whoami.is_testing_env() or self._seconds_since_last_active() >= 10:
-                # if we turn off heating and turn on again, without some sort of time to cool, the first temperature looks wonky
-                self.temperature = Temperature(
-                    temperature=self.read_external_temperature(),
-                    timestamp=current_utc_datetime(),
-                )
+        if whoami.is_testing_env() or self.seconds_since_last_active_heating() >= 10:
+            # if we turn off heating and turn on again, without some sort of time to cool, the first temperature looks wonky
+            self.temperature = Temperature(
+                temperature=self.read_external_temperature(),
+                timestamp=current_utc_datetime(),
+            )
 
     @staticmethod
-    def _seconds_since_last_active() -> float:
-        with local_intermittent_storage("last_heating_timestamp") as cache:
+    def seconds_since_last_active_heating() -> float:
+        with local_intermittent_storage("temperature_and_heating") as cache:
             if "last_heating_timestamp" in cache:
                 return (
                     current_utc_datetime() - to_datetime(cache["last_heating_timestamp"])
                 ).total_seconds()
             else:
                 return 1_000_000
 
@@ -217,15 +209,15 @@
         """
         Read the current temperature from our sensor, in Celsius
         """
         running_sum, running_count = 0.0, 0
         try:
             # check temp is fast, let's do it a few times to reduce variance.
             for i in range(5):
-                running_sum += self.tmp_driver.get_temperature()
+                running_sum += self.heating_pcb_tmp_driver.get_temperature()
                 running_count += 1
                 sleep(0.05)
 
         except OSError as e:
             self.logger.debug(e, exc_info=True)
             raise exc.HardwareNotFoundError(
                 "Is the Heating PCB attached to the Pioreactor HAT? Unable to find temperature sensor."
@@ -235,14 +227,18 @@
         if averaged_temp == 0.0 and self.automation_name != "only_record_temperature":
             # this is a hardware fluke, not sure why, see #308. We will return something very high to make it shutdown
             # todo: still needed? last observed on  July 18, 2022
             self.logger.error("Temp sensor failure. Switching off. See issue #308")
             self._update_heater(0.0)
             self.set_automation(TemperatureAutomation(automation_name="only_record_temperature"))
 
+        with local_intermittent_storage("temperature_and_heating") as cache:
+            cache["heating_pcb_temperature"] = averaged_temp
+            cache["heating_pcb_temperature_at"] = current_utc_timestamp()
+
         return averaged_temp
 
     ##### internal and private methods ########
 
     def set_automation(self, algo_metadata: TemperatureAutomation) -> None:
         # TODO: this needs a better rollback. Ex: in except, something like
         # self.automation_job.set_state("init")
@@ -302,17 +298,21 @@
                 f"Unable to find automation {algo_metadata.automation_name}. Available automations are {list(self.available_automations.keys())}. Note: You need to restart this job to have access to newly-added automations."
             )
         except Exception as e:
             self.logger.debug(f"Change failed because of {str(e)}", exc_info=True)
             self.logger.warning(f"Change failed because of {str(e)}")
 
     def _update_heater(self, new_duty_cycle: float) -> bool:
-        self.heater_duty_cycle = clamp(0, float(new_duty_cycle), 100)
+        self.heater_duty_cycle = clamp(0.0, round(float(new_duty_cycle), 2), 100.0)
         self.pwm.change_duty_cycle(self.heater_duty_cycle)
 
+        if self.heater_duty_cycle == 0.0:
+            with local_intermittent_storage("temperature_and_heating") as cache:
+                cache["last_heating_timestamp"] = current_utc_timestamp()
+
         return True
 
     def _check_if_exceeds_max_temp(self, temp: float) -> float:
         if temp > self.MAX_TEMP_TO_SHUTDOWN:
             self.logger.error(
                 f"Temperature of heating surface has exceeded {self.MAX_TEMP_TO_SHUTDOWN}℃ - currently {temp}℃. This is beyond our recommendations. Shutting down Raspberry Pi to prevent further problems. Take caution when touching the heating surface and wetware."
             )
@@ -361,17 +361,14 @@
         with suppress(AttributeError):
             self._update_heater(0)
             self.pwm.cleanup()
 
         with suppress(AttributeError):
             self.automation_job.clean_up()
 
-        with local_intermittent_storage("last_heating_timestamp") as cache:
-            cache["last_heating_timestamp"] = current_utc_timestamp()
-
     def setup_pwm(self) -> PWM:
         hertz = 8  # technically this doesn't need to be high: it could even be 1hz. However, we want to smooth it's
         # impact (mainly: current sink), over the second. Ex: imagine freq=1hz, dc=40%, and the pump needs to run for
         # 0.3s. The influence of when the heat is one on the pump can be significant in a power-constrained system.
         pin = hardware.PWM_TO_PIN[hardware.HEATER_PWM_TO_PIN]
         pwm = PWM(pin, hertz, unit=self.unit, experiment=self.experiment)
         pwm.start(0)
@@ -418,14 +415,15 @@
                     if self.state != self.READY:
                         # if our state changes in this loop, exit. Note that the finally block is still called.
                         return
 
             except exc.HardwareNotFoundError as e:
                 self.logger.debug(e, exc_info=True)
                 self.logger.error(e)
+                raise e
             finally:
                 # we turned off the heater above - we should always turn if back on if there is an error.
 
                 # update heater first before publishing the temperature. Why? A downstream process
                 # might listen for the updating temperature, and update the heater (pid_thermostat),
                 # and if we update here too late, we may overwrite their changes.
                 # We also want to remove the lock first, so close this context early.
@@ -459,60 +457,38 @@
         Extensions
         --------------
 
         1. It's possible that we can determine if the vial is in the sleeve by examining the heat loss coefficient.
         2. We have prior information about what p, q are => we have prior information about A, B. We use this.
            From the equations, B = p + q, A = -p * q, so weak prior in B ~ Normal(-0.143, ...), A = Normal(-0.00042, ....)
         3. Room temp has a moderate impact on inference: ~0.30C over a wide range of values
-
-
         """
 
         if features["previous_heater_dc"] == 0:
             return features["time_series_of_temp"][-1]
 
         import numpy as np
         from numpy import exp
 
         times_series = features["time_series_of_temp"]
         room_temp = features["room_temp"]
-
         n = len(times_series)
         y = np.array(times_series) - room_temp
         x = np.arange(n)  # scaled by factor of 1/10 seconds
 
         # first regression
         S = np.zeros(n)
         SS = np.zeros(n)
         for i in range(1, n):
             S[i] = S[i - 1] + 0.5 * (y[i - 1] + y[i]) * (x[i] - x[i - 1])
             SS[i] = SS[i - 1] + 0.5 * (S[i - 1] + S[i]) * (x[i] - x[i - 1])
 
         # priors chosen based on historical data, penalty values pretty arbitrary, note: B = p + q, A = -p * q
-        # TODO: update these priors as we develop more Pioreactors
-        # observed data:
-        #  B=-0.1244534657804866,  A=-0.00012566629719875475 (May 24, 2022)
-        #  B=-0.14928314914531557, A=-0.000376953627819461
-        #  B=-0.13807398778473443, A=-0.00021395682471394434
-        #  B=-0.14123191941209473, A=-0.0005287562253399032 (May 25, 2022)
-        #  B=-0.15192316555127186, A=-0.000894869124798112
-        #  A=-0.001295916914002933, B=-0.17905413150045976 (Sept 13, 2022, two modern Pioreactors)
-        #  A=-0.0010803409392903384, B=-0.17152656184261297
-        #  A=-0.0010674444548854495, B=-0.17115312722794235
-        #  A=-0.0011996267624624331, B=-0.17190309667476145
-        #  A=-0.0011066911804701845, B=-0.17196962637032628
-        #  A=-0.001150016228923988, B=-0.18975899991350298
-        #  A=-0.001082333547509889, B=-0.18685445997491493
-        #  A=-0.0010607908095388548, B=-0.18749701076543562
-        #  A=-0.0010514517340740343, B=-0.18756448817069307
-        #  A=-0.0012910773630121675, B=-0.19066684235126932
-        #  A=-0.0010558024149891808, B=-0.1613921733824975 (Oct 10, 2022)
-
-        A_penalizer, A_prior = 100.0, -0.0011
-        B_penalizer, B_prior = 20.0, -0.170
+        A_penalizer, A_prior = 100.0, -0.0012
+        B_penalizer, B_prior = 50.0, -0.325
 
         M1 = np.array(
             [
                 [
                     (SS**2).sum() + A_penalizer,
                     (SS * S).sum(),
                     (SS * x).sum(),
@@ -570,20 +546,19 @@
             self.logger.error("Error in temperature inference.")
             self.logger.debug("Error in temperature inference's second regression.", exc_info=True)
             self.logger.debug(f"x={x}")
             self.logger.debug(f"y={y}")
             raise ValueError()
 
         alpha, beta = b, p
-        temp_at_start_of_obs = room_temp + alpha * exp(beta * 0)
-        temp_at_end_of_obs = room_temp + alpha * exp(beta * n)
 
-        # This weighting is pretty arbitrary.
+        # this weighting is from evaluating the "average" temp over the period: 1/n int_0^n R + a*exp(b*s) ds
         # cast from numpy float to python float
-        return float(0.5 * temp_at_start_of_obs + 0.5 * temp_at_end_of_obs)
+        return float(room_temp + alpha * exp(beta * n))
+        # return float(room_temp + alpha * (exp(beta * n) - 1)/(beta * n))
 
 
 def start_temperature_control(
     automation_name: str,
     unit: Optional[str] = None,
     experiment: Optional[str] = None,
     **kwargs,
@@ -598,17 +573,17 @@
 
 @click.command(
     name="temperature_control",
     context_settings=dict(ignore_unknown_options=True, allow_extra_args=True),
 )
 @click.option(
     "--automation-name",
-    default="only_record_temperature",
     help="set the automation of the system",
     show_default=True,
+    required=True,
 )
 @click.pass_context
 def click_temperature_control(ctx, automation_name: str) -> None:
     """
     Start a temperature automation.
     """
     import os
```

## pioreactor/background_jobs/leader/mqtt_to_db_streaming.py

```diff
@@ -13,14 +13,15 @@
 from msgspec.json import decode as msgspec_loads
 
 from pioreactor import structs
 from pioreactor import types as pt
 from pioreactor.background_jobs.base import BackgroundJob
 from pioreactor.config import config
 from pioreactor.hardware import PWM_TO_PIN
+from pioreactor.pubsub import MQTT_TOPIC
 from pioreactor.pubsub import QOS
 from pioreactor.utils.sqlite_worker import Sqlite3Worker
 from pioreactor.utils.timing import current_utc_datetime
 from pioreactor.utils.timing import RepeatedTimer
 from pioreactor.utils.timing import to_iso_format
 from pioreactor.whoami import get_unit_name
 from pioreactor.whoami import UNIVERSAL_EXPERIMENT
@@ -40,21 +41,21 @@
 
     parser:
      - must return a dictionary | list[dictionary] with the column names as keys (order isn't important)
      - `produce_metadata` is a helper function, see definition.
      - parsers can return None as well, to skip adding the row to the database.
     """
 
-    topic: str | list[str]
+    topic: str | MQTT_TOPIC | list[str | MQTT_TOPIC]
     parser: Callable[[str, pt.MQTTMessagePayload], Optional[dict | list[dict]]]
     table: str
 
 
 class TopicToCallback(Struct):
-    topic: str | list[str]
+    topic: str | MQTT_TOPIC | list[str | MQTT_TOPIC]
     callback: Callable[[pt.MQTTMessage], None]
 
 
 class MqttToDBStreamer(BackgroundJob):
     topics_to_tables_from_plugins: list[TopicToParserToTable] = []
     job_name = "mqtt_to_db_streaming"
     published_settings = {
@@ -141,15 +142,15 @@
 
         return callback
 
     def initialize_callbacks(self, topics_and_callbacks: list[TopicToCallback]) -> None:
         for topic_and_callback in topics_and_callbacks:
             self.subscribe_and_callback(
                 topic_and_callback.callback,
-                topic_and_callback.topic,
+                str(topic_and_callback.topic),
                 qos=QOS.EXACTLY_ONCE,
                 allow_retained=False,
             )
 
 
 def produce_metadata(topic: str) -> MetaData:
     # helper function for parsers below
```

## pioreactor/background_jobs/leader/watchdog.py

```diff
@@ -56,17 +56,24 @@
             time.sleep(5)
 
             if self.state != self.READY:
                 # when the entire Rpi shuts down, ex via sudo reboot, monitor can publish a lost. This code will halt the shutdown.
                 # let's return early.
                 return
 
+            # this is a hack! If the monitor job is in state READY, it will no op any transition.
+            # so we set to sleeping for a second, and the back to ready.
+            self.pub_client.publish(
+                f"pioreactor/{unit}/{UNIVERSAL_EXPERIMENT}/monitor/$state/set", self.SLEEPING
+            )
+            time.sleep(1)
             self.pub_client.publish(
                 f"pioreactor/{unit}/{UNIVERSAL_EXPERIMENT}/monitor/$state/set", self.READY
             )
+            ###
             time.sleep(20)
 
             if self.state != self.READY:
                 # when the entire Rpi shuts down, ex via sudo reboot, monitor can publish a lost. This code will halt the shutdown.
                 # let's return early.
                 return
```

## pioreactor/cli/pio.py

```diff
@@ -51,16 +51,17 @@
 
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 def pio(ctx) -> None:
     """
     Execute commands on this Pioreactor.
-    See full documentation here: https://docs.pioreactor.com/user-guide/cli
-    Report errors or feedback here: https://github.com/Pioreactor/pioreactor/issues
+    Configuration available: /home/pioreactor/.pioreactor/config.ini
+    See full documentation: https://docs.pioreactor.com/user-guide/cli
+    Report errors or feedback: https://github.com/Pioreactor/pioreactor/issues
     """
 
     # if a user runs `pio`, we want the check_firstboot_successful to run, hence the invoke_without_command
     # https://click.palletsprojects.com/en/8.1.x/commands/#group-invocation-without-command
     if ctx.invoked_subcommand is None:
         click.echo(ctx.get_help())
 
@@ -135,18 +136,23 @@
         logger = create_logger(
             name,
             unit=whoami.get_unit_name(),
             experiment=whoami.UNIVERSAL_EXPERIMENT,
             to_mqtt=not local_only,
         )
         getattr(logger, level)(message)
-        sleep(0.5)  # wait to make sure msg gets to mqtt
-    except Exception:
+
+        # flush and close handlers
+        for handler in logger.logger.handlers:
+            handler.flush()
+            handler.close()
+
+    except Exception as e:
         # don't let a logging error bring down a script...
-        pass
+        print(e)
 
 
 @pio.command(name="blink", short_help="blink LED")
 def blink() -> None:
     monitor_running = is_pio_job_running("monitor")
 
     if not monitor_running:
@@ -366,19 +372,19 @@
 def update() -> None:
     """
     Update software for the app and UI
     """
     pass
 
 
-def get_non_prerelease_tags_of_pioreactor():
+def get_non_prerelease_tags_of_pioreactor(repo):
     """
     Returns a list of all the tag names associated with non-prerelease releases, sorted in descending order
     """
-    url = "https://api.github.com/repos/pioreactor/pioreactor/releases"
+    url = f"https://api.github.com/repos/{repo}/releases"
     headers = {"Accept": "application/vnd.github.v3+json"}
     response = get(url, headers=headers)
 
     if not response.ok:
         raise Exception(f"Failed to retrieve releases (status code: {response.status_code})")
 
     releases = response.json()
@@ -391,15 +397,15 @@
     def version_key(version):
         major, minor, patch = version.split(".")
         return int(major), int(minor), int(patch)
 
     return sorted(non_prerelease_tags, reverse=True, key=version_key)
 
 
-def get_tag_to_install(version_desired: Optional[str]) -> str:
+def get_tag_to_install(repo: str, version_desired: Optional[str]) -> str:
     """
     The function get_tag_to_install takes an optional argument version_desired and
     returns a string that represents the tag of a particular version of software to install.
 
     If version_desired is not provided or is None, the function determines the latest
     non-prerelease version of the software installed on the system, and returns the tag
     of the previous version as a string, or "latest" if the system is already up to date.
@@ -409,15 +415,15 @@
     Otherwise, the function returns the tag of the specified version as a string, preceded by "tags/".
     """
 
     if version_desired is None:
         # we should only update one step at a time.
         from pioreactor.version import __version__ as software_version
 
-        version_history = get_non_prerelease_tags_of_pioreactor()
+        version_history = get_non_prerelease_tags_of_pioreactor(repo)
 
         if software_version in version_history:
             ix = version_history.index(software_version)
 
             if ix >= 1:
                 tag = f"tags/{version_history[ix-1]}"  # update to the succeeding version.
             elif ix == 0:
@@ -432,17 +438,25 @@
         tag = f"tags/{version_desired}"
 
     return tag
 
 
 @update.command(name="app")
 @click.option("-b", "--branch", help="install from a branch on github")
+@click.option(
+    "-r",
+    "--repo",
+    help="install from a repo on github. Format: username/project",
+    default="pioreactor/pioreactor",
+)
 @click.option("--source", help="use a URL or whl file")
 @click.option("-v", "--version", help="install a specific version, default is latest")
-def update_app(branch: Optional[str], source: Optional[str], version: Optional[str]) -> None:
+def update_app(
+    branch: Optional[str], repo: str, source: Optional[str], version: Optional[str]
+) -> None:
     """
     Update the Pioreactor core software
     """
 
     logger = create_logger(
         "update-app", unit=whoami.get_unit_name(), experiment=whoami.UNIVERSAL_EXPERIMENT
     )
@@ -453,22 +467,22 @@
         version_installed = source
         commands_and_priority.append((f"sudo pip3 install -U --force-reinstall {source}", 1))
 
     elif branch is not None:
         version_installed = quote(branch)
         commands_and_priority.append(
             (
-                f"sudo pip3 install -U --force-reinstall https://github.com/pioreactor/pioreactor/archive/{branch}.zip",
+                f"sudo pip3 install -U --force-reinstall https://github.com/{repo}/archive/{branch}.zip",
                 1,
             )
         )
 
     else:
-        tag = get_tag_to_install(version)
-        response = get(f"https://api.github.com/repos/pioreactor/pioreactor/releases/{tag}")
+        tag = get_tag_to_install(repo, version)
+        response = get(f"https://api.github.com/repos/{repo}/releases/{tag}")
         if response.raise_for_status():
             logger.error(f"Version {version} not found")
             raise click.Abort()
 
         release_metadata = loads(response.body)
         version_installed = release_metadata["tag_name"]
         for asset in release_metadata["assets"]:
@@ -531,15 +545,15 @@
             logger.debug(p.stderr)
             logger.error("Update failed. See logs.")
             # end early
             raise click.Abort()
         else:
             logger.debug(p.stdout)
 
-    logger.notice(f"Updated Pioreactor to version {version_installed}.")  # type: ignore
+    logger.notice(f"Updated {whoami.get_unit_name()} to version {version_installed}.")  # type: ignore
 
 
 @update.command(name="firmware")
 @click.option("-v", "--version", help="install a specific version, default is latest")
 def update_firmware(version: Optional[str]) -> None:
     """
     Update the RP2040 firmware
@@ -642,15 +656,16 @@
 
         os.system(
             f"""mosquitto_sub -v -t '{topic}' -F "%19.19I  |  %t   %p" -u pioreactor -P raspberry"""
         )
 
     @pio.command(name="add-pioreactor", short_help="add a new Pioreactor to cluster")
     @click.argument("hostname")
-    def add_pioreactor(hostname: str) -> None:
+    @click.option("--password", "-p", default="raspberry")
+    def add_pioreactor(hostname: str, password: str) -> None:
         """
         Add a new pioreactor worker to the cluster. The pioreactor should already have the worker image installed and is turned on.
 
         hostname is without any .local.
         """
         # TODO: move this to its own file
         import socket
@@ -678,15 +693,15 @@
                 if checks >= max_checks:
                     logger.error(
                         f"`{hostname}` not found on network after more than {max_checks * sleep_time} seconds. Check that you provided the right WiFi credentials to the network, and that the Raspberry Pi is turned on."
                     )
                     raise click.Abort()
 
         res = subprocess.run(
-            ["bash", "/usr/local/bin/add_new_pioreactor_worker_from_leader.sh", hostname],
+            ["bash", "/usr/local/bin/add_new_pioreactor_worker_from_leader.sh", hostname, password],
             capture_output=True,
             text=True,
         )
         if res.returncode == 0:
             logger.notice(f"New pioreactor {hostname} successfully added to cluster.")  # type: ignore
         else:
             logger.error(res.stderr)
@@ -742,15 +757,17 @@
             return ip, state, reachable
 
         def display_data_for(hostname_status: tuple[str, str]) -> bool:
             hostname, status = hostname_status
 
             ip, state, reachable = get_network_metadata(hostname)
 
-            statef = click.style(f"{state:15s}", fg="green" if state == "ready" else "red")
+            statef = click.style(
+                f"{state:15s}", fg="green" if state in ("ready", "init") else "red"
+            )
             ipf = f"{ip if (ip is not None) else 'unknown':20s}"
 
             is_leaderf = f"{('Y' if hostname==get_leader_hostname() else 'N'):15s}"
             hostnamef = f"{hostname:20s}"
             reachablef = f"{(click.style('Y', fg='green') if reachable       else click.style('N', fg='red')):23s}"
             statusf = f"{(click.style('Y', fg='green') if (status == '1') else click.style('N', fg='red')):14s}"
 
@@ -771,17 +788,25 @@
             results = executor.map(display_data_for, worker_statuses)
 
         if not all(results):
             exit(1)
 
     @update.command(name="ui")
     @click.option("-b", "--branch", help="install from a branch on github")
+    @click.option(
+        "-r",
+        "--repo",
+        help="install from a repo on github. Format: username/project",
+        default="pioreactor/pioreactorui",
+    )
     @click.option("--source", help="use a tar.gz file")
     @click.option("-v", "--version", help="install a specific version")
-    def update_ui(branch: Optional[str], source: Optional[str], version: Optional[str]) -> None:
+    def update_ui(
+        branch: Optional[str], repo: str, source: Optional[str], version: Optional[str]
+    ) -> None:
         """
         Update the PioreactorUI
 
         Source, if provided, should be a .tar.gz with a top-level dir like pioreactorui-{branch}/
         This is what is provided from Github releases.
         """
         logger = create_logger(
@@ -796,24 +821,24 @@
 
         if source is not None:
             assert branch is not None, "branch must be provided with the -b option"
             version_installed = branch
 
         elif branch is not None:
             version_installed = quote(branch)
-            url = f"https://github.com/Pioreactor/pioreactorui/archive/{branch}.tar.gz"
+            url = f"https://github.com/{repo}/archive/{branch}.tar.gz"
             source = "/tmp/pioreactorui.tar.gz"
             commands.append(["wget", url, "-O", source])
 
         else:
             latest_release_metadata = loads(
-                get(f"https://api.github.com/repos/pioreactor/pioreactorui/releases/{version}").body
+                get(f"https://api.github.com/repos/{repo}/releases/{version}").body
             )
             version_installed = latest_release_metadata["tag_name"]
-            url = f"https://github.com/Pioreactor/pioreactorui/archive/refs/tags/{version_installed}.tar.gz"
+            url = f"https://github.com/{repo}/archive/refs/tags/{version_installed}.tar.gz"
             source = "/tmp/pioreactorui.tar.gz"
             commands.append(["wget", url, "-O", source])
 
         assert source is not None
         assert version_installed is not None
         commands.append(["bash", "/usr/local/bin/update_ui.sh", source, version_installed])
```

## pioreactor/cli/pios.py

```diff
@@ -17,14 +17,15 @@
 from pioreactor.utils.networking import add_local
 from pioreactor.utils.networking import cp_file_across_cluster
 from pioreactor.utils.timing import current_utc_timestamp
 from pioreactor.whoami import am_I_leader
 from pioreactor.whoami import get_latest_experiment_name
 from pioreactor.whoami import get_unit_name
 from pioreactor.whoami import is_testing_env
+from pioreactor.whoami import UNIVERSAL_EXPERIMENT
 from pioreactor.whoami import UNIVERSAL_IDENTIFIER
 
 
 @click.group()
 def pios() -> None:
     """
     Command each of the worker Pioreactors with the `pios` command.
@@ -34,15 +35,15 @@
     Report errors or feedback here: https://github.com/Pioreactor/pioreactor/issues
     """
     if not am_I_leader() and not is_testing_env():
         click.echo("workers cannot run `pios` commands. Try `pio` instead.", err=True)
         raise click.Abort()
 
     if len(get_active_workers_in_inventory()) == 0:
-        logger = create_logger("CLI", unit=get_unit_name(), experiment=get_latest_experiment_name())
+        logger = create_logger("CLI", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
         logger.warning("No active workers. See `cluster.inventory` section in config.ini.")
 
 
 if am_I_leader():
 
     def universal_identifier_to_all_active_workers(units: tuple[str, ...]) -> tuple[str, ...]:
         if units == (UNIVERSAL_IDENTIFIER,):
@@ -96,15 +97,15 @@
         2. config_{unit}.ini to the remote Pioreactor (if specific is True)
 
         Note: this function occurs in a thread
         """
 
         # move the global config.ini
         # there was a bug where if the leader == unit, the config.ini would get wiped
-        if (get_leader_hostname() != unit) and shared:
+        if shared and unit != get_leader_hostname():
             localpath = "/home/pioreactor/.pioreactor/config.ini"
             remotepath = "/home/pioreactor/.pioreactor/config.ini"
             cp_file_across_cluster(unit, localpath, remotepath)
 
         # move the specific unit config.ini
         if specific:
             try:
@@ -116,75 +117,135 @@
                 click.echo(
                     f"Did you forget to create a config_{unit}.ini to deploy to {unit}?",
                     err=True,
                 )
                 raise e
         return
 
-    @pios.command("cp", short_help="cp a file across clusters")
-    @click.argument("filepath", type=click.Path(exists=True))
+    @pios.command("cp", short_help="cp a file across the cluster")
+    @click.argument("filepath", type=click.Path(exists=True, resolve_path=True))
     @click.option(
         "--units",
         multiple=True,
         default=(UNIVERSAL_IDENTIFIER,),
         type=click.STRING,
-        help="specify a Pioreactor name, default is all active units",
+        help="specify a Pioreactor name, default is all active non-leader units",
     )
     def cp(
         filepath: str,
         units: tuple[str, ...],
     ) -> None:
-        logger = create_logger("cp", unit=get_unit_name(), experiment=get_latest_experiment_name())
+        logger = create_logger("cp", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
         units = remove_leader(universal_identifier_to_all_workers(units))
 
         def _thread_function(unit: str) -> bool:
-            logger.debug(f"Moving {filepath} to {unit}...")
+            logger.debug(f"Moving {filepath} to {unit}:{filepath}...")
             try:
                 cp_file_across_cluster(unit, filepath, filepath)
                 return True
             except Exception as e:
                 logger.error(f"Error occurred: {e}. See logs for more.")
                 logger.debug(f"Error occurred: {e}.", exc_info=True)
                 return False
 
         for unit in units:
             _thread_function(unit)
 
+    @pios.command("rm", short_help="rm a file across the cluster")
+    @click.argument("filepath", type=click.Path(exists=True, resolve_path=True))
+    @click.option(
+        "--units",
+        multiple=True,
+        default=(UNIVERSAL_IDENTIFIER,),
+        type=click.STRING,
+        help="specify a Pioreactor name, default is all active non-leader units",
+    )
+    @click.option("-y", is_flag=True, help="Skip asking for confirmation.")
+    def rm(
+        filepath: str,
+        units: tuple[str, ...],
+        y: bool,
+    ) -> None:
+        logger = create_logger("rm", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
+        units = remove_leader(universal_identifier_to_all_workers(units))
+
+        from sh import ssh  # type: ignore
+        from sh import ErrorReturnCode_255  # type: ignore
+        from sh import ErrorReturnCode_1
+        from shlex import join  # https://docs.python.org/3/library/shlex.html#shlex.quote
+
+        command = join(["rm", filepath])
+
+        if not y:
+            confirm = input(f"Confirm running `{command}` on {units}? Y/n: ").strip()
+            if confirm != "Y":
+                raise click.Abort()
+
+        def _thread_function(unit: str) -> bool:
+            logger.debug(f"Removing {unit}:{filepath}...")
+            try:
+                ssh(add_local(unit), command)
+                return True
+            except ErrorReturnCode_255 as e:
+                logger.error(f"Unable to connect to unit {unit}. {e.stderr.decode()}")
+                logger.debug(e, exc_info=True)
+                return False
+            except ErrorReturnCode_1 as e:
+                logger.error(f"Error occurred: {e}. See logs for more.")
+                logger.debug(e.stderr, exc_info=True)
+                return False
+
+        for unit in units:
+            _thread_function(unit)
+
     @pios.command("update", short_help="update PioreactorApp on workers")
     @click.option(
         "--units",
         multiple=True,
         default=(UNIVERSAL_IDENTIFIER,),
         type=click.STRING,
         help="specify a Pioreactor name, default is all active units",
     )
     @click.option("-b", "--branch", help="update to the github branch")
+    @click.option(
+        "-r",
+        "--repo",
+        help="install from a repo on github. Format: username/project",
+    )
     @click.option("-v", "--version", help="install a specific version, default is latest")
     @click.option("-y", is_flag=True, help="Skip asking for confirmation.")
     def update(
-        units: tuple[str, ...], branch: Optional[str], version: Optional[str], y: bool
+        units: tuple[str, ...],
+        branch: Optional[str],
+        repo: Optional[str],
+        version: Optional[str],
+        y: bool,
     ) -> None:
         """
-        Pulls and installs the latest code
+        Pulls and installs a Pioreactor software version across the cluster
         """
         from sh import ssh  # type: ignore
         from sh import ErrorReturnCode_255  # type: ignore
         from sh import ErrorReturnCode_1
+        from shlex import join
 
         # type: ignore
 
-        logger = create_logger(
-            "update", unit=get_unit_name(), experiment=get_latest_experiment_name()
-        )
+        logger = create_logger("update", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
         if version is not None:
-            command = f"pio update app -v {version}"
+            commands = ["pio", "update", "app", "-v", version]
         elif branch is not None:
-            command = f"pio update app -b {branch}"
+            commands = ["pio", "update", "app", "-b", branch]
         else:
-            command = "pio update app"
+            commands = ["pio", "update", "app"]
+
+        if repo is not None:
+            commands.extend(["-r", repo])
+
+        command = join(commands)
 
         units = universal_identifier_to_all_workers(units)
 
         if not y:
             confirm = input(f"Confirm running `{command}` on {units}? Y/n: ").strip()
             if confirm != "Y":
                 raise click.Abort()
@@ -223,15 +284,15 @@
         Installs a plugin to worker and leader
         """
         from sh import ssh  # type: ignore
         from sh import ErrorReturnCode_255  # type: ignore
         from sh import ErrorReturnCode_1  # type: ignore
 
         logger = create_logger(
-            "install_plugin", unit=get_unit_name(), experiment=get_latest_experiment_name()
+            "install_plugin", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT
         )
 
         command = f"pio install-plugin {plugin}"
 
         def _thread_function(unit: str):
             logger.debug(f"Executing `{command}` on {unit}...")
             try:
@@ -268,15 +329,15 @@
         """
 
         from sh import ssh  # type: ignore
         from sh import ErrorReturnCode_255  # type: ignore
         from sh import ErrorReturnCode_1  # type: ignore
 
         logger = create_logger(
-            "uninstall_plugin", unit=get_unit_name(), experiment=get_latest_experiment_name()
+            "uninstall_plugin", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT
         )
 
         command = f"pio uninstall-plugin {plugin}"
 
         def _thread_function(unit: str):
             logger.debug(f"Executing `{command}` on {unit}...")
             try:
@@ -324,15 +385,15 @@
     def sync_configs(units: tuple[str, ...], shared: bool, specific: bool, skip_save: bool) -> None:
         """
         Deploys the shared config.ini and worker specific config.inis to the workers.
 
         If neither `--shared` not `--specific` are specified, both are set to true.
         """
         logger = create_logger(
-            "sync_configs", unit=get_unit_name(), experiment=get_latest_experiment_name()
+            "sync_configs", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT
         )
         units = universal_identifier_to_all_workers(units)
 
         if not shared and not specific:
             shared = specific = True
 
         def _thread_function(unit: str) -> bool:
@@ -396,15 +457,15 @@
             ).strip()
             if confirm != "Y":
                 raise click.Abort()
 
         command = f"pio kill {' '.join(job)}"
         command += "--all-jobs" if all_jobs else ""
 
-        logger = create_logger("CLI", unit=get_unit_name(), experiment=get_latest_experiment_name())
+        logger = create_logger("CLI", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
 
         def _thread_function(unit: str):
             logger.debug(f"Executing `{command}` on {unit}.")
             try:
                 ssh(add_local(unit), command)
                 return True
 
@@ -482,24 +543,20 @@
 
         def _thread_function(unit: str) -> bool:
             click.echo(f"Executing `{core_command}` on {unit}.")
             try:
                 ssh(add_local(unit), command)
                 return True
             except ErrorReturnCode_255 as e:
-                logger = create_logger(
-                    "CLI", unit=get_unit_name(), experiment=get_latest_experiment_name()
-                )
+                logger = create_logger("CLI", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
                 logger.debug(e, exc_info=True)
                 logger.error(f"Unable to connect to unit {unit}. {e.stderr.decode()}")
                 return False
             except ErrorReturnCode_1 as e:
-                logger = create_logger(
-                    "CLI", unit=get_unit_name(), experiment=get_latest_experiment_name()
-                )
+                logger = create_logger("CLI", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
                 logger.error(f"Error occurred: {e}. See logs for more.")
                 logger.debug(e.stderr, exc_info=True)
                 return False
 
         with ThreadPoolExecutor(max_workers=len(units)) as executor:
             results = executor.map(_thread_function, units)
 
@@ -538,17 +595,15 @@
 
         def _thread_function(unit: str) -> bool:
             click.echo(f"Executing `{command}` on {unit}.")
             try:
                 ssh(add_local(unit), command)
                 return True
             except ErrorReturnCode_255 as e:
-                logger = create_logger(
-                    "CLI", unit=get_unit_name(), experiment=get_latest_experiment_name()
-                )
+                logger = create_logger("CLI", unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
                 logger.debug(e, exc_info=True)
                 logger.error(f"Unable to connect to unit {unit}. {e.stderr.decode()}")
                 return False
             except ErrorReturnCode_1 as e:
                 logger.error(f"Error occurred: {e}. See logs for more.")
                 logger.debug(e.stderr, exc_info=True)
                 return False
```

## pioreactor/experiment_profiles/profile_struct.py

```diff
@@ -10,15 +10,15 @@
 class Metadata(Struct):
     author: t.Optional[str] = None
     description: t.Optional[str] = None
 
 
 class Plugin(Struct):
     name: str
-    version: str
+    version: str  # can be a version, or version bound with version. Ex: "1.0.2", or ">=1.02", or "==1.0.2". See
 
 
 class Action(Struct, forbid_unknown_fields=True):
     type: t.Literal["start", "pause", "resume", "stop", "update"]
     hours_elapsed: float
     options: dict[str, t.Any] = {}
     args: list[str] = []
```

## pioreactor/plugin_management/__init__.py

```diff
@@ -36,14 +36,18 @@
 
      __plugin_name__
      __plugin_author__
      __plugin_summary__
      __plugin_version__
      __plugin_homepage__
 
+
+What's up with the underscore vs dashes discussion in the docs and throughout our software?
+https://chat.openai.com/share/fe432411-b1bb-47c3-be0b-8cfcc2588160
+
 """
 
 
 class Plugin(Struct):
     module: Any
     description: str
     version: str
@@ -63,15 +67,15 @@
     # Users can use Python's entry point system to create rich plugins, see
     # example here: https://github.com/Pioreactor/pioreactor-air-bubbler
 
     for plugin in discover_plugins_in_entry_points():
         try:
             md = entry_point.metadata(plugin.name)
             plugins[md["Name"]] = Plugin(
-                plugin.load(),
+                plugin.load(),  # plugin loading and execution here.
                 md["Summary"],
                 md["Version"],
                 md["Home-page"],
                 md["Author"],
                 "entry_points",
             )
         except Exception as e:
```

## pioreactor/plugin_management/uninstall_plugin.py

```diff
@@ -27,15 +27,15 @@
             "bash",
             "/usr/local/bin/uninstall_pioreactor_plugin.sh",
             quote(name_of_plugin),
         ],
         capture_output=True,
     )
     if "as it is not installed" in result.stderr.decode("utf-8"):
-        logger.warning(result.stderr)
+        logger.warning(f"Unable to uninstall: plugin {name_of_plugin} is not installed.")
     elif result.returncode == 0:
         logger.notice(f"Successfully uninstalled plugin {name_of_plugin}.")  # type: ignore
     else:
         logger.error(f"Failed to uninstall plugin {name_of_plugin}. See logs.")
         logger.debug(result.stdout)
         logger.debug(result.stderr)
```

## pioreactor/utils/__init__.py

```diff
@@ -232,15 +232,16 @@
 
 
     Notes
     -------
     Opening the same cache in a context manager is tricky, and should be avoided.
 
     """
-    # TMPDIR is in OSX and Pioreactor img (we provide it), TMP is windows
+    # gettempdir find the directory named by the TMPDIR environment variable.
+    # TMPDIR is set in the Pioreactor img.
     tmp_dir = tempfile.gettempdir()
     with Cache(f"{tmp_dir}/{cache_name}") as cache:
         yield cache  # type: ignore
 
 
 @contextmanager
 def local_persistant_storage(
```

## pioreactor/utils/streaming_calculations.py

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from json import dumps
 from threading import Timer
 from typing import Optional
 
-from pioreactor.pubsub import publish
+from pioreactor.pubsub import create_client
 
 
 class ExponentialMovingAverage:
     """
     Models the following:
 
-    y_n = (1 - ⍺)·x + ⍺·y_{n-1}
+    y_n = (1 - alpha)·x + alpha·y_{n-1}
 
-    If alpha = 0, use latest value only.
+    Ex: if alpha = 0, use latest value only.
     """
 
     def __init__(self, alpha: float):
         self.value: Optional[float] = None
         self.alpha = alpha
 
     def update(self, new_value: float) -> float:
@@ -372,72 +372,117 @@
             except np.linalg.LinAlgError:
                 return False
         else:
             return False
 
 
 class PID:
-    # used in dosing_control classes
-
     def __init__(
         self,
         Kp: float,
         Ki: float,
         Kd: float,
         setpoint: float,
-        K0: float = 0,
-        output_limits=(None, None),
+        output_limits: tuple[Optional[float], Optional[float]] = (None, None),
         sample_time: Optional[float] = None,
         unit: Optional[str] = None,
         experiment: Optional[str] = None,
         job_name: Optional[str] = None,
         target_name: Optional[str] = None,
-        **kwargs,
-    ):
-        from simple_pid import PID as simple_PID
-
-        self.K0 = K0
-        self.pid = simple_PID(
-            Kp,
-            Ki,
-            Kd,
-            setpoint=setpoint,
-            output_limits=output_limits,
-            sample_time=sample_time,
-            **kwargs,
-        )
+        derivative_smoothing=0.0,
+    ) -> None:
+        # PID coefficients
+        self.Kp = Kp
+        self.Ki = Ki
+        self.Kd = Kd
+        self.setpoint = setpoint
+
+        # The windup limit for integral term
+        self.output_limits = output_limits
+
+        # Smoothing factor for derivative term
+        assert 0.0 <= derivative_smoothing <= 1.0
+        self.derivative_smoothing = derivative_smoothing
+
+        # State variables
+        self.error_prev: Optional[float] = None
+        self._last_input: Optional[float] = None
+        self.error_sum = 0.0
+        self.derivative_prev = 0.0
+
         self.unit = unit
         self.experiment = experiment
         self.target_name = target_name
         self.job_name = job_name
+        self.client = create_client(
+            client_id=f"pid-{self.unit}-{self.experiment}-{self.target_name}"
+        )
+
+    def reset(self) -> None:
+        """
+        Resets the state variables.
+        """
+        self.error_prev = None
+        self.error_sum = 0.0
+        self.derivative_prev = 0.0
 
-    def set_setpoint(self, new_setpoint) -> None:
-        self.pid.setpoint = new_setpoint
+    def set_setpoint(self, new_setpoint: float) -> None:
+        self.setpoint = new_setpoint
+
+    def update(self, input_: float, dt: float = 1.0) -> float:
+        """
+        Updates the controller's internal state with the current error and time step,
+        and returns the controller output.
+        """
+
+        error = self.setpoint - input_
+        # Update error sum with clamping for anti-windup
+        self.error_sum += error * dt
+
+        if self.output_limits[0] is not None:
+            self.error_sum = max(self.error_sum, self.output_limits[0])
+        if self.output_limits[1] is not None:
+            self.error_sum = min(self.error_sum, self.output_limits[1])
+
+        # Calculate error derivative with smoothing
+        # derivative = ((error - self.error_prev) if self.error_prev is not None else 0) / dt
+        # http://brettbeauregard.com/blog/2011/04/improving-the-beginner%e2%80%99s-pid-derivative-kick/
+        derivative = -(input_ - self._last_input) / dt if self._last_input is not None else 0
+        derivative = (
+            1 - self.derivative_smoothing
+        ) * derivative + self.derivative_smoothing * self.derivative_prev
+
+        # Update state variables
+        self.error_prev = error
+        self.derivative_prev = derivative
+
+        # Calculate PID output
+        output = self.Kp * error + self.Ki * self.error_sum + self.Kd * derivative
+        if self.output_limits[0] is not None:
+            output = max(output, self.output_limits[0])
+        if self.output_limits[1] is not None:
+            output = min(output, self.output_limits[1])
+
+        self._last_input = input_
+        self._last_output = output
 
-    def update(self, input_: float, dt=None) -> float:
-        output = self.pid(input_, dt=dt)
-        if output is not None:
-            output += self.K0
-        else:
-            output = 0
         self.publish_pid_stats()
         return output
 
-    def publish_pid_stats(self):
+    def publish_pid_stats(self) -> None:
         # not currently being saved in database.
         to_send = {
-            "setpoint": self.pid.setpoint,
-            "output_limits_lb": self.pid.output_limits[0],
-            "output_limits_ub": self.pid.output_limits[1],
-            "Kd": self.pid.Kd,
-            "Ki": self.pid.Ki,
-            "Kp": self.pid.Kp,
-            "K0": self.K0,
-            "integral": self.pid._integral,
-            "proportional": self.pid._proportional,
-            "derivative": self.pid._derivative,
-            "latest_input": self.pid._last_input,
-            "latest_output": self.pid._last_output,
+            "setpoint": self.setpoint,
+            "output_limits_lb": self.output_limits[0],
+            "output_limits_ub": self.output_limits[1],
+            "Kd": self.Kd,
+            "Ki": self.Ki,
+            "Kp": self.Kp,
+            "integral": self.Ki * self.error_sum,
+            "proportional": self.Kp * (self.error_prev if self.error_prev is not None else 0),
+            "derivative": self.Kd * self.derivative_prev,
+            "latest_input": self._last_input,
+            "latest_output": self._last_output,
             "job_name": self.job_name,
             "target_name": self.target_name,
         }
-        publish(f"pioreactor/{self.unit}/{self.experiment}/pid_log", dumps(to_send))
+        self.client.publish(f"pioreactor/{self.unit}/{self.experiment}/pid_log", dumps(to_send))
```

## Comparing `pioreactor-23.6.7.dist-info/LICENSE` & `pioreactor-23.7.25rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pioreactor-23.6.7.dist-info/METADATA` & `pioreactor-23.7.25rc0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 Metadata-Version: 2.1
 Name: pioreactor
-Version: 23.6.7
+Version: 23.7.25rc0
 Summary: The core Python app of the Pioreactor. Control your bioreactor through Python.
 Home-page: https://github.com/pioreactor/pioreactor
 Author: Pioreactor
 Author-email: hello@pioreactor.com
 License: MIT
 Keywords: microbiology,bioreactor,turbidostat,raspberry pi,education,research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Hardware
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click (==8.1.3)
+Requires-Dist: click (==8.1.6)
 Requires-Dist: paho-mqtt (==1.6.1)
-Requires-Dist: psutil (==5.9.4)
+Requires-Dist: psutil (==5.9.5)
 Requires-Dist: sh (==1.14.3)
 Requires-Dist: JSON-log-formatter (==0.5.1)
 Requires-Dist: colorlog (==6.7.0)
-Requires-Dist: msgspec (==0.15.1)
-Requires-Dist: diskcache (==5.4.0)
+Requires-Dist: msgspec (==0.17.0)
+Requires-Dist: diskcache (==5.6.1)
 Requires-Dist: wheel (==0.38.4)
 Requires-Dist: crudini (==0.9.4)
 Provides-Extra: leader
-Requires-Dist: zeroconf (==0.47.1) ; extra == 'leader'
+Requires-Dist: zeroconf (==0.64.1) ; extra == 'leader'
 Requires-Dist: flask (==2.2.2) ; extra == 'leader'
 Requires-Dist: flup6 (==1.1.1) ; extra == 'leader'
 Requires-Dist: python-dotenv (==0.21.0) ; extra == 'leader'
-Requires-Dist: huey (==2.4.3) ; extra == 'leader'
+Requires-Dist: huey (==2.4.5) ; extra == 'leader'
 Provides-Extra: leader_worker
-Requires-Dist: zeroconf (==0.47.1) ; extra == 'leader_worker'
+Requires-Dist: zeroconf (==0.64.1) ; extra == 'leader_worker'
 Requires-Dist: flask (==2.2.2) ; extra == 'leader_worker'
 Requires-Dist: flup6 (==1.1.1) ; extra == 'leader_worker'
 Requires-Dist: python-dotenv (==0.21.0) ; extra == 'leader_worker'
-Requires-Dist: huey (==2.4.3) ; extra == 'leader_worker'
+Requires-Dist: huey (==2.4.5) ; extra == 'leader_worker'
 Requires-Dist: RPi.GPIO (==0.7.1) ; extra == 'leader_worker'
 Requires-Dist: adafruit-circuitpython-ads1x15 (==2.2.12) ; extra == 'leader_worker'
 Requires-Dist: DAC43608 (==0.2.7) ; extra == 'leader_worker'
 Requires-Dist: TMP1075 (==0.2.1) ; extra == 'leader_worker'
 Requires-Dist: rpi-hardware-pwm (==0.1.4) ; extra == 'leader_worker'
-Requires-Dist: simple-pid (==1.0.1) ; extra == 'leader_worker'
-Requires-Dist: plotext (>=5.2.8) ; extra == 'leader_worker'
+Requires-Dist: plotext (==5.2.8) ; extra == 'leader_worker'
 Provides-Extra: worker
 Requires-Dist: RPi.GPIO (==0.7.1) ; extra == 'worker'
 Requires-Dist: adafruit-circuitpython-ads1x15 (==2.2.12) ; extra == 'worker'
 Requires-Dist: DAC43608 (==0.2.7) ; extra == 'worker'
 Requires-Dist: TMP1075 (==0.2.1) ; extra == 'worker'
 Requires-Dist: rpi-hardware-pwm (==0.1.4) ; extra == 'worker'
-Requires-Dist: simple-pid (==1.0.1) ; extra == 'worker'
-Requires-Dist: plotext (>=5.2.8) ; extra == 'worker'
+Requires-Dist: plotext (==5.2.8) ; extra == 'worker'
 
 <img src="https://user-images.githubusercontent.com/884032/101398418-08e1c700-389c-11eb-8cf2-592c20383a19.png" width="250">
 <br />
 
 
 [![CI](https://github.com/Pioreactor/pioreactor/actions/workflows/ci.yaml/badge.svg)](https://github.com/Pioreactor/pioreactor/actions/workflows/ci.yaml)
```

## Comparing `pioreactor-23.6.7.dist-info/RECORD` & `pioreactor-23.7.25rc0.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 pioreactor/__init__.py,sha256=YBDDaFMxxsG_1Dg9ss9llZcW95gAh8WqpcdCjhF0T-E,117
-pioreactor/config.py,sha256=5tcwa3DNhZzT6i9amDKZYSsceuFxV06bXgAIJl8Zefo,6834
+pioreactor/config.py,sha256=xH-JXrT1Nmz9WFqG4dJfQS_Le2bhLZv89mBSYy4C2NQ,6887
 pioreactor/error_codes.py,sha256=XDfT3fPTVKN9wIGM9DdrXdvrEUn7lQkf6CJd8Xj_vFo,265
 pioreactor/exc.py,sha256=GvNp0vvgeAclxB2eIGZMnhYU3bFIYKz_AGOU9hKYstM,443
 pioreactor/hardware.py,sha256=c7IpkPCcsxtfvgUSpxv3TCltzCVSsIybDGzuWTn6N8g,3105
-pioreactor/logging.py,sha256=rVyqqxwv2voS-TMpTodnTHAI-QkhEp_I4bau9gHmMcU,6614
-pioreactor/mureq.py,sha256=XYpmNoMTqBIrtfZ_mKbfDEyLYRAeBBH29Zl5zy72iwA,14871
-pioreactor/pubsub.py,sha256=Twu4EJBTLwgObVog4ZGujbbgTGXx6TTG33EOSktFvnU,12957
-pioreactor/structs.py,sha256=eRLqrO6ldJftnXPzxzz8CoQHwnvK4W9RgniJfchUoeA,6400
+pioreactor/logging.py,sha256=uTX088TydO4UMDgBwBI8oVenr9t24xw4ju-ZR-Pnf6U,6618
+pioreactor/mureq.py,sha256=DpE7wqRwVe8FOz_mAcAAn9-GXCiRQ6VTSvcyUhF7pUU,15510
+pioreactor/pubsub.py,sha256=kFM6M3fmG1gG6hfNv8UB1LLcm9gJLzhLSM6hBHbL9NY,12950
+pioreactor/structs.py,sha256=ShLwXOezEK_dB7Hqim9jKob3dA86BYjs8kxePfypnZo,6391
 pioreactor/types.py,sha256=l5JwLlj9YFcq1RC-IrIPsBaGwwFuNs1GAputHLwl1aI,2724
-pioreactor/version.py,sha256=R9kZBsa0Nk01JR_pNbg2E9V_WY7_enuLmZByXiV806k,2152
-pioreactor/whoami.py,sha256=LnY7lP6oj89eiiR1CC1jCS9z3Ahbil2Qf7az1HRARYA,3654
+pioreactor/version.py,sha256=CBJIGjN6CHzGdXGZx2xOpgXcjL2-EikWBs5BlwW4T5M,2156
+pioreactor/whoami.py,sha256=XoXUci2kAxqNfPr8C9YaeaOQJvPkn_DP4c8HskGcKPg,4458
 pioreactor/actions/__init__.py,sha256=VuwIL8llFFqBspvBRgC9yNm-Blu9tsE2kwgIJEs786o,540
 pioreactor/actions/led_intensity.py,sha256=C705sRk7_rQsdlgmYC8YB_w3Iq30aSeJ_Bq2QHhGJAQ,8743
 pioreactor/actions/od_blank.py,sha256=-4k03BQC1i0T3rMQUicicKBufzYRC4QZD829P_XRu-Q,7755
-pioreactor/actions/od_calibration.py,sha256=YOXDPz-8gpxeq2dCv93TgF3i7UluhonRc-bCd5TPAUM,20343
+pioreactor/actions/od_calibration.py,sha256=WCXa3sLtI38CJHdO4y4xV-o5gQx56VwcAp8zF03mXE0,21010
 pioreactor/actions/pump.py,sha256=iVAVqzNSJKWfj1thiJMAV04SSSOV20k8bb7BA7dEOZo,17612
 pioreactor/actions/pump_calibration.py,sha256=SdnQ2AWbVNEdWtG00cxG_TtkYSNc_4RHDAxfH_cE0sM,21362
-pioreactor/actions/self_test.py,sha256=tZY_EwPjPBS9-Ed67SMQmB_Fqt-uWjnrm0aZxPIHG1c,16662
+pioreactor/actions/self_test.py,sha256=LeJTV_M2i0ZYzJiHaBCjB4I7GCvD3YgHkpe7bOtW2h8,17031
 pioreactor/actions/stirring_calibration.py,sha256=2uYypMe-8dTfwGBkSHBGSiqGpzQlt3wYRxJfa-1KRqw,5175
 pioreactor/actions/leader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pioreactor/actions/leader/backup_database.py,sha256=p34Cavwq7L9CN3ewoo3yUMMdm3wNiae0zKTbvtsRNZc,4744
-pioreactor/actions/leader/experiment_profile.py,sha256=j1QaD7x6Ot_N3kGLtVO40muWCHBfhevWdNlGqmY8HPc,7151
+pioreactor/actions/leader/backup_database.py,sha256=M84n8Mbtj9A_nGp6rLQqk92XLzXfkJpqsm0hUoVer8Y,4745
+pioreactor/actions/leader/experiment_profile.py,sha256=awPS-CgpcPfCRKaio0Zc81idctsNDnEasP9wTe8MpLI,8717
 pioreactor/actions/leader/export_experiment_data.py,sha256=L2lLsuj-VJ3jQJ79RfjAhu0AtlXUYF3Wff6kZPqdO1o,6426
 pioreactor/automations/__init__.py,sha256=4e_aOMdJCt9mzi9rwudECLnSCfYBoi8d3tojQVHtTV4,445
 pioreactor/automations/dosing/__init__.py,sha256=TTJ0pzbjyyLMuBC6b9ZVb820X8tmoZeHvGRI8rXr5SE,496
-pioreactor/automations/dosing/base.py,sha256=ueh2oTTVMVSDISmU96nc5ZaxJzcxFc6YRHDlvlpdKFM,28416
+pioreactor/automations/dosing/base.py,sha256=crUjY1aKoDl8yVypHjoOOTUrwNwMhS8tX3ValJB7ChM,28429
 pioreactor/automations/dosing/chemostat.py,sha256=Vs7nu3IVTUmq4XUOPvKi058Ho5gLUcyrcZNJQr6MBsc,1404
 pioreactor/automations/dosing/fed_batch.py,sha256=WURKm0iR_YbIII9CJsvzkcXjGGVw0D9t7ci_idIJxuo,1194
 pioreactor/automations/dosing/morbidostat.py,sha256=z3cjpKz4oww7E5sOnZN71uGRktMNAK6fLWC3FZ-YouM,2724
 pioreactor/automations/dosing/pid_morbidostat.py,sha256=P7SHRmecpLbZcSlONuz9qOjQkHdEueR_UV3fXa-QC5Q,4880
 pioreactor/automations/dosing/silent.py,sha256=qHF-c5Bu18eehkrdPAC8cMUPq5d2aQHKuZ-rkqWlJ-Q,468
 pioreactor/automations/dosing/turbidostat.py,sha256=6yQhp9-Rja9dx93bR_GODGhTuPT9kuLnCBIlvYT5TiA,2252
 pioreactor/automations/events/__init__.py,sha256=WxPoBeae7fD2SGOLEZ-rQf3IM83Je4SS4CztddADqlw,510
 pioreactor/automations/led/__init__.py,sha256=VnDl53GExO2Rj97MZbw4TSIuXPdklJ6biKck77boFt8,473
-pioreactor/automations/led/base.py,sha256=Bo0PMo86GZJePja1SRYQKEGmv57DNw_sRBOD80VvtU0,11851
-pioreactor/automations/led/light_dark_cycle.py,sha256=s1W5qRjK6I08Wo3MoCjLEzgX89Q1g2uiQ61c6kwAlfQ,3136
+pioreactor/automations/led/base.py,sha256=8kIv_z902yOqv7rDftBYDWS05YY3uhUKeavzy5jJeMg,11868
+pioreactor/automations/led/light_dark_cycle.py,sha256=GX50pON5HbZxIUxQMl_WfeYKV_ERtyiJjxQIgbfzNsE,3875
 pioreactor/automations/temperature/__init__.py,sha256=FSH6fKuQMpUqry6VEjPBLbwgXpgmGX5edBDsROtudlg,205
 pioreactor/automations/temperature/base.py,sha256=pFtC_0g1dirHaAGGBWORjwHDbBSNZf-rYYC6yzgftCg,9722
 pioreactor/automations/temperature/constant_duty_cycle.py,sha256=MIU3iCu_YDM0brb_5WncuN7Vv8fb5TC863YZfmbp57M,674
 pioreactor/automations/temperature/only_record_temperature.py,sha256=46p_EZs8AeM5hSQVJ8Tk_L-oQFucr32iAYSEq0GPbjg,517
-pioreactor/automations/temperature/thermostat.py,sha256=Sc8tNE3fiwfO2UhxrwHU7fnpMpGXPGDhZdPSAccLGDI,4314
+pioreactor/automations/temperature/thermostat.py,sha256=AQPb78V3eKnFAa9IYVtz9B1s2HC_k08OZVa7I8f_IhE,4086
 pioreactor/background_jobs/__init__.py,sha256=pn23vImMyfiHjbdKObOWpAwzNUbE1xnHWUYk4j4KSJM,715
-pioreactor/background_jobs/base.py,sha256=bDgxdKwDuZxf3L6DoZ6EC0BLKaMEU27zW6FkcKa7yQk,42618
-pioreactor/background_jobs/dosing_control.py,sha256=UJL5ngBzrNXb_B3tLJ4kpxSBL1PWEb_fL0qWdYgqMXA,6854
-pioreactor/background_jobs/growth_rate_calculating.py,sha256=96rGFwc9x7VGdWYlhyNMseNwPQQgBGXXeBzHhrcJHC0,20221
-pioreactor/background_jobs/led_control.py,sha256=prQEPE1xZbwadbKZtoBUzFvlmUjqcUGZ_4_DgGl63Us,5488
-pioreactor/background_jobs/monitor.py,sha256=uRiiNOW37stQefbZK7QyWpJxpOu5FMMMTP6kiMRbx3c,24314
-pioreactor/background_jobs/od_reading.py,sha256=jCH83AtT6F5Mdr6l5HF_rmGHvSgmpYfq6PEFmpreoGc,47033
-pioreactor/background_jobs/stirring.py,sha256=FE-b7Yblk0_FFczNnSKXu71S4-7oU6ciZDH1ppTYkt4,17577
-pioreactor/background_jobs/temperature_control.py,sha256=iYSkpei3fJLviFkBEzeBf2qRiKaIADwGGkPQWfcSewk,25723
+pioreactor/background_jobs/base.py,sha256=hiB6dluUbdGhM3tUASOgFYKJ72l3KaaGTvYDBa1xIV8,43584
+pioreactor/background_jobs/dosing_control.py,sha256=ach1rTYLOCcCZIXSl5FgNnxV3bPoAE-0tFbeywHvO4o,6851
+pioreactor/background_jobs/growth_rate_calculating.py,sha256=NlhJCh0iN-fQJuc4NLCUnLQHFhWf9UgHaol5Q08LWHM,20247
+pioreactor/background_jobs/led_control.py,sha256=MV_oIW6XdLSqQqju3VZqwZSV3UPWmDvNc2aQV9gi7dE,5485
+pioreactor/background_jobs/monitor.py,sha256=ERdRcZvT_VAw0vP2rgJK8Gn7YSfYLuomj8xziU1dAH0,25386
+pioreactor/background_jobs/od_reading.py,sha256=esFSNT5JDZB_6ZNSrQtc2JLJTeFnGNjBUdXPdd0_q40,48495
+pioreactor/background_jobs/stirring.py,sha256=sqknkGn_Xs6svtP-m4nLkvi9r0aCBJnQlYdnHHehW2E,17586
+pioreactor/background_jobs/temperature_control.py,sha256=AsF7k35s7lvv9VJSSmopD8_Pbciv-NQ_XxuBT8uxkMA,24346
 pioreactor/background_jobs/leader/__init__.py,sha256=Uhl2Xksfkf06lmfmz2scTxmBWDBnwkA9rSil_V94aWQ,605
-pioreactor/background_jobs/leader/mqtt_to_db_streaming.py,sha256=UM4_L-cesPGfj9wws-16GrmHEvTbBOhOmJAmxKGD7E0,16280
-pioreactor/background_jobs/leader/watchdog.py,sha256=ZJmDVqYFWrMis_riJcW6ui27s6EHZJIbdEMUoeAYXvQ,3829
+pioreactor/background_jobs/leader/mqtt_to_db_streaming.py,sha256=m8Y0dPuBdyuZrK1Wl97nF3Npflp3tlOvzk5uqQW-apY,16378
+pioreactor/background_jobs/leader/watchdog.py,sha256=fgZZt-RdJcpcIJem0-A14TYEy6N4oSjUdBy8hB60cUc,4187
 pioreactor/background_jobs/subjobs/__init__.py,sha256=pT1lJJp3c4rHSXCdBKc662uQR591Xhp16oeDpDMKEKc,609
 pioreactor/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pioreactor/cli/pio.py,sha256=6qs1WohIGqS2gD46ddNC7EvaPsMvsT9nQ2xkw5ioNmc,29779
-pioreactor/cli/pios.py,sha256=JroU6VqB20Dw97-1S-Rgg2UhlxkAWi1i7kQ3qR0M6II,22314
+pioreactor/cli/pio.py,sha256=pdGCdW1Oi-5nmjUTWD6EBFL3X9unwYkamV-4ZUPFHRU,30358
+pioreactor/cli/pios.py,sha256=ExMf3OjIL16s2WeQo6TAroQw65509h3mLb4pHrloFRw,24399
 pioreactor/experiment_profiles/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pioreactor/experiment_profiles/profile_struct.py,sha256=D_S8vRHjt_Us40FcQpuJunWdVmxD-6Q20Kvh89yrWW4,963
-pioreactor/plugin_management/__init__.py,sha256=MSu2s9kI7osSxBwKK1MQTcyw9sdabPvH2xCKnkNk16c,3517
+pioreactor/experiment_profiles/profile_struct.py,sha256=wZ8fwBtfiHVRRXZys2bJ6lrmtmof0sZlqDW3bOZGOzo,1059
+pioreactor/plugin_management/__init__.py,sha256=YJDimB7AqsoXTu0blGjM5FYL5TCl96p2wf26f58u_4s,3716
 pioreactor/plugin_management/install_plugin.py,sha256=i3KchEps5cafvuhADOLacaziL9UpuoDvMnvDVBaTCuw,1316
 pioreactor/plugin_management/list_plugins.py,sha256=blTAKhlsJJ4cwyR0_HWjC_fP0xcIUNFIJWY21moewaM,1086
-pioreactor/plugin_management/uninstall_plugin.py,sha256=iKWN51-5RoYrwTgmFLREVUT7kgs5pMFBt4Tfbt-HqPM,1605
+pioreactor/plugin_management/uninstall_plugin.py,sha256=Wg9DDwPsjWvmjC4z1EoBWdXuTGSkBI7nlpC9eVlWoN0,1657
 pioreactor/plugin_management/utils.py,sha256=s8HMBkul7vY5D82ZUNAc84GjxtdsbnycCSFD7n0ONfw,792
-pioreactor/utils/__init__.py,sha256=DHOfEEmPcOgGa2yJ1FIddNAIG8HWQRCYUoSlSTJTWfk,10951
+pioreactor/utils/__init__.py,sha256=fmu2aT7akMNwaFYX2Ppgiu3LJe7YpnXi1GGe2niIFXA,10998
 pioreactor/utils/adcs.py,sha256=f0NVEE1h1jBH0da1G3AXFCpBr1e_ZW5YltrXuC8Wobw,4096
 pioreactor/utils/dacs.py,sha256=gPAEjRseVA3-Ta5MTHpwi0HRdbWVd47pD21FcCaQwFY,1930
 pioreactor/utils/gpio_helpers.py,sha256=9lAKuEMuLIqXtTk6wRisKABo_Ab0n-zGcBjtN8gjX2I,976
 pioreactor/utils/math_helpers.py,sha256=chqxGPFRCc1Q-nIu-yw4I4mraAhYgYQatFNF6kXdbU8,2847
 pioreactor/utils/mock.py,sha256=V1_RqiD6gNctW-HxpCI0aDXepULIGWzD0tJUcfelONA,4122
 pioreactor/utils/networking.py,sha256=ePepmhpvP3uiVLhearQBeBe-csNjSqCzz81ylzDZ11g,3951
 pioreactor/utils/pwm.py,sha256=7KAdMF0w9YQbnI7swhZE_gfBLIkCOEYnQIrbHuoLxqo,7559
 pioreactor/utils/rpi_bad_power.py,sha256=CbtzIi9x8pvtVAX6aID8MG5YXNzkeIRFYfhri4qI-Xo,3393
 pioreactor/utils/sqlite_worker.py,sha256=69vb6s9bFdku7W7Akvb7dI0qYFW1ByhC_RECBRDwKPc,7749
-pioreactor/utils/streaming_calculations.py,sha256=7QLdhPKvOad18Z2rDgU5X8Eo_S1I2Kt7zqhuF1H8x5s,15186
+pioreactor/utils/streaming_calculations.py,sha256=QIkdiyysILvH4f6tHTzgLKbX4nkH6_oSLFLIH-zpR7k,17179
 pioreactor/utils/timing.py,sha256=Yc4pG9FB9Ix5fLT98LwuK6jQawzgMaM8AB09zPWKkTM,5614
-pioreactor-23.6.7.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
-pioreactor-23.6.7.dist-info/METADATA,sha256=AMEjzzsCiVkQPaNtwS4FGgGF3ORk9i9I48xSjwokSAQ,3893
-pioreactor-23.6.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioreactor-23.6.7.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
-pioreactor-23.6.7.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
-pioreactor-23.6.7.dist-info/RECORD,,
+pioreactor-23.7.25rc0.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
+pioreactor-23.7.25rc0.dist-info/METADATA,sha256=Y5JEaJ4xRmP4BHI-q2nbDncrpinfihpwoGPQmIkL6kU,3778
+pioreactor-23.7.25rc0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+pioreactor-23.7.25rc0.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
+pioreactor-23.7.25rc0.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
+pioreactor-23.7.25rc0.dist-info/RECORD,,
```

