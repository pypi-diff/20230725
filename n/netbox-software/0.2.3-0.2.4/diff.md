# Comparing `tmp/netbox_software-0.2.3.tar.gz` & `tmp/netbox_software-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.2.3.tar", max compression
+gzip compressed data, was "netbox_software-0.2.4.tar", max compression
```

## Comparing `netbox_software-0.2.3.tar` & `netbox_software-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.3/LICENSE
--rw-r--r--   0        0        0     3420 2023-07-13 12:43:26.715969 netbox_software-0.2.3/README.md
--rw-r--r--   0        0        0      534 2023-07-13 12:43:26.707969 netbox_software-0.2.3/netbox_software/__init__.py
--rw-r--r--   0        0        0      699 2023-07-13 07:09:13.118198 netbox_software-0.2.3/netbox_software/admin.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.3/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     4757 2023-07-13 08:04:55.519077 netbox_software-0.2.3/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      445 2023-07-13 08:04:55.499076 netbox_software-0.2.3/netbox_software/api/urls.py
--rw-r--r--   0        0        0     1357 2023-07-13 10:00:09.172753 netbox_software-0.2.3/netbox_software/api/views.py
--rw-r--r--   0        0        0     4830 2023-07-13 12:13:31.207506 netbox_software-0.2.3/netbox_software/filtersets.py
--rw-r--r--   0        0        0     6062 2023-07-13 11:54:22.813357 netbox_software-0.2.3/netbox_software/forms.py
--rw-r--r--   0        0        0     6229 2023-07-13 09:59:12.131848 netbox_software-0.2.3/netbox_software/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.3/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     6692 2023-07-13 11:44:23.611927 netbox_software-0.2.3/netbox_software/models.py
--rw-r--r--   0        0        0     3117 2023-07-13 10:15:17.055009 netbox_software-0.2.3/netbox_software/navigation.py
--rw-r--r--   0        0        0     1216 2023-07-13 12:12:09.530212 netbox_software-0.2.3/netbox_software/search.py
--rw-r--r--   0        0        0     4452 2023-07-13 11:47:12.302581 netbox_software-0.2.3/netbox_software/tables.py
--rw-r--r--   0        0        0     5647 2023-07-13 08:14:35.344556 netbox_software-0.2.3/netbox_software/template_content.py
--rw-r--r--   0        0        0     1435 2023-07-13 11:02:11.516704 netbox_software-0.2.3/netbox_software/templates/netbox_software/application.html
--rw-r--r--   0        0        0      613 2023-07-13 07:50:20.328737 netbox_software-0.2.3/netbox_software/templates/netbox_software/application_edit.html
--rw-r--r--   0        0        0      669 2023-07-13 07:39:13.081944 netbox_software-0.2.3/netbox_software/templates/netbox_software/applicationversion.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.3/netbox_software/templates/netbox_software/applicationversion_edit.html
--rw-r--r--   0        0        0     1704 2023-07-13 10:48:52.323169 netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0     2108 2023-07-13 10:27:29.270544 netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2477 2023-07-13 10:50:18.520568 netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.3/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0     1116 2023-07-13 11:11:57.226346 netbox_software-0.2.3/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.3/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0     1691 2023-07-13 11:40:24.952229 netbox_software-0.2.3/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.3/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     3525 2023-07-13 10:14:12.001988 netbox_software-0.2.3/netbox_software/urls.py
--rw-r--r--   0        0        0     5243 2023-07-13 10:00:09.160753 netbox_software-0.2.3/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-07-13 12:43:26.723969 netbox_software-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3420 2023-07-24 10:08:36.275629 netbox_software-0.2.4/README.md
+-rw-r--r--   0        0        0      534 2023-07-24 10:08:36.287629 netbox_software-0.2.4/netbox_software/__init__.py
+-rw-r--r--   0        0        0      699 2023-07-13 07:09:13.118198 netbox_software-0.2.4/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.4/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     4757 2023-07-13 08:04:55.519077 netbox_software-0.2.4/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      445 2023-07-13 08:04:55.499076 netbox_software-0.2.4/netbox_software/api/urls.py
+-rw-r--r--   0        0        0     1357 2023-07-13 10:00:09.172753 netbox_software-0.2.4/netbox_software/api/views.py
+-rw-r--r--   0        0        0     4830 2023-07-24 09:37:34.463592 netbox_software-0.2.4/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     5962 2023-07-24 09:38:12.495597 netbox_software-0.2.4/netbox_software/forms.py
+-rw-r--r--   0        0        0     6229 2023-07-13 09:59:12.131848 netbox_software-0.2.4/netbox_software/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.4/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     6803 2023-07-24 11:20:15.835729 netbox_software-0.2.4/netbox_software/models.py
+-rw-r--r--   0        0        0     3117 2023-07-13 10:15:17.055009 netbox_software-0.2.4/netbox_software/navigation.py
+-rw-r--r--   0        0        0     1148 2023-07-13 14:24:33.277294 netbox_software-0.2.4/netbox_software/search.py
+-rw-r--r--   0        0        0     4452 2023-07-13 11:47:12.302581 netbox_software-0.2.4/netbox_software/tables.py
+-rw-r--r--   0        0        0     5789 2023-07-24 09:51:25.461957 netbox_software-0.2.4/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1889 2023-07-24 11:23:15.074495 netbox_software-0.2.4/netbox_software/templates/netbox_software/application.html
+-rw-r--r--   0        0        0      613 2023-07-13 07:50:20.328737 netbox_software-0.2.4/netbox_software/templates/netbox_software/application_edit.html
+-rw-r--r--   0        0        0      669 2023-07-13 07:39:13.081944 netbox_software-0.2.4/netbox_software/templates/netbox_software/applicationversion.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.4/netbox_software/templates/netbox_software/applicationversion_edit.html
+-rw-r--r--   0        0        0     1704 2023-07-13 10:48:52.323169 netbox_software-0.2.4/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0     2108 2023-07-13 10:27:29.270544 netbox_software-0.2.4/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     3010 2023-07-24 10:10:07.893007 netbox_software-0.2.4/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.4/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0     1116 2023-07-13 11:11:57.226346 netbox_software-0.2.4/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.4/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0     1691 2023-07-13 11:40:24.952229 netbox_software-0.2.4/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.4/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     3525 2023-07-13 10:14:12.001988 netbox_software-0.2.4/netbox_software/urls.py
+-rw-r--r--   0        0        0     5723 2023-07-17 06:33:55.249781 netbox_software-0.2.4/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-07-24 10:08:36.283629 netbox_software-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.4/PKG-INFO
```

### Comparing `netbox_software-0.2.3/LICENSE` & `netbox_software-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/README.md` & `netbox_software-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       | 0.2.3          |
+|     3.2+       | 0.2.4          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

### Comparing `netbox_software-0.2.3/netbox_software/__init__.py` & `netbox_software-0.2.4/netbox_software/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxSoftware(PluginConfig):
     name = 'netbox_software'
     verbose_name = 'Установленное ПО'
     description = 'Manage device software in Netbox'
-    version = '0.2.3'
+    version = '0.2.4'
     author = 'Ilya Zakharov'
     author_email = 'me@izakharov.ru'
     min_version = '3.2.0'
     base_url = 'software'
     default_settings = {
         "enable_navigation_menu": True,
         "enable_device_software": True,
```

### Comparing `netbox_software-0.2.3/netbox_software/admin.py` & `netbox_software-0.2.4/netbox_software/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/api/serializers.py` & `netbox_software-0.2.4/netbox_software/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/api/views.py` & `netbox_software-0.2.4/netbox_software/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/filtersets.py` & `netbox_software-0.2.4/netbox_software/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/forms.py` & `netbox_software-0.2.4/netbox_software/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,20 +80,15 @@
         fields = ('name', 'vendor', 'software_type', 'comments', 'tags')
 
 
 class ApplicationFilterForm(NetBoxModelFilterSetForm):
     model = Application
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
-        ('Атрибуты', ('name', 'software_type_id', 'vendor_id')),
-    )
-
-    name = forms.CharField(
-        label='Название',
-        required=False
+        ('Атрибуты', ('software_type_id', 'vendor_id')),
     )
 
     software_type_id = forms.ModelMultipleChoiceField(
         label='Тип',
         queryset=SoftwareType.objects.all(),
         required=False
     )
```

### Comparing `netbox_software-0.2.3/netbox_software/migrations/0001_initial.py` & `netbox_software-0.2.4/netbox_software/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/models.py` & `netbox_software-0.2.4/netbox_software/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,17 @@
 
     def __str__(self):
         return self.name
 
     def get_all_versions(self):
         return list(set(DeviceSoftware.objects.filter(app=self).values_list('version__name', flat=True)))
 
+    def get_all_hosts(self):
+        return DeviceSoftware.objects.filter(app=self).order_by('version__name')
+
 
 class ApplicationVersion(NetBoxModel):
     name = models.CharField(verbose_name="название", max_length=50, help_text='Укажите тип ПО')
     comments = models.TextField(verbose_name="комментарий", blank=True)
 
     class Meta:
         ordering = ('name',)
```

### Comparing `netbox_software-0.2.3/netbox_software/navigation.py` & `netbox_software-0.2.4/netbox_software/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/search.py` & `netbox_software-0.2.4/netbox_software/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,12 @@
             ("name", 100),
             ("comments", 5000),
         )
 
     class DeviceSoftwareIndex(SearchIndex):
         model = DeviceSoftware
         fields = (
-            ("app__name", 100),
-            ("version__name", 500),
             ("comments", 5000),
         )
 
     # Register indexes
     indexes = [VendorIndex, SoftwareTypeIndex, ApplicationIndex, ApplicationVersionIndex, DeviceSoftwareIndex]
```

### Comparing `netbox_software-0.2.3/netbox_software/tables.py` & `netbox_software-0.2.4/netbox_software/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/template_content.py` & `netbox_software-0.2.4/netbox_software/template_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 
 class DeviceSoftwareList(PluginTemplateExtension):
     model = 'dcim.device'
     def left_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'left':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
+                'vm': False,
                 'device_software': DeviceSoftware.objects.filter(assigned_object_id=self.context['object'].id,
                                                                  assigned_object_type__model='device')[:20],
                 'soft_count': DeviceSoftware.objects.filter(assigned_object_id=self.context['object'].id,
                                                             assigned_object_type__model='device').count(),
             })
         else:
             return ""
 
     def right_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'right':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
+                'vm': False,
                 'device_software': DeviceSoftware.objects.filter(assigned_object=self.context['object'].id,
                                                                  assigned_object_type__model='device')[:20],
                 'soft_count': DeviceSoftware.objects.filter(assigned_object=self.context['object'].id,
                                                             assigned_object_type__model='device').count(),
             })
         else:
             return ""
@@ -35,26 +37,28 @@
 class VirtualMachineSoftwareList(PluginTemplateExtension):
     model = 'virtualization.virtualmachine'
 
     def left_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'left':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
+                'vm': True,
                 'device_software': DeviceSoftware.objects.filter(assigned_object_id=self.context['object'].id,
                                                                  assigned_object_type__model='virtualmachine')[:20],
                 'soft_count': DeviceSoftware.objects.filter(assigned_object_id=self.context['object'].id,
                                                             assigned_object_type__model='virtualmachine').count(),
             })
         else:
             return ""
 
     def right_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'right':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
+                'vm': True,
                 'device_software': DeviceSoftware.objects.filter(assigned_object=self.context['object'].id,
                                                                  assigned_object_type__model='virtualmachine')[:20],
                 'soft_count': DeviceSoftware.objects.filter(assigned_object=self.context['object'].id,
                                                             assigned_object_type__model='virtualmachine').count(),
             })
         else:
             return ""
@@ -98,8 +102,8 @@
 #                 )[:20],
 #                 'soft_count': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']).count(),
 #             })
 #         else:
 #             return ""
 
 
-template_extensions = [DeviceSoftwareList]
+template_extensions = [DeviceSoftwareList, VirtualMachineSoftwareList]
```

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/application.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/application.html`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,25 @@
                   {% for version in object.get_all_versions %}
                     <span>{{ version|placeholder }}; </span>
                   {% endfor%}
                 {% else %}
                   Нет установленных версий
                 {% endif %}
             </tr>
+            <tr>
+              <th scope="row">Установлено на: </th>
+              <td>
+                {% if object.get_all_hosts %}
+                  {% for host in object.get_all_hosts %}
+                    <span>{{ host.assigned_object|linkify }} | {{ host.version|linkify }}</span><br>
+                  {% endfor%}
+                {% else %}
+                  Не установлено
+                {% endif %}
+            </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
```

#### html2text {}

```diff
@@ -2,10 +2,13 @@
 ** ÐÐ **
 ÐÐ°Ð·Ð²Ð°Ð½Ð¸Ðµ ÐÐ�{{ object.name|placeholder }}
 Ð¢Ð¸Ð¿ ÐÐ                   {{ object.software_type|linkify }}
 Ð Ð°Ð·ÑÐ°Ð±Ð¾ÑÑÐ¸{{ object.vendor|linkify }}
                                         {% if object.get_all_versions %} {% for version in object.get_all_versions %} {
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½{ version|placeholder }};  {% endfor%} {% else %} ÐÐµÑ ÑÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½Ð½ÑÑ
                                         Ð²ÐµÑÑÐ¸Ð¹ {% endif %}
+                                        {% if object.get_all_hosts %} {% for host in object.get_all_hosts %} {
+Ð£ÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½{ host.assigned_object|linkify }} | {{ host.version|linkify }}
+                                        {% endfor%} {% else %} ÐÐµ ÑÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½Ð¾ {% endif %}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/application_edit.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/application_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/applicationversion.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/applicationversion.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 {% load helpers %}
 
 <div class="card">
 <h5 class="card-header">
     ПО устройства
     {% if device_software %}
-      <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?device_id={{ object.pk }}">
+      <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?{% if vm %}virtual_machine_id{% else %}device_id{% endif %}={{ object.pk }}">
         (всего: {{ soft_count }})</a>
     {% endif %}
 </h5>
 <div class="card-body">
 {% if device_software %}
     <table class="table table-hover">
         <tr>
             <th>Название</th>
             <th>версия</th>
             <th></th>
         </tr>
         {% for software in device_software %}
         <tr>
             <td>
-                <a href="{% url 'plugins:netbox_software:application' pk=software.app.pk %}">{{ software.app.name }}</a>
+                <a href="{% url 'plugins:netbox_software:application' pk=software.app.pk %}">
+                  {{ software.app.name|slice:":50" }} {% if software.app.name|length > 50 %}...{% endif %}
+                </a>
             </td>
             <td>{{ software.version.name }}</td>
             <td class="text-end noprint">
                 <a href="{% url 'plugins:netbox_software:devicesoftware' pk=software.pk %}"
                    class="btn btn-primary btn-sm lh-1" title="Просмотреть">
                     <i class="mdi mdi-book" aria-hidden="true"></i>
                   </a>
-                  <a href="{% url 'plugins:netbox_software:devicesoftware_edit' pk=software.pk %}?return_url=
-                  {% url 'dcim:device' pk=object.pk %}" class="btn btn-warning btn-sm lh-1" title="Редактировать">
+                  <a href="{% url 'plugins:netbox_software:devicesoftware_edit' pk=software.pk %}?return_url={% if vm %}{% url 'virtualization:virtualmachine' pk=object.pk %}{% else %}{% url 'dcim:device' pk=object.pk %}{% endif %}"
+                     class="btn btn-warning btn-sm lh-1" title="Редактировать">
                     <i class="mdi mdi-pencil" aria-hidden="true"></i>
                   </a>
-                  <a href="{% url 'plugins:netbox_software:devicesoftware_delete' pk=software.pk %}?return_url=
-                  {% url 'dcim:device' pk=object.pk %}" class="btn btn-danger btn-sm lh-1" title="Удалить">
+                  <a href="{% url 'plugins:netbox_software:devicesoftware_delete' pk=software.pk %}?return_url={% if vm %}{% url 'virtualization:virtualmachine' pk=object.pk %}{% else %}{% url 'dcim:device' pk=object.pk %}{% endif %}"
+                     class="btn btn-danger btn-sm lh-1" title="Удалить">
                     <i class="mdi mdi-trash-can-outline" aria-hidden="true"></i>
                   </a>
               </td>
         </tr>
         {% endfor %}
     </table>
     {% else %}
         <div class="text-muted">
             Нет
         </div>
     {% endif %}
     </div>
         <div class="card-footer text-end noprint">
-            <a href="{% url 'plugins:netbox_software:devicesoftware_add' %}?device={{ object.pk }}&return_url={% url 'dcim:device' pk=object.pk %}" class="btn btn-primary btn-sm">
-                <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
-                Добавить ПО
+            <a href="{% url 'plugins:netbox_software:devicesoftware_add' %}?{% if vm %}virtual_machine={{ object.pk }}&return_url={% url 'virtualization:virtualmachine' pk=object.pk %}{% else %}device={{ object.pk }}&return_url={% url 'dcim:device' pk=object.pk %}{% endif %}"
+               class="btn btn-primary btn-sm">
+              <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
+              Добавить ПО
             </a>
-            <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?device={{ object.pk }}" class="btn btn-primary btn-sm">
-                Все ПО хоста
+            <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?{% if vm %}virtual_machine_id{% else %}device_id{% endif %}={{ object.pk }}"
+               class="btn btn-primary btn-sm">
+              Все ПО хоста
             </a>
         </div>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% load helpers %}
 ** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° {% if device_software %} (Ð²ÑÐµÐ³Ð¾:_{
 {_soft_count_}}) {% endif %} **
 {% if device_software %}
-ÐÐ°Ð·Ð²Ð°Ð½Ð²ÐµÑÑÐ¸Ñ
-{{_software.app.name_}} {{ software.version.name }}
+ÐÐ°Ð·Ð²Ð°Ð½Ð¸Ðµ               Ð²ÐµÑÑÐ¸Ñ
+{{_software.app.name|slice:":50"_}}_{%_if      {{ software.version.name }}
+software.app.name|length_>_50_%}...{%_endif_%}
 {% else %}
 ÐÐµÑ
 {% endif %}
  ÐÐ¾Ð±Ð°Ð²Ð¸ÑÑ_ÐÐ
  ÐÑÐµ_ÐÐ_ÑÐ¾ÑÑÐ°
```

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/software_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/softwaretype.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/softwaretype.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.2.4/netbox_software/templates/netbox_software/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/urls.py` & `netbox_software-0.2.4/netbox_software/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.3/netbox_software/views.py` & `netbox_software-0.2.4/netbox_software/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from netbox.views import generic
 from . import forms, models, tables, filtersets
+#from rest_framework import status, viewsets
+#from rest_framework.response import Response
 
 
 ### Vendor
 class VendorView(PermissionRequiredMixin, generic.ObjectView):
     permission_required = ('dcim.view_site', 'dcim.view_device')
     queryset = models.Vendor.objects.all()
 
@@ -47,14 +49,21 @@
 class SoftwareTypeEditView(PermissionRequiredMixin, generic.ObjectEditView):
     permission_required = ('dcim.view_site', 'dcim.view_device')
     queryset = models.SoftwareType.objects.all()
     form = forms.SoftwareTypeForm
 
     template_name = 'netbox_software/softwaretype_edit.html'
 
+#    def create(self, request, *args, **kwargs):
+#        serializer = self.get_serializer(data=request.data, many=isinstance(request.data,list))
+#        serializer.is_valid(raise_exception=True)
+#        self.perform_create(serializer)
+#        headers=self.get_success_headers(serializer.data)
+#        return Response(serializer.data, status=status.HTTP_201_CREATED, headers=headers)
+
 
 class SoftwareTypeDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
     permission_required = ('dcim.view_site', 'dcim.view_device')
     queryset = models.SoftwareType.objects.all()
 
 
 ### Application
```

### Comparing `netbox_software-0.2.3/PKG-INFO` & `netbox_software-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,15 +27,15 @@
 * Store links to external URL's to save duplication of remote software
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       | 0.2.3          |
+|     3.2+       | 0.2.4          |
 
 
 ## Installation
 
 A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
 
 #### Package Installation from PyPi
```

