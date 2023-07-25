# Comparing `tmp/onoffmonitorserver-0.1.0-py3-none-any.whl.zip` & `tmp/onoffmonitorserver-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 6595 bytes, number of entries: 16
+Zip file size: 7258 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 17:32 onoffmonitorserver/__init__.py
 -rw-r--r--  2.0 unx      137 b- defN 23-Jul-22 16:30 onoffmonitorserver/admin.py
 -rw-r--r--  2.0 unx      204 b- defN 23-Jul-06 17:32 onoffmonitorserver/apps.py
 -rw-r--r--  2.0 unx      365 b- defN 23-Jul-06 17:32 onoffmonitorserver/filters.py
--rw-r--r--  2.0 unx     1561 b- defN 23-Jul-22 16:30 onoffmonitorserver/models.py
+-rw-r--r--  2.0 unx     1689 b- defN 23-Jul-25 09:48 onoffmonitorserver/models.py
 -rw-r--r--  2.0 unx      333 b- defN 23-Jul-06 17:32 onoffmonitorserver/permissions.py
--rw-r--r--  2.0 unx     1106 b- defN 23-Jul-22 16:30 onoffmonitorserver/serializers.py
+-rw-r--r--  2.0 unx     1120 b- defN 23-Jul-25 09:37 onoffmonitorserver/serializers.py
 -rw-r--r--  2.0 unx       60 b- defN 23-Jul-06 17:32 onoffmonitorserver/tests.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Jul-22 16:30 onoffmonitorserver/urls.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jul-22 16:41 onoffmonitorserver/views.py
+-rw-r--r--  2.0 unx     2184 b- defN 23-Jul-25 09:37 onoffmonitorserver/views.py
 -rw-r--r--  2.0 unx     2205 b- defN 23-Jul-22 16:30 onoffmonitorserver/migrations/0001_initial.py
+-rw-r--r--  2.0 unx      594 b- defN 23-Jul-25 09:51 onoffmonitorserver/migrations/0002_alter_device_gpio_pin_device_gpio_input_and_more.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 17:32 onoffmonitorserver/migrations/__init__.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-24 16:11 onoffmonitorserver-0.1.0.dist-info/RECORD
-16 files, 10990 bytes uncompressed, 4269 bytes compressed:  61.2%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1527 b- defN 23-Jul-25 09:54 onoffmonitorserver-0.2.0.dist-info/RECORD
+17 files, 11882 bytes uncompressed, 4684 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -27,23 +27,26 @@
 
 Filename: onoffmonitorserver/views.py
 Comment: 
 
 Filename: onoffmonitorserver/migrations/0001_initial.py
 Comment: 
 
+Filename: onoffmonitorserver/migrations/0002_alter_device_gpio_pin_device_gpio_input_and_more.py
+Comment: 
+
 Filename: onoffmonitorserver/migrations/__init__.py
 Comment: 
 
-Filename: onoffmonitorserver-0.1.0.dist-info/METADATA
+Filename: onoffmonitorserver-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: onoffmonitorserver-0.1.0.dist-info/WHEEL
+Filename: onoffmonitorserver-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: onoffmonitorserver-0.1.0.dist-info/top_level.txt
+Filename: onoffmonitorserver-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: onoffmonitorserver-0.1.0.dist-info/RECORD
+Filename: onoffmonitorserver-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onoffmonitorserver/models.py

```diff
@@ -22,16 +22,18 @@
     """
     Model for storing data about a device (such as "boiler")
     """
     user = models.ForeignKey(settings.AUTH_USER_MODEL,
                              on_delete=models.CASCADE)
     name = models.CharField(max_length=100)
     monitor = models.ForeignKey(Monitor, on_delete=models.CASCADE)
-    gpio_pin = models.PositiveSmallIntegerField(
-        verbose_name='GPIO pin on monitor')
+    gpio_input = models.PositiveSmallIntegerField(
+        verbose_name='GPIO input pin on monitor')
+    gpio_led = models.PositiveSmallIntegerField(
+        verbose_name='GPIO LED pin on monitor', null=True, blank=True)
 
     def __str__(self):
         return f'{self.name} ({self.user})'
 
 
 class Status(models.Model):
     """
```

## onoffmonitorserver/serializers.py

```diff
@@ -18,15 +18,15 @@
         print(attrs)
         if attrs['monitor'].user != attrs['user']:
             raise ValidationError('Device owner must be the current user')
         return super().validate(attrs)
 
     class Meta:
         model = models.Device
-        fields = ['id', 'name', 'user', 'monitor', 'gpio_pin']
+        fields = ['id', 'name', 'user', 'monitor', 'gpio_input', 'gpio_led']
 
 
 class StatusSerializer(ModelSerializer):
     user = CurrentUserDefault()
     def validate(self, attrs):
         if attrs['device'].user != self.user(self):
             raise ValidationError('Device owner must be the current user')
```

## onoffmonitorserver/views.py

```diff
@@ -21,15 +21,15 @@
     serializer_class = MonitorSerializer
     permission_classes = [IsAuthenticated, IsDeviceOwner]
     authentication_classes = [SessionAuthentication, TokenAuthentication]
     filter_backends = [DeviceOwnerFilter]
 
     @action(methods=['GET'], detail=True, url_path='conf')
     def device_list(self, request, pk: int):
-        return Response(models.Device.objects.filter(monitor_id=pk).values('id', 'gpio_pin'))
+        return Response(models.Device.objects.filter(monitor_id=pk).values('id', 'gpio_input', 'gpio_led'))
 
 
 class DeviceViewSet(ModelViewSet):
     """
     ViewSet for managing Device objects
     """
     queryset = models.Device.objects.all()
```

## Comparing `onoffmonitorserver-0.1.0.dist-info/METADATA` & `onoffmonitorserver-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onoffmonitorserver
-Version: 0.1.0
+Version: 0.2.0
 Summary: Django app for monitoring the on/off status of devices
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/onoffmonitorserver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: <4,>=3.10
```

