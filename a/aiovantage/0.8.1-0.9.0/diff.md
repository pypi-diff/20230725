# Comparing `tmp/aiovantage-0.8.1.tar.gz` & `tmp/aiovantage-0.9.0.tar.gz`

## Comparing `aiovantage-0.8.1.tar` & `aiovantage-0.9.0.tar`

### file list

```diff
@@ -1,164 +1,171 @@
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.pylintrc
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 aiovantage-0.8.1/TODO
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.vscode/settings.json
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/dump_system.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/monitor_all.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/anemo_sensors/dump_anemo_sensors.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/anemo_sensors/monitor_anemo_sensors.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/light_sensors/dump_light_sensors.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/light_sensors/monitor_light_sensors.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/load_groups/monitor_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/control_load.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/masters/dump_masters.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/masters/monitor_masters.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/stations/jingle_bells.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/tasks/run_task.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/temperature_sensors/dump_temperature_sensors.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 aiovantage-0.8.1/examples/temperature_sensors/monitor_temperature_sensors.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/connection.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/discovery.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/errors.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/events.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/query.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/commands.py
--rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/anemo_sensor.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/light_sensor.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sounder.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/command_client/interfaces/temperature.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/requests.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/close_filter.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_object.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/introspection/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/login/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/interfaces/login/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/area.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind_base.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind_group.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/blind_group_base.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/button.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/child_device.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/child_object.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/custom_device.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dc_power_profile.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dimmer.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/eq_ux.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/gmem.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/keypad.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/light_sensor.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/load.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/load_group.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/location_object.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/master.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/module.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/module_gen2.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/omni_sensor.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/pwm_power_profile.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/qis_blind.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/qube_blind.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/relay_blind.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/rgb_load_base.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/scene_point_relay.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/sensor.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_rs_485_group_child.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_rs_485_shade_child.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_urtsi_2_group_child.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/somfy_urtsi_2_shade_child.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/station_bus.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/station_object.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/system_object.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/task.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/temperature.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/vantage_ddg_color_load.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/vantage_dg_color_load.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/config_client/models/vantage_dmx_dali_gateway.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/anemo_sensors.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/light_sensors.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/modules.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aiovantage-0.8.1/src/aiovantage/controllers/temperature_sensors.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.8.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.8.1/LICENSE
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 aiovantage-0.8.1/README.md
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 aiovantage-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 aiovantage-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.pylintrc
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aiovantage-0.9.0/TODO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/dump_system.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/load_groups/monitor_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/masters/dump_masters.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/masters/monitor_masters.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/port_devices/dump_port_devices.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 aiovantage-0.9.0/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     9535 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/connection.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/discovery.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/events.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/requests.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/close_filter.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/get_object.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/introspection/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/login/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/interfaces/login/login.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/area.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/blind.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/blind_base.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/blind_group.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/blind_group_base.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/button.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/child_device.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/child_object.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/custom_device.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/dc_power_profile.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/dimmer.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/eq_ux.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/gmem.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/keypad.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/light_sensor.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/load.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/load_group.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/location_object.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/master.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/module.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/module_gen2.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/omni_sensor.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/parent_device.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/port_device.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/pwm_power_profile.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/qis_blind.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/qube_blind.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/relay_blind.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/rgb_load_base.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/sensor.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/somfy_rs_485_group_child.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/somfy_rs_485_sdn_20_port.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/somfy_rs_485_shade_child.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/somfy_urtsi_2_group_child.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/somfy_urtsi_2_port.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/somfy_urtsi_2_shade_child.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/station_bus.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/station_object.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/system_object.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/task.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/temperature.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/vantage_ddg_color_load.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/vantage_dg_color_load.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/vantage_dmx_dali_gateway.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/config_client/models/vantage_dmx_gateway.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/modules.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/port_devices.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aiovantage-0.9.0/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 aiovantage-0.9.0/README.md
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 aiovantage-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 aiovantage-0.9.0/PKG-INFO
```

### Comparing `aiovantage-0.8.1/.pre-commit-config.yaml` & `aiovantage-0.9.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.277
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.4.1"
     hooks:
       - id: mypy
         additional_dependencies:
-          - xsdata==23.6
+          - xsdata==23.7
         args: []
 
   - repo: https://github.com/thlorenz/doctoc
     rev: v2.2.0
     hooks:
       - id: doctoc
         args: ["--github", "--notitle", "--maxlevel=2", "--update-only"]
```

### Comparing `aiovantage-0.8.1/CONTRIBUTING.md` & `aiovantage-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/TODO` & `aiovantage-0.9.0/TODO`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 - Cleanup "ELAGG", etc subscriptions on shutdown to avoid memory leaks on the controller
 - Consider grouped controllers like aiohue, eg. for sensors, loads, etc.
 - Consider renaming GMemController to VariablesController, MastersController to ControllersController
 - Sphinx docs / readthedocs
 - Smarter fetching of objects?
   - Eg. combine multiple requests into one
   - Eg. If we request 50 and get < 50 don't make another request
-- Expose PortDevice objects via a PortDeviceController
 - Pure object interfaces
   - Rename command_client.interfaces to command_client.object_interfaces
   - Remove non object interface methods ("LOAD", "S:LOAD" parsing, etc)
   - Consider better typing approach
     - Calls:
       - `INVOKE id Interface.Method arg1 ... argN -> R:INVOKE id rcode Interface.Method arg1 ... argN`
       - Args are mutable to support multiple return values
```

### Comparing `aiovantage-0.8.1/.github/ISSUE_TEMPLATE/bug.yml` & `aiovantage-0.9.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiovantage-0.9.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/dump_system.py` & `aiovantage-0.9.0/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/monitor_all.py` & `aiovantage-0.9.0/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/anemo_sensors/dump_anemo_sensors.py` & `aiovantage-0.9.0/examples/anemo_sensors/dump_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/anemo_sensors/monitor_anemo_sensors.py` & `aiovantage-0.9.0/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/areas/dump_areas.py` & `aiovantage-0.9.0/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.9.0/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/blinds/dump_blinds.py` & `aiovantage-0.9.0/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/blinds/monitor_blinds.py` & `aiovantage-0.9.0/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/buttons/dump_buttons.py` & `aiovantage-0.9.0/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/buttons/monitor_buttons.py` & `aiovantage-0.9.0/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/command_client/event_log.py` & `aiovantage-0.9.0/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/command_client/status_load.py` & `aiovantage-0.9.0/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/config_client/dump_objects.py` & `aiovantage-0.9.0/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/config_client/get_version.py` & `aiovantage-0.9.0/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.9.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.9.0/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/gmem/dump_gmem.py` & `aiovantage-0.9.0/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/gmem/monitor_gmem.py` & `aiovantage-0.9.0/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/gmem/set_gmem.py` & `aiovantage-0.9.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/light_sensors/dump_light_sensors.py` & `aiovantage-0.9.0/examples/light_sensors/dump_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/light_sensors/monitor_light_sensors.py` & `aiovantage-0.9.0/examples/light_sensors/monitor_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/load_groups/dump_load_groups.py` & `aiovantage-0.9.0/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/load_groups/monitor_load_groups.py` & `aiovantage-0.9.0/examples/load_groups/monitor_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/loads/control_load.py` & `aiovantage-0.9.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/loads/dump_loads.py` & `aiovantage-0.9.0/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/loads/monitor_loads.py` & `aiovantage-0.9.0/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/loads/poll_on_loads.py` & `aiovantage-0.9.0/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/loads/toggle_load.py` & `aiovantage-0.9.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/masters/dump_masters.py` & `aiovantage-0.9.0/examples/masters/dump_masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/masters/monitor_masters.py` & `aiovantage-0.9.0/examples/masters/monitor_masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.9.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.9.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.9.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.9.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/stations/dump_stations.py` & `aiovantage-0.9.0/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/stations/jingle_bells.py` & `aiovantage-0.9.0/examples/stations/jingle_bells.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/tasks/dump_tasks.py` & `aiovantage-0.9.0/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/tasks/run_task.py` & `aiovantage-0.9.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/temperature_sensors/dump_temperature_sensors.py` & `aiovantage-0.9.0/examples/temperature_sensors/dump_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/examples/temperature_sensors/monitor_temperature_sensors.py` & `aiovantage-0.9.0/examples/temperature_sensors/monitor_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/__init__.py` & `aiovantage-0.9.0/src/aiovantage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     GMemController,
     LightSensorsController,
     LoadGroupsController,
     LoadsController,
     MastersController,
     ModulesController,
     OmniSensorsController,
+    PortDevicesController,
     RGBLoadsController,
     StationsController,
     TasksController,
     TemperatureSensorsController,
 )
 from .events import EventCallback, VantageEvent
 from .models import SystemObject
@@ -85,14 +86,15 @@
         self._light_sensors = self._add_controller(LightSensorsController)
         self._load_groups = self._add_controller(LoadGroupsController)
         self._loads = self._add_controller(LoadsController)
         self._masters = self._add_controller(MastersController)
         self._modules = self._add_controller(ModulesController)
         self._rgb_loads = self._add_controller(RGBLoadsController)
         self._omni_sensors = self._add_controller(OmniSensorsController)
+        self._port_devices = self._add_controller(PortDevicesController)
         self._stations = self._add_controller(StationsController)
         self._tasks = self._add_controller(TasksController)
         self._temperature_sensors = self._add_controller(TemperatureSensorsController)
 
     async def __aenter__(self) -> Self:
         """Return context manager."""
         return self
@@ -190,14 +192,19 @@
 
     @property
     def omni_sensors(self) -> OmniSensorsController:
         """Return the OmniSensors controller for managing omni sensors."""
         return self._omni_sensors
 
     @property
+    def port_devices(self) -> PortDevicesController:
+        """Return the PortDevices controller for managing port devices."""
+        return self._port_devices
+
+    @property
     def rgb_loads(self) -> RGBLoadsController:
         """Return the RGBLoads controller for managing RGB loads."""
         return self._rgb_loads
 
     @property
     def stations(self) -> StationsController:
         """Return the Stations controller for managing stations (keypads, etc)."""
```

### Comparing `aiovantage-0.8.1/src/aiovantage/connection.py` & `aiovantage-0.9.0/src/aiovantage/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/discovery.py` & `aiovantage-0.9.0/src/aiovantage/discovery.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/errors.py` & `aiovantage-0.9.0/src/aiovantage/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/query.py` & `aiovantage-0.9.0/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/README.md` & `aiovantage-0.9.0/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/__init__.py` & `aiovantage-0.9.0/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/commands.py` & `aiovantage-0.9.0/src/aiovantage/command_client/commands.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/events.py` & `aiovantage-0.9.0/src/aiovantage/command_client/events.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/utils.py` & `aiovantage-0.9.0/src/aiovantage/command_client/utils.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/anemo_sensor.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/anemo_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/light_sensor.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/light_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Interface for querying and controlling loads."""
 
 from enum import IntEnum
-from typing import Sequence
+from typing import Optional, Sequence
 
 from .base import Interface
 
 
 class LoadInterface(Interface):
     """Interface for querying and controlling loads."""
 
@@ -17,39 +17,45 @@
         DOWN = 4
         UP = 5
         FIXED = 6
         VARIABLE = 7
         ADJUST = 8
 
     async def turn_on(
-        self, vid: int, transition: float = 0, level: float = 100
+        self,
+        vid: int,
+        transition: Optional[float] = None,
+        level: Optional[float] = None,
     ) -> None:
         """Turn on a load.
 
         Args:
             vid: The Vantage ID of the load.
-            transition: The time in seconds to transition to the new level.
-            level: The level to set the load to (0-100).
+            transition: The time in seconds to transition to the new level, defaults to immediate.
+            level: The level to set the load to (0-100), defaults to 100.
         """
-        if transition:
-            await self.ramp(vid, level, transition)
-        else:
-            await self.set_level(vid, level)
+        if level is None:
+            level = 100
 
-    async def turn_off(self, vid: int, transition: float = 0) -> None:
+        if transition is None:
+            return await self.set_level(vid, level)
+
+        await self.ramp(vid, level, transition)
+
+    async def turn_off(self, vid: int, transition: Optional[float] = None) -> None:
         """Turn off a load.
 
         Args:
             vid: The Vantage ID of the load.
             transition: The time in seconds to ramp the load down.
         """
-        if transition:
-            await self.ramp(vid, 0, transition)
-        else:
-            await self.set_level(vid, 0)
+        if transition is None:
+            return await self.set_level(vid, 0)
+
+        await self.ramp(vid, 0, transition)
 
     async def get_level(self, vid: int) -> float:
         """Get the level of a load.
 
         Args:
             vid: The Vantage ID of the load.
```

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/sounder.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/sounder.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         # -> R:INVOKE <id> <running (0/1)> Task.IsRunning
         response = await self.invoke(vid, "Task.IsRunning")
         is_running = bool(int(response.args[1]))
 
         return is_running
 
     async def get_state(self, vid: int) -> bool:
-        """Get the state of a task.
+        """Get the LED state of a task.
 
         Args:
             vid: The Vantage ID of the task.
         """
         # INVOKE <id> Task.GetState
         # -> R:INVOKE <id> <state (0/1)> Task.GetState
         response = await self.invoke(vid, "Task.GetState")
@@ -51,42 +51,42 @@
             vid: The Vantage ID of the task.
         """
         # INVOKE <id> Task.Stop
         # -> R:INVOKE <id> <rcode> Task.Stop
         await self.invoke(vid, "Task.Stop")
 
     @classmethod
-    def parse_task_status(cls, args: Sequence[str]) -> bool:
+    def parse_task_status(cls, args: Sequence[str]) -> int:
         """Parse a simple 'S:TASK' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
-            The state of the task.
+            The LED state of the task.
         """
         # STATUS TASK
         # -> S:TASK <id> <state (0/1)>
-        return bool(int(args[0]))
+        return int(args[0])
 
     @classmethod
-    def parse_get_state_status(cls, args: Sequence[str]) -> bool:
+    def parse_get_state_status(cls, args: Sequence[str]) -> int:
         """Parse a 'Task.GetState' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
-            The state of the task.
+            The LED state of the task.
         """
         # ELLOG STATUS ON
         # -> EL: <id> Task.GetState <state (0/1)>
         # STATUS ADD <id>
         # -> S:STATUS <id> Task.GetState <state (0/1)>
-        return bool(int(args[0]))
+        return int(args[0])
 
     @classmethod
     def parse_is_running_status(cls, args: Sequence[str]) -> bool:
         """Parse a 'Task.IsRunning' event.
 
         Args:
             args: The arguments of the event.
```

### Comparing `aiovantage-0.8.1/src/aiovantage/command_client/interfaces/temperature.py` & `aiovantage-0.9.0/src/aiovantage/command_client/interfaces/temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/README.md` & `aiovantage-0.9.0/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/__init__.py` & `aiovantage-0.9.0/src/aiovantage/config_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/requests.py` & `aiovantage-0.9.0/src/aiovantage/config_client/requests.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/types.py` & `aiovantage-0.9.0/src/aiovantage/config_client/interfaces/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py` & `aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/get_object.py` & `aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/configuration/open_filter.py` & `aiovantage-0.9.0/src/aiovantage/config_client/interfaces/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/introspection/get_version.py` & `aiovantage-0.9.0/src/aiovantage/config_client/interfaces/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/interfaces/login/login.py` & `aiovantage-0.9.0/src/aiovantage/config_client/interfaces/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/__init__.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,34 +22,39 @@
 from .load import Load
 from .load_group import LoadGroup
 from .location_object import LocationObject
 from .master import Master
 from .module import Module
 from .module_gen2 import ModuleGen2
 from .omni_sensor import OmniSensor
+from .parent_device import ParentDevice
+from .port_device import PortDevice
 from .power_profile import PowerProfile
 from .pwm_power_profile import PWMPowerProfile
 from .qis_blind import QISBlind
 from .qube_blind import QubeBlind
 from .relay_blind import RelayBlind
 from .rgb_load_base import RGBLoadBase
 from .scene_point_relay import ScenePointRelay
 from .sensor import Sensor
 from .somfy_rs_485_group_child import SomfyRS485GroupChild
+from .somfy_rs_485_sdn_20_port import SomfyRS485SDN20Port
 from .somfy_rs_485_shade_child import SomfyRS485ShadeChild
 from .somfy_urtsi_2_group_child import SomfyURTSI2GroupChild
+from .somfy_urtsi_2_port import SomfyURTSI2Port
 from .somfy_urtsi_2_shade_child import SomfyURTSI2ShadeChild
 from .station_bus import StationBus
 from .station_object import StationObject
 from .system_object import SystemObject
 from .task import Task
 from .temperature import Temperature
 from .vantage_ddg_color_load import VantageDDGColorLoad
 from .vantage_dg_color_load import VantageDGColorLoad
 from .vantage_dmx_dali_gateway import VantageDmxDaliGateway
+from .vantage_dmx_gateway import VantageDmxGateway
 
 __all__ = [
     "AnemoSensor",
     "Area",
     "Blind",
     "BlindBase",
     "BlindGroup",
@@ -70,28 +75,33 @@
     "Load",
     "LoadGroup",
     "LocationObject",
     "Master",
     "Module",
     "ModuleGen2",
     "OmniSensor",
+    "ParentDevice",
+    "PortDevice",
     "PowerProfile",
     "PWMPowerProfile",
     "QISBlind",
     "QubeBlind",
     "RelayBlind",
     "RGBLoadBase",
     "ScenePointRelay",
     "Sensor",
     "SomfyRS485GroupChild",
+    "SomfyRS485SDN20Port",
     "SomfyRS485ShadeChild",
     "SomfyURTSI2GroupChild",
+    "SomfyURTSI2Port",
     "SomfyURTSI2ShadeChild",
     "StationBus",
     "StationObject",
     "SystemObject",
     "Task",
     "Temperature",
     "VantageDDGColorLoad",
     "VantageDGColorLoad",
     "VantageDmxDaliGateway",
+    "VantageDmxGateway",
 ]
```

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/blind_base.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/blind_base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/button.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/master.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-"""Button object."""
+"""Master (controller) object."""
 
 from dataclasses import dataclass, field
 from typing import Optional
 
-from .child_object import ChildObject
 from .system_object import SystemObject
 
 
 @dataclass
-class Button(ChildObject, SystemObject):
-    """Button object."""
+class Master(SystemObject):
+    """Master (controller) object."""
 
-    text1: str = field(
+    number: int = field(
         metadata={
-            "name": "Text1",
+            "name": "Number",
         }
     )
 
-    text2: str = field(
+    volts: float = field(
         metadata={
-            "name": "Text2",
+            "name": "Volts",
         }
     )
 
-    up_id: int = field(
+    amps: float = field(
         metadata={
-            "name": "Up",
+            "name": "Amps",
         }
     )
 
-    down_id: int = field(
+    module_count: int = field(
         metadata={
-            "name": "Down",
+            "name": "ModuleCount",
         }
     )
 
-    hold_id: int = field(
+    serial_number: int = field(
         metadata={
-            "name": "Hold",
+            "name": "SerialNumber",
         }
     )
 
-    pressed: Optional[bool] = field(
+    firmware_version: Optional[str] = field(
+        default=None,
+        metadata={
+            "type": "Ignore",
+        },
+    )
+
+    last_updated: Optional[int] = field(
         default=None,
         metadata={
             "type": "Ignore",
         },
     )
```

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/child_object.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/child_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/gmem.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/load.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/load_group.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/load_group.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/master.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/power_profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,40 @@
-"""Master (controller) object."""
+"""Power profile object."""
 
 from dataclasses import dataclass, field
-from typing import Optional
 
 from .system_object import SystemObject
 
 
 @dataclass
-class Master(SystemObject):
-    """Master (controller) object."""
+class PowerProfile(SystemObject):
+    """Power Profile object."""
 
-    number: int = field(
+    min: float = field(
         metadata={
-            "name": "Number",
+            "name": "Min",
         }
     )
 
-    volts: float = field(
+    max: float = field(
         metadata={
-            "name": "Volts",
+            "name": "Max",
         }
     )
 
-    amps: float = field(
+    adjust: int = field(
         metadata={
-            "name": "Amps",
+            "name": "Adjust",
         }
     )
 
-    module_count: int = field(
+    freq: int = field(
         metadata={
-            "name": "ModuleCount",
+            "name": "Freq",
         }
     )
 
-    serial_number: int = field(
+    inductive: bool = field(
         metadata={
-            "name": "SerialNumber",
+            "name": "Inductive",
         }
     )
-
-    firmware_version: Optional[str] = field(
-        default=None,
-        metadata={
-            "type": "Ignore",
-        },
-    )
-
-    last_updated: Optional[int] = field(
-        default=None,
-        metadata={
-            "type": "Ignore",
-        },
-    )
```

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/omni_sensor.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/omni_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/rgb_load_base.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/rgb_load_base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/config_client/models/system_object.py` & `aiovantage-0.9.0/src/aiovantage/config_client/models/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/__init__.py` & `aiovantage-0.9.0/src/aiovantage/controllers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .gmem import GMemController
 from .light_sensors import LightSensorsController
 from .load_groups import LoadGroupsController
 from .loads import LoadsController
 from .masters import MastersController
 from .modules import ModulesController
 from .omni_sensors import OmniSensorsController
+from .port_devices import PortDevicesController
 from .rgb_loads import RGBLoadsController
 from .stations import StationsController
 from .tasks import TasksController
 from .temperature_sensors import TemperatureSensorsController
 
 __all__ = [
     "AnemoSensorsController",
@@ -30,12 +31,13 @@
     "GMemController",
     "LightSensorsController",
     "LoadGroupsController",
     "LoadsController",
     "MastersController",
     "ModulesController",
     "OmniSensorsController",
+    "PortDevicesController",
     "RGBLoadsController",
     "StationsController",
     "TasksController",
     "TemperatureSensorsController",
 ]
```

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/anemo_sensors.py` & `aiovantage-0.9.0/src/aiovantage/controllers/anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/base.py` & `aiovantage-0.9.0/src/aiovantage/controllers/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.9.0/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/blinds.py` & `aiovantage-0.9.0/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/buttons.py` & `aiovantage-0.9.0/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.9.0/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/gmem.py` & `aiovantage-0.9.0/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/light_sensors.py` & `aiovantage-0.9.0/src/aiovantage/controllers/light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.9.0/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/loads.py` & `aiovantage-0.9.0/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/masters.py` & `aiovantage-0.9.0/src/aiovantage/controllers/masters.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.9.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.9.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/tasks.py` & `aiovantage-0.9.0/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/src/aiovantage/controllers/temperature_sensors.py` & `aiovantage-0.9.0/src/aiovantage/controllers/temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/LICENSE` & `aiovantage-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/README.md` & `aiovantage-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.8.1/pyproject.toml` & `aiovantage-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "xsdata==23.6",
+    "xsdata==23.7",
     "typing_extensions>=4.6.3,<5.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/loopj/aiovantage#readme"
 Issues = "https://github.com/loopj/aiovantage/issues"
 Source = "https://github.com/loopj/aiovantage"
 
 [project.optional-dependencies]
 dev = [
-    "black==23.3.0",
+    "black==23.7.0",
     "mypy==1.4.1",
-    "ruff==0.0.277",
+    "ruff==0.0.280",
     "pre-commit==3.3.3",
 ]
 
 [tool.hatch.version]
 path = "src/aiovantage/__about__.py"
 
 [[tool.hatch.envs.all.matrix]]
```

### Comparing `aiovantage-0.8.1/PKG-INFO` & `aiovantage-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.8.1
+Version: 0.9.0
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions<5.0,>=4.6.3
-Requires-Dist: xsdata==23.6
+Requires-Dist: xsdata==23.7
 Provides-Extra: dev
-Requires-Dist: black==23.3.0; extra == 'dev'
+Requires-Dist: black==23.7.0; extra == 'dev'
 Requires-Dist: mypy==1.4.1; extra == 'dev'
 Requires-Dist: pre-commit==3.3.3; extra == 'dev'
-Requires-Dist: ruff==0.0.277; extra == 'dev'
+Requires-Dist: ruff==0.0.280; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # aiovantage
 
 aiovantage is a Python library for interacting with and controlling Vantage InFusion home automation controllers.
 
 Uses a *controller* pattern inspired heavily by the [aiohue](https://github.com/home-assistant-libs/aiohue) library.
```

