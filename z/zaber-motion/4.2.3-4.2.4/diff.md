# Comparing `tmp/zaber_motion-4.2.3.tar.gz` & `tmp/zaber_motion-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-4.2.3.tar", last modified: Thu Jul 13 19:49:58 2023, max compression
+gzip compressed data, was "zaber_motion-4.2.4.tar", last modified: Tue Jul 25 16:25:56 2023, max compression
```

## Comparing `zaber_motion-4.2.3.tar` & `zaber_motion-4.2.4.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.776574 zaber_motion-4.2.3/
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-13 19:49:58.776638 zaber_motion-4.2.3/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-07-13 19:49:58.776887 zaber_motion-4.2.3/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.754929 zaber_motion-4.2.3/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.756739 zaber_motion-4.2.3/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.763767 zaber_motion-4.2.3/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     3136 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    41649 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    24816 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/io_port_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      268 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_data_source.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)    26067 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process.py
--rw-r--r--   0 zaber      (501) staff       (20)     3830 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     2074 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller_source.py
--rw-r--r--   0 zaber      (501) staff       (20)      281 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/process_controller_source_sensor.py
--rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      256 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      247 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/pvt_sequence.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    23693 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.765272 zaber_motion-4.2.3/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1940 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1535 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.774569 zaber_motion-4.2.3/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_pvt_point.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      396 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      326 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      285 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      341 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.775728 zaber_motion-4.2.3/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1937 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.775969 zaber_motion-4.2.3/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.776346 zaber_motion-4.2.3/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    67598 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   206262 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     9340 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-07-13 19:49:08.000000 zaber_motion-4.2.3/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-13 19:49:58.757292 zaber_motion-4.2.3/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     7890 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-13 19:49:58.000000 zaber_motion-4.2.3/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.625079 zaber_motion-4.2.4/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-25 16:25:56.625141 zaber_motion-4.2.4/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-07-25 16:25:56.625362 zaber_motion-4.2.4/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.604339 zaber_motion-4.2.4/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.606130 zaber_motion-4.2.4/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.613234 zaber_motion-4.2.4/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     3136 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    41649 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    34796 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    24816 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/io_port_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      268 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_data_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26067 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3830 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2074 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)      281 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller_source_sensor.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      256 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      247 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_sequence.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    23693 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.614672 zaber_motion-4.2.4/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1940 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19670 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1515 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4187 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2190 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.623111 zaber_motion-4.2.4/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      326 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      285 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.624249 zaber_motion-4.2.4/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1937 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.624473 zaber_motion-4.2.4/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7651 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.624843 zaber_motion-4.2.4/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    67796 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   206754 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     9340 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.606701 zaber_motion-4.2.4/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     7890 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-4.2.3/LICENSE.txt` & `zaber_motion-4.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/PKG-INFO` & `zaber_motion-4.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 4.2.3
+Version: 4.2.4
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.3/setup.py` & `zaber_motion-4.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='4.2.3',
+    version='4.2.4',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -32,12 +32,12 @@
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
     python_requires='>=3.8',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==4.2.3;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==4.2.3;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==4.2.3;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==4.2.4;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==4.2.4;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==4.2.4;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-4.2.3/test/test_integration.py` & `zaber_motion-4.2.4/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/__init__.py` & `zaber_motion-4.2.4/zaber_motion/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/__init__.py` & `zaber_motion-4.2.4/zaber_motion/ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/alert_event.py` & `zaber_motion-4.2.4/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/all_axes.py` & `zaber_motion-4.2.4/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/axis.py` & `zaber_motion-4.2.4/zaber_motion/ascii/axis.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/axis_identity.py` & `zaber_motion-4.2.4/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/axis_settings.py` & `zaber_motion-4.2.4/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/connection.py` & `zaber_motion-4.2.4/zaber_motion/ascii/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
-from typing import List, Any, Callable
+from typing import Generator, List, Any, Callable, Optional
 import asyncio
 from rx.subject import ReplaySubject
 from rx.core import Observable
 from rx import operators as rxop
 
 from ..call import call, call_async, call_sync
 from ..convert_exception import convert_exception
@@ -131,19 +131,19 @@
         request.baud_rate = baud_rate
         request.reject_routed_connection = direct
         response = main_pb2.OpenInterfaceResponse()
         call("interface/open", request, response)
         return Connection(response.interface_id)
 
     @staticmethod
-    async def open_serial_port_async(
+    def open_serial_port_async(
             port_name: str,
             baud_rate: int = DEFAULT_BAUD_RATE,
             direct: bool = False
-    ) -> 'Connection':
+    ) -> 'AsyncConnectionOpener':
         """
         Opens a serial port, if Zaber Launcher controls the port, the port will be opened through Zaber Launcher.
         Zaber Launcher allows sharing of the port between multiple applications,
         If port sharing is not desirable, use the `direct` parameter.
 
         Args:
             port_name: Name of the port to open.
@@ -155,31 +155,15 @@
             An object representing the port.
         """
         request = main_pb2.OpenInterfaceRequest()
         request.interface_type = main_pb2.SERIAL_PORT
         request.port_name = port_name
         request.baud_rate = baud_rate
         request.reject_routed_connection = direct
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("interface/open", request, response))
-
-        try:
-            await asyncio.shield(task)
-        except asyncio.CancelledError:
-            async def cancel() -> None:
-                try:
-                    await task
-                    await Connection(response.interface_id).close_async()
-                except MotionLibException:
-                    pass
-
-            asyncio.ensure_future(cancel())
-            raise
-
-        return Connection(response.interface_id)
+        return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_tcp(
             host_name: str,
             port: int = TCP_PORT_CHAIN
     ) -> 'Connection':
         """
@@ -197,49 +181,33 @@
         request.host_name = host_name
         request.port = port
         response = main_pb2.OpenInterfaceResponse()
         call("interface/open", request, response)
         return Connection(response.interface_id)
 
     @staticmethod
-    async def open_tcp_async(
+    def open_tcp_async(
             host_name: str,
             port: int = TCP_PORT_CHAIN
-    ) -> 'Connection':
+    ) -> 'AsyncConnectionOpener':
         """
         Opens a TCP connection.
 
         Args:
             host_name: Hostname or IP address.
             port: Optional port number (defaults to 55550).
 
         Returns:
             An object representing the connection.
         """
         request = main_pb2.OpenInterfaceRequest()
         request.interface_type = main_pb2.TCP
         request.host_name = host_name
         request.port = port
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("interface/open", request, response))
-
-        try:
-            await asyncio.shield(task)
-        except asyncio.CancelledError:
-            async def cancel() -> None:
-                try:
-                    await task
-                    await Connection(response.interface_id).close_async()
-                except MotionLibException:
-                    pass
-
-            asyncio.ensure_future(cancel())
-            raise
-
-        return Connection(response.interface_id)
+        return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_custom(
             transport: Transport
     ) -> 'Connection':
         """
         Opens a connection using a custom transport.
@@ -254,46 +222,30 @@
         request.interface_type = main_pb2.CUSTOM
         request.transport = transport.transport_id
         response = main_pb2.OpenInterfaceResponse()
         call("interface/open", request, response)
         return Connection(response.interface_id)
 
     @staticmethod
-    async def open_custom_async(
+    def open_custom_async(
             transport: Transport
-    ) -> 'Connection':
+    ) -> 'AsyncConnectionOpener':
         """
         Opens a connection using a custom transport.
 
         Args:
             transport: The custom connection transport.
 
         Returns:
             An object representing the connection.
         """
         request = main_pb2.OpenInterfaceRequest()
         request.interface_type = main_pb2.CUSTOM
         request.transport = transport.transport_id
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("interface/open", request, response))
-
-        try:
-            await asyncio.shield(task)
-        except asyncio.CancelledError:
-            async def cancel() -> None:
-                try:
-                    await task
-                    await Connection(response.interface_id).close_async()
-                except MotionLibException:
-                    pass
-
-            asyncio.ensure_future(cancel())
-            raise
-
-        return Connection(response.interface_id)
+        return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_iot(
             cloud_id: str,
             token: str = "unauthenticated",
             connection_name: str = "",
             realm: str = "",
@@ -324,21 +276,21 @@
         request.realm = realm
         request.api = api
         response = main_pb2.OpenInterfaceResponse()
         call("interface/open", request, response)
         return Connection(response.interface_id)
 
     @staticmethod
-    async def open_iot_async(
+    def open_iot_async(
             cloud_id: str,
             token: str = "unauthenticated",
             connection_name: str = "",
             realm: str = "",
             api: str = "https://api.zaber.io"
-    ) -> 'Connection':
+    ) -> 'AsyncConnectionOpener':
         """
         Opens a secured connection to a cloud connected device chain.
         Use this method to connect to devices on your account.
 
         Args:
             cloud_id: The cloud ID to connect to.
             token: The token to authenticate with. By default the connection will be unauthenticated.
@@ -355,31 +307,15 @@
         request = main_pb2.OpenInterfaceRequest()
         request.interface_type = main_pb2.IOT
         request.cloud_id = cloud_id
         request.token = token
         request.connection_name = connection_name
         request.realm = realm
         request.api = api
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("interface/open", request, response))
-
-        try:
-            await asyncio.shield(task)
-        except asyncio.CancelledError:
-            async def cancel() -> None:
-                try:
-                    await task
-                    await Connection(response.interface_id).close_async()
-                except MotionLibException:
-                    pass
-
-            asyncio.ensure_future(cancel())
-            raise
-
-        return Connection(response.interface_id)
+        return AsyncConnectionOpener(request)
 
     @staticmethod
     def open_network_share(
             host_name: str,
             port: int,
             connection_name: str = ""
     ) -> 'Connection':
@@ -403,19 +339,19 @@
         request.port = port
         request.connection_name = connection_name
         response = main_pb2.OpenInterfaceResponse()
         call("interface/open", request, response)
         return Connection(response.interface_id)
 
     @staticmethod
-    async def open_network_share_async(
+    def open_network_share_async(
             host_name: str,
             port: int,
             connection_name: str = ""
-    ) -> 'Connection':
+    ) -> 'AsyncConnectionOpener':
         """
         Opens a connection to Zaber Launcher in your Local Area Network.
         The connection is not secured.
 
         Args:
             host_name: Hostname or IP address.
             port: Port number.
@@ -427,31 +363,15 @@
             An object representing the connection.
         """
         request = main_pb2.OpenInterfaceRequest()
         request.interface_type = main_pb2.NETWORK_SHARE
         request.host_name = host_name
         request.port = port
         request.connection_name = connection_name
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("interface/open", request, response))
-
-        try:
-            await asyncio.shield(task)
-        except asyncio.CancelledError:
-            async def cancel() -> None:
-                try:
-                    await task
-                    await Connection(response.interface_id).close_async()
-                except MotionLibException:
-                    pass
-
-            asyncio.ensure_future(cancel())
-            raise
-
-        return Connection(response.interface_id)
+        return AsyncConnectionOpener(request)
 
     def generic_command(
             self,
             command: str,
             device: int = 0,
             axis: int = 0,
             check_errors: bool = True,
@@ -1010,7 +930,44 @@
         )
 
         events.pipe(
             rxop.filter(self.__filter_event('interface/disconnected')),
             rxop.take(1),
             rxop.map(lambda ev: convert_exception(ev[1].error_type, ev[1].error_message))
         ).subscribe(self._disconnected)
+
+
+class AsyncConnectionOpener:
+    '''Provides a connection in an asynchronous context using `await` or `async with`'''
+    def __init__(self, request: main_pb2.OpenInterfaceRequest) -> None:
+        self._request = request
+        self._resource: Optional[Connection] = None
+
+    async def _create_resource(self) -> Connection:
+        response = main_pb2.OpenInterfaceResponse()
+        task = asyncio.ensure_future(call_async("interface/open", self._request, response))
+
+        try:
+            await asyncio.shield(task)
+        except asyncio.CancelledError:
+            async def cancel() -> None:
+                try:
+                    await task
+                    await Connection(response.interface_id).close_async()
+                except MotionLibException:
+                    pass
+
+            asyncio.ensure_future(cancel())
+            raise
+
+        return Connection(response.interface_id)
+
+    def __await__(self) -> Generator[Any, None, 'Connection']:
+        return self._create_resource().__await__()
+
+    async def __aenter__(self) -> 'Connection':
+        self._resource = await self._create_resource()
+        return self._resource
+
+    async def __aexit__(self, exc_type: Any, exc: Any, trace: Any) -> None:
+        if self._resource is not None:
+            await self._resource.close_async()
```

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-4.2.4/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/device.py` & `zaber_motion-4.2.4/zaber_motion/ascii/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/device_identity.py` & `zaber_motion-4.2.4/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/device_io.py` & `zaber_motion-4.2.4/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/device_io_info.py` & `zaber_motion-4.2.4/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/device_settings.py` & `zaber_motion-4.2.4/zaber_motion/ascii/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/lockstep.py` & `zaber_motion-4.2.4/zaber_motion/ascii/lockstep.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-4.2.4/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/paramset_info.py` & `zaber_motion-4.2.4/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-4.2.4/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/process.py` & `zaber_motion-4.2.4/zaber_motion/ascii/process.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/process_controller.py` & `zaber_motion-4.2.4/zaber_motion/ascii/process_controller.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/process_controller_source.py` & `zaber_motion-4.2.4/zaber_motion/ascii/process_controller_source.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-4.2.4/zaber_motion/ascii/pvt_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-4.2.4/zaber_motion/ascii/pvt_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/pvt_sequence.py` & `zaber_motion-4.2.4/zaber_motion/ascii/pvt_sequence.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/response.py` & `zaber_motion-4.2.4/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-4.2.4/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-4.2.4/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/setting_constants.py` & `zaber_motion-4.2.4/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-4.2.4/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/storage.py` & `zaber_motion-4.2.4/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/stream.py` & `zaber_motion-4.2.4/zaber_motion/ascii/stream.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-4.2.4/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-4.2.4/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/transport.py` & `zaber_motion-4.2.4/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-4.2.4/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/warning_flags.py` & `zaber_motion-4.2.4/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/ascii/warnings.py` & `zaber_motion-4.2.4/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/__init__.py` & `zaber_motion-4.2.4/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/binary_settings.py` & `zaber_motion-4.2.4/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/command_code.py` & `zaber_motion-4.2.4/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/connection.py` & `zaber_motion-4.2.4/zaber_motion/binary/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 # pylint: disable=too-many-arguments
 
-from typing import List, Any, Callable
+from typing import Generator, List, Any, Callable, Optional
 import asyncio
 from rx.subject import ReplaySubject
 from rx.core import Observable
 from rx import operators as rxop
 
 from ..call import call, call_async, call_sync
 from ..convert_exception import convert_exception
@@ -88,19 +88,19 @@
         request.baud_rate = baud_rate
         request.use_message_ids = use_message_ids
         response = main_pb2.OpenInterfaceResponse()
         call("binary/interface/open", request, response)
         return Connection(response.interface_id)
 
     @staticmethod
-    async def open_serial_port_async(
+    def open_serial_port_async(
             port_name: str,
             baud_rate: int = DEFAULT_BAUD_RATE,
             use_message_ids: bool = False
-    ) -> 'Connection':
+    ) -> 'AsyncBinaryConnectionOpener':
         """
         Opens a serial port.
 
         Args:
             port_name: Name of the port to open.
             baud_rate: Optional baud rate (defaults to 9600).
             use_message_ids: Enable use of message IDs (defaults to disabled).
@@ -110,31 +110,15 @@
             An object representing the port.
         """
         request = main_pb2.OpenBinaryInterfaceRequest()
         request.interface_type = main_pb2.SERIAL_PORT
         request.port_name = port_name
         request.baud_rate = baud_rate
         request.use_message_ids = use_message_ids
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("binary/interface/open", request, response))
-
-        try:
-            await asyncio.shield(task)
-        except asyncio.CancelledError:
-            async def cancel() -> None:
-                try:
-                    await task
-                    await Connection(response.interface_id).close_async()
-                except MotionLibException:
-                    pass
-
-            asyncio.ensure_future(cancel())
-            raise
-
-        return Connection(response.interface_id)
+        return AsyncBinaryConnectionOpener(request)
 
     @staticmethod
     def open_tcp(
             host_name: str,
             port: int,
             use_message_ids: bool = False
     ) -> 'Connection':
@@ -156,19 +140,19 @@
         request.port = port
         request.use_message_ids = use_message_ids
         response = main_pb2.OpenInterfaceResponse()
         call("binary/interface/open", request, response)
         return Connection(response.interface_id)
 
     @staticmethod
-    async def open_tcp_async(
+    def open_tcp_async(
             host_name: str,
             port: int,
             use_message_ids: bool = False
-    ) -> 'Connection':
+    ) -> 'AsyncBinaryConnectionOpener':
         """
         Opens a TCP connection.
 
         Args:
             host_name: Hostname or IP address.
             port: Port number.
             use_message_ids: Enable use of message IDs (defaults to disabled).
@@ -178,31 +162,15 @@
             An object representing the connection.
         """
         request = main_pb2.OpenBinaryInterfaceRequest()
         request.interface_type = main_pb2.TCP
         request.host_name = host_name
         request.port = port
         request.use_message_ids = use_message_ids
-        response = main_pb2.OpenInterfaceResponse()
-        task = asyncio.ensure_future(call_async("binary/interface/open", request, response))
-
-        try:
-            await asyncio.shield(task)
-        except asyncio.CancelledError:
-            async def cancel() -> None:
-                try:
-                    await task
-                    await Connection(response.interface_id).close_async()
-                except MotionLibException:
-                    pass
-
-            asyncio.ensure_future(cancel())
-            raise
-
-        return Connection(response.interface_id)
+        return AsyncBinaryConnectionOpener(request)
 
     def close(
             self
     ) -> None:
         """
         Close the connection.
         """
@@ -531,7 +499,44 @@
         )
 
         events.pipe(
             rxop.filter(self.__filter_event('interface/disconnected')),
             rxop.take(1),
             rxop.map(lambda ev: convert_exception(ev[1].error_type, ev[1].error_message))
         ).subscribe(self._disconnected)
+
+
+class AsyncBinaryConnectionOpener:
+    '''Provides a connection in an asynchronous context using `await` or `async with`'''
+    def __init__(self, request: main_pb2.OpenBinaryInterfaceRequest) -> None:
+        self._request = request
+        self._resource: Optional[Connection] = None
+
+    async def _create_resource(self) -> Connection:
+        response = main_pb2.OpenInterfaceResponse()
+        task = asyncio.ensure_future(call_async("binary/interface/open", self._request, response))
+
+        try:
+            await asyncio.shield(task)
+        except asyncio.CancelledError:
+            async def cancel() -> None:
+                try:
+                    await task
+                    await Connection(response.interface_id).close_async()
+                except MotionLibException:
+                    pass
+
+            asyncio.ensure_future(cancel())
+            raise
+
+        return Connection(response.interface_id)
+
+    def __await__(self) -> Generator[Any, None, 'Connection']:
+        return self._create_resource().__await__()
+
+    async def __aenter__(self) -> 'Connection':
+        self._resource = await self._create_resource()
+        return self._resource
+
+    async def __aexit__(self, exc_type: Any, exc: Any, trace: Any) -> None:
+        if self._resource is not None:
+            await self._resource.close_async()
```

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/device.py` & `zaber_motion-4.2.4/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/device_identity.py` & `zaber_motion-4.2.4/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/device_settings.py` & `zaber_motion-4.2.4/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/error_code.py` & `zaber_motion-4.2.4/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/message.py` & `zaber_motion-4.2.4/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/reply_only_event.py` & `zaber_motion-4.2.4/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-4.2.4/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/bindings.py` & `zaber_motion-4.2.4/zaber_motion/bindings.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
     ext = ""
     if os_system == "linux":
         ext = ".so"
     if os_system == "darwin":
         ext = ".dylib"
 
-    lib_name = "zaber-motion-lib-{}-{}{}".format(os_system, arch, ext)
-    module_name = "zaber_motion_bindings_{}".format(os_system)
+    lib_name = f"zaber-motion-lib-{os_system}-{arch}{ext}"
+    module_name = f"zaber_motion_bindings_{os_system}"
     binding_module = importlib.import_module(module_name)
     if __version__ != binding_module.__version__:
         raise RuntimeError((
             f"The dependent module {module_name} is not compatible with "
             f"zaber_motion ({__version__} != {binding_module.__version__}). "
             f"Please install the correct version {module_name}=={__version__}."))
     return binding_module.load_library(lib_name)
```

### Comparing `zaber_motion-4.2.3/zaber_motion/call.py` & `zaber_motion-4.2.4/zaber_motion/call.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         resp_buffer = deserialize(response_data)
         promise.put(resp_buffer)
 
     cb = CALLBACK(callback)
     result = c_call(buffer, 0, cb, 1)
 
     if result != 0:
-        raise Exception("Invalid result code: {}".format(result))
+        raise RuntimeError(f"Invalid result code: {result}")
 
     response_buffers = promise.get()
 
     process_response(response_buffers, response_data)
 
 
 def set_result(future: 'asyncio.Future[List[bytes]]', resp_buffer: List[bytes]) -> None:
@@ -73,15 +73,15 @@
     cb = CallbackWrap(callback)
     with callbacks_lock:
         callbacks.add(cb)
 
     result = c_call(buffer, 0, cb.callback, 1)
 
     if result != 0:
-        raise Exception("Invalid result code: {}".format(result))
+        raise RuntimeError(f"Invalid result code: {result}")
 
     response_buffers = await future
 
     process_response(response_buffers, response_data)
 
 
 def call_sync(request: str, data: Optional[Message] = None, response_data: Optional[Message] = None) -> None:
@@ -92,15 +92,15 @@
     def callback(response_data: c_void_p, _tag: c_int64) -> None:
         resp_buffers[0] = deserialize(response_data)
 
     cb = CALLBACK(callback)
     result = c_call(buffer, 0, cb, 0)
 
     if result != 0:
-        raise Exception("Invalid result code: {}".format(result))
+        raise RuntimeError(f"Invalid result code: {result}")
 
     process_response(resp_buffers[0], response_data)
 
 
 def get_request_buffer(request: str, data: Optional[Message]) -> bytes:
     request_proto = main_pb2.Request()
     request_proto.request = request
@@ -120,12 +120,12 @@
     if response_proto.response != main_pb2.Response.OK:
         if len(response_buffers) > 1:
             raise convert_exception(response_proto.error_type, response_proto.error_message, response_buffers[1])
         raise convert_exception(response_proto.error_type, response_proto.error_message)
 
     if len(response_buffers) > 1:
         if response_data is None:
-            raise Exception("Response from library is ignored, response_data==None")
+            raise RuntimeError("Response from library is ignored, response_data==None")
         response_data.ParseFromString(response_buffers[1])
     else:
         if response_data is not None:
-            raise Exception("No response from library")
+            raise RuntimeError("No response from library")
```

### Comparing `zaber_motion-4.2.3/zaber_motion/convert_exception.py` & `zaber_motion-4.2.4/zaber_motion/convert_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/events.py` & `zaber_motion-4.2.4/zaber_motion/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,21 +54,21 @@
 
 def process_event(event_buffers: List[bytes]) -> None:
     event = main_pb2.Event()
     event.ParseFromString(event_buffers[0])
 
     EventData = parsers.get(event.event, False)
     if EventData is False:
-        raise Exception("Unknown event: {}".format(event.event))
+        raise RuntimeError(f"Unknown event: {event.event}")
 
     has_parser = EventData is not None
     has_data = len(event_buffers) > 1
 
     if has_data != has_parser:
-        raise Exception("Event has no data or parser not provided for {}".format(event.event))
+        raise RuntimeError(f"Event has no data or parser not provided for {event.event}")
 
     event_data = None
     if has_data:
         event_data = EventData()  # type: ignore
         event_data.ParseFromString(event_buffers[1])
 
     event_tuple = (event.event, event_data)
```

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/__init__.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_pvt_point.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_pvt_point.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/firmware_version.py` & `zaber_motion-4.2.4/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/__init__.py` & `zaber_motion-4.2.4/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/axis_definition.py` & `zaber_motion-4.2.4/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-4.2.4/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-4.2.4/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/device_definition.py` & `zaber_motion-4.2.4/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/offline_translator.py` & `zaber_motion-4.2.4/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/translate_message.py` & `zaber_motion-4.2.4/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/translate_result.py` & `zaber_motion-4.2.4/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/translator.py` & `zaber_motion-4.2.4/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/gcode/translator_config.py` & `zaber_motion-4.2.4/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/library.py` & `zaber_motion-4.2.4/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/measurement.py` & `zaber_motion-4.2.4/zaber_motion/measurement.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-4.2.4/zaber_motion/microscopy/objective_changer.py`

 * *Files 10% similar despite different names*

```diff
@@ -166,7 +166,43 @@
         Moves the focus stage out of the turret releasing the current objective.
         """
         request = main_pb2.ObjectiveChangerRequest()
         request.interface_id = self.connection.interface_id
         request.turret_address = self.turret_address
         request.focus_address = self.focus_address
         await call_async("objective_changer/release", request)
+
+    def get_current_objective(
+            self
+    ) -> int:
+        """
+        Returns current objective number starting from 1.
+        The value of 0 indicates that the position is either unknown or between two objectives.
+
+        Returns:
+            Current objective number starting from 1 or 0 if not applicable.
+        """
+        request = main_pb2.ObjectiveChangerRequest()
+        request.interface_id = self.connection.interface_id
+        request.turret_address = self.turret_address
+        request.focus_address = self.focus_address
+        response = main_pb2.ObjectiveChangerGetCurrentResponse()
+        call("objective_changer/get_current_objective", request, response)
+        return response.value
+
+    async def get_current_objective_async(
+            self
+    ) -> int:
+        """
+        Returns current objective number starting from 1.
+        The value of 0 indicates that the position is either unknown or between two objectives.
+
+        Returns:
+            Current objective number starting from 1 or 0 if not applicable.
+        """
+        request = main_pb2.ObjectiveChangerRequest()
+        request.interface_id = self.connection.interface_id
+        request.turret_address = self.turret_address
+        request.focus_address = self.focus_address
+        response = main_pb2.ObjectiveChangerGetCurrentResponse()
+        await call_async("objective_changer/get_current_objective", request, response)
+        return response.value
```

### Comparing `zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"\xba\x01\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\x12\x44\n\x04type\x18\x03 \x01(\x0e\x32\x36.zaber.motion.protobufs.DeviceDetectRequest.DeviceType\"-\n\nDeviceType\x12\x07\n\x03\x41NY\x10\x00\x12\x16\n\x12PROCESS_CONTROLLER\x10\x01\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xf5\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\x12\x35\n\x08\x65ndpoint\x18\x0c \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"]\n\tProcessOn\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\n\n\x02on\x18\x04 \x01(\x08\x12\x10\n\x08\x64uration\x18\x05 \x01(\x01\"7\n\x17ProcessControllerSource\x12\x0e\n\x06sensor\x18\x01 \x01(\x05\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x91\x01\n\x1aSetProcessControllerSource\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12?\n\x06source\x18\x04 \x01(\x0b\x32/.zaber.motion.protobufs.ProcessControllerSource*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"\xba\x01\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\x12\x44\n\x04type\x18\x03 \x01(\x0e\x32\x36.zaber.motion.protobufs.DeviceDetectRequest.DeviceType\"-\n\nDeviceType\x12\x07\n\x03\x41NY\x10\x00\x12\x16\n\x12PROCESS_CONTROLLER\x10\x01\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xf5\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\x12\x35\n\x08\x65ndpoint\x18\x0c \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"3\n\"ObjectiveChangerGetCurrentResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"]\n\tProcessOn\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\n\n\x02on\x18\x04 \x01(\x08\x12\x10\n\x08\x64uration\x18\x05 \x01(\x01\"7\n\x17ProcessControllerSource\x12\x0e\n\x06sensor\x18\x01 \x01(\x05\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x91\x01\n\x1aSetProcessControllerSource\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12?\n\x06source\x18\x04 \x01(\x0b\x32/.zaber.motion.protobufs.ProcessControllerSource*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protobufs.main_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\"./protobufs;zaber_motion_protobufs'
-  _MESSAGETYPE._serialized_start=22808
-  _MESSAGETYPE._serialized_end=22853
-  _ERRORS._serialized_start=22856
-  _ERRORS._serialized_end=24072
-  _INTERFACETYPE._serialized_start=24074
-  _INTERFACETYPE._serialized_end=24155
+  _MESSAGETYPE._serialized_start=22861
+  _MESSAGETYPE._serialized_end=22906
+  _ERRORS._serialized_start=22909
+  _ERRORS._serialized_end=24125
+  _INTERFACETYPE._serialized_start=24127
+  _INTERFACETYPE._serialized_end=24208
   _REQUEST._serialized_start=48
   _REQUEST._serialized_end=74
   _RESPONSE._serialized_start=77
   _RESPONSE._serialized_end=262
   _RESPONSE_RESPONSETYPE._serialized_start=229
   _RESPONSE_RESPONSETYPE._serialized_end=262
   _EVENT._serialized_start=264
@@ -451,14 +451,16 @@
   _CONVERSIONFACTOR._serialized_end=22164
   _OBJECTIVECHANGERREQUEST._serialized_start=22166
   _OBJECTIVECHANGERREQUEST._serialized_end=22260
   _OBJECTIVECHANGERCREATERESPONSE._serialized_start=22262
   _OBJECTIVECHANGERCREATERESPONSE._serialized_end=22325
   _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=22328
   _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22506
-  _PROCESSON._serialized_start=22508
-  _PROCESSON._serialized_end=22601
-  _PROCESSCONTROLLERSOURCE._serialized_start=22603
-  _PROCESSCONTROLLERSOURCE._serialized_end=22658
-  _SETPROCESSCONTROLLERSOURCE._serialized_start=22661
-  _SETPROCESSCONTROLLERSOURCE._serialized_end=22806
+  _OBJECTIVECHANGERGETCURRENTRESPONSE._serialized_start=22508
+  _OBJECTIVECHANGERGETCURRENTRESPONSE._serialized_end=22559
+  _PROCESSON._serialized_start=22561
+  _PROCESSON._serialized_end=22654
+  _PROCESSCONTROLLERSOURCE._serialized_start=22656
+  _PROCESSCONTROLLERSOURCE._serialized_end=22711
+  _SETPROCESSCONTROLLERSOURCE._serialized_start=22714
+  _SETPROCESSCONTROLLERSOURCE._serialized_end=22859
 # @@protoc_insertion_point(module_scope)
```

### Comparing `zaber_motion-4.2.3/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -5415,14 +5415,29 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["focus_offset", b"focus_offset"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["focus_address", b"focus_address", "focus_offset", b"focus_offset", "interface_id", b"interface_id", "objective", b"objective", "turret_address", b"turret_address"]) -> None: ...
 
 global___ObjectiveChangerChangeRequest = ObjectiveChangerChangeRequest
 
 @typing_extensions.final
+class ObjectiveChangerGetCurrentResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    VALUE_FIELD_NUMBER: builtins.int
+    value: builtins.int
+    def __init__(
+        self,
+        *,
+        value: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+
+global___ObjectiveChangerGetCurrentResponse = ObjectiveChangerGetCurrentResponse
+
+@typing_extensions.final
 class ProcessOn(google.protobuf.message.Message):
     """Process Controller
 
     process-controller/enable
     process-controller/on
     process_controller/bridge
     """
```

### Comparing `zaber_motion-4.2.3/zaber_motion/serialization.py` & `zaber_motion-4.2.4/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/tools.py` & `zaber_motion-4.2.4/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion/units.py` & `zaber_motion-4.2.4/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.3/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-4.2.4/zaber_motion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber-motion
-Version: 4.2.3
+Version: 4.2.4
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.3/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-4.2.4/zaber_motion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

