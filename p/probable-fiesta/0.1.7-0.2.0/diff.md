# Comparing `tmp/probable_fiesta-0.1.7.tar.gz` & `tmp/probable_fiesta-0.2.0.tar.gz`

## Comparing `probable_fiesta-0.1.7.tar` & `probable_fiesta-0.2.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/.env
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/env
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/requirements.txt
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tox.ini
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/.github/workflows/python_app.yml
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/.gitignore
--rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/coverage_html.js
--rw-r--r--   0        0        0    18544 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_0293064cae6f51b1_args_parse_py.html
--rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html
--rw-r--r--   0        0        0    17408 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_0293064cae6f51b1_parser_builder_py.html
--rw-r--r--   0        0        0    29534 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_309aba7555c96ec5_logger_factory_py.html
--rw-r--r--   0        0        0    32638 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_309aba7555c96ec5_logger_py.html
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_3b40d2e1b447d1de___about___py.html
--rw-r--r--   0        0        0    45718 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html
--rw-r--r--   0        0        0    58461 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html
--rw-r--r--   0        0        0    16956 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_app_py.html
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html
--rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_context_py.html
--rw-r--r--   0        0        0    56232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html
--rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html
--rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html
--rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_7a0574776d91e073_test_app_builder_py.html
--rw-r--r--   0        0        0    14310 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_7a0574776d91e073_test_app_py.html
--rw-r--r--   0        0        0    20353 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_929858da485d1af8_logging_config_py.html
--rw-r--r--   0        0        0    38348 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_9610c8957119e03c_main_py.html
--rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_a44f0ac069e85531_test_main_app_py.html
--rw-r--r--   0        0        0    14163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_a44f0ac069e85531_test_v1_py.html
--rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_b5ab6064aa946d24_v1_py.html
--rw-r--r--   0        0        0    38305 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_config_builder_py.html
--rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_config_factory_py.html
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_default_config_py.html
--rw-r--r--   0        0        0    12207 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_variables_py.html
--rw-r--r--   0        0        0    32979 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_builder_py.html
--rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_factory_py.html
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_py.html
--rw-r--r--   0        0        0    31733 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_queue_py.html
--rw-r--r--   0        0        0    16599 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html
--rw-r--r--   0        0        0    29275 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_py.html
--rw-r--r--   0        0        0    24515 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/favicon_32.png
--rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/status.json
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/htmlcov/style.css
--rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/scripts/build_install.sh
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/scripts/build_publish.sh
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/scripts/run_tests.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/scripts/templater.sh
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/scripts/test_coverage.sh
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/__init__.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/app_abstract_machine.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/app_builder.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/command_context_factory.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context_builder.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context_factory.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context_holder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/cli/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/my_args_parser.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/parser.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/parser_builder.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/parser_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/command/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/command/builder/__init__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/command/builder/command.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/command/builder/command_builder.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/command/builder/command_factory.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/command/builder/command_queue.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/command/builder/command_queue_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/_init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/default_config.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/module_config.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/builder/__init__.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/builder/config.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/builder/config_builder.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/config/builder/config_builder_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/logger_module.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/logging_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/__init__.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger_abstract_machine.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger_builder.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger_factory.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/run/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/src/probable_fiesta/run/main.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/__about__.py.j2
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/hatch.toml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/hatch.toml.j2
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/make_skeleton.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/pyproject.toml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/pyproject.toml.j2
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/run___init__.py.j2
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/tox.ini
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/tox.ini.j2
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/write_templates.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/src/probable_fiesta/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/src/probable_fiesta/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/src/probable_fiesta/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/src/probable_fiesta/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/src/probable_fiesta/cli/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/src/probable_fiesta/run/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/templates/src/probable_fiesta/run/main.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/test_main_app.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/test_v1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/app/builder/__init__.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/app/builder/test_app_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/cli/builder/__init__.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/cli/builder/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/command/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/command/builder/__init__.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/command/builder/test_command.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/command/builder/test_command_builder.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/command/builder/test_command_context_factory.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/command/builder/test_command_factory.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/command/builder/test_command_queue.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/config/builder/__init__.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/config/builder/test_config.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/config/builder/test_config_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/logger/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/logger/builder/__init__.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/logger/builder/test_logger.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/tests/logger/builder/test_logger_factory.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/LICENSE
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/hatch.toml
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 probable_fiesta-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/.env
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/env
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tox.ini
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/.github/workflows/python_app.yml
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0    18544 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_0293064cae6f51b1_args_parse_py.html
+-rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html
+-rw-r--r--   0        0        0    17408 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_0293064cae6f51b1_parser_builder_py.html
+-rw-r--r--   0        0        0    29534 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_309aba7555c96ec5_logger_factory_py.html
+-rw-r--r--   0        0        0    32638 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_309aba7555c96ec5_logger_py.html
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_3b40d2e1b447d1de___about___py.html
+-rw-r--r--   0        0        0    45718 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html
+-rw-r--r--   0        0        0    58461 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html
+-rw-r--r--   0        0        0    16956 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_app_py.html
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html
+-rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_context_py.html
+-rw-r--r--   0        0        0    56232 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html
+-rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html
+-rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html
+-rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_7a0574776d91e073_test_app_builder_py.html
+-rw-r--r--   0        0        0    14310 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_7a0574776d91e073_test_app_py.html
+-rw-r--r--   0        0        0    20353 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_929858da485d1af8_logging_config_py.html
+-rw-r--r--   0        0        0    38348 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_9610c8957119e03c_main_py.html
+-rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_a44f0ac069e85531_test_main_app_py.html
+-rw-r--r--   0        0        0    14163 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_a44f0ac069e85531_test_v1_py.html
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_b5ab6064aa946d24_v1_py.html
+-rw-r--r--   0        0        0    38305 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_config_builder_py.html
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_config_factory_py.html
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_default_config_py.html
+-rw-r--r--   0        0        0    12207 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_variables_py.html
+-rw-r--r--   0        0        0    32979 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_builder_py.html
+-rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_factory_py.html
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_py.html
+-rw-r--r--   0        0        0    31733 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_queue_py.html
+-rw-r--r--   0        0        0    16599 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html
+-rw-r--r--   0        0        0    29275 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_py.html
+-rw-r--r--   0        0        0    24515 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/htmlcov/style.css
+-rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/scripts/build_install.sh
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/scripts/build_publish.sh
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/scripts/run_tests.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/scripts/templater.sh
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/scripts/test_coverage.sh
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/__init__.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/app_abstract_machine.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/app_builder.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/command_context_factory.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context_builder.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context_factory.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context_holder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/cli/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/my_args_parser.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/parser.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/parser_builder.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/parser_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/command/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/command/builder/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/command/builder/command.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/command/builder/command_builder.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/command/builder/command_factory.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/command/builder/command_queue.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/command/builder/command_queue_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/_init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/default_config.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/module_config.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/builder/__init__.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/builder/config.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/builder/config_builder.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/config/builder/config_builder_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/logger_module.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/logging_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/__init__.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger_abstract_machine.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger_builder.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger_factory.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/run/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/src/probable_fiesta/run/main.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/__about__.py.j2
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/hatch.toml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/hatch.toml.j2
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/make_skeleton.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/pyproject.toml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/run___init__.py.j2
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/tox.ini
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/tox.ini.j2
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/write_templates.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/src/probable_fiesta/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/src/probable_fiesta/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/src/probable_fiesta/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/src/probable_fiesta/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/src/probable_fiesta/cli/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/src/probable_fiesta/run/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/templates/src/probable_fiesta/run/main.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/test_main_app.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/test_v1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/app/builder/__init__.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/app/builder/test_app_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/cli/builder/__init__.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/cli/builder/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/command/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/command/builder/__init__.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/command/builder/test_command.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/command/builder/test_command_builder.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/command/builder/test_command_context_factory.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/command/builder/test_command_factory.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/command/builder/test_command_queue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/config/builder/__init__.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/config/builder/test_config.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/config/builder/test_config_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/logger/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/logger/builder/__init__.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/logger/builder/test_logger.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/tests/logger/builder/test_logger_factory.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/hatch.toml
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 probable_fiesta-0.2.0/PKG-INFO
```

### Comparing `probable_fiesta-0.1.7/requirements.txt` & `probable_fiesta-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/.github/workflows/python_app.yml` & `probable_fiesta-0.2.0/.github/workflows/python_app.yml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/.github/workflows/python_publish.yml` & `probable_fiesta-0.2.0/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/coverage_html.js` & `probable_fiesta-0.2.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_0293064cae6f51b1_args_parse_py.html` & `probable_fiesta-0.2.0/htmlcov/d_0293064cae6f51b1_args_parse_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html` & `probable_fiesta-0.2.0/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_0293064cae6f51b1_parser_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_0293064cae6f51b1_parser_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html` & `probable_fiesta-0.2.0/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_309aba7555c96ec5_logger_factory_py.html` & `probable_fiesta-0.2.0/htmlcov/d_309aba7555c96ec5_logger_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_309aba7555c96ec5_logger_py.html` & `probable_fiesta-0.2.0/htmlcov/d_309aba7555c96ec5_logger_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_3b40d2e1b447d1de___about___py.html` & `probable_fiesta-0.2.0/htmlcov/d_3b40d2e1b447d1de___about___py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html` & `probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_app_py.html` & `probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_app_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html` & `probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_context_py.html` & `probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_context_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html` & `probable_fiesta-0.2.0/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html` & `probable_fiesta-0.2.0/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_7a0574776d91e073_test_app_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_7a0574776d91e073_test_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_7a0574776d91e073_test_app_py.html` & `probable_fiesta-0.2.0/htmlcov/d_7a0574776d91e073_test_app_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_929858da485d1af8_logging_config_py.html` & `probable_fiesta-0.2.0/htmlcov/d_929858da485d1af8_logging_config_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_9610c8957119e03c_main_py.html` & `probable_fiesta-0.2.0/htmlcov/d_9610c8957119e03c_main_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_a44f0ac069e85531_test_main_app_py.html` & `probable_fiesta-0.2.0/htmlcov/d_a44f0ac069e85531_test_main_app_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_a44f0ac069e85531_test_v1_py.html` & `probable_fiesta-0.2.0/htmlcov/d_a44f0ac069e85531_test_v1_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_b5ab6064aa946d24_v1_py.html` & `probable_fiesta-0.2.0/htmlcov/d_b5ab6064aa946d24_v1_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_config_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_config_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_config_factory_py.html` & `probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_config_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_default_config_py.html` & `probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_default_config_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_c005feb2a2df0035_variables_py.html` & `probable_fiesta-0.2.0/htmlcov/d_c005feb2a2df0035_variables_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_factory_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d52ee57c951d550c_command_queue_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d52ee57c951d550c_command_queue_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html` & `probable_fiesta-0.2.0/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/favicon_32.png` & `probable_fiesta-0.2.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/index.html` & `probable_fiesta-0.2.0/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/keybd_closed.png` & `probable_fiesta-0.2.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/keybd_open.png` & `probable_fiesta-0.2.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/status.json` & `probable_fiesta-0.2.0/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/htmlcov/style.css` & `probable_fiesta-0.2.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/scripts/build_install.sh` & `probable_fiesta-0.2.0/scripts/build_install.sh`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/app/main.py` & `probable_fiesta-0.2.0/src/probable_fiesta/app/main.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/app/builder/app_abstract_machine.py` & `probable_fiesta-0.2.0/src/probable_fiesta/app/builder/app_abstract_machine.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/app/builder/app_builder.py` & `probable_fiesta-0.2.0/src/probable_fiesta/app/builder/app_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context.py` & `probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context_builder.py` & `probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context_factory.py` & `probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Context Factory class."""
-from .context import Context
 from ...command.builder.command_queue import CommandQueue
-from ...command.builder.command_factory import CommandFactory
+from ...app.builder.context import Context
 
 
 class ContextFactory:
     @staticmethod
     def new_context(name=None, command_queue=None):
         if command_queue is None:
             command_queue = CommandQueue()
         return Context(name, command_queue)
 
     @staticmethod
     def new_context_one_new_command(context_name, command_name, function, *args):
-        cq = CommandQueue.new(CommandFactory.new_command(command_name, function, *args))
+        cq = CommandQueue()
+        cq.add_new_command(command_name, function, *args)
         context = ContextFactory.new_context(context_name, cq)
         return context
 
     @staticmethod
     def new_context_one_command(context_name, command):
-        cq = CommandQueue.new(command)
+        cq = CommandQueue()
+        cq.add_command(command)
         context = ContextFactory.new_context(context_name, cq)
         return context
 
     @staticmethod
     def new_context_piped_commands(context_name, commands):
         cq = CommandQueue()
         for command in commands:
```

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/app/builder/context_holder.py` & `probable_fiesta-0.2.0/src/probable_fiesta/app/builder/context_holder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/my_args_parser.py` & `probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/my_args_parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/parser.py` & `probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/parser_builder.py` & `probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/parser_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/cli/builder/parser_factory.py` & `probable_fiesta-0.2.0/src/probable_fiesta/cli/builder/parser_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/command/builder/command_builder.py` & `probable_fiesta-0.2.0/src/probable_fiesta/command/builder/command_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/command/builder/command_queue.py` & `probable_fiesta-0.2.0/src/probable_fiesta/command/builder/command_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command Queue class."""
+import inspect
 from .command_factory import CommandFactory
 from .command import Command
 
 from ...logger.builder.logger_abstract_machine import LoggerMachine
 
 machine = LoggerMachine()
 SYSTEM_LOG = machine.make_logger(
@@ -43,15 +44,22 @@
     def clear(self):
         self.queue = []
         self.length = 0
         return self
 
     def run_command(self, command, input_data=None):
         self.length -= 1
-        result = command.invoke(input_data)
+        num_params = len(inspect.signature(command.function).parameters)
+
+        # If the command has its own arguments or doesn't need any input, don't pass the input_data
+        if num_params == 0 or command.args or input_data is None:
+            result = command.invoke()
+        else:
+            result = command.invoke(input_data)
+
         self.history.append(result)
         self.output = result
         return result
 
     def run_all(self):
         if self.length <= 0:
             return self
```

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/config/module_config.py` & `probable_fiesta-0.2.0/src/probable_fiesta/config/module_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/config/variables.py` & `probable_fiesta-0.2.0/src/probable_fiesta/config/variables.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/config/builder/config.py` & `probable_fiesta-0.2.0/src/probable_fiesta/config/builder/config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/config/builder/config_builder.py` & `probable_fiesta-0.2.0/src/probable_fiesta/config/builder/config_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/config/builder/config_builder_factory.py` & `probable_fiesta-0.2.0/src/probable_fiesta/config/builder/config_builder_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from .config_builder import ConfigBuilder
 from ...logger.builder.logger_abstract_machine import LoggerMachine as loggerMachine
 from ..variables import PackageDef as pd
 from ..variables import LoggerDef as ld
 from ..variables import VariablesDef as vd
 from ..variables import DotEnvDef as ded
 
+
 class ConfigFactory:
     @staticmethod
     def new_config_builder():
         return ConfigBuilder()
 
     @staticmethod
     def new_config():
         return ConfigBuilder().build()
 
     @staticmethod
-    def new_default_config_builder(log_type='default', log_name='default'):
+    def new_default_config_builder(log_type="default", log_name="default"):
         lM = loggerMachine()
         logger = lM.make_logger(log_type, log_name)
         cB = ConfigBuilder()
-        config = cB\
-            .package\
-                .set_package_name(pd.NAME)\
-            .logger\
-                .set_logger(logger)\
-            .variables\
-                .set_variable('VERSION', vd.VERSION)\
-            .dotenv\
-                .load_dotenv()\
-                .set_vars(ded())\
+        config = (
+            cB.package.set_package_name(pd.NAME)
+            .logger.set_logger(logger)
+            .variables.set_variable("VERSION", vd.VERSION)
+            .dotenv.load_dotenv()
+            .set_vars(ded().__dict__)  # Only public variables are loaded
             .build()
+        )
         return config
```

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/logger/logging_config.py` & `probable_fiesta-0.2.0/src/probable_fiesta/logger/logging_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger.py` & `probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger_abstract_machine.py` & `probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger_abstract_machine.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger_builder.py` & `probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/logger/builder/logger_factory.py` & `probable_fiesta-0.2.0/src/probable_fiesta/logger/builder/logger_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/src/probable_fiesta/run/__init__.py` & `probable_fiesta-0.2.0/src/probable_fiesta/run/__init__.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/templates/hatch.toml` & `probable_fiesta-0.2.0/templates/hatch.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/templates/hatch.toml.j2` & `probable_fiesta-0.2.0/templates/hatch.toml.j2`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/templates/make_skeleton.py` & `probable_fiesta-0.2.0/templates/make_skeleton.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/templates/pyproject.toml` & `probable_fiesta-0.2.0/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/templates/pyproject.toml.j2` & `probable_fiesta-0.2.0/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/templates/write_templates.py` & `probable_fiesta-0.2.0/templates/write_templates.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/test_main_app.py` & `probable_fiesta-0.2.0/tests/test_main_app.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/test_v1.py` & `probable_fiesta-0.2.0/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/app/builder/test_app_builder.py` & `probable_fiesta-0.2.0/tests/app/builder/test_app_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/cli/builder/test_parser.py` & `probable_fiesta-0.2.0/tests/cli/builder/test_parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/command/builder/test_command.py` & `probable_fiesta-0.2.0/tests/command/builder/test_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,68 +5,77 @@
 from logging import DEBUG
 from unittest import TestCase
 
 # Create a logger
 LOG = set_logger("test_command", DEBUG)
 
 
-class TestCommandBuilderCommand(TestCase):
+import pytest
+
+from src.probable_fiesta.command.builder import command
+
+
+class TestCommand(TestCase):
+    def test_init_valid(self):
+        name = "test"
+        func = lambda x: x
+        args = (1, 2, 3)
+
+        cmd = command.Command(name, func, *args)
+
+        assert cmd.name == name
+        assert cmd.function == func
+        assert cmd.args == args
+
+    def test_invoke_valid(self):
+        # Setup
+        func = lambda x, y: x**y
+        cmd = command.Command("square", func, 3, 2)
 
+        # Invoke
+        result = cmd.invoke()
+
+        # Assertions
+        self.assertEqual(result, 9)
+
+
+class TestCommandBuilderCommand(TestCase):
     def setUp(self):
         self.command = None
 
     def test_init(self):
-        LOG.info("Test init")
         self.command = command.Command(None, None, None)
         self.assertEqual(self.command.name, None)
         self.assertEqual(self.command.function, None)
         self.assertEqual(self.command.args, (None,))
-        # test _str__
-        LOG.debug(str(self.command))
-        self.assertEqual(str(self.command), "Command: {'name': None, 'function': None, 'args': (None,)}")
 
     def test_init_with_args(self):
-        LOG.info("Test new with args")
         function = lambda: "Hello World!"
         self.command = command.Command("test", function, "--version")
         self.assertEqual(self.command.name, "test")
-        self.assertAlmostEqual(self.command.function, function)
-        self.assertEqual(self.command.args, ('--version',))
-        # test _str__
-        LOG.debug(str(self.command))
-        self.assertEqual(str(self.command), "Command: {'name': 'test', "+f"'function': {function},"+" 'args': ('--version',)}")
+        self.assertEqual(self.command.function, function)
+        self.assertEqual(self.command.args, ("--version",))
 
     def test_factory(self):
-        LOG.info("Test factory")
         function = lambda: "Hello World!"
-        self.command = command.Command.Factory.new_command("test", function, "--version")
+        self.command = command.CommandFactory.new_command("test", function, "--version")
         self.assertEqual(self.command.name, "test")
         self.assertEqual(self.command.function, function)
-        self.assertEqual(self.command.args, ('--version',))
-        # test _str__
-        LOG.debug(str(self.command))
-        self.assertEqual(str(self.command), "Command: {'name': 'test', "+f"'function': {function},"+" 'args': ('--version',)}")
+        self.assertEqual(self.command.args, ("--version",))
 
     def test_invoke(self):
-        LOG.info("Test invoke")
-        self.command = command.Command("test", lambda: "Hello World!", None)
-        stdout = self.command.invoke()
-        print(stdout)
-        LOG.debug(stdout)
-        self.assertEqual(stdout, "Hello World!")
+        function = lambda x: x
+        self.command = command.Command("test", function, None)
+        result = self.command.invoke()
+        self.assertEqual(result, None)
 
     def test_invoke_with_args(self):
-        LOG.info("Test invoke with args")
-        function = lambda x: (self.command.args)
         args = "--version"
+        function = lambda x: x
         self.command = command.Command("test", function, args)
-        stdout = self.command.invoke()
-        LOG.debug(stdout)
-        self.assertEqual(stdout, self.command.args)
+        result = self.command.invoke()
+        self.assertEqual(result, args)
 
     def test_invoke_without_function(self):
-        LOG.info("Test invoke without function expect error log")
         self.command = command.Command(None, None, None)
-        stdout = self.command.invoke()
-        LOG.debug(stdout)
-        self.assertEqual(stdout, None)
-
+        with pytest.raises(TypeError):
+            self.command.invoke()
```

### Comparing `probable_fiesta-0.1.7/tests/command/builder/test_command_builder.py` & `probable_fiesta-0.2.0/tests/command/builder/test_command_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/command/builder/test_command_context_factory.py` & `probable_fiesta-0.2.0/tests/command/builder/test_command_context_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,35 +16,28 @@
         def sample_function(a, b):
             return str(a + b)
 
         context_name = "sample_context"
         command_name = "sample_command"
         arg1, arg2 = 1, 2
 
-        # Create a CommandQueue object and add the command
-        command_queue = CommandQueue.new(
-            [[CommandFactory.new_command(command_name, sample_function, "repeated")]]
-        )
-
+        # Create a CommandContext object with the command
         command_context = CommandContextFactory.create_command_context(
-            context_name, command_queue, sample_function
+            context_name, command_name, sample_function, arg1, arg2
         )
+
         self.app_builder.context.add_context(command_context)
 
         # Run the created command
-        self.app_builder.build().run(context_name)
+        app = self.app_builder.build()
+        app.run(context_name)
 
         # Check the output
-        run_history = self.app_builder.build().get_run_history()
-        if run_history:
-            stdout = self.app_builder.build().get_output()
-        else:
-            stdout = None
+        stdout = app.get_run_history()
 
-        print("Run history:", run_history)  # Add this print statement for debugging
         print("Actual output:", stdout)  # Add this print statement for debugging
 
         expected_output = sample_function(arg1, arg2)
         print(
             "Expected output:", expected_output
         )  # Add this print statement for debugging
```

### Comparing `probable_fiesta-0.1.7/tests/command/builder/test_command_factory.py` & `probable_fiesta-0.2.0/tests/command/builder/test_command_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/command/builder/test_command_queue.py` & `probable_fiesta-0.2.0/tests/command/builder/test_command_queue.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from unittest import TestCase
 
 # Create a logger
 LOG = set_logger("test_command_queue", DEBUG)
 
 
 class TestCommandBuilderCommandQueue(TestCase):
-
     def setUp(self):
         self.command_queue = command_queue.CommandQueue()
 
     def test_init(self):
         LOG.info("Test init")
         self.command_queue = command_queue.CommandQueue()
         self.assertEqual(self.command_queue.queue, [])
@@ -24,39 +23,42 @@
         function = lambda: "Hello World!"
         self.command_queue = command_queue.CommandQueue()
         self.command_queue.add_new_command("test", function, "--version")
         # test _str__
         LOG.debug(str(self.command_queue))
         exp = "CommandQueue: loaded commands: 1 executed commands: [] "
         self.assertEqual(str(self.command_queue), exp)
-    
+
     def test_show(self):
         LOG.info("Test show")
         function = lambda: "Hello World!"
         self.command_queue = command_queue.CommandQueue()
         self.command_queue.add_new_command("test", function, "--version")
         # test _str__
         queue = self.command_queue.show()
         for command in queue:
             print(command)
         LOG.debug(str(queue))
         self.assertEqual(len(queue), 1)
 
     def test_run_all(self):
         LOG.info("Test run all")
-        args = "--version"
-        function = lambda x: (args)
+        function = lambda: "Hello World!"
+        function2 = lambda x: f"Hello {x}"
         self.command_queue = command_queue.CommandQueue()
-        self.command_queue.add_new_command("test1", function, args)
-        self.command_queue.add_new_command("test2", function, args)
+        self.command_queue.add_new_command("test1", function)
+        self.command_queue.add_new_command("test2", function2)
         self.command_queue.run_all()
-        self.assertEqual(str(self.command_queue), "CommandQueue: loaded commands: 0 executed commands: ['--version', '--version'] ")
+        self.assertEqual(
+            str(self.command_queue),
+            "CommandQueue: loaded commands: 0 executed commands: ['Hello World!', 'Hello Hello World!'] ",
+        )
 
     def test_get_history(self):
         LOG.info("Test get history")
-        function = lambda x: (x)
+        function = lambda x: f"{x}"
         self.command_queue = command_queue.CommandQueue()
         self.command_queue.add_new_command("test1", function, "--test1")
         self.command_queue.add_new_command("test2", function, "--test2")
         self.command_queue.run_all()
         history = self.command_queue.get_history()
-        self.assertEqual(history, ["--test1", "--test2"])
+        self.assertEqual(history, ["--test1", "--test2"])
```

### Comparing `probable_fiesta-0.1.7/tests/config/builder/test_config.py` & `probable_fiesta-0.2.0/tests/config/builder/test_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/config/builder/test_config_builder.py` & `probable_fiesta-0.2.0/tests/config/builder/test_config_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/logger/builder/test_logger.py` & `probable_fiesta-0.2.0/tests/logger/builder/test_logger.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/tests/logger/builder/test_logger_factory.py` & `probable_fiesta-0.2.0/tests/logger/builder/test_logger_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/.gitignore` & `probable_fiesta-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/LICENSE` & `probable_fiesta-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/README.md` & `probable_fiesta-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/hatch.toml` & `probable_fiesta-0.2.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/pyproject.toml` & `probable_fiesta-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.7/PKG-INFO` & `probable_fiesta-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probable_fiesta
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python Core Package.
 Project-URL: Homepage, https://github.com/sergio-munoz/probable_fiesta/
 Project-URL: Bug Tracker, https://github.com/sergio-munoz/probable_fiesta/issues
 Project-URL: Documentation, https://github.com/sergio-munoz/probable_fiesta#readme
 Project-URL: Issues, https://github.com/sergio-munoz/probable_fiesta/issues
 Project-URL: Source, https://github.com/sergio-munoz/probable_fiesta
 Author-email: Sergio Munoz <sergio.munoz@pubnub.com>
```

