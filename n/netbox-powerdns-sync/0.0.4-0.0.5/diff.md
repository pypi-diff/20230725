# Comparing `tmp/netbox_powerdns_sync-0.0.4.tar.gz` & `tmp/netbox_powerdns_sync-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_powerdns_sync-0.0.4.tar", max compression
+gzip compressed data, was "netbox_powerdns_sync-0.0.5.tar", max compression
```

## Comparing `netbox_powerdns_sync-0.0.4.tar` & `netbox_powerdns_sync-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1062 2023-07-24 17:31:08.060448 netbox_powerdns_sync-0.0.4/LICENSE
--rw-r--r--   0        0        0     4971 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/README.md
--rw-r--r--   0        0        0      707 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/__init__.py
--rw-r--r--   0        0        0      808 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/nested_serializers.py
--rw-r--r--   0        0        0     1934 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/serializers.py
--rw-r--r--   0        0        0      251 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/urls.py
--rw-r--r--   0        0        0      739 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/views.py
--rw-r--r--   0        0        0      925 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/choices.py
--rw-r--r--   0        0        0      334 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/constants.py
--rw-r--r--   0        0        0      295 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/exceptions.py
--rw-r--r--   0        0        0      705 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/fields.py
--rw-r--r--   0        0        0     2620 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/filtersets.py
--rw-r--r--   0        0        0       73 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/__init__.py
--rw-r--r--   0        0        0     2288 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/filtersets.py
--rw-r--r--   0        0        0     3654 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/model_forms.py
--rw-r--r--   0        0        0      719 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/sync.py
--rw-r--r--   0        0        0    15260 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/jobs.py
--rw-r--r--   0        0        0     4094 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/migrations/__init__.py
--rw-r--r--   0        0        0    10555 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/models.py
--rw-r--r--   0        0        0     4065 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/naming.py
--rw-r--r--   0        0        0     1113 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/navigation.py
--rw-r--r--   0        0        0      533 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/querysets.py
--rw-r--r--   0        0        0     1654 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/record.py
--rw-r--r--   0        0        0     4855 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/signals.py
--rw-r--r--   0        0        0     3881 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/tables.py
--rw-r--r--   0        0        0     2060 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html
--rw-r--r--   0        0        0     2047 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html
--rw-r--r--   0        0        0     1531 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html
--rw-r--r--   0        0        0     1378 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html
--rw-r--r--   0        0        0     1147 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html
--rw-r--r--   0        0        0     5565 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html
--rw-r--r--   0        0        0     1449 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/urls.py
--rw-r--r--   0        0        0     3312 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/utils.py
--rw-r--r--   0        0        0      280 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/validators.py
--rw-r--r--   0        0        0       22 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/version.py
--rw-r--r--   0        0        0       69 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/__init__.py
--rw-r--r--   0        0        0     2166 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/api_servers.py
--rw-r--r--   0        0        0     5085 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/syncs.py
--rw-r--r--   0        0        0     1546 2023-07-24 17:31:08.064448 netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/zones.py
--rw-r--r--   0        0        0      653 2023-07-24 17:31:08.068448 netbox_powerdns_sync-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 netbox_powerdns_sync-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-25 05:52:12.874738 netbox_powerdns_sync-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5598 2023-07-25 05:52:12.874738 netbox_powerdns_sync-0.0.5/README.md
+-rw-r--r--   0        0        0      707 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/__init__.py
+-rw-r--r--   0        0        0      808 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/nested_serializers.py
+-rw-r--r--   0        0        0     1934 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/serializers.py
+-rw-r--r--   0        0        0      251 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/urls.py
+-rw-r--r--   0        0        0      739 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/views.py
+-rw-r--r--   0        0        0      925 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/choices.py
+-rw-r--r--   0        0        0      334 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/constants.py
+-rw-r--r--   0        0        0      295 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/exceptions.py
+-rw-r--r--   0        0        0      705 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/fields.py
+-rw-r--r--   0        0        0     2620 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/filtersets.py
+-rw-r--r--   0        0        0       73 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/forms/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/forms/filtersets.py
+-rw-r--r--   0        0        0     3654 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/forms/model_forms.py
+-rw-r--r--   0        0        0      719 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/forms/sync.py
+-rw-r--r--   0        0        0    15260 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/jobs.py
+-rw-r--r--   0        0        0     4094 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/migrations/__init__.py
+-rw-r--r--   0        0        0    10587 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/models.py
+-rw-r--r--   0        0        0     4065 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/naming.py
+-rw-r--r--   0        0        0     1113 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/navigation.py
+-rw-r--r--   0        0        0      533 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/querysets.py
+-rw-r--r--   0        0        0     1654 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/record.py
+-rw-r--r--   0        0        0     4855 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/signals.py
+-rw-r--r--   0        0        0     3881 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/tables.py
+-rw-r--r--   0        0        0     2060 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html
+-rw-r--r--   0        0        0     2047 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html
+-rw-r--r--   0        0        0     1531 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html
+-rw-r--r--   0        0        0     1378 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html
+-rw-r--r--   0        0        0     1147 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html
+-rw-r--r--   0        0        0     5565 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html
+-rw-r--r--   0        0        0     1449 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/urls.py
+-rw-r--r--   0        0        0     3312 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/utils.py
+-rw-r--r--   0        0        0      280 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/validators.py
+-rw-r--r--   0        0        0       22 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/version.py
+-rw-r--r--   0        0        0       69 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/views/__init__.py
+-rw-r--r--   0        0        0     2166 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/views/api_servers.py
+-rw-r--r--   0        0        0     5085 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/views/syncs.py
+-rw-r--r--   0        0        0     1546 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/views/zones.py
+-rw-r--r--   0        0        0      653 2023-07-25 05:52:12.878738 netbox_powerdns_sync-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 netbox_powerdns_sync-0.0.5/PKG-INFO
```

### Comparing `netbox_powerdns_sync-0.0.4/LICENSE` & `netbox_powerdns_sync-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/README.md` & `netbox_powerdns_sync-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # NetBox PowerDNS sync plugin
 
 A [Netbox](https://github.com/netbox-community/netbox) plugin to manage
 DNS records in PowerDNS based on netbox IP Address and Device objects.
 
 ## Features
 
-- Automatically generates A & AAAA records based on IP Address & Device objects
-  and DNS zone settings
+- Automatically generates A, AAAA & PTR records based on IP Address & Device
+  objects and DNS zone settings
 - Can manage multiple DNS Zones across multiple PowerDNS servers
 - Flexible rules to match netbox IP Addresses into DNS zones
 - Multiple options how to generate DNS name from IP address or Device
 - Option to schedule sync of DNS zones from netbox to PowerDNS
 - Can add DNS records for new zones immediately
+- Setup synchronization schedule for each zone individually
 
 ## Generating DNS names
 
 Each zone can define tags on IPAddress, Interface/VMInterface, FGRPGroup
 or Device/VirtualMachine that match that zone. You can also match on
 device role. A zone can also be only used for IPs that are assigned to management
 only interfaces. 
@@ -31,24 +32,24 @@
 If no match is found then it will try to match based on assigned tags in this
 order: IPAddress.tags, Interface.tags, VMInterface.tags, Device.tags,
 VirtualMachine.tags, Device.device_role, VM.role.
 
 If there is still not matching zone found, default zone is used (if set).
 
 When a zone is set for an IP address, the DNS name is generated by using
-set methods set on the zone. THe IP naming method is tried first, then the
+set methods set on the zone. The IP naming method is tried first, then the
 device and lastly the FHRP group method.
 
 ## Compatibility
 
 This plugin requires netbox version 3.5.x to work. Here is s compatibility table:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|       3.5      |      1.0.x     |
+|       3.5      | 0.0.1 - 1.0.x  |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
@@ -111,30 +112,50 @@
 
 PLUGINS_CONFIG = {
     "netbox_powerdns_sync": {
         # Example settings below, see "Available settings"
         # in README.md for all possible settings
         "ttl_custom_field": "",
         "powerdns_managed_record_comment": None,
+|       "post_save_enabled": False,
     },
 }
 ```
 
 ### Available settings
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
-| `ttl_custom_field` | `None`| Name of netbox Custom field applied to IP Address objects. See [Custom TTL field](#CustomTTLfield) below. |
+| `ttl_custom_field` | `None`| Name of netbox Custom field applied to IP Address objects. See [Custom TTL field](#custom-ttl-field) below. |
 | `powerdns_managed_record_comment` | `"netbox-powerdns-sync"`| Is set, the plugin will only touch records in PowerDNS API that have matching comment and ignore others. Set to `None` to make plugin manage all supported records. |
+| `post_save_enabled` | `False`| When creating or updating an IP Address, Device or FHRP Group, immediately create its DNS records using `post_save` signals. |
 
 #### Custom TTL field
 
 Normaly TTL for records is set by Default TTL on each Zone. There is an option to
 set TTL for each DNS record individually. You need to define a netbox
 [Custom field](https://docs.netbox.dev/en/stable/customization/custom-fields/)
 of type integer and apply it to IP Address objects. Then set plugin option
 `ttl_custom_field` to the name of that field.
 
 ![TTL custom field](docs/img/ttl_custom_field.png)
 
 Now you can set TTL on each IP Address and any corresponding DNS records will get
 that TTL value.
+
+## Screenshots
+
+List of DNS zones:
+
+![DNS Zone list](docs/img/netbox_powerdns_sync-zone_list.png)
+
+DNS Zone details:
+
+![DNS Zone details](docs/img/netbox_powerdns_sync-zone_details.png)
+
+Scheduling Zone sync:
+
+![Sync schedule](docs/img/netbox_powerdns_sync-sync_schedule.png)
+
+Sync results for Zone:
+
+![Sync result](docs/img/netbox_powerdns_sync-sync_result.png)
```

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/__init__.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/nested_serializers.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/serializers.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/api/views.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/choices.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/fields.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/fields.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/filtersets.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/filtersets.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/forms/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/model_forms.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/forms/sync.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/forms/sync.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/jobs.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/jobs.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/migrations/0001_initial.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/models.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,16 +186,17 @@
         if self.is_reverse and self.is_default:
             msg = "Reverse zone cannot be set as default"
             if exclude and "is_default" in exclude:
                 raise ValidationError(msg)
             else:
                 raise ValidationError({"is_default": msg})
         
-        if not any((self.naming_ip_method, self.naming_fgrpgroup_method, \
-            self.naming_device_method)):
+        if not self.is_reverse and not any((
+            self.naming_ip_method, self.naming_fgrpgroup_method, self.naming_device_method
+        )):
             raise ValidationError("At least one of naming methods must be set")
 
     def delete(self, *args, **kwargs):
         # delete any scheduled jobs fot this zone
         if self.pk:
             jobs = Job.objects.filter(
                 object_type_id=ContentType.objects.get_for_model(self).pk,
```

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/naming.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/naming.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/navigation.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/querysets.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/querysets.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/record.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/record.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/signals.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/tables.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/apiserver.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/htmx/sync_result.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_result.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/sync_schedule.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/syncs.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/templates/netbox_powerdns_sync/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/urls.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/utils.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/api_servers.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/views/api_servers.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/syncs.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/views/syncs.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/netbox_powerdns_sync/views/zones.py` & `netbox_powerdns_sync-0.0.5/netbox_powerdns_sync/views/zones.py`

 * *Files identical despite different names*

### Comparing `netbox_powerdns_sync-0.0.4/pyproject.toml` & `netbox_powerdns_sync-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-powerdns-sync"
-version = "0.0.4"
+version = "0.0.5"
 description = "Sync DNS records in PowerDNS with NetBox"
 authors = ["Matej Vadnjal <matej.vadnjal@arnes.si>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ArnesSI/netbox-powerdns-sync/"
 keywords = ["netbox", "netbox-plugin", "powerdns"]
 packages = [{include = "netbox_powerdns_sync"}]
```

### Comparing `netbox_powerdns_sync-0.0.4/PKG-INFO` & `netbox_powerdns_sync-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-powerdns-sync
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sync DNS records in PowerDNS with NetBox
 Home-page: https://github.com/ArnesSI/netbox-powerdns-sync/
 License: MIT
 Keywords: netbox,netbox-plugin,powerdns
 Author: Matej Vadnjal
 Author-email: matej.vadnjal@arnes.si
 Requires-Python: >=3.9
@@ -19,21 +19,22 @@
 # NetBox PowerDNS sync plugin
 
 A [Netbox](https://github.com/netbox-community/netbox) plugin to manage
 DNS records in PowerDNS based on netbox IP Address and Device objects.
 
 ## Features
 
-- Automatically generates A & AAAA records based on IP Address & Device objects
-  and DNS zone settings
+- Automatically generates A, AAAA & PTR records based on IP Address & Device
+  objects and DNS zone settings
 - Can manage multiple DNS Zones across multiple PowerDNS servers
 - Flexible rules to match netbox IP Addresses into DNS zones
 - Multiple options how to generate DNS name from IP address or Device
 - Option to schedule sync of DNS zones from netbox to PowerDNS
 - Can add DNS records for new zones immediately
+- Setup synchronization schedule for each zone individually
 
 ## Generating DNS names
 
 Each zone can define tags on IPAddress, Interface/VMInterface, FGRPGroup
 or Device/VirtualMachine that match that zone. You can also match on
 device role. A zone can also be only used for IPs that are assigned to management
 only interfaces. 
@@ -49,24 +50,24 @@
 If no match is found then it will try to match based on assigned tags in this
 order: IPAddress.tags, Interface.tags, VMInterface.tags, Device.tags,
 VirtualMachine.tags, Device.device_role, VM.role.
 
 If there is still not matching zone found, default zone is used (if set).
 
 When a zone is set for an IP address, the DNS name is generated by using
-set methods set on the zone. THe IP naming method is tried first, then the
+set methods set on the zone. The IP naming method is tried first, then the
 device and lastly the FHRP group method.
 
 ## Compatibility
 
 This plugin requires netbox version 3.5.x to work. Here is s compatibility table:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|       3.5      |      1.0.x     |
+|       3.5      | 0.0.1 - 1.0.x  |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
@@ -129,31 +130,51 @@
 
 PLUGINS_CONFIG = {
     "netbox_powerdns_sync": {
         # Example settings below, see "Available settings"
         # in README.md for all possible settings
         "ttl_custom_field": "",
         "powerdns_managed_record_comment": None,
+|       "post_save_enabled": False,
     },
 }
 ```
 
 ### Available settings
 
 | Setting | Default value | Description |
 |---------|---------------|-------------|
-| `ttl_custom_field` | `None`| Name of netbox Custom field applied to IP Address objects. See [Custom TTL field](#CustomTTLfield) below. |
+| `ttl_custom_field` | `None`| Name of netbox Custom field applied to IP Address objects. See [Custom TTL field](#custom-ttl-field) below. |
 | `powerdns_managed_record_comment` | `"netbox-powerdns-sync"`| Is set, the plugin will only touch records in PowerDNS API that have matching comment and ignore others. Set to `None` to make plugin manage all supported records. |
+| `post_save_enabled` | `False`| When creating or updating an IP Address, Device or FHRP Group, immediately create its DNS records using `post_save` signals. |
 
 #### Custom TTL field
 
 Normaly TTL for records is set by Default TTL on each Zone. There is an option to
 set TTL for each DNS record individually. You need to define a netbox
 [Custom field](https://docs.netbox.dev/en/stable/customization/custom-fields/)
 of type integer and apply it to IP Address objects. Then set plugin option
 `ttl_custom_field` to the name of that field.
 
 ![TTL custom field](docs/img/ttl_custom_field.png)
 
 Now you can set TTL on each IP Address and any corresponding DNS records will get
 that TTL value.
 
+## Screenshots
+
+List of DNS zones:
+
+![DNS Zone list](docs/img/netbox_powerdns_sync-zone_list.png)
+
+DNS Zone details:
+
+![DNS Zone details](docs/img/netbox_powerdns_sync-zone_details.png)
+
+Scheduling Zone sync:
+
+![Sync schedule](docs/img/netbox_powerdns_sync-sync_schedule.png)
+
+Sync results for Zone:
+
+![Sync result](docs/img/netbox_powerdns_sync-sync_result.png)
+
```

