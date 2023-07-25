# Comparing `tmp/easypcd-0.0.27-py3-none-any.whl.zip` & `tmp/easypcd-0.0.28-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 8283 bytes, number of entries: 7
+Zip file size: 9049 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Jul-24 02:49 easypcd/__init__.py
--rw-rw-rw-  2.0 fat     4681 b- defN 23-Jul-24 07:41 easypcd/easypcd.py
--rw-rw-rw-  2.0 fat     9719 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2400 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      539 b- defN 23-Jul-24 07:43 easypcd-0.0.27.dist-info/RECORD
-7 files, 17485 bytes uncompressed, 7327 bytes compressed:  58.1%
+-rw-rw-rw-  2.0 fat     5866 b- defN 23-Jul-25 09:22 easypcd/easypcd.py
+-rw-rw-rw-  2.0 fat      471 b- defN 23-Jul-25 09:14 easypcd/test.py
+-rw-rw-rw-  2.0 fat     9719 b- defN 23-Jul-25 09:38 easypcd-0.0.28.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2562 b- defN 23-Jul-25 09:38 easypcd-0.0.28.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-25 09:38 easypcd-0.0.28.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-25 09:38 easypcd-0.0.28.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      610 b- defN 23-Jul-25 09:38 easypcd-0.0.28.dist-info/RECORD
+8 files, 19379 bytes uncompressed, 7987 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: easypcd/__init__.py
 Comment: 
 
 Filename: easypcd/easypcd.py
 Comment: 
 
-Filename: easypcd-0.0.27.dist-info/LICENSE
+Filename: easypcd/test.py
 Comment: 
 
-Filename: easypcd-0.0.27.dist-info/METADATA
+Filename: easypcd-0.0.28.dist-info/LICENSE
 Comment: 
 
-Filename: easypcd-0.0.27.dist-info/WHEEL
+Filename: easypcd-0.0.28.dist-info/METADATA
 Comment: 
 
-Filename: easypcd-0.0.27.dist-info/top_level.txt
+Filename: easypcd-0.0.28.dist-info/WHEEL
 Comment: 
 
-Filename: easypcd-0.0.27.dist-info/RECORD
+Filename: easypcd-0.0.28.dist-info/top_level.txt
+Comment: 
+
+Filename: easypcd-0.0.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## easypcd/easypcd.py

```diff
@@ -3,24 +3,26 @@
 @Project ：easypcd
 @File    ：easypcd.py
 @Author  ：王泽辉
 @Date    ：2023-05-09 15:02 
 '''
 import numpy as np
 
+
 class DotDict(dict):
     def __init__(self, *args, **kwargs):
         super(DotDict, self).__init__(*args, **kwargs)
 
     def __getattr__(self, key):
         value = self[key]
         if isinstance(value, dict):
             value = DotDict(value)
         return value
 
+
 class ep():
     def __init__(self):
         self.format_dic = {0: 'pcd', 1: "txt"}
         self.pcd_head = '# .PCD v0.7 - Point Cloud Data file format'
         self.VERSION = 'VERSION 0.7'
 
     def processing_str(self, input, s, length):
@@ -53,14 +55,15 @@
                     pass
                 else:
                     tmp = []
                     for i in range(len(line)):
                         tmp.append(format_type[pcd_type[i]](line[i]))
                     pcd_data.append(tmp)
             points = np.array(pcd_data)
+
             pcd_information.update({"points": points})
         return DotDict(pcd_information)
 
     def write_pcd(self, save_name, points, color=False, normal=False, _SIZE=4,
                   _TYPE="F", _COUNT=1, _HEIGHT=1, _VIEWPOINT='0 0 0 1 0 0 0', _DATA='ascii'):
         """功能：写入pcd文件
             必要参数：
@@ -71,31 +74,39 @@
                 color：是否有颜色信息（True/False），默认False
                 normal：是否有向量信息（True/False），默认False
                 _SIZE：字节数量，默认为4
                 _TYPE：字符类型，默认为F
                 _DATA：编码格式
         """
         if color == True and normal == False:
-            length = 6
-            FIELDS = "FIELDS x y z r g b"
+            length = 4
+            TYPE = self.processing_str("TYPE", _TYPE, length - 1) + ' U'
+            FIELDS = "FIELDS x y z rgb"
+            points = self.encode_rgb(length, points)
+
         if color == False and normal == False:
             length = 3
+            TYPE = self.processing_str("TYPE", _TYPE, length)
             FIELDS = "FIELDS x y z"
         if color == False and normal == True:
             length = 6
+            TYPE = self.processing_str("TYPE", _TYPE, length)
             FIELDS = "FIELDS x y z nx ny nz"
         if color == True and normal == True:
-            length = 9
-            FIELDS = "FIELDS x y z r g b nx ny nz"
+            length = 7
+            TYPE = self.processing_str("TYPE", _TYPE, length - 4) + " U" + self.processing_str("", _TYPE,
+                                                                                               length - 4)
+            FIELDS = "FIELDS x y z rgb nx ny nz"
+            points = self.encode_rgb(length, points)
         pcd_init = {
             "pcd_head": self.pcd_head,
             "VERSION": self.VERSION,
             "FIELDS": FIELDS,
             "SIZE": self.processing_str("SIZE", _SIZE, length),
-            "TYPE": self.processing_str("TYPE", _TYPE, length),
+            "TYPE": TYPE,
             "COUNT": self.processing_str("COUNT", _COUNT, length),
             "WIDTH": "WIDTH " + str(len(points)),
             "HEIGHT": 'HEIGHT ' + str(_HEIGHT),
             "VIEWPOINT": 'VIEWPOINT ' + str(_VIEWPOINT),
             "POINTS": "POINTS " + str(len(points)),
             "DATA": 'DATA ' + str(_DATA)
         }
@@ -116,12 +127,30 @@
             for line in points:
                 for p in line:
                     p = str(int(p))
                     f.write(p)
                     f.write(" ")
                 f.write("\n")
 
+    def encode_rgb(self, length, points):
+        # rgb编码
+        xyz = points[:, :3]  # 位置
+        color = points[:, 3:6]  # 颜色
+        color_tmp = []
+        for i in range(color.shape[0]):
+            color_tmp.append([int(color[i, 0]) << 16 | int(color[i, 1]) << 8 | int(color[i, 2])])  # 颜色重新编码
+        if length == 4:
+            ep_points = np.concatenate((xyz, np.asarray(color_tmp)), axis=1)  # 拼接位置信息和颜色信息
+
+        if length == 7:
+            nxyz = points[:, 6:]
+            ep_points = np.concatenate((xyz, np.asarray(color_tmp), nxyz), axis=1)  # 拼接位置信息和颜色信息
+        return ep_points
+
+    def decode_rgb(self, rgb):
+        r = (rgb >> 16) & 0x0000ff
+        g = (rgb >> 8) & 0x0000ff
+        b = (rgb) & 0x0000ff
+        return [r, g, b]
+
+
 
-if __name__ == '__main__':
-    easypcd1 = ep()
-    pcd = easypcd1.read_pcd("point.pcd")
-    easypcd1.write_pcd("1.pcd", pcd.points, True, True)
```

## Comparing `easypcd-0.0.27.dist-info/LICENSE` & `easypcd-0.0.28.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `easypcd-0.0.27.dist-info/METADATA` & `easypcd-0.0.28.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,67 @@
-Metadata-Version: 2.1
-Name: easypcd
-Version: 0.0.27
-Summary: a package for pcd
-Home-page: https://gitee.com/wang2wan/easypcd_project
-Author: GentleWang
-Author-email: 189030005@stu.just.edu.cn
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-
-#### Easypcd使你更专注与代码本身，而不需要因为pcd格式所带来的烦恼。  
-
-**1、 调用easypcd**  
-`from easypcd import ep`  
-`import open3d as o3d`   
-`import numpy as np`   
-
-**2、 读取pcd文件**  
-`ep_pcd = ep.read_pcd("point.pcd")# 读取pcd文件`  
-`print("point indormation:", ep_pcd)# 打印所有信息`  
-`print("point:", ep_pcd.points)# 打印点云坐标`  
-`print("points type:", type(ep_pcd.points))# 打印点云类型`  
-
-**3、 写入pcd文件**  
-`ep.write_pcd(save_name="ep-sample.pcd", points=ep_pcd.points)`
-
-**必要参数：**  
-`save_name:保存的文件名`  
-`points：需要保存的点云数据`
-
-**可选参数**  
-`color：是否有颜色信息（True/False），默认False`  
-`normal：是否有向量信息（True/False），默认False`  
-`_SIZE：字节数量，默认为4`  
-`_TYPE：字符类型，默认为F`  
-
-**4、 其他用法**     
-**4.1、 open3d读取写入**    
-`o3d_read = o3d.io.read_point_cloud("point.pcd")# 加载三维点云`  
-`ep.write_pcd(save_name="sample.pcd", points=o3d_read.points)# 写入pcd`    
-
-**4.2、 创建有颜色信息的点云**  
-`points_xyz = np.random.randint(100, size=(100, 3))  # 点云坐标`  
-`points_color = np.random.randint(5, size=(100, 3))  # 点云颜色`  
-`ep_points = np.concatenate((points_xyz, points_color), axis=1)  # 拼接位置信息和颜色信息`  
-`ep.write_pcd("ep-points.pcd", ep_points, color=True)  # 写入pcd`  
-
-
-**4.3、 点云信息转为open3d**  
-`o3d_object = o3d.geometry.PointCloud()  # 初始化点云`  
-`o3d_object.points = o3d.utility.Vector3dVector(ep_points[:, 0:3])  # 转为open3d的坐标`     
-`o3d_object.colors = o3d.utility.Vector3dVector(ep_points[:, 3:])  # 转为open3d的颜色信息`  
-`o3d.visualization.draw_geometries([o3d_object], window_name="POINT", width=400, height=300, mesh_show_back_face=True)  # 显示`  
-
+Metadata-Version: 2.1
+Name: easypcd
+Version: 0.0.28
+Summary: a package for pcd
+Home-page: https://gitee.com/wang2wan/easypcd_project
+Author: GentleWang
+Author-email: 189030005@stu.just.edu.cn
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+
+#### Easypcd使你更专注与代码本身，而不需要因为pcd格式所带来的烦恼。
+**v0.0.28更新：错误的rgb色彩空间** 
+
+**0、 安装easypcd** 
+`pip install easypcd`  
+
+**1、 调用easypcd**  
+`from easypcd import ep`  
+`import open3d as o3d`   
+`import numpy as np`   
+
+**2、 读取pcd文件**  
+`ep_pcd = ep.read_pcd("point.pcd")# 读取pcd文件`  
+`print("point indormation:", ep_pcd)# 打印所有信息`  
+`print("point:", ep_pcd.points)# 打印点云坐标`  
+`print("points type:", type(ep_pcd.points))# 打印点云类型`  
+
+**3、 写入pcd文件**  
+`ep.write_pcd(save_name="ep-sample.pcd", points=ep_pcd.points)`
+
+**必要参数：**  
+`save_name:保存的文件名`  
+`points：需要保存的点云数据`
+
+**可选参数**  
+`color：是否有颜色信息（True/False），默认False`  
+`normal：是否有向量信息（True/False），默认False`  
+`_SIZE：字节数量，默认为4`  
+`_TYPE：字符类型，默认为F`  
+
+**4、 其他用法**     
+**4.1、 open3d读取写入**    
+`o3d_read = o3d.io.read_point_cloud("point.pcd")# 加载三维点云`  
+`ep.write_pcd(save_name="sample.pcd", points=o3d_read.points)# 写入pcd`    
+
+**4.2、 创建有颜色信息的点云**  
+`points_xyz = np.random.randint(100, size=(100, 3))  # 点云坐标`  
+`points_color = np.random.randint(5, size=(100, 3))  # 点云颜色`  
+`points_nxyz = np.random.randint(100, size=(100, 3))  # 点云向量`  
+`ep_points = np.concatenate((points_xyz, points_color, points_nxyz), axis=1)  # 拼接位置信息、颜色信息和向量信息`  
+`ep.write_pcd(save_name="ep-points.pcd", points=ep_points, color=True, normal=True)  # 写入pcd`  
+
+
+**4.3、 点云信息转为open3d**  
+`o3d_object = o3d.geometry.PointCloud()  # 初始化点云`  
+`o3d_object.points = o3d.utility.Vector3dVector(ep_points[:, 0:3])  # 转为open3d的坐标`     
+`o3d_object.colors = o3d.utility.Vector3dVector(ep_points[:, 3:6])  # 转为open3d的颜色信息`  
+`o3d.visualization.draw_geometries([o3d_object], window_name="POINT", width=400, height=300, mesh_show_back_face=True)  # 显示`  
+
+
+
```

