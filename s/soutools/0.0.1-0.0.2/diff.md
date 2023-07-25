# Comparing `tmp/soutools-0.0.1.tar.gz` & `tmp/soutools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soutools-0.0.1.tar", last modified: Tue Jul 18 04:42:41 2023, max compression
+gzip compressed data, was "soutools-0.0.2.tar", last modified: Tue Jul 25 03:15:15 2023, max compression
```

## Comparing `soutools-0.0.1.tar` & `soutools-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 04:42:41.851621 soutools-0.0.1/
--rw-rw-rw-   0        0        0     3670 2023-07-18 04:01:00.000000 soutools-0.0.1/.gitignore
--rw-rw-rw-   0        0        0     1089 2023-07-18 04:01:00.000000 soutools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       78 2023-07-18 04:42:41.851621 soutools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4734 2023-07-18 04:01:01.000000 soutools-0.0.1/README.md
--rw-rw-rw-   0        0        0      308 2023-07-18 04:01:01.000000 soutools-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      243 2023-07-18 04:01:01.000000 soutools-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 04:42:41.851621 soutools-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 04:42:41.770411 soutools-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 04:42:41.820388 soutools-0.0.1/src/soutools/
--rw-rw-rw-   0        0        0        0 2023-07-18 04:01:01.000000 soutools-0.0.1/src/soutools/__init__.py
--rw-rw-rw-   0        0        0     2913 2023-07-18 04:01:01.000000 soutools-0.0.1/src/soutools/controller.py
--rw-rw-rw-   0        0        0     2655 2023-07-18 04:01:01.000000 soutools-0.0.1/src/soutools/helpers.py
--rw-rw-rw-   0        0        0     2434 2023-07-18 04:01:01.000000 soutools-0.0.1/src/soutools/main.py
--rw-rw-rw-   0        0        0     1628 2023-07-18 04:01:01.000000 soutools-0.0.1/src/soutools/menu.py
--rw-rw-rw-   0        0        0     6918 2023-07-18 04:01:01.000000 soutools-0.0.1/src/soutools/model.py
--rw-rw-rw-   0        0        0     2919 2023-07-18 04:01:01.000000 soutools-0.0.1/src/soutools/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-18 04:42:41.851621 soutools-0.0.1/src/soutools.egg-info/
--rw-rw-rw-   0        0        0       78 2023-07-18 04:42:41.000000 soutools-0.0.1/src/soutools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-07-18 04:42:41.000000 soutools-0.0.1/src/soutools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 04:42:41.000000 soutools-0.0.1/src/soutools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-18 04:42:41.000000 soutools-0.0.1/src/soutools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      231 2023-07-18 04:42:41.000000 soutools-0.0.1/src/soutools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 04:42:41.000000 soutools-0.0.1/src/soutools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 04:42:41.851621 soutools-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-18 04:01:01.000000 soutools-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1776 2023-07-18 04:01:01.000000 soutools-0.0.1/tests/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.142420 soutools-0.0.2/
+-rw-rw-rw-   0        0        0     3670 2023-07-12 21:52:49.000000 soutools-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1089 2023-07-12 21:56:03.000000 soutools-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       78 2023-07-25 03:15:15.141424 soutools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4734 2023-07-18 03:33:41.000000 soutools-0.0.2/README.md
+-rw-rw-rw-   0        0        0      308 2023-07-25 03:13:59.000000 soutools-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      246 2023-07-25 02:52:40.000000 soutools-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 03:15:15.142420 soutools-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.008787 soutools-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.095558 soutools-0.0.2/src/soutools/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:01:06.000000 soutools-0.0.2/src/soutools/__init__.py
+-rw-rw-rw-   0        0        0     2915 2023-07-25 01:47:05.000000 soutools-0.0.2/src/soutools/controller.py
+-rw-rw-rw-   0        0        0     5268 2023-07-25 00:37:59.000000 soutools-0.0.2/src/soutools/helpers.py
+-rw-rw-rw-   0        0        0     2345 2023-07-24 14:56:11.000000 soutools-0.0.2/src/soutools/main.py
+-rw-rw-rw-   0        0        0     1506 2023-07-24 14:56:11.000000 soutools-0.0.2/src/soutools/menu.py
+-rw-rw-rw-   0        0        0     7654 2023-07-25 02:53:54.000000 soutools-0.0.2/src/soutools/model.py
+-rw-rw-rw-   0        0        0     3839 2023-07-25 00:38:00.000000 soutools-0.0.2/src/soutools/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.129455 soutools-0.0.2/src/soutools.egg-info/
+-rw-rw-rw-   0        0        0       78 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      232 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.136437 soutools-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:10:13.000000 soutools-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1776 2023-07-14 17:45:04.000000 soutools-0.0.2/tests/test_settings.py
```

### Comparing `soutools-0.0.1/.gitignore` & `soutools-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `soutools-0.0.1/LICENSE` & `soutools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soutools-0.0.1/README.md` & `soutools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `soutools-0.0.1/src/soutools/controller.py` & `soutools-0.0.2/src/soutools/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,87 @@
-#controller.py
+# controller.py
 
 """Controlls the main logic of the program"""
 
-import logging, sys
+import logging
+import sys
 
 from soutools import menu, model, helpers
 
 logger = logging.getLogger(__name__)
-
 dashboard = model.MerakiModel()
 org_id = helpers.get_settings.get_value('default_org_id')
 org_name = helpers.get_settings.get_value('default_org_name')
 
+
 def select_organization():
     global org_id, org_name
     logger.debug('The "select_organization" function called')
     org_id, org_name = dashboard.select_organization()
     logger.debug(f'The selected organization ID is "{org_id}"')
-    logger.debug(f'The selected organization name is "{org_name}"')
     logger.info(f'The selected organization name is "{org_name}"')
 
+
 def view_organization():
     logger.debug('The "view_organization" function called')
-    logger.debug("Checking if organization name is set")
+    logger.debug('Checking if organization name is set')
     if not org_name:
-        print("You have not selected an organization yet\n")
-        logger.debug("Notified user that organization name is not set")
+        print('\nYou have not selected an organization yet\n')
+        logger.debug('Notified user that organization name is not set')
     else:
-        print(f'You have choosen the "{org_name}"" organization\n')
-        logger.debug(f"Notified user that organization name is set to {org_name}")
+        blue_highlight = helpers.colorme(org_name, 'blue')
+        print(f'\nThe "{blue_highlight}" organization is currently selected\n')
+        logger.debug(f'Notified user that organization name is set to {org_name}')
     input('Press [ENTER] to continue...')
 
+
 def wireless_options():
     menu_title = helpers.menu_title
     wireless_menu = menu.Menu(
     menu_title, [
     ('Generate a report of all sites of type wireless', wireless_report),
-    ('Generate a report of all sites with a particular SSID', wireless_with_ssid_x_report),
+    ('Generate a report of all sites with a particular SSID', wireless_report_with_ssid_number),
     ('Update radius servers for a particular SSID', update_radius_settings),
     ('Return to the main menu', main_menu),
     ('Exit', quit)])
-
     while True:
-        wireless_menu.display()
         wireless_menu.get_input()
 
+
 def wireless_report():
     logger.debug('The "wireless_report" function called')
     if org_id:
         networks = dashboard.get_wireless_networks(org_id)
     else:
         print('No organization selected, please select organization first\n')
     path = helpers.get_settings.get_value('wireless_networks.output_file')
     helpers.writelines_to_file(path, networks)
     input('Press [ENTER] to continue...')
 
-def wireless_with_ssid_x_report():
+
+def wireless_report_with_ssid_number():
     logger.debug('The "wireless_with_ssid_x_report" function called')
-    dashboard.wheres_ssid_x()
+    dashboard.find_ssid_number()
     input('Press [ENTER] to continue...')
 
+
 def update_radius_settings():
     logger.debug('The "update_radius_settings" function called')
     dashboard.update_radius_servers()
     input('Press [ENTER] to continue...')
 
+
 def quit():
+    helpers.clear_screen()
     sys.exit()
 
+
 def main_menu():
     menu_title = helpers.menu_title
     main_menu = menu.Menu(
     menu_title, [
     ('Select an organization', select_organization),
     ('View the selected organization', view_organization),
     ('Wireless options', wireless_options),
     ('Exit', quit)])
-
     while True:
-        main_menu.display()
         main_menu.get_input()
```

### Comparing `soutools-0.0.1/src/soutools/main.py` & `soutools-0.0.2/src/soutools/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,65 @@
-# main.py
+#!/usr/bin/env python3
+
 """Initialize logger and hand off control to the controller module"""
 
 from datetime import datetime
 import logging
 import os
+import sys
 
 from soutools import settings, controller, helpers
 
+helpers.clear_screen()
+
 def main():
     get_settings = settings.Settings()
 
     # Get logging information from settings
     file_log_level = get_settings.get_value('logging.file_log_level')
     file_log_path = get_settings.get_value('logging.file_log_path')
-    log_to_console = get_settings.get_value('logging.log_to_console')
-    console_log_level = get_settings.get_value('logging.console_log_level')
 
     # Setup log path and ensure that folders exist and if not, then create them
-    home_dir = os.path.expanduser("~")
+    home_dir = os.path.expanduser('~')
     log_path = os.path.join(home_dir, file_log_path)
     helpers.setup_folder_structure(log_path)
     log_file = f'{log_path}soutools_log__{datetime.now():%Y-%m-%d_%H-%M-%S}.log'
 
     # Setup a basic logger
     logger = logging.getLogger('soutools')
     logger.setLevel(logging.DEBUG)
 
     # Setup file handler and add it to the logger
     fh = logging.FileHandler(filename=log_file)
     # Validate log level is a proper instance
     file_level = getattr(logging, file_log_level.upper(), None)
-    if not isinstance(file_level, int):
-        raise ValueError('Invalid log level: %s' % file_log_level)
-    else:
+    if isinstance(file_level, int):
         fh.setLevel(level = file_level)
+    else:
+        error = f'Invalid value "{file_log_level}" specified for the file_log_level'
+        error = helpers.colorme(error, 'red')
+        blue_text = helpers.colorme('file_log_level', 'blue')
+        error += f'\n  Check {blue_text} in the settings.toml'
+        error += '\n  Valid values are "debug", "info", "warning", "error", and "critical"'
+        print()
+        sys.exit('  ' + error)
     # create formatter and add it to the handler
     formatter = logging.Formatter('%(asctime)2s - %(name)19s - %(levelname)8s - %(message)s')
     fh.setFormatter(formatter)
-    # add the handlers to the logger
+    # add the handler to the logger
     logger.addHandler(fh)
 
     # create console handler and add it to the logger
-    if log_to_console:
-        ch = logging.StreamHandler()
-                # Validate log level is a proper instance
-        console_level = getattr(logging, console_log_level.upper(), None)
-        if not isinstance(console_level, int):
-            raise ValueError('Invalid log level: %s' % console_log_level)
-        else:
-            ch.setLevel(level = console_level)
-        # create formatter and add it to the handler
-        formatter = logging.Formatter('%(levelname)8s - %(message)s')
-        ch.setFormatter(formatter)
-        # add the handlers to the logger
-        logger.addHandler(ch)
+    ch = logging.StreamHandler()
+    ch.setLevel(level = 'WARNING')
+    # create formatter and add it to the handler
+    formatter = logging.Formatter('%(levelname)8s - %(message)s')
+    ch.setFormatter(formatter)
+    # add the handlers to the logger
+    logger.addHandler(ch)
     
-    logger.debug("Logger initialized, calling controller menu")
+    logger.debug('Logger initialized, calling controller menu function')
     controller.main_menu()
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()
```

### Comparing `soutools-0.0.1/src/soutools/menu.py` & `soutools-0.0.2/src/soutools/menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 # menu.py
 
 """This is used to handle the menu system"""
 
 from collections import namedtuple
-import platform, os
+
+from soutools import helpers
 
 Option = namedtuple('Option', ['label', 'callback'])
 
 class Menu:
     def __init__(self, title, options):
         self.title = title
         self._options = [Option(*option) for option in options]
 
     def display(self):
-        self.clear_screen()
-        print(f"\033[38;2;245;90;66m{self.title}\033[0m")
-        string = ''
+        helpers.clear_screen()
+        print(self.title)
+        menu_item = ''
         for i, option in enumerate(self._options, start=1):
-            string += f"    \033[38;2;90;200;66m{i} - {option.label}\033[0m\n"
-        print(string)
+            menu_item += helpers.colorme(f'    {str(i)} - {option.label}\n', 'green')
+        print(menu_item)
 
     def callback(self, i):
         if i <= len(self._options):
             return self._options[i - 1].callback
 
     def get_input(self):
         while True:
             try:
-                selection = int(input("\nPlease enter your selection number: "))
+                self.display()
+                selection = int(input('\n  Select an option >> '))
                 if selection not in range(1,len(self._options)+1):
                     print('\nEntry not in range, please try again: ')
                     input("Press Enter to Continue\n")
                     self.display()
                     continue
                 else:
+                    self.display()
                     return self._options[selection-1].callback()
             except ValueError:
                 print('\nEntry needs to be an integer, please try again: ')
-                input("Press Enter to Continue\n")
+                input('Press Enter to Continue\n')
                 self.display()
                 continue
-
-    def clear_screen(self):
-        if(platform.system().lower()=='windows'):
-            cmd = 'cls'
-        else:
-            cmd = 'clear'
-        os.system(cmd)
```

### Comparing `soutools-0.0.1/src/soutools/model.py` & `soutools-0.0.2/src/soutools/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-#!/usr/bin/env python3
+# model.py
 
-"""This module handles the interface between the controller and the Meraki Dashboard
-"""
+"""This module handles the interface between the controller and the Meraki Dashboard"""
 
 import logging
 import os
 import sys
 
 import meraki
 
 from soutools import helpers
 
 logger = logging.getLogger(__name__)
-
-logger.info("Loading settings for the dashboard instance")
+logger.info('Loading settings for the dashboard instance')
 
 
 class MerakiModel:
     def __init__(self) -> None:
         self.logger = logging.getLogger(__name__)
-        logger.info("Instantiated an instance of the model.MerakiModel class")
+        logger.info('Instantiated an instance of the model.MerakiModel class')
         if helpers.get_settings.get_value('meraki.api_key'):
             api_key = helpers.get_settings.get_value('meraki.api_key')
         elif helpers.get_settings.get_value('meraki.api_key_environment_variable') in os.environ:
             api_key = os.environ.get(helpers.get_settings.get_value('meraki.api_key_environment_variable'))
         else:
-            logger.error("API Key not found")
-            sys.exit("ERROR: API Key not found")
+            logger.error('API Key not found')
+            sys.exit('ERROR: API Key not found')
 
 
         # Instantiate an instance of the Meraki dashboard
         self.dashboard = meraki.DashboardAPI(
             api_key=api_key,
             output_log=helpers.get_settings.get_value('meraki.output_log'), 
             print_console=helpers.get_settings.get_value('meraki.print_to_console'), 
@@ -49,105 +47,125 @@
         Returns:
             str: the selected organization ID
             str: the selected organization name
         """
         logger.debug('The "select_organization" function called from the model')
         organizations = None
         try:
-            logger.debug("Trying to get organizations from the Meraki dashboard")
+            logger.debug('Trying to get organizations from the Meraki dashboard')
             organizations = self.dashboard.organizations.getOrganizations()
-            logger.debug(f"organizations is equal to {organizations}")
+            logger.debug(f'organizations is equal to {organizations}')
         except meraki.exceptions.APIError:
-            sys.exit("Check network connection and/or DNS settings.")
-        counter = 0
-        print("\nSelect organization:\n")
+        
+            sys.exit('Check network settings and verify API Key')
+        counter = 1
+        print('  Organizations to choose from:\n')
         for organization in organizations:
-            name = organization["name"]
-            print(f"{counter} - {name}")
+            name = helpers.colorme(f"{str(counter)} - {organization['name']}", 'green')
+            print(f'    {name}')
             counter += 1
-        selected = int(input("\nMake a choice: ")) # misc.validate_integer_in_range(counter)
+        selected = helpers.validate_integer_in_range(counter)
         return (
-            organizations[int(selected)]["id"],
-            organizations[int(selected)]["name"]
+            organizations[int(selected) - 1]['id'],
+            organizations[int(selected) - 1]['name']
         )
 
 
     def get_wireless_networks(self, organization_id):
         logger.debug(f'The "get_wireless_networks" function called with org_id {organization_id}')
         networks = self.dashboard.organizations.getOrganizationNetworks(
         organization_id, total_pages='all')
+        total = 0
         wireless = 0
         no_wireless = 0
         wireless_networks = []
         for network in networks:
             if 'wireless' in network['productTypes']:
                 wireless_networks.append(network['id'] + ',' + network['name'] + '\n')
                 logger.info(f'network {network["name"]}, was identified as having some type of wireless')
                 wireless += 1
+                total += 1
             else:
                 logger.info(f'network {network["name"]}, was identified as not having some type of wireless')
                 no_wireless += 1
-        
-        logger.info(f"INFO: There are {wireless} sites with some type of wireless device")
-        logger.info(f"INFO: There were {no_wireless} sites with no wireless")
+        logger.info(f'INFO: There are {wireless} sites with some type of wireless device')
+        logger.info(f'INFO: There were {no_wireless} sites with no wireless')
         
         return wireless_networks
 
 
-    def wheres_ssid_x(self):
+    def find_ssid_number(self):
         logger.debug('The "wheres_ssid" function called')
         search_ssid = helpers.get_settings.get_value('networks_with_ssid.ssid')
         input_file = helpers.get_settings.get_value('networks_with_ssid.input_file')
         networks = helpers.get_networks_list(input_file)
         path = helpers.get_settings.get_value('networks_with_ssid.output_file')
-        logger.debug(f'We are searching for ssid "{search_ssid}"')
-        logger.debug(f'We are searching for networks found in "{input_file}"')
-        logger.debug(f'We are writting to the path "{path}"')
-        found_count = not_found_count = 0 
+        logger.debug(f'Searching for ssid "{search_ssid}"')
+        logger.debug(f'Searching for networks found in "{input_file}"')
+        logger.debug(f'Writting to path "{path}"')
+        progress = found_count = not_found_count = 0 
+        total = len(networks)
+        logger.info(f'The total networks is {total}')
         ssid_sites = []
+        print()
         for network in networks:
+            bar = helpers.progress_bar(progress, total)
+            print(bar, end='', flush=True)
             site = network.split(',')
             site_id = site[0]
-            site_name = site[1].strip('\n')
+            site_name = site[1]
             logger.debug(f'Calling Meraki dashboard to pull all SSIDs for network {site_id}')
             ssids = self.dashboard.wireless.getNetworkWirelessSsids(site_id)
             found_ssid = False
             for ssid in ssids:
-                if (ssid['name'] == search_ssid and ssid['enabled'] == True and ssid['authMode'] == "8021x-radius"):
+                if (ssid['name'] == search_ssid and ssid['enabled'] == True and ssid['authMode'] == '8021x-radius'):
                     found_ssid = True
-                    newline = f"{site_id},{site_name},{ssid['name']},{ssid['number']}\n"
+                    newline = f'{site_id},{site_name},{ssid["name"]},{ssid["number"]}\n'
                     ssid_sites.append(newline)
                     logger.info(f'Found SSID {search_ssid} for "{site_name}"')
                     found_count += 1
+                    progress += 1
             if not found_ssid:
                 logger.info(f'SSID {search_ssid} was not found for "{site_name}"')
                 not_found_count += 1
+                progress += 1
+            print('\b' * len(bar), end='', flush=True)
+        bar = helpers.progress_bar(progress, total)
+        print(bar, end='', flush=True)
+        print('\n')
         helpers.writelines_to_file(path, ssid_sites)
-        logger.info(f"Sites with SSID {search_ssid}, found {found_count}")
-        logger.info(f"Sites without SSID {search_ssid}, found {not_found_count}")
+        logger.info(f'Sites with SSID {search_ssid}, found {found_count}')
+        logger.info(f'Sites without SSID {search_ssid}, found {not_found_count}')
 
 
     def update_radius_servers(self):
         logger.debug('The "update_radius_servers" function called')
         input_file = helpers.get_settings.get_value('radius.input_file')
         networks = helpers.get_networks_list(input_file)
         radius, accounting = helpers.format_radius()
-        logger.debug(f'We are searching for networks "{networks}"')
-        logger.debug(f'We are searching for radius servers "{radius}"')
-        logger.debug(f'We are searching for accounting servers "{accounting}"')
+        logger.debug(f'Searching for networks "{networks}"')
+        logger.debug(f'Searching for radius servers "{radius}"')
+        logger.debug(f'Searching for accounting servers "{accounting}"')
         
-        counter = 0
+        progress = 0
+        total = len(networks)
         for network in networks:
+            bar = helpers.progress_bar(progress, total)
+            print(bar, end='', flush=True)
             site = network.split(',')
             net_id = site[0]
             net_name = site[1]
-            ssid_num = site[3].strip('\n')
+            ssid_num = site[3]
             logger.info(f'Updating radius settings for {net_name} and SSID number {ssid_num}')
             logger.debug(f'Calling Meraki dashboard with {net_id} {ssid_num} {radius} {accounting}')
-        #    self.dashboard.wireless.updateNetworkWirelessSsid(
-        #        networkId=net_id,
-        #        number=ssid_num, 
-        #        radiusServers=radius,
-        #        radiusAccountingServers=accounting
-        #    )
-            counter += 1
-        logger.info(f'Updated radius settings on {counter} SSIDs')
+            self.dashboard.wireless.updateNetworkWirelessSsid(
+                networkId=net_id,
+                number=ssid_num, 
+                radiusServers=radius,
+                radiusAccountingServers=accounting
+            )
+            progress += 1
+            print('\b' * len(bar), end='', flush=True)
+        logger.info(f'Updated radius settings on {progress} SSIDs')
+        bar = helpers.progress_bar(progress, total)
+        print(bar, end='', flush=True)
+        print('\n')
```

### Comparing `soutools-0.0.1/tests/test_settings.py` & `soutools-0.0.2/tests/test_settings.py`

 * *Files identical despite different names*

