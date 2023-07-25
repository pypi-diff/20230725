# Comparing `tmp/radtract-0.1.4.tar.gz` & `tmp/radtract-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radtract-0.1.4.tar", last modified: Fri May 26 08:20:21 2023, max compression
+gzip compressed data, was "radtract-0.1.6.tar", last modified: Tue Jul 25 14:23:26 2023, max compression
```

## Comparing `radtract-0.1.4.tar` & `radtract-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/LICENSES/
--rw-rw-r--   0 neher     (1000) neher     (1000)    10280 2023-05-24 07:39:53.000000 radtract-0.1.4/LICENSES/Apache-2.0.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)      154 2023-05-24 07:39:53.000000 radtract-0.1.4/MANIFEST.in
--rw-rw-r--   0 neher     (1000) neher     (1000)    15632 2023-05-26 08:20:21.110918 radtract-0.1.4/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)     4157 2023-05-26 08:18:16.000000 radtract-0.1.4/README.md
--rw-rw-r--   0 neher     (1000) neher     (1000)     1393 2023-05-26 08:11:23.000000 radtract-0.1.4/pyproject.toml
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/radtract/
--rw-rw-r--   0 neher     (1000) neher     (1000)      357 2023-05-26 08:11:23.000000 radtract-0.1.4/radtract/__init__.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    12193 2023-05-24 07:39:53.000000 radtract-0.1.4/radtract/features.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    22994 2023-05-24 10:34:33.000000 radtract-0.1.4/radtract/parcellation.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     3626 2023-05-24 07:39:53.000000 radtract-0.1.4/radtract/pyrad.yaml
--rw-rw-r--   0 neher     (1000) neher     (1000)     6925 2023-05-24 10:41:28.000000 radtract-0.1.4/radtract/tractdensity.py
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/radtract.egg-info/
--rw-rw-r--   0 neher     (1000) neher     (1000)    15632 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)      389 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/SOURCES.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/dependency_links.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)      152 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/entry_points.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)       77 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/requires.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        9 2023-05-26 08:20:21.000000 radtract-0.1.4/radtract.egg-info/top_level.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-05-26 08:20:21.110918 radtract-0.1.4/setup.cfg
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-05-26 08:20:21.110918 radtract-0.1.4/tests/
--rw-rw-r--   0 neher     (1000) neher     (1000)     4928 2023-05-26 08:11:23.000000 radtract-0.1.4/tests/test_radtract.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-07-25 14:23:26.554360 radtract-0.1.6/
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-07-25 14:23:26.550360 radtract-0.1.6/LICENSES/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    10280 2023-05-24 07:39:53.000000 radtract-0.1.6/LICENSES/Apache-2.0.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)      154 2023-05-24 07:39:53.000000 radtract-0.1.6/MANIFEST.in
+-rw-rw-r--   0 neher     (1000) neher     (1000)    15632 2023-07-25 14:23:26.554360 radtract-0.1.6/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)     4157 2023-05-26 08:18:16.000000 radtract-0.1.6/README.md
+-rw-rw-r--   0 neher     (1000) neher     (1000)     1393 2023-07-25 14:21:55.000000 radtract-0.1.6/pyproject.toml
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-07-25 14:23:26.554360 radtract-0.1.6/radtract/
+-rw-rw-r--   0 neher     (1000) neher     (1000)      357 2023-07-25 14:22:04.000000 radtract-0.1.6/radtract/__init__.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    12409 2023-07-25 14:06:35.000000 radtract-0.1.6/radtract/features.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    23631 2023-07-25 13:06:38.000000 radtract-0.1.6/radtract/parcellation.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3626 2023-05-24 07:39:53.000000 radtract-0.1.6/radtract/pyrad.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3570 2023-07-25 14:02:39.000000 radtract-0.1.6/radtract/pyrad_nofilter.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3578 2023-07-25 14:15:52.000000 radtract-0.1.6/radtract/pyrad_nofilter_D.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     7665 2023-05-30 10:44:51.000000 radtract-0.1.6/radtract/tractdensity.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-07-25 14:23:26.554360 radtract-0.1.6/radtract.egg-info/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    15632 2023-07-25 14:23:26.000000 radtract-0.1.6/radtract.egg-info/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)      449 2023-07-25 14:23:26.000000 radtract-0.1.6/radtract.egg-info/SOURCES.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        1 2023-07-25 14:23:26.000000 radtract-0.1.6/radtract.egg-info/dependency_links.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)      152 2023-07-25 14:23:26.000000 radtract-0.1.6/radtract.egg-info/entry_points.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)       77 2023-07-25 14:23:26.000000 radtract-0.1.6/radtract.egg-info/requires.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        9 2023-07-25 14:23:26.000000 radtract-0.1.6/radtract.egg-info/top_level.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)       38 2023-07-25 14:23:26.554360 radtract-0.1.6/setup.cfg
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2023-07-25 14:23:26.554360 radtract-0.1.6/tests/
+-rw-rw-r--   0 neher     (1000) neher     (1000)     4928 2023-05-26 08:11:23.000000 radtract-0.1.6/tests/test_radtract.py
```

### Comparing `radtract-0.1.4/LICENSES/Apache-2.0.txt` & `radtract-0.1.6/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `radtract-0.1.4/PKG-INFO` & `radtract-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radtract
-Version: 0.1.4
+Version: 0.1.6
 Summary: Radiomic Tractometry for advanced along-tract analysis of diffusion-weighted MRI
 Author-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 Maintainer-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
```

### Comparing `radtract-0.1.4/README.md` & `radtract-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `radtract-0.1.4/pyproject.toml` & `radtract-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "radtract"
-version = "0.1.4"
+version = "0.1.6"
 authors = [
   { name="Peter Neher", email="p.neher@dkfz-heidelberg.de" },
 ]
 maintainers = [
   { name="Peter Neher", email="p.neher@dkfz-heidelberg.de" },
 ]
```

### Comparing `radtract-0.1.4/radtract/features.py` & `radtract-0.1.6/radtract/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,33 +123,43 @@
             except Exception:
                 pass
 
     if out_csv_file is not None:
         if not out_csv_file.endswith('.csv'):
             out_csv_file += '.csv'
         print('pyradiomics saving results ...')
-        features = pd.DataFrame(features)
-        features.to_csv(out_csv_file, index=False)
+        features_df = pd.DataFrame(features)
+        features_df.to_csv(out_csv_file, index=False)
     print('pyradiomics finished processing')
 
     return features
 
 
 def calc_tractometry(point_label_file_name: str,
                      parameter_map_file_name: str,
                      out_csv_file: str,
+                     features: dict = None,
                      num_parcels: int = None):
     """
     Calculate tractometry features using points and corresponding parcel labels
     :param point_label_file_name:
     :param parameter_map_file_name:
     :param out_csv_file:
+    :param features: append new features to this dict, if none, create empty dict
     :param num_parcels: optional to ensure that all labels are present in the parcellation
     :return:
     """
+
+    if features is None:
+        features = dict()
+        features['map'] = []
+        features['parcellation'] = []
+        features['label'] = []
+        features['tractometry-mean'] = []
+
     streamline_point_parcels = joblib.load(point_label_file_name)
     map = nib.load(parameter_map_file_name)
     map_data = map.get_fdata()
     print('Calculating tractometry ...')
     points = apply_affine(np.linalg.inv(map.affine), streamline_point_parcels['points'])
     values = map_coordinates(map_data, points.T, order=1)
     vals_per_parcel = dict()
@@ -174,34 +184,29 @@
     #         text += '<point><id>' + str(i) + '</id><specification>0</specification>'
     #         text += '<x>' + str(p[0]) + '</x>'
     #         text += '<y>' + str(p[1]) + '</y>'
     #         text += '<z>' + str(p[2]) + '</z>'
     #         text += '</point>'
     #         i += 1
     #     text += '</time_series></point_set></point_set_file>'
-    #     with open(os.path.join(os.path.dirname(point_label_file_name), 'tractometry_centerline_points_' + str(parcel) + '.mps'), 'w') as f:
+    #     with open(os.path.join(os.path.dirname(point_label_file_name), 'tractometry_points_' + str(parcel) + '.mps'), 'w') as f:
     #         f.write(text)
 
-    features = dict()
-    features['map'] = []
-    features['parcellation'] = []
-    features['label'] = []
-    features['tractometry-mean'] = []
     for parcel in sorted(vals_per_parcel.keys()):
         features['map'].append(parameter_map_file_name)
         features['parcellation'].append(point_label_file_name)
         features['label'].append(parcel)
         features['tractometry-mean'].append(np.nanmean(vals_per_parcel[parcel]))
 
     if out_csv_file is not None:
         if not out_csv_file.endswith('.csv'):
             out_csv_file += '.csv'
         print('tractometry saving results ...')
-        features = pd.DataFrame(features)
-        features.to_csv(out_csv_file, index=False)
+        features_df = pd.DataFrame(features)
+        features_df.to_csv(out_csv_file, index=False)
     print('tractometry finished processing')
 
     return features
 
 
 def load_features(feature_file_names: list, feature_filter: str = None, expected_parcels: int = None):
     """
@@ -214,14 +219,15 @@
     out_df = None
     for feature_file_name in feature_file_names:
         feature_names = []
 
         feature_df = pd.read_csv(feature_file_name)
 
         parcels = feature_df['label'].tolist()
+        maps = feature_df['map'].tolist()
         if expected_parcels is not None and len(parcels) != expected_parcels:
             raise Exception('ERROR: Feature file does not contain ' + str(expected_parcels) + ' parcels:', feature_file_name)
 
         feature_df = feature_df.drop(columns=['map', 'parcellation', 'label'])
 
         col_list = [col for col in feature_df if not col.startswith('diagnostic')]
```

### Comparing `radtract-0.1.4/radtract/parcellation.py` & `radtract-0.1.6/radtract/parcellation.py`

 * *Files 4% similar despite different names*

```diff
@@ -302,15 +302,15 @@
     if type(start_region) is str and os.path.isfile(start_region):
         start_region = nib.load(start_region)
 
     assert type(streamlines) is nib.streamlines.array_sequence.ArraySequence, 'Streamlines must be in dipy format!'
     assert type(binary_envelope) is nib.Nifti1Image, 'Binary envelope must be Nifti1Image!'
     if start_region is not None:
         assert type(start_region) is nib.Nifti1Image, 'Start region must be Nifti1Image!'
-    assert parcellation_type in ['hyperplane', 'centerline'], 'Parcellation type must be hyperplane or centerline!'
+    assert parcellation_type in ['hyperplane', 'centerline', 'static_resampling'], 'Parcellation type must be hyperplane or centerline!'
 
     print('Input number of fibers:', len(streamlines))
     assert len(streamlines) > 0, 'No streamlines found!'
 
     if num_parcels is None:
         num_parcels = estimate_num_parcels(streamlines=streamlines, reference_image=binary_envelope)
 
@@ -458,14 +458,25 @@
                     if i not in check:
                         print('WARNING: empty parcel ' + str(i+1) + '. Adding corresponding centerline point to file ' + out_parcellation_filename)
                         streamline_point_parcels['parcels'] = np.append(streamline_point_parcels['parcels'], i+1)
                         streamline_point_parcels['points'] = np.append(streamline_point_parcels['points'], [centerline[i]], axis=0)
 
         print('Finished centerline-based parcellation')
 
+    elif num_parcels > 1 and parcellation_type == 'static_resampling' and streamline_space:
+        print('Creating static resampling-based parcellation')
+        envelope_data = None
+        resampled_streamlines = resample_streamlines(oriented_streamlines, nb_points=num_parcels)
+        streamline_point_parcels = dict()
+        streamline_point_parcels['points'] = []
+        streamline_point_parcels['parcels'] = []
+        for s in resampled_streamlines:
+            streamline_point_parcels['points'] += s.tolist()
+            streamline_point_parcels['parcels'] += np.arange(1, num_parcels + 1, 1).tolist()
+
     elif num_parcels == 1:
         print('Only 1 parcel requested, parcellation equals envelope.')
     else:
         print('Invalid parcellation type')
         envelope_data = None
 
     if postprocess and envelope_data is not None:
```

### Comparing `radtract-0.1.4/radtract/pyrad.yaml` & `radtract-0.1.6/radtract/pyrad.yaml`

 * *Files identical despite different names*

### Comparing `radtract-0.1.4/radtract/tractdensity.py` & `radtract-0.1.6/radtract/tractdensity.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,44 +94,49 @@
     :param do_closing: morphological closing of the binary image to remove holes
     :param out_image_filename: if not None, the output image will be saved to this file
     :return:
     """
     return tract_density(streamlines, reference_image, True, do_closing, out_image_filename)
 
 
-def tract_density(streamlines: nib.streamlines.array_sequence.ArraySequence,
-                  reference_image: nib.Nifti1Image,
-                  binary: bool = False,
-                  do_closing: bool = False,
-                  out_image_filename: str = None):
+def tract_density(streamlines: nib.streamlines.array_sequence.ArraySequence, # input streamlines
+                   reference_image: nib.Nifti1Image, # defines geometry of output image
+                   binary: bool = False, # if true, the output image will be a binary image with 1 for voxels that are part of the bundle and 0 outside
+                   do_closing: bool = False, # morphological closing of the binary image to remove holes
+                   out_image_filename: str = None): # if not None, the output image will be saved to this file
     """
     Calculate the tract density image for a set of streamlines using the true length of each streamline segment in each voxel.
     :param streamlines: input streamlines
     :param reference_image: defines geometry of output image
     :param binary: if true, the output image will be a binary image with 1 for voxels that are part of the bundle and 0 outside
     :param do_closing: morphological closing of the binary image to remove holes
     :param out_image_filename: if not None, the output image will be saved to this file
     :return:
     """
     if binary:
         print('Calculating bundle envelope')
     else:
         print('Calculating tract density image')
 
+    # Load streamlines and reference image if they are file paths
     if type(streamlines) is str:
         streamlines = load_trk_streamlines(streamlines)
     if type(reference_image) is str:
         reference_image = nib.load(reference_image)
 
+    # Create an empty image with the same dimensions as the reference image
     image_data = np.copy(reference_image.get_fdata())
     image_data.fill(0)
     affine = reference_image.affine
     spacing = reference_image.header['pixdim'][1:4]
+
+    # Transform streamlines to voxel space
     streamlines = transform_streamlines(streamlines, np.linalg.inv(affine))
 
+    # Loop over each streamline and calculate the intersection with the image
     for s in streamlines:
         num_points = len(s)
         for j in range(num_points-1):
             start_index_cont = s[j]
             start_index = np.round(start_index_cont).astype('int64')
 
             end_index_cont = s[j+1]
@@ -140,23 +145,29 @@
             segments = intersect_image(spacing, start_index, end_index, start_index_cont, end_index_cont)
             for seg in segments:
                 if binary:
                     image_data[seg[0][0], seg[0][1], seg[0][2]] = 1
                 else:
                     image_data[seg[0][0], seg[0][1], seg[0][2]] += seg[1]
 
+    # Perform morphological closing if binary and do_closing is True
     if binary and do_closing:
         image_data = binary_closing(image_data)
+
+    # Create Nifti1Image object with the image data
     if binary:
         image_data = image_data.astype('uint8')
         tdi = nib.Nifti1Image(image_data, header=reference_image.header, affine=reference_image.affine, dtype='uint8')
     else:
         tdi = nib.Nifti1Image(image_data, header=reference_image.header, affine=reference_image.affine)
+
+    # Save the image to file if out_image_filename is not None
     if out_image_filename is not None:
         nib.save(tdi, out_image_filename)
+
     print('done')
 
     return tdi
 
 
 def main():
     parser = argparse.ArgumentParser(description='RadTract Tract Density Image')
```

### Comparing `radtract-0.1.4/radtract.egg-info/PKG-INFO` & `radtract-0.1.6/radtract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radtract
-Version: 0.1.4
+Version: 0.1.6
 Summary: Radiomic Tractometry for advanced along-tract analysis of diffusion-weighted MRI
 Author-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 Maintainer-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
```

### Comparing `radtract-0.1.4/tests/test_radtract.py` & `radtract-0.1.6/tests/test_radtract.py`

 * *Files identical despite different names*

