# Comparing `tmp/lite_fastapi_local-0.0.39.tar.gz` & `tmp/lite_fastapi_local-0.0.40.tar.gz`

## Comparing `lite_fastapi_local-0.0.39.tar` & `lite_fastapi_local-0.0.40.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/QR_READ_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/__init__.py
--rw-r--r--   0        0        0     8932 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/requirements.txt
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/common/__init__.py
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/common/function.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/common/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/boxDoorModel.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/drimmLedModel.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/innerLedModel.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/motorModel.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/setupModel.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/solModel.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/sprayModel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/router/__init__.py
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/router/motorRouter.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/router/sensorRouter.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/src/lite_fastapi_local/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.39/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/__init__.py
+-rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/common/__init__.py
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/drimmLedModel.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/innerLedModel.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/registrationModel.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/router/__init__.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.40/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/QR_CHK_dep.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/QR_READ_dep.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/main.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 async def message(client, topic, payload, qos, properties):
     print('message: ', client, topic, payload, properties)
     last_topic = topic.split('/')[2]
     if last_topic == 'state':
         data = json.loads(payload.decode())
         if 'tof' in data:
             common.set_distance_of_lidar(int(data['tof']))
+        if 'motor' in data and data['motor'] == 'safe_mode_on':
+            common.set_safe_mode(True)
     elif last_topic == 'event':
         data = json.loads(payload.decode())
         common.set_count_max(data['qr_valid_count_max'])
         common.set_current_count(data['qr_valid_count'])
     elif last_topic == 'sendVideo':
         filepath_date = data['date']
         video_name = data['video_name']
@@ -87,14 +89,15 @@
     
 @mqtt.subscribe("tg/#")
 async def message_to_topic(client, topic, payload, qos, properties):
     if common.get_MACHINE_MAC():
         return
     mac_address = topic.split('/')[1]
     common.set_MACHINE_MAC(mac_address)
+    registration.register_iot_core_by_mac_address()
     # common.set_MACHINE_MAC(data["MAC"])
     # data = json.loads(payload.decode())
     mqtt.client.unsubscribe("tg/#")
     mqtt.client.subscribe(f"tg/{mac_address}/#")
     print('get mac address!!')
     
 @app.get('/', response_class=PlainTextResponse)
@@ -179,20 +182,20 @@
 
 @app.on_event('startup')
 def startup_event():
     camera_index_list = find_camera_index_list('HD USB Camera')
     print(find_camera_index(camera_index_list))
     camera_inner_index, camera_cctv_index = find_camera_index(camera_index_list)
     
-    port = find_lidar_sensor_port_number()
-    if port:
-        print('find lidar port!')
-        common.set_lidar_sensor_port(port)
-    else:
-        print('fail to find lidar port...')
+    # port = find_lidar_sensor_port_number()
+    # if port:
+    #     print('find lidar port!')
+    #     common.set_lidar_sensor_port(port)
+    # else:
+    #     print('fail to find lidar port...')
     
     common.set_camera_inner_index(camera_inner_index)
     common.set_camera_cctv_index(camera_cctv_index)
     
 @app.on_event('startup')
 @repeat_every(seconds=60 * 60 * 2)
 def delete_old_log_file():
@@ -223,29 +226,27 @@
     json_response = response.json()
     RESP = json_response['RESP_DATA'][0]['ACCT_NM']
     return RESP
     #return response.text
     
     
 @app.get('/transfer')
-async def send_post_request(RCV_ACCT_NO: str, RCV_BNK_CD: str):
+async def send_post_request(RCV_ACCT_NO: str, RCV_BNK_CD: str, TRSC_AMT: str, customer_phone_number: str, returned_qr_code_list: list):
     mac_address = common.get_MACHINE_MAC()
-    returned_qr_code_list = common.get_returned_qr_code_list()
+    # returned_qr_code_list = common.get_returned_qr_code_list()
     url = 'http://54.180.21.162/coocon/transfer'
     data = {
         'RCV_BNK_CD': RCV_BNK_CD,
         'RCV_ACCT_NO': RCV_ACCT_NO,
-        'TRSC_AMT': '914',
+        'TRSC_AMT': TRSC_AMT,
         'accountName': '',
         'classQr': returned_qr_code_list,
-        'classNum': [
-            '050',
-            '051'
-        ],
-        'mac_address': mac_address
+        'return_ECIS': mac_address,
+        'customer_Id': customer_phone_number,
+        'dbType': 'op01'
     }
     response = requests.post(url, json=data)
     return response.json()
 
 
 def start_server():
     uvicorn.run(app, host="127.0.0.1", port=8000)
```

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/requirements.txt` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/settings.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/common/function.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/common/function.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/common/variable.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/common/variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         self.camera_inner_index = -1
         self.camera_cctv_index = -1
         self.lider_sensor_port = ""
         self.image_directory = ""
         self.uploading_videos = []
         self.returned_qr_code_list = []
         self.distance_of_lider = 110
+        self.safe_mode = False
 
     def get_current_device_data(self):
         return self.current_device_data
     
     def set_current_device_data(self, data):
         self.current_device_data = data
 
@@ -121,9 +122,15 @@
         self.returned_qr_code_list = []
         
     def get_distance_of_lidar(self):
         return self.distance_of_lider
     
     def set_distance_of_lidar(self, distance):
         self.distance_of_lider = distance
+    
+    def get_safe_mode(self):
+        return self.safe_mode
+    
+    def set_safe_mode(self, mode):
+        self.safe_mode = mode
 
 common = Common()
```

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/motorModel.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/model/solModel.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/router/motorRouter.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/router/motorRouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         content = {
             "code_number": 25,
             "code_name": "no_mac_address",
         }
         return JSONResponse(status_code=status.HTTP_400_BAD_REQUEST, content=content)
     if move == "open":
         common.set_operating_status('opening')
+        common.set_safe_mode(False)
         common.add_returned_qr_code_list(qr_code)
         current_count = common.get_current_count()
         count_max = common.get_count_max()
         # if count_max == current_count:
         #     content = {
         #         "code_number": 23,
         #         "code_name": "unacceptable",
@@ -170,8 +171,24 @@
     elif power == 'off':
         sol.turn_off_sol(str(int(index) - 1))
     content = {
         "code_number": 11,
         "code_name": "accepted",
     }
     return JSONResponse(status_code=status.HTTP_202_ACCEPTED, content=content)
-    
+    
+@router.get("isEmergency")
+def checkEmergency():
+    safe_mode = common.get_safe_mode()
+    if safe_mode == True:
+        content = {
+            "code_number": 10,
+            "code_name": "success",
+            "isEmergency": True
+        }
+    else:
+        content = {
+            "code_number": 10,
+            "code_name": "success",
+            "isEmergency": False
+        }
+    return JSONResponse(status_code=status.HTTP_200_OK, content=content)
```

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/router/sensorRouter.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/src/lite_fastapi_local/router/setupRouter.py` & `lite_fastapi_local-0.0.40/src/lite_fastapi_local/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/LICENSE` & `lite_fastapi_local-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.39/pyproject.toml` & `lite_fastapi_local-0.0.40/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.39"
+version = "0.0.40"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.39/PKG-INFO` & `lite_fastapi_local-0.0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.39
+Version: 0.0.40
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

