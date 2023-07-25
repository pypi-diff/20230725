# Comparing `tmp/comun_va-0.6.tar.gz` & `tmp/comun_va-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-0.6.tar", last modified: Tue Jul 25 08:09:53 2023, max compression
+gzip compressed data, was "comun_va-0.7.tar", last modified: Tue Jul 25 08:19:06 2023, max compression
```

## Comparing `comun_va-0.6.tar` & `comun_va-0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:09:53.386731 comun_va-0.6/
--rw-rw-rw-   0        0        0       53 2023-07-25 08:09:53.386731 comun_va-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 08:09:53.385248 comun_va-0.6/comun_va.egg-info/
--rw-rw-rw-   0        0        0       53 2023-07-25 08:09:53.000000 comun_va-0.6/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-25 08:09:53.000000 comun_va-0.6/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:09:53.000000 comun_va-0.6/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-25 08:09:53.000000 comun_va-0.6/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 08:09:53.000000 comun_va-0.6/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4870 2023-07-25 08:07:13.000000 comun_va-0.6/comun_va.py
--rw-rw-rw-   0        0        0       42 2023-07-25 08:09:53.386731 comun_va-0.6/setup.cfg
--rw-rw-rw-   0        0        0      192 2023-07-25 08:09:12.000000 comun_va-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:19:06.394415 comun_va-0.7/
+-rw-rw-rw-   0        0        0       53 2023-07-25 08:19:06.393280 comun_va-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 08:19:06.390877 comun_va-0.7/comun_va.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-07-25 08:19:06.000000 comun_va-0.7/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-07-25 08:19:06.000000 comun_va-0.7/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:19:06.000000 comun_va-0.7/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-25 08:19:06.000000 comun_va-0.7/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 08:19:06.000000 comun_va-0.7/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5089 2023-07-25 08:18:43.000000 comun_va-0.7/comun_va.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:19:06.394415 comun_va-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      192 2023-07-25 08:18:43.000000 comun_va-0.7/setup.py
```

### Comparing `comun_va-0.6/comun_va.py` & `comun_va-0.7/comun_va.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,29 +25,32 @@
                 Date: {self.date_time},
                 Endpoint name: {self.endpoint_name},
                 Endpoint received data: {self.endpoint_data_received},
                 Result: {self.result},
                 Prediction: {self.prediction}         
                 """
 
-    def save_log(self, mssql_srv: str, database: str, user: str, passwd: str):
+    def save_log(self, mssql_srv: str, database: str, user: str, passwd: str, rescale_size: tuple = None):
         """
         Save the image in local path and the data into the DB
         :param mssql_srv: IP of the MSsql server
         :param database: Name of the database
         :param user: User of the database
         :param passwd: Password of the user
+        :param rescale_size: A tuple with the HxW to save the image, p.e.: (500x500)
         :return: doesn't return anything
         """
         # SAVE IMAGE:
         if self.img_frame is not None:
             if self.img_name is None:
                 self.img_name = f'{self.date_time.strftime("%Y_%m_%d_%H_%M_%S")}.jpg'
             if self.img_path is None:
                 self.img_path = f'img_save/{self.img_name}'
+            if rescale_size:
+                self.img_frame = cv2.resize(self.img_frame, rescale_size)
             cv2.imwrite(self.img_path, self.img_frame)
 
         # SAVE LOG IN DB:
         mssql = comun_sqlsrv.Sql(mssql_srv, database, user, passwd)
         query = f"""
                 INSERT INTO T_VA_API_LOG
                 (FECHA_HORA, ENDPOINT, RESULTADO, DATO_RECIBIDO, PREDICCION_VA, NOMBRE_IMAGEN, COD_BAR, ERROR)
```

