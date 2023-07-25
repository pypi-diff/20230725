# Comparing `tmp/mapa-0.8.0.tar.gz` & `tmp/mapa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapa-0.8.0.tar", max compression
+gzip compressed data, was "mapa-0.9.0.tar", max compression
```

## Comparing `mapa-0.8.0.tar` & `mapa-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1071 2022-04-07 18:27:46.318665 mapa-0.8.0/LICENSE
--rw-r--r--   0        0        0     5986 2022-04-07 18:27:46.322665 mapa-0.8.0/README.md
--rw-r--r--   0        0        0     8159 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/__init__.py
--rw-r--r--   0        0        0    22107 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/algorithm.py
--rw-r--r--   0        0        0      325 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/caching.py
--rw-r--r--   0        0        0     3286 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/cli.py
--rw-r--r--   0        0        0      487 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/conf.py
--rw-r--r--   0        0        0       43 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/exceptions.py
--rw-r--r--   0        0        0      776 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/map.py
--rw-r--r--   0        0        0     6565 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/mapa.ipynb
--rw-r--r--   0        0        0     4896 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/raster.py
--rw-r--r--   0        0        0     2022 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/stac.py
--rw-r--r--   0        0        0     1332 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/stl_file.py
--rw-r--r--   0        0        0      438 2022-04-07 18:27:46.322665 mapa-0.8.0/mapa/utils.py
--rw-r--r--   0        0        0     1251 2022-04-07 18:27:46.322665 mapa-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7144 2022-04-07 18:27:58.660025 mapa-0.8.0/setup.py
--rw-r--r--   0        0        0     7086 2022-04-07 18:27:58.660906 mapa-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-04-24 20:11:32.488009 mapa-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5986 2022-04-24 20:11:32.488009 mapa-0.9.0/README.md
+-rw-r--r--   0        0        0    10002 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/__init__.py
+-rw-r--r--   0        0        0    21668 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/algorithm.py
+-rw-r--r--   0        0        0      323 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/caching.py
+-rw-r--r--   0        0        0     3286 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/cli.py
+-rw-r--r--   0        0        0      487 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/conf.py
+-rw-r--r--   0        0        0       43 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/exceptions.py
+-rw-r--r--   0        0        0      776 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/map.py
+-rw-r--r--   0        0        0     7674 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/mapa.ipynb
+-rw-r--r--   0        0        0     4895 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/raster.py
+-rw-r--r--   0        0        0     2053 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/stac.py
+-rw-r--r--   0        0        0     1420 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/stl_file.py
+-rw-r--r--   0        0        0     1111 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/tiling.py
+-rw-r--r--   0        0        0     1117 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/utils.py
+-rw-r--r--   0        0        0     1029 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/verification.py
+-rw-r--r--   0        0        0      673 2022-04-24 20:11:32.488009 mapa-0.9.0/mapa/zip.py
+-rw-r--r--   0        0        0     1251 2022-04-24 20:11:32.488009 mapa-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7144 2022-04-24 20:11:39.934291 mapa-0.9.0/setup.py
+-rw-r--r--   0        0        0     7086 2022-04-24 20:11:39.934960 mapa-0.9.0/PKG-INFO
```

### Comparing `mapa-0.8.0/LICENSE` & `mapa-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapa-0.8.0/README.md` & `mapa-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mapa-0.8.0/mapa/__init__.py` & `mapa-0.9.0/mapa/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,215 +1,245 @@
 import logging
 import os
 from pathlib import Path
-from typing import Union
+from typing import List, Union
 
 import numpy as np
 import rasterio as rio
 
 from mapa import conf
-from mapa.algorithm import compute_all_triangles, reduce_resolution
+from mapa.algorithm import ModelSize, compute_all_triangles, reduce_resolution
 from mapa.caching import get_hash_of_geojson, tiff_for_bbox_is_cached
 from mapa.raster import (
     clip_tiff_to_bbox,
     cut_array_to_format,
     determine_elevation_scale,
     merge_tiffs,
     remove_empty_first_and_last_rows_and_cols,
+    tiff_to_array,
 )
 from mapa.stac import fetch_stac_items_for_bbox
 from mapa.stl_file import save_to_stl_file
-from mapa.utils import _path_to_clipped_tiff
+from mapa.tiling import get_x_y_from_tiles_format, split_array_into_tiles
+from mapa.utils import ProgressBar, path_to_clipped_tiff
+from mapa.verification import verify_input_and_output_are_valid
+from mapa.zip import create_zip_archive
 
 log = logging.getLogger(__name__)
 logging.basicConfig()
 log.setLevel(os.getenv("MAPA_LOG_LEVEL", "INFO"))
 
 
-def _verify_input_is_valid(input: str):
-    input_path = Path(input)
-    if not input_path.is_file():
-        raise FileNotFoundError(f"input file: '{input}' does not seem to be a file")
-    if input_path.suffix in conf.SUPPORTED_INPUT_FORMAT:
-        pass  # ok
-    else:
-        raise IOError(
-            f"input file '{input}' does not seem to be a tiff file, only {conf.SUPPORTED_INPUT_FORMAT} are supported."
-        )
-
-
-def _verify_output_is_valid(output: str):
-    output_path = Path(output)
-    if not output_path.parent.is_dir():
-        raise FileNotFoundError(
-            f"parent directory of output file '{output_path.parent}' does not seem to be a valid directory."
-        )
-
-
 def convert_array_to_stl(
     array: np.ndarray,
     as_ascii: bool,
-    model_size: int,
+    desired_size: ModelSize,
     max_res: bool,
-    z_offset: float,
+    z_offset: Union[None, float],
     z_scale: float,
-    cut_to_format_ratio: Union[None, float],
     elevation_scale: float,
     output_file: Path,
 ) -> Path:
-    # drop higher dimension to get 2-dimensional (x * y) array
-    array = array[0, :, :]
     x, y = array.shape
     # when merging tiffs, sometimes an empty row/col is added, which should be dropped (in case the array size suffices)
     if x > 1 and y > 1:
         array = remove_empty_first_and_last_rows_and_cols(array)
-    if cut_to_format_ratio:
-        array = cut_array_to_format(array, cut_to_format_ratio)
 
     if max_res:
         if x * y > conf.PERFORMANCE_WARNING_THRESHOLD:
             log.warning(
                 "⛔️  Warning: Using max_res=True on the given bounding box might consume a lot of time and memory. "
                 "Consider setting max_res=False."
             )
     else:
         bin_fac = round((x / conf.MAXIMUM_RESOLUTION + y / conf.MAXIMUM_RESOLUTION) / 2)
         if bin_fac > 1:
             log.debug("🔍  reducing image resolution...")
             array = reduce_resolution(array, bin_factor=bin_fac)
 
-    triangles = compute_all_triangles(array, model_size, z_offset, z_scale, elevation_scale, cut_to_format_ratio)
+    triangles = compute_all_triangles(array, desired_size, z_offset, z_scale, elevation_scale)
     log.debug("💾  saving data to stl file...")
 
     output_file = save_to_stl_file(triangles, output_file, as_ascii)
-    log.info(f"🎉  successfully generated STL file: {Path(output_file).absolute()}\n")
+    log.info(f"🎉  successfully generated STL file: {Path(output_file).absolute()}")
     return Path(output_file)
 
 
+def _get_desired_size(array: np.ndarray, x: float, y: float, cut_to_format_ratio: Union[None, float]) -> ModelSize:
+    if cut_to_format_ratio:
+        return ModelSize(x=x, y=y * cut_to_format_ratio)
+    else:
+        rows, cols = array.shape
+        return ModelSize(x=x, y=y / rows * cols)
+
+
 def convert_tiff_to_stl(
     input_file: str,
     as_ascii: bool,
     model_size: int,
     output_file: Union[str, None],
     max_res: bool,
-    z_offset: float,
+    z_offset: Union[None, float],
     z_scale: float,
     cut_to_format_ratio: Union[None, float],
 ) -> Path:
 
-    _verify_input_is_valid(input_file)
-    if output_file is None:
-        output_file = Path.home() / str(Path(input_file).name).replace(".tiff", ".stl").replace(".tif", ".stl")
-    _verify_output_is_valid(output_file)
+    output_file = verify_input_and_output_are_valid(input=input_file, output=output_file)
 
     tiff = rio.open(input_file)
     elevation_scale = determine_elevation_scale(tiff, model_size)
-    array = tiff.read()
+    array = tiff_to_array(tiff)
+
+    if cut_to_format_ratio:
+        array = cut_array_to_format(array, cut_to_format_ratio)
+    desired_size = _get_desired_size(array=array, x=model_size, y=model_size, cut_to_format_ratio=cut_to_format_ratio)
 
     return convert_array_to_stl(
         array=array,
         as_ascii=as_ascii,
-        model_size=model_size,
+        desired_size=desired_size,
         max_res=max_res,
         z_offset=z_offset,
         z_scale=z_scale,
-        cut_to_format_ratio=cut_to_format_ratio,
         elevation_scale=elevation_scale,
         output_file=output_file,
     )
 
 
 def _fetch_merge_and_clip_tiffs(
     bbox_geojson: dict,
     bbox_hash: str,
     allow_caching: bool,
-    progress_bar: Union[None, object] = None,
+    progress_bar: Union[None, ProgressBar] = None,
 ) -> Path:
     tiffs = fetch_stac_items_for_bbox(bbox_geojson, allow_caching, progress_bar)
     if len(tiffs) > 1:
         merged_tiff = merge_tiffs(tiffs, bbox_hash)
     else:
         merged_tiff = tiffs[0]
     return clip_tiff_to_bbox(merged_tiff, bbox_geojson, bbox_hash)
 
 
-def _get_tiff_for_bbox(bbox_geojson: dict, allow_caching: bool, progress_bar: Union[None, object] = None) -> Path:
+def _get_tiff_for_bbox(bbox_geojson: dict, allow_caching: bool, progress_bar: Union[None, ProgressBar] = None) -> Path:
     bbox_hash = get_hash_of_geojson(bbox_geojson)
     if tiff_for_bbox_is_cached(bbox_hash) and allow_caching:
         log.info("🚀  using cached tiff!")
-        return _path_to_clipped_tiff(bbox_hash)
+        return path_to_clipped_tiff(bbox_hash)
     else:
         return _fetch_merge_and_clip_tiffs(bbox_geojson, bbox_hash, allow_caching, progress_bar)
 
 
 def convert_bbox_to_stl(
     bbox_geometry: dict,
     as_ascii: bool = False,
     model_size: int = 200,
-    output_file: str = "output.stl",
+    output_file: str = "output",
     max_res: bool = False,
-    z_offset: float = 0.0,
+    z_offset: Union[None, float] = 0.0,
     z_scale: float = 1.0,
     cut_to_format_ratio: Union[None, float] = None,
+    split_area_in_tiles: str = "1x1",
+    compress: bool = True,
     allow_caching: bool = True,
     progress_bar: Union[None, object] = None,
-) -> Path:
+) -> Union[Path, List[Path]]:
     """
     Takes a GeoJSON containing a bounding box as input, fetches the required STAC GeoTIFFs for the
     given bounding box and creates a STL file with elevation data from the GeoTIFFs.
 
     Parameters
     ----------
     bbox_geometry : dict
-        GeoJSON containing the coordinates of the bounding box, selected on the ipyleaflet widget.
-        Usually the value of `drawer.last_draw["geometry"]` is used for this.
+        GeoJSON containing the coordinates of the bounding box, selected on the ipyleaflet widget. Usually the
+        value of `drawer.last_draw["geometry"]` is used for this.
     as_ascii : bool, optional
         Save output STL as ascii file. If False, output file will be binary. By default False
     model_size : int, optional
         Desired size of the (larger side of the) generated 3d model in millimeter. By default 200
     output_file : str, optional
-        Path to output STL file. By default "output.stl"
+        Name and path to output file. File ending should not be provided. Mapa will add .zip or .stl depending
+        on the settings. By default "output"
     max_res : bool, optional
         Whether maximum resolution should be used. Note, that this flag potentially increases compute time
         and memory consumption dramatically. The default behavior (i.e. max_res=False) should return 3d models
         with sufficient resolution, while the output stl file should be < ~300 MB. By default False
-    z_offset : float, optional
+    z_offset : Union[None, float], optional
         Offset distance in millimeter to be put below the 3d model. Is not influenced by z-scale. Set to None
         if you want your model to have the natural offset, corresponding to height above mean sea level.
         By default 0.0
     z_scale : float, optional
-        Value to be multiplied to the z-axis elevation data to scale up the height of the model.
-        By default 1.0
+        Value to be multiplied to the z-axis elevation data to scale up the height of the model. By default 1.0
     cut_to_format_ratio : Union[None, float], optional
         Cut the input tiff file to a specified format. Set to `1` if you want the output model to be squared.
         Set to `0.5` if you want one side to be half the length of the other side. Omit this flag to keep the
         input format. This option is particularly useful when an exact output format ratio is required for
         example when planning to put the 3d printed model into a picture frame. Using this option will always
         try to cut the shorter side of the input tiff. By default None
+    split_area_in_tiles : str, optional
+        Split the selected bounding box into tiles with this option. The allowed format of a given string is
+        "n*m" e.g. "1*1`, "2*3", "4*4" or similar, where "1*1" would not split at all and result in only
+        one stl file. If an allowed tile format is specified, `n*m` stl files will be computed. By default "1*1"
+    compress : bool, optional
+        If enabled, the output stl file(s) will be compressed to a zip file. Compressing is recommended as it
+        reduces the data volume of typical stl files by a factor of ~4.
     allow_caching : bool, optional
         Whether caching previous downloaded GeoTIFF files should be enabled/disabled. By default True
     progress_bar : Union[None, object], optional
-        A streamlit progress bar object can be used to indicate the progress of downloading the STAC items.
+        A streamlit progress bar object can be used to indicate the progress of downloading the STAC items. By
+        default None
 
     Returns
     -------
-    Path
-        Path to the resulting STL file on your local machine.
+    Union[Path, List[Path]]
+        Path or list of paths to the resulting output file(s) on your local machine.
     """
 
+    # fail early in case of missing requirements
     if bbox_geometry is None:
-        log.error("⛔️  ERROR: make sure to draw a rectangle on the map first!")
-        return
+        raise ValueError("⛔️  ERROR: make sure to draw a rectangle on the map first!")
 
-    log.info(f"⏳  converting bounding box to STL file with arguments: {locals()}")
-    tiff = _get_tiff_for_bbox(bbox_geometry, allow_caching, progress_bar)
-    output_file = convert_tiff_to_stl(
-        input_file=tiff,
-        as_ascii=as_ascii,
-        model_size=model_size,
-        output_file=output_file,
-        max_res=max_res,
-        z_offset=z_offset,
-        z_scale=z_scale,
+    # evaluate tile format to fail early in case of invalid input value
+    tiles = get_x_y_from_tiles_format(split_area_in_tiles)
+
+    args = locals().copy()
+    args.pop("progress_bar", None)
+    log.info(f"⏳  converting bounding box to STL file with arguments: {args}")
+
+    if progress_bar:
+        steps = tiles.x * tiles.y * 2 if compress else tiles.x * tiles.y
+        progress_bar = ProgressBar(progress_bar=progress_bar, steps=steps)
+
+    path_to_tiff = _get_tiff_for_bbox(bbox_geometry, allow_caching, progress_bar)
+    tiff = rio.open(path_to_tiff)
+    elevation_scale = determine_elevation_scale(tiff, model_size)
+    array = tiff_to_array(tiff)
+    if cut_to_format_ratio:
+        array = cut_array_to_format(array, cut_to_format_ratio)
+
+    desired_size = _get_desired_size(
+        array=array,
+        x=model_size / tiles.x,
+        y=model_size / tiles.y,
         cut_to_format_ratio=cut_to_format_ratio,
     )
-    return output_file
+
+    tiled_arrays = split_array_into_tiles(array, tiles)
+    stl_files = []
+    for i, array in enumerate(tiled_arrays):
+        stl_files.append(
+            convert_array_to_stl(
+                array=array,
+                as_ascii=as_ascii,
+                desired_size=desired_size,
+                max_res=max_res,
+                z_offset=z_offset,
+                z_scale=z_scale,
+                elevation_scale=elevation_scale,
+                output_file=f"{output_file}_{i+1}.stl" if len(tiled_arrays) > 1 else f"{output_file}.stl",
+            )
+        )
+        if progress_bar:
+            progress_bar.step()
+    if compress:
+        return create_zip_archive(files=stl_files, output_file=f"{output_file}.zip", progress_bar=progress_bar)
+    else:
+        return stl_files[0] if len(stl_files) == 1 else stl_files
```

### Comparing `mapa-0.8.0/mapa/algorithm.py` & `mapa-0.9.0/mapa/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,26 +109,32 @@
 ------------------------------
 
 This is not considered part of the algorithm and is taken care of by `mapa/__init__._save_to_stl_file`. It boils down to
 the usage of numpy-stl, which has a super convenient and efficient interface for writing triangles to a (binary of ascii)
 STL file.
 """
 
-
 import logging
-from typing import Tuple, Union
+from dataclasses import dataclass
+from typing import Union
 
 import numba as nb
 import numpy as np
 import numpy.typing as npt
 from numpy.lib.stride_tricks import as_strided
 
 log = logging.getLogger(__name__)
 
 
+@dataclass
+class ModelSize:
+    x: float
+    y: float
+
+
 @nb.njit(fastmath=True, cache=True)
 def _create_raster(array: npt.ArrayLike, max_x: int, max_y: int) -> np.ndarray:
     max_x, max_y = array.shape
     raster = np.zeros((max_x + 1, max_y + 1))
     # loop over raster elements to determine z value of raster elements
     for ix in range(0, raster.shape[0]):
         for iy in range(0, raster.shape[1]):
@@ -421,52 +427,39 @@
     center_triangles[1, 2, 0] = 0 * x_scale
     center_triangles[1, 2, 1] = 1 * y_scale
     center_triangles[1, 2, 2] = 0
 
     return np.vstack((fr_triangles, lr_triangles, fc_triangles, lc_triangles, center_triangles))
 
 
-def _determine_x_y_scales(target_size: int, max_x: int, max_y: int, cut_to_format_ratio: float) -> Tuple[float, float]:
-    x_scale = target_size / max_x
-    if cut_to_format_ratio:
-        if cut_to_format_ratio > 1.0:
-            # ensure ratio is between 0.0 and 1.0 and transpose ratio
-            cut_to_format_ratio = cut_to_format_ratio**-1
-        y_scale = target_size * cut_to_format_ratio / max_y
-    else:
-        y_scale = target_size / max_x
-    return x_scale, y_scale
-
-
-def _determine_z_offset(z_offset: float, minimum: float, elevation_scale: float) -> float:
+def _determine_z_offset(z_offset: Union[None, float], minimum: float, elevation_scale: float) -> float:
     if z_offset is None:
         # using the natural height, i.e. islands will have an z_offset of ~0 and mountains will have a larger z_offset
         return minimum * elevation_scale
     else:
         if z_offset < 0:
             log.warning("☝️  Warning: Be careful using negative z_offsets, as it might break your 3D model.")
         # subtract scaled minimum from z_offset to ensure the input z_offset will remain
         return z_offset - minimum * elevation_scale
 
 
 def compute_all_triangles(
     array: npt.ArrayLike,
-    target_size: int,
-    z_offset: float,
+    desired_size: ModelSize,
+    z_offset: Union[None, float],
     z_scale: float,
     elevation_scale: float,
-    cut_to_format_ratio: Union[float, None],
 ) -> np.ndarray:
 
     max_x, max_y = array.shape
 
     log.debug("🗺  creating base raster for tiff...")
     raster = _create_raster(array, max_x, max_y)
 
-    x_scale, y_scale = _determine_x_y_scales(target_size, max_x, max_y, cut_to_format_ratio)
+    x_scale, y_scale = desired_size.x / max_x, desired_size.y / max_y
     z_offset = _determine_z_offset(z_offset, raster.min(), elevation_scale)
     combined_z_scale = elevation_scale * z_scale
 
     # compute triangles for 3d surface, sides and bottom
     log.debug("⛰  computing triangles of 3d surface...")
     dem_triangles = _compute_triangles_of_3d_surface(
         raster=raster,
```

### Comparing `mapa-0.8.0/mapa/cli.py` & `mapa-0.9.0/mapa/cli.py`

 * *Files identical despite different names*

### Comparing `mapa-0.8.0/mapa/map.py` & `mapa-0.9.0/mapa/map.py`

 * *Files identical despite different names*

### Comparing `mapa-0.8.0/mapa/mapa.ipynb` & `mapa-0.9.0/mapa/mapa.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992760257202438%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'data': {'application/vnd.jupyter.widget-view+json': "*

 * *            "{'model_id': '3b4e99a39be34a15acd39c6ecaaa0abc'}}}}}, 4: {'execution_count': 7, "*

 * *            '\'outputs\': {0: {\'name\': \'stderr\', \'text\': ["INFO:mapa:⏳  converting bounding '*

 * *            "box to STL file with arguments: {'bbox_geometry': {'type': 'Polygon', 'coordinates': "*

 * *            '[[[-3.317262, 41.013549], [-3.317262, 41.183271], [-3.190925, 41.183271], [-3.190925, '*

 * *            "41.013549], [- […]*

```diff
@@ -28,15 +28,15 @@
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "5548cc169d75427eaefa57f4eee343de",
+                            "model_id": "3b4e99a39be34a15acd39c6ecaaa0abc",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Map(center=[40.5566, 23.466], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoo\u2026"
                         ]
                     },
@@ -62,50 +62,43 @@
             "metadata": {},
             "source": [
                 "\u26a0\ufe0f First draw a rectangle on the above map before executing the next cell!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 7,
             "id": "39c8fef3",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
-                    "name": "stdout",
+                    "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "\u23f3  converting bounding box to STL file... \n",
-                        "\n",
-                        "\u2b07\ufe0f  fetching 2 stac items...\n",
-                        "\ud83c\udfde  downloading stac item ALPSMLC30_N046E008_DSM   \u2705 (6.4s)            \n",
-                        "\ud83c\udfde  downloading stac item ALPSMLC30_N046E007_DSM   \u2705 (5.0s)            \n",
-                        "\ud83d\udd2a  clipping region of interest...                 \u2705 (0.1s)            \n",
-                        "\ud83d\uddfa  creating base raster for tiff...               \u2705 (0.8s)            \n",
-                        "\u26f0  computing triangles of 3d surface...           \u2705 (1.5s)            \n",
-                        "\ud83d\udcd0  computing triangles of body sides...           \u2705 (0.2s)            \n",
-                        "\ud83d\udcbe  saving data to stl file...                     \u2705 (0.9s)            \n",
-                        "\n",
-                        "\ud83c\udf89  successfully generated STL file: /home/fabian/make/mapa/mapa/output.stl\n"
+                        "INFO:mapa:\u23f3  converting bounding box to STL file with arguments: {'bbox_geometry': {'type': 'Polygon', 'coordinates': [[[-3.317262, 41.013549], [-3.317262, 41.183271], [-3.190925, 41.183271], [-3.190925, 41.013549], [-3.317262, 41.013549]]]}, 'as_ascii': False, 'model_size': 200, 'output_file': 'mapa_output', 'max_res': False, 'z_offset': 3.0, 'z_scale': 2.0, 'cut_to_format_ratio': None, 'split_area_in_tiles': '1*1', 'compress': True, 'allow_caching': True}\n",
+                        "INFO:mapa:\ud83d\ude80  using cached tiff!\n",
+                        "INFO:mapa:\ud83c\udf89  successfully generated STL file: /Users/ppqw/dev/geospacial/mapa/mapa/mapa_output.stl\n",
+                        "INFO:mapa.zip:\ud83d\udce6  compressing stl files: ['mapa_output.stl']\n",
+                        "INFO:mapa.zip:\u2705  finished compressing STL files into: mapa_output.zip\n"
                     ]
                 }
             ],
             "source": [
-                "stl_file_name = \"output.stl\"\n",
-                "\n",
                 "path = convert_bbox_to_stl(\n",
                 "    bbox_geometry=drawer.last_draw[\"geometry\"],\n",
-                "    output_file=stl_file_name,\n",
+                "    output_file=\"mapa_output\",\n",
                 "    model_size=200,\n",
                 "    z_offset=3.0,\n",
                 "    z_scale=2.0,\n",
                 "    max_res=False,\n",
                 "    cut_to_format_ratio=None,\n",
+                "    split_area_in_tiles=\"1*1\",\n",
+                "    compress=True,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d29e1ade",
             "metadata": {},
@@ -116,72 +109,82 @@
                 "<br>\n",
                 "\n",
                 "For more info on the available arguments, simply print the function docstrings:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "id": "cd7e9b13",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "    Takes a GeoJSON containing a bounding box as input, fetches the required STAC GeoTIFFs for the\n",
                         "    given bounding box and creates a STL file with elevation data from the GeoTIFFs.\n",
                         "\n",
                         "    Parameters\n",
                         "    ----------\n",
                         "    bbox_geometry : dict\n",
-                        "        GeoJSON containing the coordinates of the bounding box, selected on the ipyleaflet widget.\n",
-                        "        Usually the value of `drawer.last_draw[\"geometry\"]` is used for this.\n",
+                        "        GeoJSON containing the coordinates of the bounding box, selected on the ipyleaflet widget. Usually the\n",
+                        "        value of `drawer.last_draw[\"geometry\"]` is used for this.\n",
                         "    as_ascii : bool, optional\n",
                         "        Save output STL as ascii file. If False, output file will be binary. By default False\n",
                         "    model_size : int, optional\n",
                         "        Desired size of the (larger side of the) generated 3d model in millimeter. By default 200\n",
                         "    output_file : str, optional\n",
-                        "        Path to output STL file. By default \"output.stl\"\n",
+                        "        Name and path to output file. File ending should not be provided. Mapa will add .zip or .stl depending\n",
+                        "        on the settings. By default \"output\"\n",
                         "    max_res : bool, optional\n",
                         "        Whether maximum resolution should be used. Note, that this flag potentially increases compute time\n",
                         "        and memory consumption dramatically. The default behavior (i.e. max_res=False) should return 3d models\n",
                         "        with sufficient resolution, while the output stl file should be < ~300 MB. By default False\n",
-                        "    z_offset : float, optional\n",
-                        "        Offset distance in millimeter to be put below the 3d model. Is not influenced by z-scale.\n",
+                        "    z_offset : Union[None, float], optional\n",
+                        "        Offset distance in millimeter to be put below the 3d model. Is not influenced by z-scale. Set to None\n",
+                        "        if you want your model to have the natural offset, corresponding to height above mean sea level.\n",
                         "        By default 0.0\n",
                         "    z_scale : float, optional\n",
-                        "        Value to be multiplied to the z-axis elevation data to scale up the height of the model.\n",
-                        "        By default 1.0\n",
+                        "        Value to be multiplied to the z-axis elevation data to scale up the height of the model. By default 1.0\n",
                         "    cut_to_format_ratio : Union[None, float], optional\n",
                         "        Cut the input tiff file to a specified format. Set to `1` if you want the output model to be squared.\n",
                         "        Set to `0.5` if you want one side to be half the length of the other side. Omit this flag to keep the\n",
                         "        input format. This option is particularly useful when an exact output format ratio is required for\n",
                         "        example when planning to put the 3d printed model into a picture frame. Using this option will always\n",
                         "        try to cut the shorter side of the input tiff. By default None\n",
+                        "    split_area_in_tiles: str, optional\n",
+                        "        Split the selected bounding box into tiles with this option. The allowed format of a given string is\n",
+                        "        \"n*m\" e.g. \"1*1`, \"2*3\", \"4*4\" or similar, where \"1*1\" would not split at all and result in only\n",
+                        "        one stl file. If an allowed tile format is specified, `n*m` stl files will be computed. By default \"1*1\"\n",
+                        "    compress: bool, optional\n",
+                        "        If enabled, the output stl file(s) will be compressed to a zip file. Compressing is recommended as it\n",
+                        "        reduces the data volume of typical stl files by a factor of ~4.\n",
                         "    allow_caching : bool, optional\n",
                         "        Whether caching previous downloaded GeoTIFF files should be enabled/disabled. By default True\n",
+                        "    progress_bar : Union[None, object], optional\n",
+                        "        A streamlit progress bar object can be used to indicate the progress of downloading the STAC items.\n",
                         "\n",
                         "    Returns\n",
                         "    -------\n",
-                        "    Path\n",
-                        "        Path to the resulting STL file on your local machine.\n",
+                        "    Union[Path, List[Path]]\n",
+                        "        Path or list of paths to the resulting output file(s) on your local machine.\n",
                         "    \n"
                     ]
                 }
             ],
             "source": [
                 "print(convert_bbox_to_stl.__doc__)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "954f9732",
+            "id": "551ff015",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -195,13 +198,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.8.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mapa-0.8.0/mapa/raster.py` & `mapa-0.9.0/mapa/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import rasterio as rio
 from haversine import haversine
 from rasterio.io import DatasetReader
 from rasterio.mask import mask
 from rasterio.merge import merge
 from rasterio.windows import Window
 
-from mapa.utils import _path_to_clipped_tiff, _path_to_merged_tiff
+from mapa.utils import path_to_clipped_tiff, path_to_merged_tiff
 
 log = logging.getLogger(__name__)
 
 
 def clip_tiff_to_bbox(input_tiff: Path, bbox_geometry: dict, bbox_hash: str) -> Path:
     log.debug("🔪  clipping region of interest...")
     data = rio.open(input_tiff)
@@ -26,22 +26,22 @@
             "driver": "GTiff",
             "height": out_img.shape[1],
             "width": out_img.shape[2],
             "transform": out_transform,
             "crs": data.crs,
         }
     )
-    clipped_tiff = _path_to_clipped_tiff(bbox_hash)
+    clipped_tiff = path_to_clipped_tiff(bbox_hash)
     with rio.open(clipped_tiff, "w", **out_meta) as file:
         file.write(out_img)
     return clipped_tiff
 
 
-def read_tiff(path: Path) -> np.ndarray:
-    array = rio.open(path).read()
+def tiff_to_array(tiff: DatasetReader) -> np.ndarray:
+    array = tiff.read()
     # drop higher dimension to get 2-dimensional (x * y) array
     return array[0, :, :]
 
 
 def remove_empty_first_and_last_rows_and_cols(array: npt.ArrayLike) -> np.ndarray:
     # remove first and last cols in case of all zero
     if not array[:, 0].any():
@@ -136,11 +136,11 @@
             "driver": "GTiff",
             "height": mosaic.shape[1],
             "width": mosaic.shape[2],
             "transform": out_trans,
             "crs": data.crs,
         }
     )
-    tiff = _path_to_merged_tiff(bbox_hash)
+    tiff = path_to_merged_tiff(bbox_hash)
     with rio.open(tiff, "w", **out_meta) as dest:
         dest.write(mosaic)
     return tiff
```

### Comparing `mapa-0.8.0/mapa/stac.py` & `mapa-0.9.0/mapa/stac.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import geojson
 from pystac.item import Item
 from pystac_client import Client
 
 from mapa import conf
 from mapa.exceptions import NoSTACItemFound
-from mapa.utils import TMPDIR
+from mapa.utils import TMPDIR, ProgressBar
 
 log = logging.getLogger(__name__)
 
 
 def _download_file(url: str, local_file: Path) -> Path:
     request.urlretrieve(url, local_file)
     return local_file
@@ -39,24 +39,26 @@
         return tiff
     else:
         log.info(f"🏞  downloading stac item {stac_item.id}")
         return _download_file(stac_item.assets["data"].href, tiff)
 
 
 def fetch_stac_items_for_bbox(
-    geojson: dict, allow_caching: bool, progress_bar: Union[None, object] = None
+    geojson: dict, allow_caching: bool, progress_bar: Union[None, ProgressBar] = None
 ) -> List[Path]:
     bbox = _turn_geojson_into_bbox(geojson)
     client = Client.open(conf.PLANETARY_COMPUTER_API_URL, ignore_conformance=True)
     search = client.search(collections=[conf.PLANETARY_COMPUTER_COLLECTION], bbox=bbox)
     items = list(search.get_items())
     n = len(items)
+    if progress_bar:
+        progress_bar.steps += n
     if n > 0:
         log.info(f"⬇️  fetching {n} stac items...")
         files = []
-        for i, item in enumerate(items):
+        for item in items:
             files.append(_get_tiff_file(item, allow_caching))
             if progress_bar:
-                progress_bar.progress(int(100 / n * (i + 1)))
+                progress_bar.step()
         return files
     else:
         raise NoSTACItemFound("Could not find the desired STAC item for the given bounding box.")
```

### Comparing `mapa-0.8.0/mapa/stl_file.py` & `mapa-0.9.0/mapa/stl_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,9 +35,10 @@
     x = maxx - minx
     y = maxy - miny
     z = maxz - minz
     return x, y, z
 
 
 def get_dimensions_of_stl_file(stl_path: Path) -> Tuple[float]:
+    assert Path(stl_path).suffix == ".stl", "can compute dimensions of stl files only!"
     main_body = mesh.Mesh.from_file(stl_path)
     return _find_dimensions_of_mesh(main_body)
```

### Comparing `mapa-0.8.0/pyproject.toml` & `mapa-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mapa"
-version = "0.8.0"
+version = "0.9.0"
 description = "🌍 Create 3d-printable STLs from satellite elevation data 🌏"
 authors = ["Fabian Gebhart"]
 repository = "https://github.com/fgebhart/mapa"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `mapa-0.8.0/setup.py` & `mapa-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'rasterio>=1.2.10,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['dem2stl = mapa.cli:dem2stl', 'mapa = mapa.cli:mapa']}
 
 setup_kwargs = {
     'name': 'mapa',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': '🌍 Create 3d-printable STLs from satellite elevation data 🌏',
     'long_description': '# mapa 🌍\n\n[![PyPI](https://badge.fury.io/py/mapa.svg)](https://badge.fury.io/py/mapa)\n[![Python](https://img.shields.io/pypi/pyversions/mapa.svg?style=plastic)](https://badge.fury.io/py/mapa)\n[![Downloads](https://pepy.tech/badge/mapa/month)](https://pepy.tech/project/mapa)\n[![Python Tests](https://github.com/fgebhart/mapa/actions/workflows/test.yml/badge.svg)](https://github.com/fgebhart/mapa/actions/workflows/test.yml)\n\n`mapa` let\'s you create 3d-printable [STL](https://en.wikipedia.org/wiki/STL_(file_format)) files from satellite\nelevation data (using [DEM](https://en.wikipedia.org/wiki/Digital_elevation_model) data).\n\nUnder the hood `mapa` uses:\n* [numpy](https://numpy.org/) and [numba](https://numba.pydata.org/) to crunch large amounts of data in little time\n* [ALOS DEM](https://planetarycomputer.microsoft.com/dataset/alos-dem) satellite data (max resolution of 30m) provided by\n  [Planetary Computer](https://planetarycomputer.microsoft.com/)\n\n\n## Installation\n```\npip install mapa\n```\n\n## Usage\n`mapa` provides the following approaches for creating STL files:\n\n### 1. Using the `mapa` streamlit web app 🎈\nCertainly the easiest way to interact with `mapa` is to use the streamlit web app. No need to install anything. Simply\naccess it via your browser. It is based on the [mapa-streamlit repo](https://github.com/fgebhart/mapa-streamlit) and can\nbe accessed at:\n\nhttps://share.streamlit.io/fgebhart/mapa-streamlit/main/app.py\n\nNote, that the streamlit web app however, does not use the maximal available resolution of the ALOS DEM GeoTIFFs, as it\nwould take too much time and cloud resources to compute STL files of e.g. multiple GBs. If you are keen in getting STL\nfiles with the highest resolution possible, I\'d recommend following the next step.\n\n### 2. Using the `mapa` interactive map 🗺\nThe second easiest way is using the `mapa` cli. After installing `mapa`, simply type\n```\nmapa\n```\nA [jupyter notebook](https://jupyter.org/) will be started with an interactive map. Follow the described steps by\nexecuting the cells to create a 3d model of whatever place you like.\n\n Choose bounding box    | Create STL file\n:-------------------------:|:-------------------------:\n![](https://i.imgur.com/76hcx9Nh.jpg)  |  ![](https://i.imgur.com/llvxlrkh.png)\n\n Slice STL file         | 3D print\n:-------------------------:|:-------------------------:\n![](https://i.imgur.com/AKSRHbKh.jpg)  |  ![](https://i.imgur.com/DTc1yTBh.jpg)\n\n### 3. Using the dem2stl cli 💻\nThe `dem2stl` cli lets you create a 3d-printable STL file based on your tiff file. You can run a demo computation to get\na feeling of how the output STL will look like:\n```\ndem2stl --demo\n```\nIf you have your tiff file ready, you may run something like\n```\ndem2stl --input your_file.tiff --output output.stl --model-size 200 --z-offset 3.0 --z-scale 1.5\n```\nThe full list of options and their intention can be found with `dem2stl --help`:\n```\nUsage: dem2stl [OPTIONS]\n\n  🌍 Convert DEM data into STL files 🌏\n\nOptions:\n  --input TEXT                Path to input TIFF file.\n  --output TEXT               Path to output STL file.\n  --as-ascii                  Save output STL as ascii file. If not provided,\n                              output file will be binary.\n  --model-size INTEGER        Desired size of the generated 3d model in\n                              millimeter.\n  --max-res                   Whether maximum resolution should be used. Note,\n                              that this flag potentially increases compute\n                              time dramatically. The default behavior (i.e.\n                              max_res=False) should return 3d models with\n                              sufficient resolution, while the output stl file\n                              should be < ~400 MB.\n  --z-offset FLOAT            Offset distance in millimeter to be put below\n                              the 3d model. Defaults to 4.0. Is not influenced\n                              by z-scale.\n  --z-scale FLOAT             Value to be multiplied to the z-axis elevation\n                              data to scale up the height of the model.\n                              Defaults to 1.0.\n  --demo                      Converts a demo tiff of Hawaii into a STL file.\n  --cut-to-format-ratio TEXT  Cut the input tiff file to a specified format.\n                              Set to `1` if you want the output model to be\n                              squared. Set to `0.5` if you want one side to be\n                              half the length of the other side. Omit this\n                              flag to keep the input format. This option is\n                              particularly useful when an exact output format\n                              ratio is required for example when planning to\n                              put the 3d printed model into a picture frame.\n                              Using this option will always try to cut the\n                              shorter side of the input tiff.\n  --version                   Show the version and exit.\n  --help                      Show this message and exit.\n```\n\n### 4. Using `mapa` as python library 📚\nIn case you are building your own application you can simply use `mapa`\'s functionality within your application by importing the functions of the module.\n```python\nfrom mapa import convert_tiff_to_stl\n\npath_to_stl = convert_tiff_to_stl(\n    input_file="path/to/your/input_file.tiff",\n    as_ascii=False,\n    model_size=200,\n    output_file="path/to/your/output_file.stl",\n    max_res=False,\n    z_offset=3.0,\n    z_scale=1.5,\n)\n```\n\n\n## Algorithm Deep Dive\n\nIn case you are curios about the algorithm which turns a GeoTIFF into a STL file, I\'d recommend reading the header of\n[`algorithm.py`](https://github.com/fgebhart/mapa/blob/main/mapa/algorithm.py).\n\n\n## Changelog\n\nSee [Releases](https://github.com/fgebhart/mapa/releases).\n\n\n## Contributing\n\nContributions, feedback or issues are welcome.\n',
     'author': 'Fabian Gebhart',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fgebhart/mapa',
```

### Comparing `mapa-0.8.0/PKG-INFO` & `mapa-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapa
-Version: 0.8.0
+Version: 0.9.0
 Summary: 🌍 Create 3d-printable STLs from satellite elevation data 🌏
 Home-page: https://github.com/fgebhart/mapa
 Author: Fabian Gebhart
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
```

