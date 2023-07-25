# Comparing `tmp/ipctk-1.0.0.tar.gz` & `tmp/ipctk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipctk-1.0.0.tar", last modified: Mon Mar 20 05:45:52 2023, max compression
+gzip compressed data, was "ipctk-1.1.0.tar", last modified: Tue Jul 25 16:48:15 2023, max compression
```

## Comparing `ipctk-1.0.0.tar` & `ipctk-1.1.0.tar`

### file list

```diff
@@ -1,225 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.422297 ipctk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-03-20 05:45:43.000000 ipctk-1.0.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-20 05:45:43.000000 ipctk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-20 05:45:43.000000 ipctk-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-03-20 05:45:52.422297 ipctk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-03-20 05:45:43.000000 ipctk-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.398296 ipctk-1.0.0/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.402296 ipctk-1.0.0/cmake/find/
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/find/FindAVX.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/find/FindFMA.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/find/FindGMP.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/find/FindSSE.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.402296 ipctk-1.0.0/cmake/ipc_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/ipc_toolkit/ipc_toolkit_prepend_current_path.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/ipc_toolkit/ipc_toolkit_set_source_group.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/ipc_toolkit/ipc_toolkit_target_link_system_libraries.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/ipc_toolkit/ipc_toolkit_use_colors.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/ipc_toolkit/ipc_toolkit_warnings.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.402296 ipctk-1.0.0/cmake/recipes/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/abseil.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/catch2.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/evouga_ccd.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/finite_diff.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/gmp.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/gpu_ccd.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/json.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/libigl.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/onetbb.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/robin_map.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/spdlog.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/sweep_and_tiniest_queue.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-20 05:45:43.000000 ipctk-1.0.0/cmake/recipes/tight_inclusion.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.402296 ipctk-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-03-20 05:45:43.000000 ipctk-1.0.0/docs/PYPI_README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-20 05:45:43.000000 ipctk-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.402296 ipctk-1.0.0/python/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1874 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.402296 ipctk-1.0.0/python/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.402296 ipctk-1.0.0/python/src/barrier/
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/barrier/adaptive_stiffness.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/barrier/barrier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.406296 ipctk-1.0.0/python/src/broad_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/broad_phase/aabb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/broad_phase/broad_phase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/broad_phase/brute_force.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/broad_phase/hash_grid.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/broad_phase/spatial_hash.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/broad_phase/sweep_and_tiniest_queue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/broad_phase/voxel_size_heuristic.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.406296 ipctk-1.0.0/python/src/candidates/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/candidates/candidates.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/candidates/continuous_collision_candidate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/candidates/edge_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/candidates/edge_face.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/candidates/edge_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/candidates/face_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/candidates/vertex_vertex.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.406296 ipctk-1.0.0/python/src/ccd/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/ccd/aabb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/ccd/ccd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/ccd/inexact_point_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/ccd/point_static_plane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/collision_constraint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/collision_mesh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/common.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.406296 ipctk-1.0.0/python/src/distance/
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/distance_type.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/edge_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/edge_edge_mollifier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/line_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/point_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/point_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/point_plane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/point_point.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/distance/point_triangle.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.406296 ipctk-1.0.0/python/src/friction/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/friction/closest_point.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/friction/friction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/friction/friction_constraint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/friction/normal_force_magnitude.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/friction/relative_displacement.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/friction/smooth_friction_mollifier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/friction/tangent_basis.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/ipc.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.410297 ipctk-1.0.0/python/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/utils/eigen_ext.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/utils/intersection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/utils/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/utils/thread_limiter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-20 05:45:43.000000 ipctk-1.0.0/python/src/utils/world_bbox_diagonal_length.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 05:45:52.422297 ipctk-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5394 2023-03-20 05:45:43.000000 ipctk-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.398296 ipctk-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.410297 ipctk-1.0.0/src/ipc/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.410297 ipctk-1.0.0/src/ipc/barrier/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/barrier/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/barrier/adaptive_stiffness.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/barrier/adaptive_stiffness.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/barrier/barrier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/barrier/barrier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/barrier/barrier.tpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.410297 ipctk-1.0.0/src/ipc/broad_phase/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/aabb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/aabb.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/broad_phase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/broad_phase.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/brute_force.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/brute_force.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/hash_grid.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/hash_grid.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34347 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/spatial_hash.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/spatial_hash.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/sweep_and_tiniest_queue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/sweep_and_tiniest_queue.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/voxel_size_heuristic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/broad_phase/voxel_size_heuristic.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.414297 ipctk-1.0.0/src/ipc/candidates/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/candidates.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/candidates.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/continuous_collision_candidate.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/edge_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/edge_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/edge_face.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/edge_face.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/edge_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/edge_vertex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/face_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/face_vertex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/vertex_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/candidates/vertex_vertex.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.414297 ipctk-1.0.0/src/ipc/ccd/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/aabb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/aabb.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/ccd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/ccd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/inexact_point_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/inexact_point_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/point_static_plane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ccd/point_static_plane.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collision_mesh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collision_mesh.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.414297 ipctk-1.0.0/src/ipc/collisions/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/collision_constraint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/collision_constraint.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/constraints.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/constraints.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/edge_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/edge_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/edge_vertex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/face_vertex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/plane_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/plane_vertex.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/collisions/vertex_vertex.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.418297 ipctk-1.0.0/src/ipc/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/distance_type.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/distance_type.tpp
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/edge_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/edge_edge_mollifier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/edge_edge_mollifier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22339 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/line_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/line_line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/point_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/point_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/point_line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/point_plane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/point_plane.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/point_point.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/distance/point_triangle.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.418297 ipctk-1.0.0/src/ipc/friction/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26016 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/closest_point.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/closest_point.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/friction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/friction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/friction.tpp
--rw-r--r--   0 runner    (1001) docker     (123)    27434 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/friction_constraint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/friction_constraint.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/normal_force_magnitude.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/normal_force_magnitude.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/relative_displacement.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/smooth_friction_mollifier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/smooth_friction_mollifier.tpp
--rw-r--r--   0 runner    (1001) docker     (123)    30311 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/tangent_basis.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/friction/tangent_basis.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.422297 ipctk-1.0.0/src/ipc/implicits/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/implicits/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/implicits/plane.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/implicits/plane.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ipc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/ipc.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.422297 ipctk-1.0.0/src/ipc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/area_gradient.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/area_gradient.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/eigen_ext.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/eigen_ext.tpp
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/intersection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/local_to_global.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/logger.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/merge_thread_local.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/rational.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/save_obj.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/save_obj.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/unordered_map_and_set.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/vertex_to_min_edge.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/vertex_to_min_edge.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-20 05:45:43.000000 ipctk-1.0.0/src/ipc/utils/world_bbox_diagonal_length.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 05:45:52.422297 ipctk-1.0.0/src/ipctk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-03-20 05:45:52.000000 ipctk-1.0.0/src/ipctk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-03-20 05:45:52.000000 ipctk-1.0.0/src/ipctk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 05:45:52.000000 ipctk-1.0.0/src/ipctk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 05:45:52.000000 ipctk-1.0.0/src/ipctk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-20 05:45:52.000000 ipctk-1.0.0/src/ipctk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-20 05:45:52.000000 ipctk-1.0.0/src/ipctk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.105862 ipctk-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-07-25 16:48:01.000000 ipctk-1.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 16:48:01.000000 ipctk-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 16:48:01.000000 ipctk-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-25 16:48:15.105862 ipctk-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-25 16:48:01.000000 ipctk-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.057858 ipctk-1.1.0/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.065859 ipctk-1.1.0/cmake/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/find/FindAVX.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/find/FindFMA.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/find/FindGMP.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/find/FindSSE.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.065859 ipctk-1.1.0/cmake/ipc_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/ipc_toolkit/ipc_toolkit_cpm_cache.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/ipc_toolkit/ipc_toolkit_filter_flags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/ipc_toolkit/ipc_toolkit_use_colors.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/ipc_toolkit/ipc_toolkit_warnings.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.069859 ipctk-1.1.0/cmake/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/CPM.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/abseil.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/catch2.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/evouga_ccd.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/finite_diff.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/gmp.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/gpu_ccd.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/json.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/libigl.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/onetbb.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/robin_map.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/spdlog.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/sweep_and_tiniest_queue.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-25 16:48:01.000000 ipctk-1.1.0/cmake/recipes/tight_inclusion.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.069859 ipctk-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-25 16:48:01.000000 ipctk-1.1.0/docs/PYPI_README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-25 16:48:01.000000 ipctk-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.069859 ipctk-1.1.0/python/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2495 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.069859 ipctk-1.1.0/python/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.069859 ipctk-1.1.0/python/src/barrier/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/barrier/adaptive_stiffness.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/barrier/barrier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/barrier/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/bindings.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.069859 ipctk-1.1.0/python/src/broad_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/aabb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/broad_phase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/brute_force.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/hash_grid.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/spatial_hash.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/sweep_and_tiniest_queue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/broad_phase/voxel_size_heuristic.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.073860 ipctk-1.1.0/python/src/candidates/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/candidates.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/collision_stencil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/continuous_collision_candidate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/edge_face.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/edge_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/face_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/candidates/vertex_vertex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.073860 ipctk-1.1.0/python/src/ccd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/ccd/aabb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/ccd/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/ccd/ccd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/ccd/inexact_point_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/ccd/point_static_plane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collision_mesh.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.073860 ipctk-1.1.0/python/src/collisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/collision_constraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/collision_constraints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/edge_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/face_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/plane_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/collisions/vertex_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/common.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.077860 ipctk-1.1.0/python/src/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/distance_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/edge_edge_mollifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/line_line.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/point_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/point_line.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/point_plane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/point_point.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/distance/point_triangle.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.077860 ipctk-1.1.0/python/src/friction/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/closest_point.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.077860 ipctk-1.1.0/python/src/friction/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/constraints/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/constraints/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/constraints/edge_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/constraints/face_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/constraints/friction_constraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/constraints/vertex_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/friction_constraints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/normal_force_magnitude.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/relative_velocity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/smooth_friction_mollifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/friction/tangent_basis.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.077860 ipctk-1.1.0/python/src/implicits/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/implicits/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/implicits/plane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/ipc.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.077860 ipctk-1.1.0/python/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/area_gradient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/bindings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/eigen_ext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/intersection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/thread_limiter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/vertex_to_min_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-25 16:48:01.000000 ipctk-1.1.0/python/src/utils/world_bbox_diagonal_length.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:48:15.105862 ipctk-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5502 2023-07-25 16:48:01.000000 ipctk-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.061859 ipctk-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.081860 ipctk-1.1.0/src/ipc/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.081860 ipctk-1.1.0/src/ipc/barrier/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/barrier/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/barrier/adaptive_stiffness.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/barrier/adaptive_stiffness.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/barrier/barrier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/barrier/barrier.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.085861 ipctk-1.1.0/src/ipc/broad_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/aabb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/aabb.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/broad_phase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/broad_phase.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/brute_force.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/brute_force.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/hash_grid.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/hash_grid.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/spatial_hash.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/spatial_hash.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/sweep_and_tiniest_queue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/sweep_and_tiniest_queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/voxel_size_heuristic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/broad_phase/voxel_size_heuristic.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.085861 ipctk-1.1.0/src/ipc/candidates/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/candidates.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/candidates.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/collision_stencil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/collision_stencil.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/continuous_collision_candidate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/continuous_collision_candidate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/edge_edge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/edge_face.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/edge_face.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/edge_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/edge_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/face_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/face_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/vertex_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/candidates/vertex_vertex.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.085861 ipctk-1.1.0/src/ipc/ccd/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/aabb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/aabb.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/ccd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/ccd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/inexact_point_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/inexact_point_edge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/point_static_plane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ccd/point_static_plane.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collision_mesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collision_mesh.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.089861 ipctk-1.1.0/src/ipc/collisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/collision_constraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/collision_constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/collision_constraints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/collision_constraints.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/collision_constraints_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/collision_constraints_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/edge_edge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/edge_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/face_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/plane_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/plane_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/collisions/vertex_vertex.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.093861 ipctk-1.1.0/src/ipc/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/distance_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/distance_type.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/edge_edge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/edge_edge_mollifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/edge_edge_mollifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23680 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/line_line.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/line_line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_edge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_line.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25192 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_plane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_plane.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_point.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_point.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_triangle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/distance/point_triangle.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.093861 ipctk-1.1.0/src/ipc/friction/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29666 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/closest_point.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/closest_point.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.101862 ipctk-1.1.0/src/ipc/friction/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/edge_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/edge_edge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/edge_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/edge_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/face_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/face_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13895 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/friction_constraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/friction_constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/vertex_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/constraints/vertex_vertex.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/friction_constraints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/friction_constraints.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/normal_force_magnitude.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/normal_force_magnitude.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/relative_velocity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/relative_velocity.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/smooth_friction_mollifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/smooth_friction_mollifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    36159 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/tangent_basis.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/friction/tangent_basis.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.101862 ipctk-1.1.0/src/ipc/implicits/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/implicits/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/implicits/plane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/implicits/plane.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ipc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/ipc.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.105862 ipctk-1.1.0/src/ipc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/area_gradient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/area_gradient.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/eigen_ext.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/eigen_ext.tpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/intersection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/local_to_global.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/logger.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/merge_thread_local.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/rational.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/save_obj.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/save_obj.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/unordered_map_and_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/unordered_map_and_set.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/vertex_to_min_edge.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/vertex_to_min_edge.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-25 16:48:01.000000 ipctk-1.1.0/src/ipc/utils/world_bbox_diagonal_length.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:48:15.105862 ipctk-1.1.0/src/ipctk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-25 16:48:15.000000 ipctk-1.1.0/src/ipctk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-07-25 16:48:15.000000 ipctk-1.1.0/src/ipctk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:48:15.000000 ipctk-1.1.0/src/ipctk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:48:14.000000 ipctk-1.1.0/src/ipctk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 16:48:15.000000 ipctk-1.1.0/src/ipctk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 16:48:15.000000 ipctk-1.1.0/src/ipctk.egg-info/top_level.txt
```

### Comparing `ipctk-1.0.0/CMakeLists.txt` & `ipctk-1.1.0/CMakeLists.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,100 @@
 # Detects whether this is a top-level project
 get_directory_property(HAS_PARENT PARENT_DIRECTORY)
 if(HAS_PARENT)
-    set(IPC_TOOLKIT_TOPLEVEL_PROJECT OFF)
+  set(IPC_TOOLKIT_TOPLEVEL_PROJECT OFF)
 else()
-    set(IPC_TOOLKIT_TOPLEVEL_PROJECT ON)
+  set(IPC_TOOLKIT_TOPLEVEL_PROJECT ON)
 endif()
 
 # Check required CMake version
-set(REQUIRED_CMAKE_VERSION "3.14.0")
+set(REQUIRED_CMAKE_VERSION "3.18.0")
 if(IPC_TOOLKIT_TOPLEVEL_PROJECT)
-    cmake_minimum_required(VERSION ${REQUIRED_CMAKE_VERSION})
+  cmake_minimum_required(VERSION ${REQUIRED_CMAKE_VERSION})
 else()
-    # Don't use cmake_minimum_required here to avoid implicitly overriding parent policies
-    if(${CMAKE_VERSION} VERSION_LESS ${REQUIRED_CMAKE_VERSION})
-        message(FATAL_ERROR "CMake required version to build IPC Toolkit is ${REQUIRED_CMAKE_VERSION}")
-    endif()
+  # Don't use cmake_minimum_required here to avoid implicitly overriding parent policies
+  if(${CMAKE_VERSION} VERSION_LESS ${REQUIRED_CMAKE_VERSION})
+    message(FATAL_ERROR "CMake required version to build IPC Toolkit is ${REQUIRED_CMAKE_VERSION}")
+  endif()
 endif()
 
 # Include user-provided default options if available. We do that before the main
 # `project()` so that we can define the C/C++ compilers from the option file.
 if(EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/IPCToolkitOptions.cmake)
-    message(STATUS "Using local options file: ${CMAKE_CURRENT_SOURCE_DIR}/IPCToolkitOptions.cmake")
-    include(${CMAKE_CURRENT_SOURCE_DIR}/IPCToolkitOptions.cmake)
+  message(STATUS "Using local options file: ${CMAKE_CURRENT_SOURCE_DIR}/IPCToolkitOptions.cmake")
+  include(${CMAKE_CURRENT_SOURCE_DIR}/IPCToolkitOptions.cmake)
+endif()
+
+# Enable ccache if available
+find_program(CCACHE_PROGRAM ccache)
+if(CCACHE_PROGRAM)
+  option(IPC_TOOLKIT_WITH_CCACHE "Enable ccache when building IPC Toolkit" ${IPC_TOOLKIT_TOPLEVEL_PROJECT})
+else()
+  option(IPC_TOOLKIT_WITH_CCACHE "Enable ccache when building IPC Toolkit" OFF)
+endif()
+if(IPC_TOOLKIT_WITH_CCACHE AND CCACHE_PROGRAM)
+  message(STATUS "Enabling Ccache support")
+  set(ccacheEnv
+    CCACHE_BASEDIR=${CMAKE_BINARY_DIR}
+    CCACHE_SLOPPINESS=clang_index_store,include_file_ctime,include_file_mtime,locale,pch_defines,time_macros
+  )
+  foreach(lang IN ITEMS C CXX)
+    set(CMAKE_${lang}_COMPILER_LAUNCHER
+      ${CMAKE_COMMAND} -E env ${ccacheEnv} ${CCACHE_PROGRAM}
+    )
+  endforeach()
+endif()
+
+
+################################################################################
+# CMake Policies
+################################################################################
+
+cmake_policy(SET CMP0054 NEW) # Only interpret if() arguments as variables or keywords when unquoted.
+cmake_policy(SET CMP0076 NEW) # target_sources() command converts relative paths to absolute.
+if(CMAKE_VERSION VERSION_GREATER_EQUAL "3.24")
+  cmake_policy(SET CMP0135 NEW) # Set the timestamps of all extracted contents to the time of the extraction.
 endif()
 
 ################################################################################
 
 project(IPCToolkit
         DESCRIPTION "A set of reusable functions to integrate IPC into an existing simulation."
         LANGUAGES CXX
-        VERSION "1.0.0")
+        VERSION "1.1.0")
 
 option(IPC_TOOLKIT_BUILD_TESTS                "Build unit-tests"  ${IPC_TOOLKIT_TOPLEVEL_PROJECT})
 option(IPC_TOOLKIT_BUILD_PYTHON               "Build Python bindings"                         OFF)
 option(IPC_TOOLKIT_WITH_CORRECT_CCD           "Use the TightInclusion CCD"                     ON)
 option(IPC_TOOLKIT_WITH_SIMD                  "Enable SIMD"                                   OFF)
 option(IPC_TOOLKIT_WITH_CUDA                  "Enable CUDA CCD"                               OFF)
 option(IPC_TOOLKIT_WITH_RATIONAL_INTERSECTION "Use rational edge-triangle intersection check" OFF)
+option(IPC_TOOLKIT_WITH_ROBIN_MAP             "Use Tessil's robin-map rather than std maps"    ON)
+option(IPC_TOOLKIT_WITH_ABSEIL                "Use Abseil's hash functions"                    ON)
 
 # Set default minimum C++ standard
 if(IPC_TOOLKIT_TOPLEVEL_PROJECT)
-    set(CMAKE_CXX_STANDARD 17)
-    set(CMAKE_CXX_STANDARD_REQUIRED ON)
-    set(CMAKE_CXX_EXTENSIONS OFF)
+  set(CMAKE_CXX_STANDARD 17)
+  set(CMAKE_CXX_STANDARD_REQUIRED ON)
+  set(CMAKE_CXX_EXTENSIONS OFF)
 endif()
 
 ### Configuration
 set(IPC_TOOLKIT_SOURCE_DIR "${PROJECT_SOURCE_DIR}/src/ipc")
 set(IPC_TOOLKIT_INCLUDE_DIR "${PROJECT_SOURCE_DIR}/src")
 
 list(APPEND CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/cmake/ipc_toolkit/")
 list(APPEND CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/cmake/recipes/")
 list(APPEND CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/cmake/find/")
 
-# Color output
+# General CMake utils
+include(ipc_toolkit_cpm_cache)
 include(ipc_toolkit_use_colors)
 
-# IPC Toolkit utils
-include(ipc_toolkit_prepend_current_path)
-include(ipc_toolkit_set_source_group)
-include(ipc_toolkit_target_link_system_libraries)
-
-# Generate position independent code by default
+# Generate position-independent code by default
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
 ################################################################################
 # IPC Toolkit Library
 ################################################################################
 
 # Add an empty library and fill in the list of sources in `src/CMakeLists.txt`.
@@ -93,62 +122,66 @@
 ################################################################################
 # Dependencies
 ################################################################################
 
 # libigl
 include(eigen)
 include(libigl)
-ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC
+target_link_libraries(ipc_toolkit PUBLIC
   Eigen3::Eigen
   igl::core
   igl::predicates
 )
 
 # TBB
 include(onetbb)
-ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC TBB::tbb)
+target_link_libraries(ipc_toolkit PUBLIC TBB::tbb)
 
 # CCD
 if(IPC_TOOLKIT_WITH_CORRECT_CCD)
   # Provably conservative CCD of [Wang and Ferguson et al. 2021]
   include(tight_inclusion)
-  ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC tight_inclusion::tight_inclusion)
+  target_link_libraries(ipc_toolkit PUBLIC tight_inclusion::tight_inclusion)
 else()
   # Etienne Vouga's CTCD Library for the floating point root finding algorithm
   include(evouga_ccd)
-  ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC evouga::ccd)
+  target_link_libraries(ipc_toolkit PUBLIC evouga::ccd)
 endif()
 
 # Logger
 include(spdlog)
-ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC spdlog::spdlog)
+target_link_libraries(ipc_toolkit PUBLIC spdlog::spdlog)
 
 if(IPC_TOOLKIT_WITH_RATIONAL_INTERSECTION)
   include(gmp)
-  ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC GMP::GMP)
+  target_link_libraries(ipc_toolkit PUBLIC GMP::GMP)
 endif()
 
 # Sweep and Tiniest Queue and CCD
 if(IPC_TOOLKIT_WITH_CUDA)
   include(gpu_ccd)
-  ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC gpu_ccd::gpu_ccd)
-  ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC STQ::CPU)
+  target_link_libraries(ipc_toolkit PUBLIC gpu_ccd::gpu_ccd)
+  target_link_libraries(ipc_toolkit PUBLIC STQ::CPU)
 else()
   set(STQ_WITH_CUDA OFF CACHE BOOL "Enable CUDA Implementation" FORCE)
   include(sweep_and_tiniest_queue)
-  ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC STQ::CPU)
+  target_link_libraries(ipc_toolkit PUBLIC STQ::CPU)
 endif()
 
 # Faster unordered map
-include(robin_map)
-ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC tsl::robin_map)
+if(IPC_TOOLKIT_WITH_ROBIN_MAP)
+  include(robin_map)
+  target_link_libraries(ipc_toolkit PUBLIC tsl::robin_map)
+endif()
 
 # Hashes
-include(abseil)
-ipc_toolkit_target_link_system_libraries(ipc_toolkit PUBLIC absl::hash)
+if(IPC_TOOLKIT_WITH_ABSEIL)
+  include(abseil)
+  target_link_libraries(ipc_toolkit PUBLIC absl::hash)
+endif()
 
 # Extra warnings (link last for highest priority)
 include(ipc_toolkit_warnings)
 target_link_libraries(ipc_toolkit PRIVATE ipc::toolkit::warnings)
 
 ################################################################################
 # Compiler options
@@ -187,33 +220,37 @@
   endif()
 
   # We need to explicitly state that we need all CUDA files in the particle
   # library to be built with -dc as the member functions could be called by
   # other libraries and executables.
   set_target_properties(ipc_toolkit PROPERTIES CUDA_SEPARABLE_COMPILATION ON)
 
-  # Nvidia RTX8000 -> compute_75
-  # Nvidia V100 -> compute_70
-  # Nvidia 1080/1080Ti -> compute_61
-  # Nvidia 3080Ti -> compute_86
-  if(NOT DEFINED CMAKE_CUDA_ARCHITECTURES)
-    set(CMAKE_CUDA_ARCHITECTURES 70 75 86)
+  if(${CMAKE_VERSION} VERSION_GREATER_EQUAL "3.24.0")
+    set(CMAKE_CUDA_ARCHITECTURES "native")
+    set_target_properties(ipc_toolkit PROPERTIES CUDA_ARCHITECTURES "native")
+  else()
+    include(FindCUDA/select_compute_arch)
+    CUDA_DETECT_INSTALLED_GPUS(CUDA_ARCH_LIST)
+    string(STRIP "${CUDA_ARCH_LIST}" CUDA_ARCH_LIST)
+    string(REPLACE " " ";" CUDA_ARCH_LIST "${CUDA_ARCH_LIST}")
+    string(REPLACE "." "" CUDA_ARCH_LIST "${CUDA_ARCH_LIST}")
+    set(CMAKE_CUDA_ARCHITECTURES ${CUDA_ARCH_LIST})
+    set_target_properties(ipc_toolkit PROPERTIES CUDA_ARCHITECTURES "${CUDA_ARCH_LIST}")
   endif()
-  set_target_properties(ipc_toolkit PROPERTIES CUDA_ARCHITECTURES "70;75;86")
 
   if(APPLE)
     # We need to add the path to the driver (libcuda.dylib) as an rpath,
     # so that the static cuda runtime can find it at runtime.
     set_property(TARGET ipc_toolkit
                  PROPERTY
                  BUILD_RPATH ${CMAKE_CUDA_IMPLICIT_LINK_DIRECTORIES})
   endif()
 
   find_package(CUDAToolkit)
-  ipc_toolkit_target_link_system_libraries(ipc_toolkit PRIVATE CUDA::cudart)
+  target_link_libraries(ipc_toolkit PRIVATE CUDA::cudart)
 endif()
 
 ################################################################################
 # Tests
 ################################################################################
 
 # Enable unit testing at the root level
```

### Comparing `ipctk-1.0.0/LICENSE` & `ipctk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/PKG-INFO` & `ipctk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipctk
-Version: 1.0.0
+Version: 1.1.0
 Summary: A set of reusable functions to integrate Incremental Potential Contact (IPC) into a simulation.
 Author-email: Zachary Ferguson <zfergus@nyu.edu>
 License: MIT License
         
         Copyright (c) 2020 IPC-Sim
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ipctk-1.0.0/README.md` & `ipctk-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 ```cmake
 include(FetchContent)
 FetchContent_Declare(
     ipc_toolkit
     GIT_REPOSITORY https://github.com/ipc-sim/ipc-toolkit.git
     GIT_TAG ${IPC_TOOLKIT_GIT_TAG}
-    GIT_SHALLOW TRUE
 )
 FetchContent_MakeAvailable(ipc_toolkit)
 ```
 
 where `IPC_TOOLKIT_GIT_TAG` is set to the version of the toolkit you want to use. This will download and add the toolkit to CMake. The toolkit can then be linked against using
 
 ```cmake
@@ -56,19 +55,23 @@
 The following libraries are used in this project:
 
 * [Eigen](https://eigen.tuxfamily.org/): linear algebra
 * [libigl](https://github.com/libigl/libigl): basic geometry functions and predicates
 * [TBB](https://github.com/wjakob/tbb): parallelization
 * [Tight-Inclusion](https://github.com/Continuous-Collision-Detection/Tight-Inclusion): correct (conservative) CCD
 * [spdlog](https://github.com/gabime/spdlog): logging information
-* [robin-map](https://github.com/Tessil/robin-map): faster hash set/map than `std::unordered_set`/`std::unordered_map`
-* [Abseil](https://abseil.io/): hashing utilities
 
 #### Optional
 
+* [robin-map](https://github.com/Tessil/robin-map): faster hash set/map than `std::unordered_set`/`std::unordered_map`
+    * Enable by using the CMake option `IPC_TOOLKIT_WITH_ROBIN_MAP`
+    * Enabled by default
+* [Abseil](https://abseil.io/): hashing utilities
+    * Enable by using the CMake option `IPC_TOOLKIT_WITH_ABSEIL`
+    * Enabled by default
 * [GMP](https://gmplib.org/): rational arithmetic used for exact intersection checks
     * Enable by using the CMake option `IPC_TOOLKIT_WITH_RATIONAL_INTERSECTION`
     * GMP must be installed at a system level
 * [Etienne Vouga's Collision Detection Library](https://github.com/evouga/collisiondetection): inexact CCD
     * Included for comparison with the original IPC library
     * Enable by disabling the CMake option `IPC_TOOLKIT_WITH_CORRECT_CCD`
     * Replaces the default Tight-Inclusion CCD
```

### Comparing `ipctk-1.0.0/cmake/find/FindAVX.cmake` & `ipctk-1.1.0/cmake/find/FindAVX.cmake`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/cmake/find/FindFMA.cmake` & `ipctk-1.1.0/cmake/find/FindFMA.cmake`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/cmake/find/FindGMP.cmake` & `ipctk-1.1.0/cmake/find/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/cmake/find/FindSSE.cmake` & `ipctk-1.1.0/cmake/find/FindSSE.cmake`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/cmake/ipc_toolkit/ipc_toolkit_warnings.cmake` & `ipctk-1.1.0/cmake/ipc_toolkit/ipc_toolkit_warnings.cmake`

 * *Files 10% similar despite different names*

```diff
@@ -3,166 +3,158 @@
 # http://stackoverflow.com/questions/5088460/flags-to-enable-thorough-and-verbose-g-warnings
 ################################################################################
 
 if(TARGET ipc::toolkit::warnings)
   return()
 endif()
 
-set(IPC_TOOLKIT_FLAGS
-    -Wall
-    -Wextra
-    -pedantic
-
-    # -Wconversion
-    #-Wunsafe-loop-optimizations # broken with C++11 loops
-    -Wunused
-
-    -Wno-long-long
-    -Wpointer-arith
-    -Wformat=2
-    -Wuninitialized
-    -Wcast-qual
-    # -Wmissing-noreturn
-    -Wmissing-format-attribute
-    # -Wredundant-decls
-
-    -Werror=implicit
-    -Werror=nonnull
-    -Werror=init-self
-    -Werror=main
-    -Werror=missing-braces
-    -Werror=sequence-point
-    -Werror=return-type
-    -Werror=trigraphs
-    -Warray-bounds
-    -Werror=write-strings
-    -Werror=address
-    -Werror=int-to-pointer-cast
-    -Werror=pointer-to-int-cast
-
-    -Wno-unused-variable
-    -Wunused-but-set-variable
-    -Wno-unused-parameter
-
-    #-Weffc++
-    -Wno-old-style-cast
-    # -Wno-sign-conversion
-    #-Wsign-conversion
-
-    # -Wshadow
-
-    -Wstrict-null-sentinel
-    -Woverloaded-virtual
-    -Wsign-promo
-    -Wstack-protector
-    -Wstrict-aliasing
-    -Wstrict-aliasing=2
-
-    # Warn whenever a switch statement has an index of enumerated type and
-    # lacks a case for one or more of the named codes of that enumeration.
-    -Wswitch
-    # This is annoying if all cases are already covered.
-    # -Wswitch-default
-    # This is annoying if there is a default that covers the rest.
-    # -Wswitch-enum
-    -Wswitch-unreachable
-    # -Wcovered-switch-default # Annoying warnings from nlohmann::json
-
-    -Wcast-align
-    -Wdisabled-optimization
-    #-Winline # produces warning on default implicit destructor
-    -Winvalid-pch
-    # -Wmissing-include-dirs
-    -Wpacked
-    -Wno-padded
-    -Wstrict-overflow
-    -Wstrict-overflow=2
-
-    # -Wctor-dtor-privacy
-    -Wlogical-op
-    # -Wnoexcept
-    -Woverloaded-virtual
-    # -Wundef
-
-    -Wnon-virtual-dtor
-    -Wdelete-non-virtual-dtor
-    -Werror=non-virtual-dtor
-    -Werror=delete-non-virtual-dtor
-
-    -Wno-sign-compare
-
-    ###########
-    # GCC 6.1 #
-    ###########
-
-    -Wnull-dereference
-    -fdelete-null-pointer-checks
-    -Wduplicated-cond
-    -Wmisleading-indentation
-
-    #-Weverything
-
-    ###########################
-    # Enabled by -Weverything #
-    ###########################
-
-    #-Wdocumentation
-    #-Wdocumentation-unknown-command
-    #-Wfloat-equal
-
-    #-Wglobal-constructors
-    #-Wexit-time-destructors
-    #-Wmissing-variable-declarations
-    #-Wextra-semi
-    #-Wweak-vtables
-    #-Wno-source-uses-openmp
-    #-Wdeprecated
-    #-Wnewline-eof
-    #-Wmissing-prototypes
-
-    #-Wno-c++98-compat
-    #-Wno-c++98-compat-pedantic
-
-    ################################################
-    # Need to check if those are still valid today #
-    ################################################
-
-    #-Wimplicit-atomic-properties
-    #-Wmissing-declarations
-    #-Wmissing-prototypes
-    #-Wstrict-selector-match
-    #-Wundeclared-selector
-    #-Wunreachable-code
-
-    # Not a warning, but enable link-time-optimization
-    # TODO: Check out modern CMake version of setting this flag
-    # https://cmake.org/cmake/help/latest/module/CheckIPOSupported.html
-    #-flto
-
-    # Gives meaningful stack traces
-    -fno-omit-frame-pointer
-    -fno-optimize-sibling-calls
+set(IPC_TOOLKIT_WARNING_FLAGS
+  -Wall
+  -Wextra
+  -pedantic
+
+  # -Wconversion
+  #-Wunsafe-loop-optimizations # broken with C++11 loops
+  -Wunused
+
+  -Wno-long-long
+  -Wpointer-arith
+  -Wformat=2
+  -Wuninitialized
+  -Wcast-qual
+  # -Wmissing-noreturn
+  -Wmissing-format-attribute
+  # -Wredundant-decls
+
+  -Werror=implicit
+  -Werror=nonnull
+  -Werror=init-self
+  -Werror=main
+  -Werror=missing-braces
+  -Werror=sequence-point
+  -Werror=return-type
+  -Werror=trigraphs
+  -Warray-bounds
+  -Werror=write-strings
+  -Werror=address
+  -Werror=int-to-pointer-cast
+  -Werror=pointer-to-int-cast
+
+  -Wno-unused-variable
+  -Wunused-but-set-variable
+  -Wno-unused-parameter
+
+  #-Weffc++
+  -Wno-old-style-cast
+  # -Wno-sign-conversion
+  #-Wsign-conversion
+
+  # -Wshadow
+
+  -Wstrict-null-sentinel
+  -Woverloaded-virtual
+  -Wsign-promo
+  -Wstack-protector
+  -Wstrict-aliasing
+  -Wstrict-aliasing=2
+
+  # Warn whenever a switch statement has an index of enumerated type and
+  # lacks a case for one or more of the named codes of that enumeration.
+  -Wswitch
+  # This is annoying if all cases are already covered.
+  # -Wswitch-default
+  # This is annoying if there is a default that covers the rest.
+  # -Wswitch-enum
+  -Wswitch-unreachable
+  # -Wcovered-switch-default # Annoying warnings from nlohmann::json
+
+  -Wcast-align
+  -Wdisabled-optimization
+  #-Winline # produces warning on default implicit destructor
+  -Winvalid-pch
+  # -Wmissing-include-dirs
+  -Wpacked
+  -Wno-padded
+  -Wstrict-overflow
+  -Wstrict-overflow=2
+
+  # -Wctor-dtor-privacy
+  -Wlogical-op
+  # -Wnoexcept
+  -Woverloaded-virtual
+  # -Wundef
+
+  -Wnon-virtual-dtor
+  -Wdelete-non-virtual-dtor
+  -Werror=non-virtual-dtor
+  -Werror=delete-non-virtual-dtor
+
+  -Wno-sign-compare
+
+  ###########
+  # GCC 6.1 #
+  ###########
+
+  -Wnull-dereference
+  -fdelete-null-pointer-checks
+  -Wduplicated-cond
+  -Wmisleading-indentation
+
+  #-Weverything
+
+  ###########################
+  # Enabled by -Weverything #
+  ###########################
+
+  #-Wdocumentation
+  #-Wdocumentation-unknown-command
+  #-Wfloat-equal
+
+  #-Wglobal-constructors
+  #-Wexit-time-destructors
+  #-Wmissing-variable-declarations
+  #-Wextra-semi
+  #-Wweak-vtables
+  #-Wno-source-uses-openmp
+  #-Wdeprecated
+  #-Wnewline-eof
+  #-Wmissing-prototypes
+
+  #-Wno-c++98-compat
+  #-Wno-c++98-compat-pedantic
+
+  ################################################
+  # Need to check if those are still valid today #
+  ################################################
+
+  #-Wimplicit-atomic-properties
+  #-Wmissing-declarations
+  #-Wmissing-prototypes
+  #-Wstrict-selector-match
+  #-Wundeclared-selector
+  #-Wunreachable-code
+
+  # Not a warning, but enable link-time-optimization
+  # TODO: Check out modern CMake version of setting this flag
+  # https://cmake.org/cmake/help/latest/module/CheckIPOSupported.html
+  #-flto
+
+  # Gives meaningful stack traces
+  -fno-omit-frame-pointer
+  -fno-optimize-sibling-calls
 
-    -Wno-pedantic
+  -Wno-pedantic
 
-    -Wno-redundant-decls
+  -Wno-redundant-decls
 )
 
 # Flags above don't make sense for MSVC
 if(MSVC)
-  set(IPC_TOOLKIT_FLAGS)
+  set(IPC_TOOLKIT_WARNING_FLAGS)
 endif()
 
-include(CheckCXXCompilerFlag)
-
 add_library(ipc_toolkit_warnings INTERFACE)
 add_library(ipc::toolkit::warnings ALIAS ipc_toolkit_warnings)
 
-foreach(FLAG IN ITEMS ${IPC_TOOLKIT_FLAGS})
-  string(REPLACE "=" "-" FLAG_VAR "${FLAG}")
-  if(NOT DEFINED IS_SUPPORTED_${FLAG_VAR})
-    check_cxx_compiler_flag("${FLAG}" IS_SUPPORTED_${FLAG_VAR})
-  endif()
-  if(IS_SUPPORTED_${FLAG_VAR})
-    target_compile_options(ipc_toolkit_warnings INTERFACE ${FLAG})
-  endif()
-endforeach()
+include(ipc_toolkit_filter_flags)
+ipc_toolkit_filter_flags(IPC_TOOLKIT_WARNING_FLAGS)
+target_compile_options(ipc_toolkit_warnings INTERFACE ${IPC_TOOLKIT_WARNING_FLAGS})
```

### Comparing `ipctk-1.0.0/cmake/recipes/abseil.cmake` & `ipctk-1.1.0/cmake/recipes/abseil.cmake`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 if(TARGET absl::flat_hash_map)
     return()
 endif()
 
 message(STATUS "Third-party: creating target 'absl::flat_hash_map'")
 
 option(ABSL_PROPAGATE_CXX_STD "Use CMake C++ standard meta features (e.g. cxx_std_11) that propagate to targets that link to Abseil" ON)
+option(ABSL_USE_SYSTEM_INCLUDES "Silence warnings in Abseil headers by marking them as SYSTEM includes" ON)
 option(ABSL_BUILD_TESTING "If ON, Abseil will build all of Abseil's own tests." OFF)
 
-include(FetchContent)
-FetchContent_Declare(
-    abseil
-    GIT_REPOSITORY https://github.com/abseil/abseil-cpp.git
-    GIT_TAG 20220623.0
-    GIT_SHALLOW TRUE
-)
-FetchContent_MakeAvailable(abseil)
+include(CPM)
+CPMAddPackage("gh:abseil/abseil-cpp#20230125.3")
```

### Comparing `ipctk-1.0.0/cmake/recipes/catch2.cmake` & `ipctk-1.1.0/cmake/ipc_toolkit/ipc_toolkit_filter_flags.cmake`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #
-# Copyright 2020 Adobe. All rights reserved.
+# Copyright 2021 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-if(TARGET Catch2::Catch2)
-    return()
-endif()
-
-message(STATUS "Third-party: creating target 'Catch2::Catch2'")
-
-include(FetchContent)
-FetchContent_Declare(
-    catch2
-    GIT_REPOSITORY https://github.com/catchorg/Catch2.git
-    GIT_TAG v2.13.6
-    GIT_SHALLOW TRUE
-)
-FetchContent_MakeAvailable(catch2)
+function(ipc_toolkit_filter_flags flags)
+  include(CheckCXXCompilerFlag)
+  set(output_flags)
+  foreach(FLAG IN ITEMS ${${flags}})
+    string(REPLACE "=" "-" FLAG_VAR "${FLAG}")
+    if(NOT DEFINED IS_SUPPORTED_${FLAG_VAR})
+      check_cxx_compiler_flag("${FLAG}" IS_SUPPORTED_${FLAG_VAR})
+    endif()
+    if(IS_SUPPORTED_${FLAG_VAR})
+      list(APPEND output_flags $<$<COMPILE_LANGUAGE:CXX>:${FLAG}>)
+    endif()
+  endforeach()
+  set(${flags} ${output_flags} PARENT_SCOPE)
+endfunction()
```

### Comparing `ipctk-1.0.0/cmake/recipes/eigen.cmake` & `ipctk-1.1.0/cmake/recipes/eigen.cmake`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,68 @@
 #
-# Copyright 2020 Adobe. All rights reserved.
+# Copyright 2019 Adobe. All rights reserved.
 # This file is licensed to you under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 if(TARGET Eigen3::Eigen)
     return()
 endif()
 
-# option(EIGEN_WITH_MKL "Use Eigen with MKL" OFF)
-
-if(EIGEN_ROOT)
-    message(STATUS "Third-party: creating target 'Eigen3::Eigen' for external path: ${EIGEN_ROOT}")
-    set(EIGEN_INCLUDE_DIRS ${EIGEN_ROOT})
-else()
-    message(STATUS "Third-party: creating target 'Eigen3::Eigen'")
-
-    include(FetchContent)
-    FetchContent_Declare(
-        eigen
-        GIT_REPOSITORY https://gitlab.com/libeigen/eigen.git
-        GIT_TAG tags/3.4.0
-        GIT_SHALLOW TRUE
-    )
-    FetchContent_GetProperties(eigen)
-    if(NOT eigen_POPULATED)
-        FetchContent_Populate(eigen)
-    endif()
-    set(EIGEN_INCLUDE_DIRS ${eigen_SOURCE_DIR})
-
-    install(DIRECTORY ${EIGEN_INCLUDE_DIRS}/Eigen
-        DESTINATION include
-    )
-endif()
+option(EIGEN_WITH_MKL "Use Eigen with MKL" OFF)
+option(EIGEN_DONT_VECTORIZE "Disable Eigen vectorization" OFF)
+option(EIGEN_MPL2_ONLY "Enable Eigen MPL2 license only" OFF)
+
+message(STATUS "Third-party: creating target 'Eigen3::Eigen'")
+
+include(CPM)
+CPMAddPackage(
+    NAME eigen
+    GITLAB_REPOSITORY libeigen/eigen
+    GIT_TAG 3.4.0
+    DOWNLOAD_ONLY ON
+)
 
 add_library(Eigen3_Eigen INTERFACE)
 add_library(Eigen3::Eigen ALIAS Eigen3_Eigen)
 
 include(GNUInstallDirs)
 target_include_directories(Eigen3_Eigen SYSTEM INTERFACE
-    $<BUILD_INTERFACE:${EIGEN_INCLUDE_DIRS}>
+    $<BUILD_INTERFACE:${eigen_SOURCE_DIR}>
     $<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>
 )
-# target_compile_definitions(Eigen3_Eigen INTERFACE EIGEN_MPL2_ONLY)
 
-# if(EIGEN_WITH_MKL)
-#     # TODO: Checks that, on 64bits systems, `mkl::mkl` is using the LP64 interface
-#     # (by looking at the compile definition of the target)
-#     include(mkl)
-#     target_link_libraries(Eigen3_Eigen INTERFACE mkl::mkl)
-#     target_compile_definitions(Eigen3_Eigen INTERFACE
-#         EIGEN_USE_MKL_ALL
-#         EIGEN_USE_LAPACKE_STRICT
-#     )
-# endif()
+if(EIGEN_MPL2_ONLY)
+  target_compile_definitions(Eigen3_Eigen INTERFACE EIGEN_MPL2_ONLY)
+endif()
+
+if(EIGEN_DONT_VECTORIZE)
+  target_compile_definitions(Eigen3_Eigen INTERFACE EIGEN_DONT_VECTORIZE)
+endif()
+
+if(EIGEN_WITH_MKL)
+    # TODO: Checks that, on 64bits systems, `mkl::mkl` is using the LP64 interface
+    # (by looking at the compile definition of the target)
+    include(mkl)
+    target_link_libraries(Eigen3_Eigen INTERFACE mkl::mkl)
+    target_compile_definitions(Eigen3_Eigen INTERFACE
+        EIGEN_USE_MKL_ALL
+        EIGEN_USE_LAPACKE_STRICT
+    )
+endif()
 
 # On Windows, enable natvis files to improve debugging experience
 if(WIN32 AND eigen_SOURCE_DIR)
     target_sources(Eigen3_Eigen INTERFACE $<BUILD_INTERFACE:${eigen_SOURCE_DIR}/debug/msvc/eigen.natvis>)
 endif()
 
 # Install rules
 set(CMAKE_INSTALL_DEFAULT_COMPONENT_NAME eigen)
 set_target_properties(Eigen3_Eigen PROPERTIES EXPORT_NAME Eigen)
-install(DIRECTORY ${EIGEN_INCLUDE_DIRS} DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
+install(DIRECTORY ${eigen_SOURCE_DIR} DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
 install(TARGETS Eigen3_Eigen EXPORT Eigen_Targets)
-install(EXPORT Eigen_Targets DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/eigen NAMESPACE Eigen3::)
+install(EXPORT Eigen_Targets DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/eigen NAMESPACE Eigen3::)
```

### Comparing `ipctk-1.0.0/cmake/recipes/json.cmake` & `ipctk-1.1.0/cmake/recipes/json.cmake`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,29 @@
 # of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
-
-# JSON MIT
 if(TARGET nlohmann_json::nlohmann_json)
     return()
 endif()
 
 message(STATUS "Third-party: creating target 'nlohmann_json::nlohmann_json'")
 
 # nlohmann_json is a big repo for a single header, so we just download the release archive
-set(NLOHMANNJSON_VERSION "v3.10.2")
+set(NLOHMANNJSON_VERSION "v3.11.2")
 
-include(FetchContent)
-FetchContent_Declare(
-    nlohmann_json
+include(CPM)
+CPMAddPackage(
+    NAME nlohmann_json
     URL "https://github.com/nlohmann/json/releases/download/${NLOHMANNJSON_VERSION}/include.zip"
-    URL_HASH SHA256=61e605be15e88deeac4582aaf01c09d616f8302edde7adcaba9261ddc3b4ceca
+    URL_HASH SHA256=e5c7a9f49a16814be27e4ed0ee900ecd0092bfb7dbfca65b5a421b774dccaaed
 )
-FetchContent_MakeAvailable(nlohmann_json)
 
 add_library(nlohmann_json INTERFACE)
 add_library(nlohmann_json::nlohmann_json ALIAS nlohmann_json)
 
 include(GNUInstallDirs)
 target_include_directories(nlohmann_json INTERFACE
     "$<BUILD_INTERFACE:${nlohmann_json_SOURCE_DIR}>/include"
@@ -38,8 +35,8 @@
 )
 
 # Install rules
 set(CMAKE_INSTALL_DEFAULT_COMPONENT_NAME nlohmann_json)
 install(DIRECTORY ${nlohmann_json_SOURCE_DIR}/include/nlohmann DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
 install(TARGETS nlohmann_json EXPORT NlohmannJson_Targets)
 install(EXPORT NlohmannJson_Targets DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/nlohmann_json NAMESPACE nlohmann_json::)
-export(EXPORT NlohmannJson_Targets FILE "${CMAKE_CURRENT_BINARY_DIR}/NlohmannJsonTargets.cmake")
+export(EXPORT NlohmannJson_Targets FILE "${CMAKE_CURRENT_BINARY_DIR}/NlohmannJsonTargets.cmake")
```

### Comparing `ipctk-1.0.0/cmake/recipes/pybind11.cmake` & `ipctk-1.1.0/cmake/recipes/pybind11.cmake`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,14 @@
 #
 if(TARGET pybind11::pybind11)
     return()
 endif()
 
 message(STATUS "Third-party: creating target 'pybind11::pybind11'")
 
-include(FetchContent)
-FetchContent_Declare(
-    pybind11
-    GIT_REPOSITORY https://github.com/pybind/pybind11.git
-    GIT_TAG v2.9.2
-    GIT_SHALLOW TRUE
-)
-
 if (POLICY CMP0094)  # https://cmake.org/cmake/help/latest/policy/CMP0094.html
     cmake_policy(SET CMP0094 NEW)  # FindPython should return the first matching Python
 endif ()
 
 # needed on GitHub Actions CI: actions/setup-python does not touch registry/frameworks on Windows/macOS
 # this mirrors PythonInterp behavior which did not consult registry/frameworks first
 if (NOT DEFINED Python_FIND_REGISTRY)
@@ -38,8 +30,9 @@
 
 # Pybind11 still uses the deprecated FindPythonInterp. So let's call CMake's
 # new FindPython module and set PYTHON_EXECUTABLE for Pybind11 to pick up.
 # This works well with conda environments.
 find_package(Python COMPONENTS Interpreter Development.Module REQUIRED)
 set(PYTHON_EXECUTABLE ${Python_EXECUTABLE})
 
-FetchContent_MakeAvailable(pybind11)
+include(CPM)
+CPMAddPackage("gh:pybind/pybind11@2.10.3")
```

### Comparing `ipctk-1.0.0/cmake/recipes/spdlog.cmake` & `ipctk-1.1.0/cmake/recipes/spdlog.cmake`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,19 @@
 #
 if(TARGET spdlog::spdlog)
     return()
 endif()
 
 message(STATUS "Third-party: creating target 'spdlog::spdlog'")
 
-include(FetchContent)
-FetchContent_Declare(
-    spdlog
-    GIT_REPOSITORY https://github.com/gabime/spdlog.git
-    GIT_TAG v1.10.0
-    GIT_SHALLOW TRUE
-)
-
 option(SPDLOG_INSTALL "Generate the install target" ON)
 set(CMAKE_INSTALL_DEFAULT_COMPONENT_NAME "spdlog")
-FetchContent_MakeAvailable(spdlog)
+
+include(CPM)
+CPMAddPackage("gh:gabime/spdlog@1.11.0")
 
 set_target_properties(spdlog PROPERTIES POSITION_INDEPENDENT_CODE ON)
 
 set_target_properties(spdlog PROPERTIES FOLDER external)
 
 if("${CMAKE_CXX_COMPILER_ID}" STREQUAL "AppleClang" OR
    "${CMAKE_CXX_COMPILER_ID}" STREQUAL "Clang")
```

### Comparing `ipctk-1.0.0/docs/PYPI_README.md` & `ipctk-1.1.0/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/pyproject.toml` & `ipctk-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,44 +5,32 @@
     "ninja",
     # "cmake>=3.14",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ipctk"
-version = "1.0.0"
-authors = [
-  { name="Zachary Ferguson", email="zfergus@nyu.edu" },
-]
+version = "1.1.0"
+authors = [{ name = "Zachary Ferguson", email = "zfergus@nyu.edu" }]
 description = "A set of reusable functions to integrate Incremental Potential Contact (IPC) into a simulation."
 readme = "docs/PYPI_README.md"
-license = { file="LICENSE" }
+license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: C++",
     "Programming Language :: Python :: 3",
     "Topic :: Games/Entertainment :: Simulation",
     "Topic :: Scientific/Engineering :: Physics",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
 ]
 requires-python = ">=3.6"
-dependencies = [
-    "numpy",
-    "scipy",
-]
-keywords = [
-    "IPC",
-    "simulation",
-    "physics",
-    "science",
-    "reserch",
-]
+dependencies = ["numpy", "scipy"]
+keywords = ["IPC", "simulation", "physics", "science", "reserch"]
 
 [project.urls]
 "Homepage" = "https://ipc-sim.github.io/ipc-toolkit/"
 "Bug Tracker" = "https://github.com/ipc-sim/ipc-toolkit/issues"
 "Source Code" = "https://github.com/ipc-sim/ipc-toolkit"
 
 [tools.cibuildwheel]
 build-frontend = "build"
-
```

### Comparing `ipctk-1.0.0/python/CMakeLists.txt` & `ipctk-1.1.0/python/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -13,55 +13,73 @@
   src/broad_phase/brute_force.cpp
   src/broad_phase/hash_grid.cpp
   src/broad_phase/spatial_hash.cpp
   src/broad_phase/sweep_and_tiniest_queue.cpp
   src/broad_phase/voxel_size_heuristic.cpp
 
   src/candidates/candidates.cpp
+  src/candidates/collision_stencil.cpp
   src/candidates/continuous_collision_candidate.cpp
   src/candidates/edge_edge.cpp
   src/candidates/edge_face.cpp
   src/candidates/edge_vertex.cpp
   src/candidates/face_vertex.cpp
   src/candidates/vertex_vertex.cpp
 
   src/ccd/aabb.cpp
   src/ccd/ccd.cpp
   src/ccd/inexact_point_edge.cpp
   src/ccd/point_static_plane.cpp
 
+  src/collisions/collision_constraint.cpp
+  src/collisions/collision_constraints.cpp
+  src/collisions/edge_edge.cpp
+  src/collisions/edge_vertex.cpp
+  src/collisions/face_vertex.cpp
+  src/collisions/plane_vertex.cpp
+  src/collisions/vertex_vertex.cpp
+
   src/distance/distance_type.cpp
   src/distance/edge_edge.cpp
   src/distance/edge_edge_mollifier.cpp
   src/distance/line_line.cpp
   src/distance/point_edge.cpp
   src/distance/point_line.cpp
   src/distance/point_plane.cpp
   src/distance/point_point.cpp
   src/distance/point_triangle.cpp
 
   src/friction/closest_point.cpp
-  src/friction/friction_constraint.cpp
-  src/friction/friction.cpp
+  src/friction/friction_constraints.cpp
   src/friction/normal_force_magnitude.cpp
-  src/friction/relative_displacement.cpp
+  src/friction/relative_velocity.cpp
   src/friction/smooth_friction_mollifier.cpp
   src/friction/tangent_basis.cpp
 
+  src/friction/constraints/edge_edge.cpp
+  src/friction/constraints/edge_vertex.cpp
+  src/friction/constraints/face_vertex.cpp
+  src/friction/constraints/friction_constraint.cpp
+  src/friction/constraints/vertex_vertex.cpp
+
+  src/implicits/plane.cpp
+
+  src/utils/area_gradient.cpp
   src/utils/eigen_ext.cpp
   src/utils/intersection.cpp
   src/utils/logger.cpp
   src/utils/thread_limiter.cpp
+  src/utils/vertex_to_min_edge.cpp
   src/utils/world_bbox_diagonal_length.cpp
 
-  src/collision_constraint.cpp
   src/collision_mesh.cpp
   src/ipc.cpp
 )
 
 target_link_libraries(ipctk PRIVATE ipc::toolkit)
+target_include_directories(ipctk PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}/src")
 
 # Extra warnings
 # target_link_libraries(ipctk PRIVATE IPCToolkit::warnings)
 
 # Move Python library to build root
 set_target_properties(ipctk PROPERTIES LIBRARY_OUTPUT_PATH "${CMAKE_BINARY_DIR}")
```

### Comparing `ipctk-1.0.0/python/src/barrier/adaptive_stiffness.cpp` & `ipctk-1.1.0/python/src/barrier/adaptive_stiffness.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/barrier/adaptive_stiffness.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_adaptive_stiffness(py::module_& m)
```

### Comparing `ipctk-1.0.0/python/src/barrier/barrier.cpp` & `ipctk-1.1.0/python/src/barrier/barrier.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/barrier/barrier.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_barrier(py::module_& m)
 {
     m.def(
-        "barrier", &barrier<double>,
+        "barrier", &barrier,
         R"ipc_Qu8mg5v7(
         Function that grows to infinity as d approaches 0 from the right.
 
         .. math:: b(d) = -(d-\hat{d})^2\ln\left(\frac{d}{\hat{d}}\right)
 
         Parameters:
             d: distance
```

### Comparing `ipctk-1.0.0/python/src/broad_phase/aabb.cpp` & `ipctk-1.1.0/python/src/broad_phase/aabb.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/broad_phase/aabb.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_aabb(py::module_& m)
@@ -16,29 +16,31 @@
             py::init<const AABB&, const AABB&>(), "", py::arg("aabb1"),
             py::arg("aabb2"))
         .def(
             py::init<const AABB&, const AABB&, const AABB&>(), "",
             py::arg("aabb1"), py::arg("aabb2"), py::arg("aabb3"))
         .def_static(
             "from_point",
-            py::overload_cast<const VectorMax3d&, double>(&AABB::from_point),
+            py::overload_cast<const VectorMax3d&, const double>(
+                &AABB::from_point),
             R"ipc_Qu8mg5v7(
             Compute a AABB for a static point.
 
             Parameters:
                 p: The point's position.
                 inflation_radius: Radius of a sphere around the point which the AABB encloses.
 
             Returns:
                 The constructed AABB.
             )ipc_Qu8mg5v7",
             py::arg("p"), py::arg("inflation_radius") = 0)
         .def_static(
             "from_point",
-            py::overload_cast<const VectorMax3d&, const VectorMax3d&, double>(
+            py::overload_cast<
+                const VectorMax3d&, const VectorMax3d&, const double>(
                 &AABB::from_point),
             R"ipc_Qu8mg5v7(
             Compute a AABB for a moving point (i.e. temporal edge).
 
             Parameters:
                 p_t0: The point's position at time t=0.
                 p_t1: The point's position at time t=1.
@@ -56,51 +58,64 @@
             Parameters:
                 other: The other AABB.
 
             Returns:
                 If the two AABBs intersect.
             )ipc_Qu8mg5v7",
             py::arg("other"))
+        .def_static(
+            "conservative_inflation",
+            [](ArrayMax3d min, ArrayMax3d max, const double inflation_radius) {
+                AABB::conservative_inflation(min, max, inflation_radius);
+                return std::make_tuple(min, max);
+            },
+            "Compute a conservative inflation of the AABB.", py::arg("min"),
+            py::arg("max"), py::arg("inflation_radius"))
         .def_readwrite("min", &AABB::min, "Minimum corner of the AABB.")
         .def_readwrite("max", &AABB::max, "Maximum corner of the AABB.")
         .def_readwrite(
             "vertex_ids", &AABB::vertex_ids,
             "Vertex IDs attached to the AABB.");
 
     m.def(
         "build_vertex_boxes",
-        [](const Eigen::MatrixXd& V, double inflation_radius = 0) {
+        [](const Eigen::MatrixXd& vertices, const double inflation_radius = 0) {
             std::vector<AABB> vertex_boxes;
-            build_vertex_boxes(V, vertex_boxes, inflation_radius);
+            build_vertex_boxes(vertices, vertex_boxes, inflation_radius);
             return vertex_boxes;
         },
-        "Build one AABB per vertex position (row of V).", py::arg("V"),
+        "Build one AABB per vertex position (row of V).", py::arg("vertices"),
         py::arg("inflation_radius") = 0);
 
     m.def(
         "build_vertex_boxes",
-        [](const Eigen::MatrixXd& V0, const Eigen::MatrixXd& V1,
-           double inflation_radius = 0) {
+        [](const Eigen::MatrixXd& vertices_t0,
+           const Eigen::MatrixXd& vertices_t1,
+           const double inflation_radius = 0) {
             std::vector<AABB> vertex_boxes;
-            build_vertex_boxes(V0, V1, vertex_boxes, inflation_radius);
+            build_vertex_boxes(
+                vertices_t0, vertices_t1, vertex_boxes, inflation_radius);
             return vertex_boxes;
         },
-        "", py::arg("V0"), py::arg("V1"), py::arg("inflation_radius") = 0);
+        "", py::arg("vertices_t0"), py::arg("vertices_t1"),
+        py::arg("inflation_radius") = 0);
 
     m.def(
         "build_edge_boxes",
-        [](const std::vector<AABB>& vertex_boxes, const Eigen::MatrixXi& E) {
+        [](const std::vector<AABB>& vertex_boxes,
+           const Eigen::MatrixXi& edges) {
             std::vector<AABB> edge_boxes;
-            build_edge_boxes(vertex_boxes, E, edge_boxes);
+            build_edge_boxes(vertex_boxes, edges, edge_boxes);
             return edge_boxes;
         },
-        "", py::arg("vertex_boxes"), py::arg("E"));
+        "", py::arg("vertex_boxes"), py::arg("edges"));
 
     m.def(
         "build_face_boxes",
-        [](const std::vector<AABB>& vertex_boxes, const Eigen::MatrixXi& F) {
+        [](const std::vector<AABB>& vertex_boxes,
+           const Eigen::MatrixXi& faces) {
             std::vector<AABB> face_boxes;
-            build_face_boxes(vertex_boxes, F, face_boxes);
+            build_face_boxes(vertex_boxes, faces, face_boxes);
             return face_boxes;
         },
-        "", py::arg("vertex_boxes"), py::arg("F"));
+        "", py::arg("vertex_boxes"), py::arg("faces"));
 }
```

### Comparing `ipctk-1.0.0/python/src/broad_phase/broad_phase.cpp` & `ipctk-1.1.0/python/src/broad_phase/broad_phase.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/broad_phase/broad_phase.hpp>
+#include <ipc/candidates/candidates.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_broad_phase(py::module_& m)
 {
     py::enum_<BroadPhaseMethod>(
@@ -12,68 +13,66 @@
         "Enumeration of implemented broad phase methods.")
         .value("BRUTE_FORCE", BroadPhaseMethod::BRUTE_FORCE, "")
         .value("HASH_GRID", BroadPhaseMethod::HASH_GRID, "")
         .value("SPATIAL_HASH", BroadPhaseMethod::SPATIAL_HASH, "")
         .value(
             "SWEEP_AND_TINIEST_QUEUE",
             BroadPhaseMethod::SWEEP_AND_TINIEST_QUEUE, "")
-#ifdef IPC_TOOLKIT_WITH_CUDA
         .value(
             "SWEEP_AND_TINIEST_QUEUE_GPU",
             BroadPhaseMethod::SWEEP_AND_TINIEST_QUEUE_GPU, "")
-#endif
         .export_values();
 
     py::class_<BroadPhase>(m, "BroadPhase")
         .def_static(
             "make_broad_phase", &BroadPhase::make_broad_phase,
             R"ipc_Qu8mg5v7(
             Construct a registered broad phase object.
 
             Parameters:
-                method: The broad phase method to use.
+                broad_phase_method: The broad phase method to use.
 
             Returns:
                 The constructed broad phase object.
             )ipc_Qu8mg5v7",
-            py::arg("method"))
+            py::arg("broad_phase_method"))
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXi&,
                 const Eigen::MatrixXi&, double>(&BroadPhase::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for static collision detection.
 
             Parameters:
-                V0: Positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices: Vertex positions
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V"), py::arg("E"), py::arg("F"),
+            py::arg("vertices"), py::arg("edges"), py::arg("faces"),
             py::arg("inflation_radius") = 0)
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXd&,
                 const Eigen::MatrixXi&, const Eigen::MatrixXi&, double>(
                 &BroadPhase::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for continuous collision detection.
 
             Parameters:
-                V0: Starting positions of the vertices.
-                V1: Ending positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices_t0: Starting vertices of the vertices.
+                vertices_t1: Ending vertices of the vertices.
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("inflation_radius") = 0)
+            py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
+            py::arg("faces"), py::arg("inflation_radius") = 0)
         .def("clear", &BroadPhase::clear, "Clear any built data.")
         .def(
             "detect_edge_vertex_candidates",
             [](BroadPhase& self) {
                 std::vector<EdgeVertexCandidate> candidates;
                 self.detect_edge_vertex_candidates(candidates);
                 return candidates;
@@ -131,69 +130,13 @@
                 return candidates;
             },
             R"ipc_Qu8mg5v7(
             Detect all collision candidates needed for a given dimensional simulation.
 
             Parameters:
                 dim: The dimension of the simulation (i.e., 2 or 3).
-                candidates: The detected collision candidates.
             )ipc_Qu8mg5v7",
             py::arg("dim"))
         .def_readwrite(
             "can_vertices_collide", &BroadPhase::can_vertices_collide,
             "Function for determining if two vertices can collide.");
-
-    m.def(
-        "construct_collision_candidates",
-        [](const CollisionMesh& mesh, const Eigen::MatrixXd& V,
-           double inflation_radius = 0,
-           const BroadPhaseMethod method = BroadPhaseMethod::HASH_GRID) {
-            Candidates candidates;
-            construct_collision_candidates(
-                mesh, V, candidates, inflation_radius, method);
-            return candidates;
-        },
-        R"ipc_Qu8mg5v7(
-        Construct a set of discrete collision detection candidates.
-
-        Parameters:
-            mesh: The surface of the contact mesh.
-            V: Surface Vertex positions at start as rows of a matrix.
-            inflation_radius: Amount to inflate the bounding boxes.
-            method: Broad phase method to use.
-
-        Returns:
-            The constructed candidate set as output.
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V"), py::arg("inflation_radius") = 0,
-        py::arg("method") = BroadPhaseMethod::HASH_GRID);
-
-    m.def(
-        "construct_collision_candidates",
-        [](const CollisionMesh& mesh, const Eigen::MatrixXd& V0,
-           const Eigen::MatrixXd& V1, double inflation_radius = 0,
-           const BroadPhaseMethod method = BroadPhaseMethod::HASH_GRID) {
-            Candidates candidates;
-            construct_collision_candidates(
-                mesh, V0, V1, candidates, inflation_radius, method);
-            return candidates;
-        },
-        R"ipc_Qu8mg5v7(
-        Construct a set of continuous collision detection candidates.
-
-        Note:
-            Assumes the trajectory is linear.
-
-        Parameters:
-            mesh: The surface of the contact mesh.
-            V0: Surface vertex positions at start as rows of a matrix.
-            V1: Surface vertex positions at end as rows of a matrix.
-            inflation_radius: Amount to inflate the bounding boxes.
-            method: Broad phase method to use.
-
-        Returns:
-            The constructed candidate set as output.
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V0"), py::arg("V1"),
-        py::arg("inflation_radius") = 0,
-        py::arg("method") = BroadPhaseMethod::HASH_GRID);
 }
```

### Comparing `ipctk-1.0.0/python/src/broad_phase/brute_force.cpp` & `ipctk-1.1.0/python/src/broad_phase/brute_force.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/broad_phase/brute_force.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_brute_force(py::module_& m)
```

### Comparing `ipctk-1.0.0/python/src/broad_phase/hash_grid.cpp` & `ipctk-1.1.0/python/src/broad_phase/hash_grid.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/broad_phase/hash_grid.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_hash_grid(py::module_& m)
@@ -25,39 +25,39 @@
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXi&,
                 const Eigen::MatrixXi&, double>(&HashGrid::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for static collision detection.
 
             Parameters:
-                V0: Positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices_t0: Vertex positions
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V"), py::arg("E"), py::arg("F"),
+            py::arg("vertices"), py::arg("edges"), py::arg("faces"),
             py::arg("inflation_radius") = 0)
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXd&,
                 const Eigen::MatrixXi&, const Eigen::MatrixXi&, double>(
                 &HashGrid::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for continuous collision detection.
 
             Parameters:
-                V0: Starting positions of the vertices.
-                V1: Ending positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices_t0: Starting vertices of the vertices.
+                vertices_t1: Ending vertices of the vertices.
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("inflation_radius") = 0)
+            py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
+            py::arg("faces"), py::arg("inflation_radius") = 0)
         .def("clear", &HashGrid::clear, "Clear the hash grid.")
         .def(
             "detect_edge_vertex_candidates",
             [](HashGrid& self) {
                 std::vector<EdgeVertexCandidate> candidates;
                 self.detect_edge_vertex_candidates(candidates);
                 return candidates;
```

### Comparing `ipctk-1.0.0/python/src/broad_phase/spatial_hash.cpp` & `ipctk-1.1.0/python/src/broad_phase/spatial_hash.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/broad_phase/spatial_hash.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_spatial_hash(py::module_& m)
 {
     py::class_<SpatialHash, BroadPhase>(m, "SpatialHash")
         .def(py::init())
         .def(
             py::init<
                 const Eigen::MatrixXd&, const Eigen::MatrixXi&,
                 const Eigen::MatrixXi&, double, double>(),
-            "", py::arg("V"), py::arg("E"), py::arg("F"),
+            "", py::arg("vertices"), py::arg("edges"), py::arg("faces"),
             py::arg("inflation_radius") = 0, py::arg("voxelSize") = -1)
         .def(
             py::init<
                 const Eigen::MatrixXd&, const Eigen::MatrixXd&,
                 const Eigen::MatrixXi&, const Eigen::MatrixXi&, double,
                 double>(),
-            "", py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("inflation_radius") = 0, py::arg("voxelSize") = -1)
+            "", py::arg("vertices_t0"), py::arg("vertices_t1"),
+            py::arg("edges"), py::arg("faces"), py::arg("inflation_radius") = 0,
+            py::arg("voxelSize") = -1)
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXi&,
                 const Eigen::MatrixXi&, double>(&SpatialHash::build),
-            "", py::arg("V"), py::arg("E"), py::arg("F"),
+            "", py::arg("vertices"), py::arg("edges"), py::arg("faces"),
             py::arg("inflation_radius") = 0)
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXd&,
                 const Eigen::MatrixXi&, const Eigen::MatrixXi&, double>(
                 &SpatialHash::build),
-            "", py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("inflation_radius") = 0)
+            "", py::arg("vertices_t0"), py::arg("vertices_t1"),
+            py::arg("edges"), py::arg("faces"), py::arg("inflation_radius") = 0)
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXi&,
                 const Eigen::MatrixXi&, double, double>(&SpatialHash::build),
-            "", py::arg("V"), py::arg("E"), py::arg("F"),
+            "", py::arg("vertices"), py::arg("edges"), py::arg("faces"),
             py::arg("inflation_radius"), py::arg("voxelSize"))
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXd&,
                 const Eigen::MatrixXi&, const Eigen::MatrixXi&, double, double>(
                 &SpatialHash::build),
-            "", py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("inflation_radius"), py::arg("voxelSize"))
+            "", py::arg("vertices_t0"), py::arg("vertices_t1"),
+            py::arg("edges"), py::arg("faces"), py::arg("inflation_radius"),
+            py::arg("voxelSize"))
         .def("clear", &SpatialHash::clear, "")
         .def(
             "queryPointForTriangles",
             [](SpatialHash& self, const VectorMax3d& p, double radius = 0) {
                 unordered_set<int> triInds;
                 self.queryPointForTriangles(p, triInds, radius);
                 return triInds;
@@ -100,24 +102,24 @@
                 self.queryEdgeForEdges(ea0, ea1, edgeInds, radius, eai);
                 return edgeInds;
             },
             "", py::arg("ea0"), py::arg("ea1"), py::arg("radius") = 0,
             py::arg("eai") = -1)
         .def(
             "queryEdgeForEdgesWithBBoxCheck",
-            [](SpatialHash& self, const Eigen::MatrixXd& V,
-               const Eigen::MatrixXi& E, const VectorMax3d& ea0,
+            [](SpatialHash& self, const Eigen::MatrixXd& vertices,
+               const Eigen::MatrixXi& edges, const VectorMax3d& ea0,
                const VectorMax3d& ea1, double radius = 0, int eai = -1) {
                 std::vector<int> edgeInds;
                 self.queryEdgeForEdgesWithBBoxCheck(
-                    V, E, ea0, ea1, edgeInds, radius, eai);
+                    vertices, edges, ea0, ea1, edgeInds, radius, eai);
                 return edgeInds;
             },
-            "", py::arg("V"), py::arg("E"), py::arg("ea0"), py::arg("ea1"),
-            py::arg("radius") = 0, py::arg("eai") = -1)
+            "", py::arg("vertices"), py::arg("edges"), py::arg("ea0"),
+            py::arg("ea1"), py::arg("radius") = 0, py::arg("eai") = -1)
         .def(
             "queryEdgeForEdges",
             [](SpatialHash& self, const VectorMax3d& ea0_t0,
                const VectorMax3d& ea1_t0, const VectorMax3d& ea0_t1,
                const VectorMax3d& ea1_t1, double radius = 0, int eai = -1) {
                 std::vector<int> edgeInds;
                 self.queryEdgeForEdges(
@@ -202,21 +204,24 @@
                 unordered_set<int> edgeInds;
                 self.queryEdgeForEdges(eai, edgeInds);
                 return edgeInds;
             },
             "", py::arg("eai"))
         .def(
             "queryEdgeForEdgesWithBBoxCheck",
-            [](SpatialHash& self, const Eigen::MatrixXd& V0,
-               const Eigen::MatrixXd& V1, const Eigen::MatrixXi& E, int eai) {
+            [](SpatialHash& self, const Eigen::MatrixXd& vertices_t0,
+               const Eigen::MatrixXd& vertices_t1, const Eigen::MatrixXi& edges,
+               int eai) {
                 unordered_set<int> edgeInds;
-                self.queryEdgeForEdgesWithBBoxCheck(V0, V1, E, eai, edgeInds);
+                self.queryEdgeForEdgesWithBBoxCheck(
+                    vertices_t0, vertices_t1, edges, eai, edgeInds);
                 return edgeInds;
             },
-            "", py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("eai"))
+            "", py::arg("vertices_t0"), py::arg("vertices_t1"),
+            py::arg("edges"), py::arg("eai"))
         .def(
             "queryEdgeForTriangles",
             [](SpatialHash& self, int ei) {
                 unordered_set<int> triInds;
                 self.queryEdgeForTriangles(ei, triInds);
                 return triInds;
             },
```

### Comparing `ipctk-1.0.0/python/src/broad_phase/sweep_and_tiniest_queue.cpp` & `ipctk-1.1.0/python/src/broad_phase/sweep_and_tiniest_queue.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/broad_phase/sweep_and_tiniest_queue.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_sweep(py::module_& m)
@@ -17,39 +17,39 @@
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXi&,
                 const Eigen::MatrixXi&, double>(&SweepAndTiniestQueue::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for static collision detection.
 
             Parameters:
-                V0: Positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices: Vertex positions
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V"), py::arg("E"), py::arg("F"),
+            py::arg("vertices"), py::arg("edges"), py::arg("faces"),
             py::arg("inflation_radius") = 0)
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXd&,
                 const Eigen::MatrixXi&, const Eigen::MatrixXi&, double>(
                 &SweepAndTiniestQueue::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for continuous collision detection.
 
             Parameters:
-                V0: Starting positions of the vertices.
-                V1: Ending positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices_t0: Starting vertex positions
+                vertices_t1: Ending vertex positions
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("inflation_radius") = 0)
+            py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
+            py::arg("faces"), py::arg("inflation_radius") = 0)
         .def("clear", &SweepAndTiniestQueue::clear, "Clear any built data.")
         .def(
             "detect_edge_vertex_candidates",
             [](SweepAndTiniestQueue& self) {
                 std::vector<EdgeVertexCandidate> candidates;
                 self.detect_edge_vertex_candidates(candidates);
                 return candidates;
@@ -110,39 +110,39 @@
                 const Eigen::MatrixXd&, const Eigen::MatrixXi&,
                 const Eigen::MatrixXi&, double>(
                 &SweepAndTiniestQueueGPU::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for static collision detection.
 
             Parameters:
-                V0: Positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices: Vertex positions
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V"), py::arg("E"), py::arg("F"),
+            py::arg("vertices"), py::arg("edges"), py::arg("faces"),
             py::arg("inflation_radius") = 0)
         .def(
             "build",
             py::overload_cast<
                 const Eigen::MatrixXd&, const Eigen::MatrixXd&,
                 const Eigen::MatrixXi&, const Eigen::MatrixXi&, double>(
                 &SweepAndTiniestQueueGPU::build),
             R"ipc_Qu8mg5v7(
             Build the broad phase for continuous collision detection.
 
             Parameters:
-                V0: Starting positions of the vertices.
-                V1: Ending positions of the vertices.
-                E: Edges of the mesh.
-                F: Faces of the mesh.
+                vertices_t0: Starting vertex positions
+                vertices_t1: Ending vertex positions
+                edges: Collision mesh edges
+                faces: Collision mesh faces
                 inflation_radius: Radius of inflation around all elements.
             )ipc_Qu8mg5v7",
-            py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("inflation_radius") = 0)
+            py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
+            py::arg("faces"), py::arg("inflation_radius") = 0)
         .def("clear", &SweepAndTiniestQueueGPU::clear, "Clear any built data.")
         .def(
             "detect_edge_vertex_candidates",
             [](SweepAndTiniestQueueGPU& self) {
                 std::vector<EdgeVertexCandidate> candidates;
                 self.detect_edge_vertex_candidates(candidates);
                 return candidates;
```

### Comparing `ipctk-1.0.0/python/src/broad_phase/voxel_size_heuristic.cpp` & `ipctk-1.1.0/python/src/broad_phase/voxel_size_heuristic.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,64 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/broad_phase/voxel_size_heuristic.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_voxel_size_heuristic(py::module_& m)
 {
     m.def(
         "suggest_good_voxel_size",
         py::overload_cast<
             const Eigen::MatrixXd&, const Eigen::MatrixXi&, double>(
             &suggest_good_voxel_size),
-        "", py::arg("V"), py::arg("E"), py::arg("inflation_radius") = 0);
+        "", py::arg("vertices"), py::arg("edges"),
+        py::arg("inflation_radius") = 0);
 
     m.def(
         "suggest_good_voxel_size",
         py::overload_cast<
             const Eigen::MatrixXd&, const Eigen::MatrixXd&,
             const Eigen::MatrixXi&, double>(&suggest_good_voxel_size),
-        "", py::arg("V0"), py::arg("V1"), py::arg("E"),
+        "", py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
         py::arg("inflation_radius") = 0);
 
     m.def(
         "mean_edge_length",
-        [](const Eigen::MatrixXd& V0, const Eigen::MatrixXd& V1,
-           const Eigen::MatrixXi& E) {
+        [](const Eigen::MatrixXd& vertices_t0,
+           const Eigen::MatrixXd& vertices_t1, const Eigen::MatrixXi& edges) {
             double std_deviation;
-            double r = mean_edge_length(V0, V1, E, std_deviation);
+            double r = mean_edge_length(
+                vertices_t0, vertices_t1, edges, std_deviation);
             return std::make_tuple(r, std_deviation);
         },
-        "Compute the average edge length of a mesh.", py::arg("V0"),
-        py::arg("V1"), py::arg("E"));
+        "Compute the average edge length of a mesh.", py::arg("vertices_t0"),
+        py::arg("vertices_t1"), py::arg("edges"));
 
     m.def(
         "mean_displacement_length",
-        [](const Eigen::MatrixXd& U) {
+        [](const Eigen::MatrixXd& displacements) {
             double std_deviation;
-            double r = mean_displacement_length(U, std_deviation);
+            double r = mean_displacement_length(displacements, std_deviation);
             return std::make_tuple(r, std_deviation);
         },
-        "Compute the average displacement length.", py::arg("U"));
+        "Compute the average displacement length.", py::arg("displacements"));
 
     m.def(
         "median_edge_length", &median_edge_length,
-        "Compute the median edge length of a mesh.", py::arg("V0"),
-        py::arg("V1"), py::arg("E"));
+        "Compute the median edge length of a mesh.", py::arg("vertices_t0"),
+        py::arg("vertices_t1"), py::arg("edges"));
 
     m.def(
         "median_displacement_length", &median_displacement_length,
-        "Compute the median displacement length.", py::arg("U"));
+        "Compute the median displacement length.", py::arg("displacements"));
+
+    m.def(
+        "max_edge_length", &max_edge_length,
+        "Compute the maximum edge length of a mesh.", py::arg("vertices_t0"),
+        py::arg("vertices_t1"), py::arg("edges"));
+
+    m.def(
+        "max_displacement_length", &max_displacement_length,
+        "Compute the maximum displacement length.", py::arg("displacements"));
 }
```

### Comparing `ipctk-1.0.0/python/src/candidates/continuous_collision_candidate.cpp` & `ipctk-1.1.0/python/src/candidates/continuous_collision_candidate.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/candidates/continuous_collision_candidate.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_continuous_collision_candidate(py::module_& m)
 {
     py::class_<ContinuousCollisionCandidate>(m, "ContinuousCollisionCandidate")
         .def(
             "ccd",
-            [](ContinuousCollisionCandidate& self, const Eigen::MatrixXd& V0,
-               const Eigen::MatrixXd& V1, const Eigen::MatrixXi& E,
-               const Eigen::MatrixXi& F, const double min_distance = 0.0,
+            [](ContinuousCollisionCandidate& self,
+               const Eigen::MatrixXd& vertices_t0,
+               const Eigen::MatrixXd& vertices_t1, const Eigen::MatrixXi& edges,
+               const Eigen::MatrixXi& faces, const double min_distance = 0.0,
                const double tmax = 1.0,
                const double tolerance = DEFAULT_CCD_TOLERANCE,
                const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
                const double conservative_rescaling =
                    DEFAULT_CCD_CONSERVATIVE_RESCALING) {
                 double toi;
                 bool r = self.ccd(
-                    V0, V1, E, F, toi, tmax, tolerance, max_iterations,
-                    conservative_rescaling);
+                    vertices_t0, vertices_t1, edges, faces, toi, min_distance,
+                    tmax, tolerance, max_iterations, conservative_rescaling);
                 return std::make_tuple(r, toi);
             },
             R"ipc_Qu8mg5v7(
             Perform narrow-phase CCD on the candidate.
 
             Parameters:
-                V0: Mesh vertex positions at the start of the time step.
-                V1: Mesh vertex positions at the end of the time step.
-                E: Mesh edges as rows of indicies into V.
-                F: Mesh triangular faces as rows of indicies into V.
+                vertices_t0: Mesh vertices at the start of the time step.
+                vertices_t1: Mesh vertices at the end of the time step.
+                edges: Collision mesh edges as rows of indicies into vertices.
+                faces: Collision mesh triangular faces as rows of indicies into vertices.
+                min_distance: Minimum separation distance between primitives.
                 tmax: Maximum time (normalized) to look for collisions. Should be in [0, 1].
                 tolerance: CCD tolerance used by Tight-Inclusion CCD.
                 max_iterations: Maximum iterations used by Tight-Inclusion CCD.
                 conservative_rescaling: Conservative rescaling value used to avoid taking steps exactly to impact.
 
             Returns:
                 Tuple of:
                 If the candidate had a collision over the time interval.
                 Computed time of impact (normalized).
             )ipc_Qu8mg5v7",
-            py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("min_distance") = 0.0, py::arg("tmax") = 1.0,
-            py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
+            py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
+            py::arg("faces"), py::arg("min_distance") = 0.0,
+            py::arg("tmax") = 1.0, py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
             py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
             py::arg("conservative_rescaling") =
                 DEFAULT_CCD_CONSERVATIVE_RESCALING)
         .def(
             "print_ccd_query", &ContinuousCollisionCandidate::print_ccd_query,
-            "", py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"));
+            "", py::arg("vertices_t0"), py::arg("vertices_t1"),
+            py::arg("edges"), py::arg("faces"));
 }
```

### Comparing `ipctk-1.0.0/python/src/candidates/edge_edge.cpp` & `ipctk-1.1.0/python/src/candidates/edge_edge.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,84 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/candidates/edge_edge.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_edge_edge_candidate(py::module_& m)
 {
-    py::class_<EdgeEdgeCandidate, ContinuousCollisionCandidate>(
+    py::class_<
+        EdgeEdgeCandidate, CollisionStencil, ContinuousCollisionCandidate>(
         m, "EdgeEdgeCandidate")
         .def(
-            py::init<long, long>(), "", py::arg("edge0_index"),
-            py::arg("edge1_index"))
+            py::init<long, long>(), "", py::arg("edge0_id"),
+            py::arg("edge1_id"))
         .def(
             "__str__",
             [](const EdgeEdgeCandidate& ev) {
-                return fmt::format(
-                    "[{:d}, {:d}]", ev.edge0_index, ev.edge1_index);
+                return fmt::format("[{:d}, {:d}]", ev.edge0_id, ev.edge1_id);
             })
         .def(
             "__repr__",
             [](const EdgeEdgeCandidate& ev) {
                 return fmt::format(
-                    "EdgeEdgeCandidate({:d}, {:d})", ev.edge0_index,
-                    ev.edge1_index);
+                    "EdgeEdgeCandidate({:d}, {:d})", ev.edge0_id, ev.edge1_id);
             })
         .def("num_vertices", &EdgeEdgeCandidate::num_vertices, "")
         .def(
-            "vertex_indices", &EdgeEdgeCandidate::vertex_indices, "",
-            py::arg("E"), py::arg("F"))
-        .def(
-            "compute_distance", &EdgeEdgeCandidate::compute_distance, "",
-            py::arg("V"), py::arg("E"), py::arg("F"),
-            py::arg("dtype") = EdgeEdgeDistanceType::AUTO)
-        .def(
-            "compute_distance_gradient",
-            &EdgeEdgeCandidate::compute_distance_gradient, "", py::arg("V"),
-            py::arg("E"), py::arg("F"),
-            py::arg("dtype") = EdgeEdgeDistanceType::AUTO)
-        .def(
-            "compute_distance_hessian",
-            &EdgeEdgeCandidate::compute_distance_hessian, "", py::arg("V"),
-            py::arg("E"), py::arg("F"),
-            py::arg("dtype") = EdgeEdgeDistanceType::AUTO)
+            "vertex_ids", &EdgeEdgeCandidate::vertex_ids, "", py::arg("edges"),
+            py::arg("faces"))
         .def(
             "ccd",
-            [](EdgeEdgeCandidate& self, const Eigen::MatrixXd& V0,
-               const Eigen::MatrixXd& V1, const Eigen::MatrixXi& E,
-               const Eigen::MatrixXi& F, const double min_distance = 0.0,
+            [](EdgeEdgeCandidate& self, const Eigen::MatrixXd& vertices_t0,
+               const Eigen::MatrixXd& vertices_t1, const Eigen::MatrixXi& edges,
+               const Eigen::MatrixXi& faces, const double min_distance = 0.0,
                const double tmax = 1.0,
                const double tolerance = DEFAULT_CCD_TOLERANCE,
                const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
                const double conservative_rescaling =
                    DEFAULT_CCD_CONSERVATIVE_RESCALING) {
                 double toi;
                 bool r = self.ccd(
-                    V0, V1, E, F, toi, tmax, tolerance, max_iterations,
-                    conservative_rescaling);
+                    vertices_t0, vertices_t1, edges, faces, toi, min_distance,
+                    tmax, tolerance, max_iterations, conservative_rescaling);
                 return std::make_tuple(r, toi);
             },
             R"ipc_Qu8mg5v7(
             Perform narrow-phase CCD on the candidate.
 
             Parameters:
-                V0: Mesh vertex positions at the start of the time step.
-                V1: Mesh vertex positions at the end of the time step.
-                E: Mesh edges as rows of indicies into V.
-                F: Mesh triangular faces as rows of indicies into V.
+                vertices_t0: Mesh vertices at the start of the time step.
+                vertices_t1: Mesh vertices at the end of the time step.
+                edges: Collision mesh edges as rows of indicies into vertices.
+                faces: Collision mesh triangular faces as rows of indicies into vertices.
                 tmax: Maximum time (normalized) to look for collisions. Should be in [0, 1].
                 tolerance: CCD tolerance used by Tight-Inclusion CCD.
                 max_iterations: Maximum iterations used by Tight-Inclusion CCD.
                 conservative_rescaling: Conservative rescaling value used to avoid taking steps exactly to impact.
 
             Returns:
                 Tuple of:
                 If the candidate had a collision over the time interval.
                 Computed time of impact (normalized).
             )ipc_Qu8mg5v7",
-            py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"),
-            py::arg("min_distance") = 0.0, py::arg("tmax") = 1.0,
-            py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
+            py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
+            py::arg("faces"), py::arg("min_distance") = 0.0,
+            py::arg("tmax") = 1.0, py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
             py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
             py::arg("conservative_rescaling") =
                 DEFAULT_CCD_CONSERVATIVE_RESCALING)
         .def(
             "print_ccd_query", &EdgeEdgeCandidate::print_ccd_query, "",
-            py::arg("V0"), py::arg("V1"), py::arg("E"), py::arg("F"))
+            py::arg("vertices_t0"), py::arg("vertices_t1"), py::arg("edges"),
+            py::arg("faces"))
         .def("__eq__", &EdgeEdgeCandidate::operator==, "", py::arg("other"))
         .def("__ne__", &EdgeEdgeCandidate::operator!=, "", py::arg("other"))
         .def(
             "__lt__", &EdgeEdgeCandidate::operator<,
             "Compare EdgeEdgeCandidates for sorting.", py::arg("other"))
-        .def_readwrite("edge0_index", &EdgeEdgeCandidate::edge0_index, "")
-        .def_readwrite("edge1_index", &EdgeEdgeCandidate::edge1_index, "");
+        .def_readwrite(
+            "edge0_id", &EdgeEdgeCandidate::edge0_id, "ID of the first edge")
+        .def_readwrite(
+            "edge1_id", &EdgeEdgeCandidate::edge1_id, "ID of the second edge");
 }
```

### Comparing `ipctk-1.0.0/python/src/candidates/edge_face.cpp` & `ipctk-1.1.0/python/src/candidates/edge_face.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/candidates/edge_face.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_edge_face_candidate(py::module_& m)
 {
     py::class_<EdgeFaceCandidate>(m, "EdgeFaceCandidate")
-        .def(
-            py::init<long, long>(), "", py::arg("edge_index"),
-            py::arg("face_index"))
+        .def(py::init<long, long>(), "", py::arg("edge_id"), py::arg("face_id"))
         .def(
             "__str__",
             [](const EdgeFaceCandidate& ev) {
-                return fmt::format(
-                    "[{:d}, {:d}]", ev.edge_index, ev.face_index);
+                return fmt::format("[{:d}, {:d}]", ev.edge_id, ev.face_id);
             })
         .def(
             "__repr__",
             [](const EdgeFaceCandidate& ev) {
                 return fmt::format(
-                    "EdgeFaceCandidate({:d}, {:d})", ev.edge_index,
-                    ev.face_index);
+                    "EdgeFaceCandidate({:d}, {:d})", ev.edge_id, ev.face_id);
             })
         .def("__eq__", &EdgeFaceCandidate::operator==, "", py::arg("other"))
         .def("__ne__", &EdgeFaceCandidate::operator!=, "", py::arg("other"))
         .def(
             "__lt__", &EdgeFaceCandidate::operator<,
             "Compare EdgeFaceCandidate for sorting.", py::arg("other"))
-        .def_readwrite("edge_index", &EdgeFaceCandidate::edge_index, "")
-        .def_readwrite("face_index", &EdgeFaceCandidate::face_index, "");
+        .def_readwrite("edge_id", &EdgeFaceCandidate::edge_id, "ID of the edge")
+        .def_readwrite(
+            "face_id", &EdgeFaceCandidate::face_id, "ID of the face");
 }
```

### Comparing `ipctk-1.0.0/python/src/candidates/vertex_vertex.cpp` & `ipctk-1.1.0/python/src/candidates/vertex_vertex.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,53 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/candidates/vertex_vertex.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_vertex_vertex_candidate(py::module_& m)
 {
-    py::class_<VertexVertexCandidate>(m, "VertexVertexCandidate")
+    py::class_<VertexVertexCandidate, CollisionStencil>(
+        m, "VertexVertexCandidate")
         .def(
-            py::init<long, long>(), "", py::arg("vertex0_index"),
-            py::arg("vertex1_index"))
+            py::init<long, long>(), "", py::arg("vertex0_id"),
+            py::arg("vertex1_id"))
         .def(
             "__str__",
             [](const VertexVertexCandidate& ev) {
                 return fmt::format(
-                    "[{:d}, {:d}]", ev.vertex0_index, ev.vertex1_index);
+                    "[{:d}, {:d}]", ev.vertex0_id, ev.vertex1_id);
             })
         .def(
             "__repr__",
             [](const VertexVertexCandidate& ev) {
                 return fmt::format(
-                    "VertexVertexCandidate({:d}, {:d})", ev.vertex0_index,
-                    ev.vertex1_index);
+                    "VertexVertexCandidate({:d}, {:d})", ev.vertex0_id,
+                    ev.vertex1_id);
             })
         .def("num_vertices", &VertexVertexCandidate::num_vertices, "")
         .def(
-            "vertex_indices", &VertexVertexCandidate::vertex_indices,
+            "vertex_ids", &VertexVertexCandidate::vertex_ids,
             R"ipc_Qu8mg5v7(
             Get the indices of the vertices
 
             Parameters:
-                E: edge matrix of mesh
-                F: face matrix of mesh
+                edges: edge matrix of mesh
+                faces: face matrix of mesh
 
             Returns:
                 List of vertex indices
             )ipc_Qu8mg5v7",
-            py::arg("E"), py::arg("F"))
-        .def(
-            "compute_distance", &VertexVertexCandidate::compute_distance, "",
-            py::arg("V"), py::arg("E"), py::arg("F"))
-        .def(
-            "compute_distance_gradient",
-            &VertexVertexCandidate::compute_distance_gradient, "", py::arg("V"),
-            py::arg("E"), py::arg("F"))
-        .def(
-            "compute_distance_hessian",
-            &VertexVertexCandidate::compute_distance_hessian, "", py::arg("V"),
-            py::arg("E"), py::arg("F"))
+            py::arg("edges"), py::arg("faces"))
         .def("__eq__", &VertexVertexCandidate::operator==, "", py::arg("other"))
         .def("__ne__", &VertexVertexCandidate::operator!=, "", py::arg("other"))
         .def(
             "__lt__", &VertexVertexCandidate::operator<,
             "Compare EdgeVertexCandidates for sorting.", py::arg("other"))
         .def_readwrite(
-            "vertex0_index", &VertexVertexCandidate::vertex0_index, "")
+            "vertex0_id", &VertexVertexCandidate::vertex0_id,
+            "ID of the first vertex")
         .def_readwrite(
-            "vertex1_index", &VertexVertexCandidate::vertex1_index, "");
+            "vertex1_id", &VertexVertexCandidate::vertex1_id,
+            "ID of the second vertex");
 }
```

### Comparing `ipctk-1.0.0/python/src/ccd/aabb.cpp` & `ipctk-1.1.0/python/src/ccd/aabb.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/ccd/aabb.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_ccd_aabb(py::module_& m)
```

### Comparing `ipctk-1.0.0/python/src/ccd/ccd.cpp` & `ipctk-1.1.0/python/src/ccd/ccd.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/ccd/ccd.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_ccd(py::module_& m)
@@ -15,16 +15,16 @@
            const double min_distance = 0.0, const double tmax = 1.0,
            const double tolerance = DEFAULT_CCD_TOLERANCE,
            const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
            const double conservative_rescaling =
                DEFAULT_CCD_CONSERVATIVE_RESCALING) {
             double toi;
             bool r = point_edge_ccd_2D(
-                p_t0, e0_t0, e1_t0, p_t1, e0_t1, e1_t1, toi, tmax, tolerance,
-                max_iterations, conservative_rescaling);
+                p_t0, e0_t0, e1_t0, p_t1, e0_t1, e1_t1, toi, min_distance, tmax,
+                tolerance, max_iterations, conservative_rescaling);
             return std::make_tuple(r, toi);
         },
         "", py::arg("p_t0"), py::arg("e0_t0"), py::arg("e1_t0"),
         py::arg("p_t1"), py::arg("e0_t1"), py::arg("e1_t1"),
         py::arg("min_distance") = 0.0, py::arg("tmax") = 1.0,
         py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
         py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
@@ -37,15 +37,15 @@
            const double min_distance = 0.0, const double tmax = 1.0,
            const double tolerance = DEFAULT_CCD_TOLERANCE,
            const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
            const double conservative_rescaling =
                DEFAULT_CCD_CONSERVATIVE_RESCALING) {
             double toi;
             bool r = point_point_ccd(
-                p0_t0, p1_t0, p0_t1, p1_t1, toi, tmax, tolerance,
+                p0_t0, p1_t0, p0_t1, p1_t1, toi, min_distance, tmax, tolerance,
                 max_iterations, conservative_rescaling);
             return std::make_tuple(r, toi);
         },
         "", py::arg("p0_t0"), py::arg("p1_t0"), py::arg("p0_t1"),
         py::arg("p1_t1"), py::arg("min_distance") = 0.0, py::arg("tmax") = 1.0,
         py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
         py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
@@ -59,16 +59,16 @@
            const double min_distance = 0.0, const double tmax = 1.0,
            const double tolerance = DEFAULT_CCD_TOLERANCE,
            const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
            const double conservative_rescaling =
                DEFAULT_CCD_CONSERVATIVE_RESCALING) {
             double toi;
             bool r = point_edge_ccd_3D(
-                p_t0, e0_t0, e1_t0, p_t1, e0_t1, e1_t1, toi, tmax, tolerance,
-                max_iterations, conservative_rescaling);
+                p_t0, e0_t0, e1_t0, p_t1, e0_t1, e1_t1, toi, min_distance, tmax,
+                tolerance, max_iterations, conservative_rescaling);
             return std::make_tuple(r, toi);
         },
         "", py::arg("p_t0"), py::arg("e0_t0"), py::arg("e1_t0"),
         py::arg("p_t1"), py::arg("e0_t1"), py::arg("e1_t1"),
         py::arg("min_distance") = 0.0, py::arg("tmax") = 1.0,
         py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
         py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
@@ -83,16 +83,17 @@
            const double min_distance = 0.0, const double tmax = 1.0,
            const double tolerance = DEFAULT_CCD_TOLERANCE,
            const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
            const double conservative_rescaling =
                DEFAULT_CCD_CONSERVATIVE_RESCALING) {
             double toi;
             bool r = point_triangle_ccd(
-                p_t0, t0_t0, t1_t0, t2_t0, p_t1, t0_t1, t1_t1, t2_t1, toi, tmax,
-                tolerance, max_iterations, conservative_rescaling);
+                p_t0, t0_t0, t1_t0, t2_t0, p_t1, t0_t1, t1_t1, t2_t1, toi,
+                min_distance, tmax, tolerance, max_iterations,
+                conservative_rescaling);
             return std::make_tuple(r, toi);
         },
         "", py::arg("p_t0"), py::arg("t0_t0"), py::arg("t1_t0"),
         py::arg("t2_t0"), py::arg("p_t1"), py::arg("t0_t1"), py::arg("t1_t1"),
         py::arg("t2_t1"), py::arg("min_distance") = 0.0, py::arg("tmax") = 1.0,
         py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
         py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
@@ -108,15 +109,16 @@
            const double tolerance = DEFAULT_CCD_TOLERANCE,
            const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
            const double conservative_rescaling =
                DEFAULT_CCD_CONSERVATIVE_RESCALING) {
             double toi;
             bool r = edge_edge_ccd(
                 ea0_t0, ea1_t0, eb0_t0, eb1_t0, ea0_t1, ea1_t1, eb0_t1, eb1_t1,
-                toi, tmax, tolerance, max_iterations, conservative_rescaling);
+                toi, min_distance, tmax, tolerance, max_iterations,
+                conservative_rescaling);
             return std::make_tuple(r, toi);
         },
         "", py::arg("ea0_t0"), py::arg("ea1_t0"), py::arg("eb0_t0"),
         py::arg("eb1_t0"), py::arg("ea0_t1"), py::arg("ea1_t1"),
         py::arg("eb0_t1"), py::arg("eb1_t1"), py::arg("min_distance") = 0.0,
         py::arg("tmax") = 1.0, py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
         py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
@@ -130,16 +132,16 @@
            const double min_distance = 0.0, const double tmax = 1.0,
            const double tolerance = DEFAULT_CCD_TOLERANCE,
            const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
            const double conservative_rescaling =
                DEFAULT_CCD_CONSERVATIVE_RESCALING) {
             double toi;
             bool r = point_edge_ccd(
-                p_t0, e0_t0, e1_t0, p_t1, e0_t1, e1_t1, toi, tmax, tolerance,
-                max_iterations, conservative_rescaling);
+                p_t0, e0_t0, e1_t0, p_t1, e0_t1, e1_t1, toi, min_distance, tmax,
+                tolerance, max_iterations, conservative_rescaling);
             return std::make_tuple(r, toi);
         },
         "", py::arg("p_t0"), py::arg("e0_t0"), py::arg("e1_t0"),
         py::arg("p_t1"), py::arg("e0_t1"), py::arg("e1_t1"),
         py::arg("min_distance") = 0.0, py::arg("tmax") = 1.0,
         py::arg("tolerance") = DEFAULT_CCD_TOLERANCE,
         py::arg("max_iterations") = DEFAULT_CCD_MAX_ITERATIONS,
```

### Comparing `ipctk-1.0.0/python/src/ccd/inexact_point_edge.cpp` & `ipctk-1.1.0/python/src/ccd/inexact_point_edge.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/ccd/inexact_point_edge.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_inexact_point_edge(py::module_& m)
```

### Comparing `ipctk-1.0.0/python/src/ccd/point_static_plane.cpp` & `ipctk-1.1.0/python/src/ccd/point_static_plane.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/ccd/point_static_plane.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_point_static_plane(py::module_& m)
```

### Comparing `ipctk-1.0.0/python/src/common.hpp` & `ipctk-1.1.0/python/src/common.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/iostream.h>
 #include <pybind11/operators.h>
 #include <pybind11/eigen.h>
+#include <pybind11/functional.h>
 
 #include <Eigen/Core>
+#include <Eigen/Sparse>
 
 template <typename Derived>
 void assert_2D_or_3D_vector(
     const Eigen::MatrixBase<Derived>& v, const std::string& name)
 {
     if ((v.size() != 2 && v.size() != 3) || (v.rows() != 1 && v.cols() != 1)) {
         throw pybind11::value_error(
@@ -26,14 +28,26 @@
         throw pybind11::value_error(
             "Parameter " + name + " has invalid size: expected " + name
             + " to be a 3D vector but got " + name + ".shape = ["
             + std::to_string(v.rows()) + ", " + std::to_string(v.cols()) + "]");
     }
 }
 
+template <typename T>
+inline void assert_is_sparse_vector(
+    const Eigen::SparseMatrix<T>& M, const std::string& name)
+{
+    if (M.cols() != 1) {
+        throw pybind11::value_error(
+            "Parameter " + name + " has invalid size: expected " + name
+            + " to be a sparse vector but got " + name + ".shape = ["
+            + std::to_string(M.rows()) + ", " + std::to_string(M.cols()) + "]");
+    }
+}
+
 template <typename DerivedV, typename DerivedVCopy>
 inline void copy_vector(
     const Eigen::MatrixBase<DerivedV>& v,
     Eigen::MatrixBase<DerivedVCopy>& v_copy)
 {
     if (v.cols() == 1) {
         v_copy = v;
```

### Comparing `ipctk-1.0.0/python/src/distance/distance_type.cpp` & `ipctk-1.1.0/python/src/distance/distance_type.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/distance/distance_type.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_distance_type(py::module_& m)
@@ -83,40 +83,30 @@
             "edges are closest at an interior point of edge A and B")
         .value(
             "AUTO", EdgeEdgeDistanceType::AUTO,
             "automatically determine the closest point")
         .export_values();
 
     m.def(
-        "point_edge_distance_type",
-        [](const VectorMax3d& p, const VectorMax3d& e0, const VectorMax3d& e1) {
-            assert_2D_or_3D_vector(p, "p");
-            assert_2D_or_3D_vector(e0, "e0");
-            assert_2D_or_3D_vector(e1, "e1");
-            return point_edge_distance_type(p, e0, e1);
-        },
+        "point_edge_distance_type", &point_edge_distance_type,
         R"ipc_Qu8mg5v7(
         Determine the closest pair between a point and edge.
 
         Parameters:
             p: point
             e0: first vertex of the edge
             e1: second vertex of the edge
 
         Returns:
             The distance type of the point-edge pair.
         )ipc_Qu8mg5v7",
         py::arg("p"), py::arg("e0"), py::arg("e1"));
 
     m.def(
-        "point_triangle_distance_type",
-        [](const Eigen::Vector3d& p, const Eigen::Vector3d& t0,
-           const Eigen::Vector3d& t1, const Eigen::Vector3d& t2) {
-            return point_triangle_distance_type(p, t0, t1, t2);
-        },
+        "point_triangle_distance_type", &point_triangle_distance_type,
         R"ipc_Qu8mg5v7(
         Determine the closest pair between a point and triangle.
 
         Parameters:
             p: point
             t0: first vertex of the triangle
             t1: second vertex of the triangle
@@ -124,19 +114,15 @@
 
         Returns:
             The distance type of the point-triangle pair.
         )ipc_Qu8mg5v7",
         py::arg("p"), py::arg("t0"), py::arg("t1"), py::arg("t2"));
 
     m.def(
-        "edge_edge_distance_type",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
-            return edge_edge_distance_type(ea0, ea1, eb0, eb1);
-        },
+        "edge_edge_distance_type", &edge_edge_distance_type,
         R"ipc_Qu8mg5v7(
         Determine the closest pair between two edges.
 
         Parameters:
             ea0: first vertex of the first edge
             ea1: second vertex of the first edge
             eb0: first vertex of the second edge
```

### Comparing `ipctk-1.0.0/python/src/distance/edge_edge.cpp` & `ipctk-1.1.0/python/src/distance/edge_edge.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/distance/distance_type.hpp>
 #include <ipc/distance/edge_edge.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_edge_edge_distance(py::module_& m)
 {
     m.def(
-        "edge_edge_distance",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1,
-           const EdgeEdgeDistanceType dtype) {
-            return edge_edge_distance(ea0, ea1, eb0, eb1, dtype);
-        },
+        "edge_edge_distance", &edge_edge_distance,
         R"ipc_Qu8mg5v7(
         Compute the distance between a two lines segments in 3D.
 
         Parameters:
             ea0: first vertex of the first edge
             ea1: second vertex of the first edge
             eb0: first vertex of the second edge
@@ -31,22 +26,15 @@
         Note:
             The distance is actually squared distance.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"),
         py::arg("dtype") = EdgeEdgeDistanceType::AUTO);
 
     m.def(
-        "edge_edge_distance_gradient",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1,
-           const EdgeEdgeDistanceType dtype) {
-            Vector<double, 12> grad;
-            edge_edge_distance_gradient(ea0, ea1, eb0, eb1, grad, dtype);
-            return grad;
-        },
+        "edge_edge_distance_gradient", &edge_edge_distance_gradient,
         R"ipc_Qu8mg5v7(
         Compute the gradient of the distance between a two lines segments.
 
         Parameters:
             ea0: first vertex of the first edge
             ea1: second vertex of the first edge
             eb0: first vertex of the second edge
@@ -59,22 +47,15 @@
         Note:
             The distance is actually squared distance.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"),
         py::arg("dtype") = EdgeEdgeDistanceType::AUTO);
 
     m.def(
-        "edge_edge_distance_hessian",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1,
-           const EdgeEdgeDistanceType dtype) {
-            Eigen::Matrix<double, 12, 12> hess;
-            edge_edge_distance_hessian(ea0, ea1, eb0, eb1, hess, dtype);
-            return hess;
-        },
+        "edge_edge_distance_hessian", &edge_edge_distance_hessian,
         R"ipc_Qu8mg5v7(
         Compute the hessian of the distance between a two lines segments.
 
         Parameters:
             ea0: first vertex of the first edge
             ea1: second vertex of the first edge
             eb0: first vertex of the second edge
```

### Comparing `ipctk-1.0.0/python/src/distance/edge_edge_mollifier.cpp` & `ipctk-1.1.0/python/src/distance/edge_edge_mollifier.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/distance/edge_edge_mollifier.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_edge_edge_mollifier(py::module_& m)
 {
     m.def(
-        "edge_edge_cross_squarednorm",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
-            return edge_edge_cross_squarednorm(ea0, ea1, eb0, eb1);
-        },
+        "edge_edge_cross_squarednorm", &edge_edge_cross_squarednorm,
         R"ipc_Qu8mg5v7(
         Compute the squared norm of the edge-edge cross product.
 
         Parameters:
             ea0: first vertex of the first edge
             ea1: second vertex of the first edge
             eb0: first vertex of the second edge
@@ -25,20 +21,20 @@
         Returns:
             The squared norm of the edge-edge cross product.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"));
 
     m.def(
         "edge_edge_cross_squarednorm_gradient",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
-            Vector<double, 12> grad;
-            edge_edge_cross_squarednorm_gradient(ea0, ea1, eb0, eb1, grad);
-            return grad;
-        },
+        py::overload_cast<
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&>(
+            &edge_edge_cross_squarednorm_gradient),
         R"ipc_Qu8mg5v7(
         Compute the gradient of the squared norm of the edge cross product.
 
         Parameters:
             ea0: first vertex of the first edge
             ea1: second vertex of the first edge
             eb0: first vertex of the second edge
@@ -47,20 +43,20 @@
         Returns:
             The gradient of the squared norm of the edge cross product wrt ea0, ea1, eb0, and eb1.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"));
 
     m.def(
         "edge_edge_cross_squarednorm_hessian",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
-            Eigen::Matrix<double, 12, 12> hess;
-            edge_edge_cross_squarednorm_hessian(ea0, ea1, eb0, eb1, hess);
-            return hess;
-        },
+        py::overload_cast<
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&>(
+            &edge_edge_cross_squarednorm_hessian),
         R"ipc_Qu8mg5v7(
         Compute the hessian of the squared norm of the edge cross product.
 
         Parameters:
             ea0: first vertex of the first edge
             ea1: second vertex of the first edge
             eb0: first vertex of the second edge
@@ -68,137 +64,136 @@
 
         Returns:
             The hessian of the squared norm of the edge cross product wrt ea0, ea1, eb0, and eb1.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"));
 
     m.def(
-        "edge_edge_mollifier", &edge_edge_mollifier<double>,
+        "edge_edge_mollifier",
+        py::overload_cast<const double, const double>(&edge_edge_mollifier),
         R"ipc_Qu8mg5v7(
         Mollifier function for edge-edge distance.
 
         Parameters:
-            - x: squared norm of the edge-edge cross product
-            - eps_x: mollifier activation threshold
+            x: squared norm of the edge-edge cross product
+            eps_x: mollifier activation threshold
 
         Returns:
             The mollifier coefficient to premultiply the edge-edge distance.
         )ipc_Qu8mg5v7",
         py::arg("x"), py::arg("eps_x"));
 
     m.def(
-        "edge_edge_mollifier_gradient", &edge_edge_mollifier_gradient<double>,
+        "edge_edge_mollifier_gradient",
+        py::overload_cast<const double, const double>(
+            &edge_edge_mollifier_gradient),
         R"ipc_Qu8mg5v7(
         The gradient of the mollifier function for edge-edge distance.
 
         Parameters:
-            - x: squared norm of the edge-edge cross product
-            - eps_x: mollifier activation threshold
+            x: squared norm of the edge-edge cross product
+            eps_x: mollifier activation threshold
 
         Returns:
             The gradient of the mollifier function for edge-edge distance wrt x.
         )ipc_Qu8mg5v7",
         py::arg("x"), py::arg("eps_x"));
 
     m.def(
-        "edge_edge_mollifier_hessian", &edge_edge_mollifier_hessian<double>,
+        "edge_edge_mollifier_hessian",
+        py::overload_cast<const double, const double>(
+            &edge_edge_mollifier_hessian),
         R"ipc_Qu8mg5v7(
         The hessian of the mollifier function for edge-edge distance.
 
         Parameters:
-            - x: squared norm of the edge-edge cross product
-            - eps_x: mollifier activation threshold
+            x: squared norm of the edge-edge cross product
+            eps_x: mollifier activation threshold
 
         Returns:
             The hessian of the mollifier function for edge-edge distance wrt x.
         )ipc_Qu8mg5v7",
         py::arg("x"), py::arg("eps_x"));
 
     m.def(
         "edge_edge_mollifier",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1,
-           const double eps_x) {
-            return edge_edge_mollifier(ea0, ea1, eb0, eb1, eps_x);
-        },
+        py::overload_cast<
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&, const double>(
+            &edge_edge_mollifier),
         R"ipc_Qu8mg5v7(
         Compute a mollifier for the edge-edge distance.
 
         This helps smooth the non-smoothness at close to parallel edges.
 
         Parameters:
-            - ea0: first vertex of the first edge
-            - ea1: second vertex of the first edge
-            - eb0: first vertex of the second edge
-            - eb1: second vertex of the second edge
-            - eps_x: mollifier activation threshold
+            ea0: first vertex of the first edge
+            ea1: second vertex of the first edge
+            eb0: first vertex of the second edge
+            eb1: second vertex of the second edge
+            eps_x: mollifier activation threshold
 
         Returns:
             The mollifier coefficient to premultiply the edge-edge distance.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"),
         py::arg("eps_x"));
 
     m.def(
         "edge_edge_mollifier_gradient",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1,
-           const double eps_x) {
-            Vector<double, 12> grad;
-            edge_edge_mollifier_gradient(ea0, ea1, eb0, eb1, eps_x, grad);
-            return grad;
-        },
+        py::overload_cast<
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&, const double>(
+            &edge_edge_mollifier_gradient),
         R"ipc_Qu8mg5v7(
         Compute the gradient of the mollifier for the edge-edge distance.
 
         Parameters:
-            - ea0: first vertex of the first edge
-            - ea1: second vertex of the first edge
-            - eb0: first vertex of the second edge
-            - eb1: second vertex of the second edge
-            - eps_x: mollifier activation threshold
+            ea0: first vertex of the first edge
+            ea1: second vertex of the first edge
+            eb0: first vertex of the second edge
+            eb1: second vertex of the second edge
+            eps_x: mollifier activation threshold
 
         Returns:
             The gradient of the mollifier.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"),
         py::arg("eps_x"));
 
     m.def(
         "edge_edge_mollifier_hessian",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1,
-           const double eps_x) {
-            Eigen::Matrix<double, 12, 12> hess;
-            edge_edge_mollifier_hessian(ea0, ea1, eb0, eb1, eps_x, hess);
-            return hess;
-        },
+        py::overload_cast<
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&,
+            const Eigen::Ref<const Eigen::Vector3d>&, const double>(
+            &edge_edge_mollifier_hessian),
         R"ipc_Qu8mg5v7(
         Compute the hessian of the mollifier for the edge-edge distance.
 
         Parameters:
-            - ea0: first vertex of the first edge
-            - ea1: second vertex of the first edge
-            - eb0: first vertex of the second edge
-            - eb1: second vertex of the second edge
-            - eps_x: mollifier activation threshold
+            ea0: first vertex of the first edge
+            ea1: second vertex of the first edge
+            eb0: first vertex of the second edge
+            eb1: second vertex of the second edge
+            eps_x: mollifier activation threshold
 
         Returns:
             The hessian of the mollifier.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"),
         py::arg("eps_x"));
 
     m.def(
-        "edge_edge_mollifier_threshold",
-        [](const Eigen::Vector3d& ea0_rest, const Eigen::Vector3d& ea1_rest,
-           const Eigen::Vector3d& eb0_rest, const Eigen::Vector3d& eb1_rest) {
-            return edge_edge_mollifier_threshold(
-                ea0_rest, ea1_rest, eb0_rest, eb1_rest);
-        },
+        "edge_edge_mollifier_threshold", &edge_edge_mollifier_threshold,
         R"ipc_Qu8mg5v7(
         Compute the threshold of the mollifier edge-edge distance.
 
         This values is computed based on the edges at rest length.
 
         Parameters:
             ea0_rest: rest position of the first vertex of the first edge
```

### Comparing `ipctk-1.0.0/python/src/distance/line_line.cpp` & `ipctk-1.1.0/python/src/distance/line_line.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/distance/line_line.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_line_line_distance(py::module_& m)
 {
     m.def(
-        "line_line_distance",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
-            return line_line_distance(ea0, ea1, eb0, eb1);
-        },
+        "line_line_distance", &line_line_distance,
         R"ipc_Qu8mg5v7(
         Compute the distance between a two infinite lines in 3D.
 
         Parameters:
             ea0: first vertex of the edge defining the first line
             ea1: second vertex of the edge defining the first line
             eb0: first vertex of the edge defining the second line
@@ -30,21 +26,15 @@
 
         Warning:
             If the lines are parallel this function returns a distance of zero.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"));
 
     m.def(
-        "line_line_distance_gradient",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
-            Vector<double, 12> grad;
-            line_line_distance_gradient(ea0, ea1, eb0, eb1, grad);
-            return grad;
-        },
+        "line_line_distance_gradient", &line_line_distance_gradient,
         R"ipc_Qu8mg5v7(
         Compute the gradient of the distance between a two lines in 3D.
 
         Parameters:
             ea0: first vertex of the edge defining the first line
             ea1: second vertex of the edge defining the first line
             eb0: first vertex of the edge defining the second line
@@ -58,21 +48,15 @@
 
         Warning:
             If the lines are parallel this function returns a distance of zero.
         )ipc_Qu8mg5v7",
         py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"));
 
     m.def(
-        "line_line_distance_hessian",
-        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
-           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
-            Eigen::Matrix<double, 12, 12> hess;
-            line_line_distance_hessian(ea0, ea1, eb0, eb1, hess);
-            return hess;
-        },
+        "line_line_distance_hessian", &line_line_distance_hessian,
         R"ipc_Qu8mg5v7(
         Compute the hessian of the distance between a two lines in 3D.
 
         Parameters:
             ea0: first vertex of the edge defining the first line
             ea1: second vertex of the edge defining the first line
             eb0: first vertex of the edge defining the second line
```

### Comparing `ipctk-1.0.0/python/src/distance/point_plane.cpp` & `ipctk-1.1.0/python/src/friction/closest_point.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,63 @@
-#include "../common.hpp"
+#include <common.hpp>
 
-#include <ipc/distance/point_plane.hpp>
+#include <ipc/friction/closest_point.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
-void define_point_plane_distance(py::module_& m)
+void define_closest_point(py::module_& m)
 {
     m.def(
-        "point_plane_distance",
-        [](const Eigen::Vector3d& p, const Eigen::Vector3d& t0,
-           const Eigen::Vector3d& t1, const Eigen::Vector3d& t2) {
-            return point_plane_distance(p, t0, t1, t2);
+        "point_edge_closest_point",
+        [](const VectorMax3d& p, const VectorMax3d& e0, const VectorMax3d& e1) {
+            assert_2D_or_3D_vector(p, "p");
+            assert_2D_or_3D_vector(e0, "e0");
+            assert_2D_or_3D_vector(e1, "e1");
+            return point_edge_closest_point(p, e0, e1);
         },
-        R"ipc_Qu8mg5v7(
-        Compute the distance between a point and a plane.
-
-        Parameters:
-            p: point
-            t0: first vertex of the triangle
-            t1: second vertex of the triangle
-            t2: third vertex of the triangle
+        "", py::arg("p"), py::arg("e0"), py::arg("e1"));
 
-        Returns:
-            The distance between the point and plane.
-
-        Note:
-            The distance is actually squared distance.
-        )ipc_Qu8mg5v7",
-        py::arg("p"), py::arg("t0"), py::arg("t1"), py::arg("t1"));
+    m.def(
+        "edge_edge_closest_point",
+        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
+           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
+            return edge_edge_closest_point(ea0, ea1, eb0, eb1);
+        },
+        "Compute the barycentric coordinates of the closest points",
+        py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"));
 
     m.def(
-        "point_plane_distance_gradient",
+        "point_triangle_closest_point",
         [](const Eigen::Vector3d& p, const Eigen::Vector3d& t0,
            const Eigen::Vector3d& t1, const Eigen::Vector3d& t2) {
-            Vector<double, 12> grad;
-            point_plane_distance_gradient(p, t0, t1, t2, grad);
-            return grad;
+            return point_triangle_closest_point(p, t0, t1, t2);
         },
-        R"ipc_Qu8mg5v7(
-        Compute the gradient of the distance between a point and a plane.
+        "Compute the barycentric coordinates of the closest point on the triangle.",
+        py::arg("p"), py::arg("t0"), py::arg("t1"), py::arg("t2"));
 
-        Parameters:
-            p: point
-            t0: first vertex of the triangle
-            t1: second vertex of the triangle
-            t2: third vertex of the triangle
-
-        Returns:
-            The gradient of the distance wrt p, t0, t1, and t2.
+    m.def(
+        "point_edge_closest_point_jacobian",
+        [](const VectorMax3d& p, const VectorMax3d& e0, const VectorMax3d& e1) {
+            assert_2D_or_3D_vector(p, "p");
+            assert_2D_or_3D_vector(e0, "e0");
+            assert_2D_or_3D_vector(e1, "e1");
+            return point_edge_closest_point_jacobian(p, e0, e1);
+        },
+        "", py::arg("p"), py::arg("e0"), py::arg("e1"));
 
-        Note:
-            The distance is actually squared distance.
-        )ipc_Qu8mg5v7",
-        py::arg("p"), py::arg("t0"), py::arg("t1"), py::arg("t1"));
+    m.def(
+        "edge_edge_closest_point_jacobian",
+        [](const Eigen::Vector3d& ea0, const Eigen::Vector3d& ea1,
+           const Eigen::Vector3d& eb0, const Eigen::Vector3d& eb1) {
+            return edge_edge_closest_point_jacobian(ea0, ea1, eb0, eb1);
+        },
+        "", py::arg("ea0"), py::arg("ea1"), py::arg("eb0"), py::arg("eb1"));
 
     m.def(
-        "point_plane_distance_hessian",
+        "point_triangle_closest_point_jacobian",
         [](const Eigen::Vector3d& p, const Eigen::Vector3d& t0,
            const Eigen::Vector3d& t1, const Eigen::Vector3d& t2) {
-            Eigen::Matrix<double, 12, 12> hess;
-            point_plane_distance_hessian(p, t0, t1, t2, hess);
-            return hess;
-        },
-        R"ipc_Qu8mg5v7(
-        Compute the hessian of the distance between a point and a plane.
-
-        Parameters:
-            p: point
-            t0: first vertex of the triangle
-            t1: second vertex of the triangle
-            t2: third vertex of the triangle
-
-        Returns:
-            The hessian of the distance wrt p, t0, t1, and t2.
-
-        Note:
-            The distance is actually squared distance.
-        )ipc_Qu8mg5v7",
-        py::arg("p"), py::arg("t0"), py::arg("t1"), py::arg("t1"));
+            return point_triangle_closest_point_jacobian(p, t0, t1, t2);
+        },
+        "", py::arg("p"), py::arg("t0"), py::arg("t1"), py::arg("t2"));
 }
```

### Comparing `ipctk-1.0.0/python/src/friction/normal_force_magnitude.cpp` & `ipctk-1.1.0/python/src/friction/normal_force_magnitude.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/friction/normal_force_magnitude.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_normal_force_magnitude(py::module_& m)
```

### Comparing `ipctk-1.0.0/python/src/friction/tangent_basis.cpp` & `ipctk-1.1.0/python/src/friction/tangent_basis.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/friction/tangent_basis.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_tangent_basis(py::module_& m)
@@ -10,15 +10,25 @@
     m.def(
         "point_point_tangent_basis",
         [](const VectorMax3d& p0, const VectorMax3d& p1) {
             assert_2D_or_3D_vector(p0, "p0");
             assert_2D_or_3D_vector(p1, "p1");
             return point_point_tangent_basis(p0, p1);
         },
-        "", py::arg("p0"), py::arg("p1"));
+        R"ipc_Qu8mg5v7(
+        Compute a basis for the space tangent to the point-point pair.
+
+        Parameters:
+            p0: First point
+            p1: Second point
+
+        Returns:
+            A 3x2 matrix whose columns are the basis vectors.
+        )ipc_Qu8mg5v7",
+        py::arg("p0"), py::arg("p1"));
 
     m.def(
         "point_edge_tangent_basis",
         [](const VectorMax3d& p, const VectorMax3d& e0, const VectorMax3d& e1) {
             assert_2D_or_3D_vector(p, "p");
             assert_2D_or_3D_vector(e0, "e0");
             assert_2D_or_3D_vector(e1, "e1");
@@ -37,15 +47,33 @@
 
     m.def(
         "point_triangle_tangent_basis",
         [](const Eigen::Vector3d& p, const Eigen::Vector3d& t0,
            const Eigen::Vector3d& t1, const Eigen::Vector3d& t2) {
             return point_triangle_tangent_basis(p, t0, t1, t2);
         },
-        "Compute a basis for the space tangent to the point-triangle pair.",
+        R"ipc_Qu8mg5v7(
+        Compute a basis for the space tangent to the point-triangle pair.
+
+        .. math::
+
+            \begin{bmatrix}
+            \frac{t_1 - t_0}{\|t_1 - t_0\|} & \frac{((t_1 - t_0)\times(t_2 - t_0))
+            \times(t_1 - t_0)}{\|((t_1 - t_0)\times(t_2 - t_0))\times(t_1 - t_0)\|}
+            \end{bmatrix}
+
+        Parameters:
+            p: Point
+            t0: Triangle's first vertex
+            t1: Triangle's second vertex
+            t2: Triangle's third vertex
+
+        Returns:
+            A 3x2 matrix whose columns are the basis vectors.
+        )ipc_Qu8mg5v7",
         py::arg("p"), py::arg("t0"), py::arg("t1"), py::arg("t2"));
 
     m.def(
         "point_point_tangent_basis_jacobian",
         [](const VectorMax3d& p0, const VectorMax3d& p1) {
             assert_2D_or_3D_vector(p0, "p0");
             assert_2D_or_3D_vector(p1, "p1");
```

### Comparing `ipctk-1.0.0/python/src/ipc.cpp` & `ipctk-1.1.0/python/src/collisions/collision_constraints.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,211 +1,165 @@
-#include "common.hpp"
+#include <common.hpp>
 
-#include <ipc/ipc.hpp>
-#include <igl/edges.h>
+#include <ipc/collisions/collision_constraints.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
-void define_ipc(py::module_& m)
+void define_collision_constraints(py::module_& m)
 {
-    m.def(
-        "compute_barrier_potential", &compute_barrier_potential,
-        R"ipc_Qu8mg5v7(
-        Compute the barrier potential for a given constraint set.
-
-        Parameters:
-            mesh: The collision mesh.
-            V: Vertices of the collision mesh.
-            constraint_set: The set of constraints.
-            dhat: The activation distance of the barrier.
-
-        Returns:
-            The sum of all barrier potentials (not scaled by the barrier stiffness).
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V"), py::arg("constraint_set"),
-        py::arg("dhat"));
-
-    m.def(
-        "compute_barrier_potential_gradient",
-        &compute_barrier_potential_gradient,
-        R"ipc_Qu8mg5v7(
-        Compute the gradient of the barrier potential.
-
-        Parameters:
-            mesh: The collision mesh.
-            V: Vertices of the collision mesh.
-            constraint_set: The set of constraints.
-            dhat: The activation distance of the barrier.
-
-        Returns:
-            The gradient of all barrier potentials (not scaled by the barrier stiffness). This will have a size of `V.size`.
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V"), py::arg("constraint_set"),
-        py::arg("dhat"));
-
-    m.def(
-        "compute_barrier_potential_hessian", &compute_barrier_potential_hessian,
-        R"ipc_Qu8mg5v7(
-        Compute the hessian of the barrier potential.
-
-        Parameters:
-            mesh: The collision mesh.
-            V: Vertices of the collision mesh.
-            constraint_set: The set of constraints.
-            dhat: The activation distance of the barrier.
-            project_hessian_to_psd: Make sure the hessian is positive semi-definite.
-
-        Returns:
-            The hessian of all barrier potentials (not scaled by the barrier stiffness). This will have a shape of `(V.size, V.size).
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V"), py::arg("constraint_set"),
-        py::arg("dhat"), py::arg("project_hessian_to_psd") = true);
-
-    m.def(
-        "is_step_collision_free",
-        py::overload_cast<
-            const CollisionMesh&, const Eigen::MatrixXd&,
-            const Eigen::MatrixXd&, const BroadPhaseMethod, const double,
-            const double, const long>(&is_step_collision_free),
-        R"ipc_Qu8mg5v7(
-        Determine if the step is collision free.
-
-        Note:
-            Assumes the trajectory is linear.
-
-        Parameters:
-            mesh: The collision mesh.
-            V0: Surface vertex positions at start as rows of a matrix.
-            V1: Surface vertex positions at end as rows of a matrix.
-
-        Returns:
-            True if <b>any</b> collisions occur.
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V0"), py::arg("V1"),
-        py::arg("method") = BroadPhaseMethod::HASH_GRID,
-        py::arg("min_distance") = 0.0, py::arg("tolerance") = 1e-6,
-        py::arg("max_iterations") = long(1e7));
-
-    m.def(
-        "is_step_collision_free",
-        py::overload_cast<
-            const Candidates&, const CollisionMesh&, const Eigen::MatrixXd&,
-            const Eigen::MatrixXd&, const double, const double, const long>(
-            &is_step_collision_free),
-        R"ipc_Qu8mg5v7(
-        Determine if the step is collision free from a set of candidates.
-
-        Note:
-            Assumes the trajectory is linear.
-
-        Parameters:
-            candidates: Set of candidates to check for collisions.
-            mesh: The collision mesh.
-            V0: Surface vertex positions at start as rows of a matrix.
-            V1: Surface vertex positions at end as rows of a matrix.
-
-        Returns:
-            True if <b>any</b> collisions occur.
-        )ipc_Qu8mg5v7",
-        py::arg("candidates"), py::arg("mesh"), py::arg("V0"), py::arg("V1"),
-        py::arg("min_distance") = 0.0, py::arg("tolerance") = 1e-6,
-        py::arg("max_iterations") = long(1e7));
-
-    m.def(
-        "compute_collision_free_stepsize",
-        py::overload_cast<
-            const CollisionMesh&, const Eigen::MatrixXd&,
-            const Eigen::MatrixXd&, const BroadPhaseMethod, const double,
-            const double, const long>(&compute_collision_free_stepsize),
-        R"ipc_Qu8mg5v7(
-        Computes a maximal step size that is collision free.
-
-        Note:
-            Assumes the trajectory is linear.
-
-        Parameters:
-            mesh: The collision mesh.
-            V0: Vertex positions at start as rows of a matrix. Assumes V0 is intersection free.
-            V1: Surface vertex positions at end as rows of a matrix.
-
-        Returns:
-            A step-size $\in [0, 1]$ that is collision free. A value of 1.0 if a full step and 0.0 is no step.
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V0"), py::arg("V1"),
-        py::arg("method") = BroadPhaseMethod::HASH_GRID,
-        py::arg("min_distance") = 0.0, py::arg("tolerance") = 1e-6,
-        py::arg("max_iterations") = long(1e7));
-
-    m.def(
-        "compute_collision_free_stepsize",
-        py::overload_cast<
-            const Candidates&, const CollisionMesh&, const Eigen::MatrixXd&,
-            const Eigen::MatrixXd&, const double, const double, const long>(
-            &compute_collision_free_stepsize),
-        R"ipc_Qu8mg5v7(
-        Computes a maximal step size that is collision free using a set of collision candidates.
-
-        Note:
-            Assumes the trajectory is linear.
-
-        Parameters:
-            candidates: Set of candidates to check for collisions.
-            mesh: The collision mesh.
-            V0: Vertex positions at start as rows of a matrix. Assumes V0 is intersection free.
-            V1: Surface vertex positions at end as rows of a matrix.
-
-        Returns:
-            A step-size $\in [0, 1]$ that is collision free. A value of 1.0 if a full step and 0.0 is no step.
-        )ipc_Qu8mg5v7",
-        py::arg("candidates"), py::arg("mesh"), py::arg("V0"), py::arg("V1"),
-        py::arg("min_distance") = 0.0, py::arg("tolerance") = 1e-6,
-        py::arg("max_iterations") = long(1e7));
-
-    m.def(
-        "compute_minimum_distance", &compute_minimum_distance,
-        R"ipc_Qu8mg5v7(
-        Computes the minimum distance between any non-adjacent elements.
-
-        Parameters:
-            mesh: The collision mesh.
-            V: Vertices of the collision mesh.
-
-        Returns:
-            The minimum distance between any non-adjacent elements.
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V"), py::arg("constraint_set"));
-
-    m.def(
-        "has_intersections", &has_intersections,
-        R"ipc_Qu8mg5v7(
-        Determine if the mesh has self intersections.
-
-        Parameters:
-            mesh: The collision mesh.
-            V: Vertices of the collision mesh.
-            method: The broad-phase method to use.
-
-        Returns:
-            A boolean for if the mesh has intersections.
-        )ipc_Qu8mg5v7",
-        py::arg("mesh"), py::arg("V"),
-        py::arg("method") = BroadPhaseMethod::HASH_GRID);
-
-    m.def(
-        "edges",
-        [](const Eigen::MatrixXi& F) {
-            Eigen::MatrixXi E;
-            igl::edges(F, E);
-            return E;
-        },
-        R"ipc_Qu8mg5v7(
-        Constructs a list of unique edges represented in a given mesh F
-
-        Parameters:
-            F: #F by 3 list of mesh faces (must be triangles)
-
-        Returns:
-            #E by 2 list of edges in no particular order
-        )ipc_Qu8mg5v7",
-        py::arg("F"));
+    py::class_<CollisionConstraints>(m, "CollisionConstraints")
+        .def(py::init(), "")
+        .def(
+            "build",
+            py::overload_cast<
+                const CollisionMesh&, const Eigen::MatrixXd&, const double,
+                const double, const BroadPhaseMethod>(
+                &CollisionConstraints::build),
+            R"ipc_Qu8mg5v7(
+            Initialize the set of constraints used to compute the barrier potential.
+
+            Parameters:
+                mesh: The collision mesh.
+                vertices: Vertices of the collision mesh.
+                dhat: The activation distance of the barrier.
+                dmin: Minimum distance.
+                broad_phase_method: Broad-phase method to use.
+            )ipc_Qu8mg5v7",
+            py::arg("mesh"), py::arg("vertices"), py::arg("dhat"),
+            py::arg("dmin") = 0,
+            py::arg("broad_phase_method") = BroadPhaseMethod::HASH_GRID)
+        .def(
+            "build",
+            py::overload_cast<
+                const Candidates&, const CollisionMesh&, const Eigen::MatrixXd&,
+                const double, const double>(&CollisionConstraints::build),
+            R"ipc_Qu8mg5v7(
+            Initialize the set of constraints used to compute the barrier potential.
+
+            Parameters:
+                candidates: Distance candidates from which the constraint set is built.
+                mesh: The collision mesh.
+                vertices: Vertices of the collision mesh.
+                dhat: The activation distance of the barrier.
+                dmin:  Minimum distance.
+            )ipc_Qu8mg5v7",
+            py::arg("candidates"), py::arg("mesh"), py::arg("vertices"),
+            py::arg("dhat"), py::arg("dmin") = 0)
+        .def(
+            "compute_potential", &CollisionConstraints::compute_potential,
+            R"ipc_Qu8mg5v7(
+            Compute the barrier potential for a given constraint set.
+
+            Parameters:
+                mesh: The collision mesh.
+                vertices: Vertices of the collision mesh.
+                dhat: The activation distance of the barrier.
+
+            Returns:
+                The sum of all barrier potentials (not scaled by the barrier stiffness).
+            )ipc_Qu8mg5v7",
+            py::arg("mesh"), py::arg("vertices"), py::arg("dhat"))
+        .def(
+            "compute_potential_gradient",
+            &CollisionConstraints::compute_potential_gradient,
+            R"ipc_Qu8mg5v7(
+            Compute the gradient of the barrier potential.
+
+            Parameters:
+                mesh: The collision mesh.
+                vertices: Vertices of the collision mesh.
+                dhat: The activation distance of the barrier.
+
+            Returns:
+                The gradient of all barrier potentials (not scaled by the barrier stiffness). This will have a size of |vertices|.
+            )ipc_Qu8mg5v7",
+            py::arg("mesh"), py::arg("vertices"), py::arg("dhat"))
+        .def(
+            "compute_potential_hessian",
+            &CollisionConstraints::compute_potential_hessian,
+            R"ipc_Qu8mg5v7(
+            Compute the hessian of the barrier potential.
+
+            Parameters:
+                mesh: The collision mesh.
+                vertices: Vertices of the collision mesh.
+                dhat: The activation distance of the barrier.
+                project_hessian_to_psd: Make sure the hessian is positive semi-definite.
+
+            Returns:
+                The hessian of all barrier potentials (not scaled by the barrier stiffness). This will have a size of |vertices|x|vertices|.
+            )ipc_Qu8mg5v7",
+            py::arg("mesh"), py::arg("vertices"), py::arg("dhat"),
+            py::arg("project_hessian_to_psd") = false)
+        .def(
+            "compute_shape_derivative",
+            &CollisionConstraints::compute_shape_derivative,
+            R"ipc_Qu8mg5v7(
+            Compute the barrier shape derivative.
+
+            std::runtime_error If the collision constraints were not built with shape derivatives enabled.
+
+            Parameters:
+                mesh: The collision mesh.
+                vertices: Vertices of the collision mesh.
+                dhat: The activation distance of the barrier.
+
+            Returns:
+                The derivative of the force with respect to X, the rest vertices.
+            )ipc_Qu8mg5v7",
+            py::arg("mesh"), py::arg("vertices"), py::arg("dhat"))
+        .def(
+            "compute_minimum_distance",
+            &CollisionConstraints::compute_minimum_distance,
+            R"ipc_Qu8mg5v7(
+            Computes the minimum distance between any non-adjacent elements.
+
+            Parameters:
+                mesh: The collision mesh.
+                vertices: Vertices of the collision mesh.
+
+            Returns:
+                The minimum distance between any non-adjacent elements.
+            )ipc_Qu8mg5v7",
+            py::arg("mesh"), py::arg("vertices"))
+        .def(
+            "__len__", &CollisionConstraints::size,
+            "Get the number of collision constraints.")
+        .def(
+            "empty", &CollisionConstraints::empty,
+            "Get if the collision constraints are empty.")
+        .def(
+            "clear", &CollisionConstraints::clear,
+            "Clear the collision constraints.")
+        .def(
+            "__getitem__",
+            [](CollisionConstraints& self, size_t idx) -> CollisionConstraint& {
+                return self[idx];
+            },
+            py::return_value_policy::reference,
+            R"ipc_Qu8mg5v7(
+            Get a reference to constriant idx.
+
+            Parameters:
+                idx: The index of the constraint.
+
+            Returns:
+                A reference to the constraint.
+            )ipc_Qu8mg5v7",
+            py::arg("idx"))
+        .def_property(
+            "use_convergent_formulation",
+            &CollisionConstraints::use_convergent_formulation,
+            &CollisionConstraints::set_use_convergent_formulation,
+            "If the collision constraints should use the convergent formulation.")
+        .def_property(
+            "are_shape_derivatives_enabled",
+            &CollisionConstraints::are_shape_derivatives_enabled,
+            &CollisionConstraints::set_are_shape_derivatives_enabled,
+            "If the collision constraints are using the convergent formulation.")
+        .def_readwrite("vv_constraints", &CollisionConstraints::vv_constraints)
+        .def_readwrite("ev_constraints", &CollisionConstraints::ev_constraints)
+        .def_readwrite("ee_constraints", &CollisionConstraints::ee_constraints)
+        .def_readwrite("fv_constraints", &CollisionConstraints::fv_constraints)
+        .def_readwrite("pv_constraints", &CollisionConstraints::pv_constraints);
 }
```

### Comparing `ipctk-1.0.0/python/src/utils/logger.cpp` & `ipctk-1.1.0/python/src/utils/logger.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <ipc/utils/logger.hpp>
 
 namespace py = pybind11;
 using namespace ipc;
 
 void define_logger(py::module_& m)
```

### Comparing `ipctk-1.0.0/python/src/utils/thread_limiter.cpp` & `ipctk-1.1.0/python/src/utils/thread_limiter.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include "../common.hpp"
+#include <common.hpp>
 
 #include <memory>
 
 #include <tbb/info.h>
 #include <tbb/global_control.h>
 
 #include <ipc/utils/logger.hpp>
```

### Comparing `ipctk-1.0.0/setup.py` & `ipctk-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -112,17 +112,19 @@
                     "-DCMAKE_OSX_ARCHITECTURES={}".format(";".join(archs))]
 
         # Set CMAKE_BUILD_PARALLEL_LEVEL to control the parallel build level
         # across all generators.
         if "CMAKE_BUILD_PARALLEL_LEVEL" not in os.environ:
             # self.parallel is a Python 3 only way to set parallel jobs by hand
             # using -j in the build_ext call, not supported by pip or PyPA-build.
-            if hasattr(self, "parallel") and self.parallel:
-                # CMake 3.12+ only.
-                build_args += [f"-j{self.parallel}"]
+            if not (hasattr(self, "parallel") and self.parallel):
+                self.parallel = os.cpu_count()
+                print(f"Using {self.parallel} parallel jobs.")
+            # CMake 3.12+ only.
+            build_args += [f"-j{self.parallel}"]
 
         build_temp = os.path.join(self.build_temp, ext.name)
         if not os.path.exists(build_temp):
             os.makedirs(build_temp)
 
         subprocess.check_call(["cmake", ext.sourcedir] +
                               cmake_args, cwd=build_temp)
```

### Comparing `ipctk-1.0.0/src/ipc/barrier/adaptive_stiffness.cpp` & `ipctk-1.1.0/src/ipc/barrier/adaptive_stiffness.cpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/barrier/adaptive_stiffness.hpp` & `ipctk-1.1.0/src/ipc/barrier/adaptive_stiffness.hpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/barrier/barrier.cpp` & `ipctk-1.1.0/src/ipc/barrier/barrier.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 // Barrier functions that grow to infinity as x -> 0+. Includes gradient and
 // hessian functions, too. These barrier functions can be used to impose
 // inequlity constraints on a function.
 #include "barrier.hpp"
 
+#include <cmath>
+#include <limits>
+
 namespace ipc {
 
+double barrier(const double d, const double dhat)
+{
+    if (d <= 0.0) {
+        return std::numeric_limits<double>::infinity();
+    }
+    if (d >= dhat) {
+        return 0;
+    }
+    // b(d) = -(d-d̂)²ln(d / d̂)
+    const double d_minus_dhat = (d - dhat);
+    return -d_minus_dhat * d_minus_dhat * log(d / dhat);
+}
+
 double barrier_gradient(const double d, const double dhat)
 {
     if (d <= 0.0 || d >= dhat) {
         return 0.0;
     }
     // b(d) = -(d - d̂)²ln(d / d̂)
     // b'(d) = -2(d - d̂)ln(d / d̂) - (d-d̂)²(1 / d)
```

### Comparing `ipctk-1.0.0/src/ipc/barrier/barrier.hpp` & `ipctk-1.1.0/src/ipc/barrier/barrier.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 /// \f\[
 ///     b(d) = -(d-\hat{d})^2\ln\left(\frac{d}{\hat{d}}\right)
 /// \f\]
 ///
 /// @param d The distance.
 /// @param dhat Activation distance of the barrier.
 /// @return The value of the barrier function at d.
-template <typename T> T barrier(const T& d, const double dhat);
+double barrier(const double d, const double dhat);
 
 /// @brief Derivative of the barrier function.
 ///
 /// \f\[
 ///     b'(d) = (\hat{d}-d) \left( 2\ln\left( \frac{d}{\hat{d}} \right) -
 ///     \frac{\hat{d}}{d} + 1\right)
 /// \f\]
@@ -42,9 +42,7 @@
 ///
 /// @param d The distance.
 /// @param dhat Activation distance of the barrier.
 /// @return The second derivative of the barrier wrt d.
 double barrier_hessian(const double d, const double dhat);
 
 } // namespace ipc
-
-#include "barrier.tpp"
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/aabb.cpp` & `ipctk-1.1.0/src/ipc/broad_phase/aabb.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 #include "aabb.hpp"
 
 #include <tbb/parallel_for.h>
 #include <tbb/blocked_range.h>
 
+#include <cfenv>
+
 namespace ipc {
 
-AABB::AABB(const ArrayMax3d& min, const ArrayMax3d& max)
-    : min(min)
-    , max(max)
+AABB::AABB(const ArrayMax3d& min, const ArrayMax3d& max) : min(min), max(max)
 {
     assert(min.size() == max.size());
     assert((min <= max).all());
     // half_extent = (max() - min()) / 2;
     // center = min() + half_extent();
 }
 
+AABB AABB::from_point(const VectorMax3d& p, const double inflation_radius)
+{
+    ArrayMax3d min = p.array(), max = p.array();
+    conservative_inflation(min, max, inflation_radius);
+    return AABB(min, max);
+}
+
 bool AABB::intersects(const AABB& other) const
 {
     assert(this->min.size() == other.max.size());
     assert(this->max.size() == other.min.size());
 
     // NOTE: This is a faster check (https://gamedev.stackexchange.com/a/587),
     // but it is inexact and can result in false negatives.
@@ -30,81 +37,98 @@
     //         || std::abs(a.center.z() - b.center.z())
     //             <= (a.half_extent.z() + b.half_extent.z()));
 
     // This on the otherhand, is exact because there is no rounding.
     return (this->min <= other.max).all() && (other.min <= this->max).all();
 };
 
+void AABB::conservative_inflation(
+    ArrayMax3d& min, ArrayMax3d& max, const double inflation_radius)
+{
+#pragma STDC FENV_ACCESS ON
+    const int current_round = std::fegetround();
+
+    std::fesetround(FE_DOWNWARD);
+    min -= inflation_radius;
+
+    std::fesetround(FE_UPWARD);
+    max += inflation_radius;
+
+    std::fesetround(current_round);
+}
+
 void build_vertex_boxes(
-    const Eigen::MatrixXd& V,
+    const Eigen::MatrixXd& vertices,
     std::vector<AABB>& vertex_boxes,
     double inflation_radius)
 {
-    vertex_boxes.resize(V.rows());
+    vertex_boxes.resize(vertices.rows());
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0, V.rows()),
+        tbb::blocked_range<size_t>(0, vertices.rows()),
         [&](const tbb::blocked_range<size_t>& r) {
             for (size_t i = r.begin(); i < r.end(); i++) {
-                vertex_boxes[i] = AABB::from_point(V.row(i), inflation_radius);
+                vertex_boxes[i] =
+                    AABB::from_point(vertices.row(i), inflation_radius);
                 vertex_boxes[i].vertex_ids = { { long(i), -1, -1 } };
             }
         });
 }
 
 void build_vertex_boxes(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
     std::vector<AABB>& vertex_boxes,
     double inflation_radius)
 {
-    vertex_boxes.resize(V0.rows());
+    vertex_boxes.resize(vertices_t0.rows());
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0, V0.rows()),
+        tbb::blocked_range<size_t>(0, vertices_t0.rows()),
         [&](const tbb::blocked_range<size_t>& r) {
             for (size_t i = r.begin(); i < r.end(); i++) {
-                vertex_boxes[i] =
-                    AABB::from_point(V0.row(i), V1.row(i), inflation_radius);
+                vertex_boxes[i] = AABB::from_point(
+                    vertices_t0.row(i), vertices_t1.row(i), inflation_radius);
                 vertex_boxes[i].vertex_ids = { { long(i), -1, -1 } };
             }
         });
 }
 
 void build_edge_boxes(
     const std::vector<AABB>& vertex_boxes,
-    const Eigen::MatrixXi& E,
+    const Eigen::MatrixXi& edges,
     std::vector<AABB>& edge_boxes)
 {
-    edge_boxes.resize(E.rows());
+    edge_boxes.resize(edges.rows());
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0, E.rows()),
+        tbb::blocked_range<size_t>(0, edges.rows()),
         [&](const tbb::blocked_range<size_t>& r) {
             for (size_t i = r.begin(); i < r.end(); i++) {
                 edge_boxes[i] =
-                    AABB(vertex_boxes[E(i, 0)], vertex_boxes[E(i, 1)]);
-                edge_boxes[i].vertex_ids = { { E(i, 0), E(i, 1), -1 } };
+                    AABB(vertex_boxes[edges(i, 0)], vertex_boxes[edges(i, 1)]);
+                edge_boxes[i].vertex_ids = { { edges(i, 0), edges(i, 1), -1 } };
             }
         });
 }
 
 void build_face_boxes(
     const std::vector<AABB>& vertex_boxes,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXi& faces,
     std::vector<AABB>& face_boxes)
 {
-    face_boxes.resize(F.rows());
+    face_boxes.resize(faces.rows());
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0, F.rows()),
+        tbb::blocked_range<size_t>(0, faces.rows()),
         [&](const tbb::blocked_range<size_t>& r) {
             for (size_t i = r.begin(); i < r.end(); i++) {
                 face_boxes[i] = AABB(
-                    vertex_boxes[F(i, 0)], vertex_boxes[F(i, 1)],
-                    vertex_boxes[F(i, 2)]);
-                face_boxes[i].vertex_ids = { { F(i, 0), F(i, 1), F(i, 2) } };
+                    vertex_boxes[faces(i, 0)], vertex_boxes[faces(i, 1)],
+                    vertex_boxes[faces(i, 2)]);
+                face_boxes[i].vertex_ids = { { faces(i, 0), faces(i, 1),
+                                               faces(i, 2) } };
             }
         });
 }
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/aabb.hpp` & `ipctk-1.1.0/src/ipc/broad_phase/aabb.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -22,54 +22,55 @@
         : AABB(
             aabb1.min.min(aabb2.min).min(aabb3.min),
             aabb1.max.max(aabb2.max).max(aabb3.max))
     {
     }
 
     /// @brief Compute a AABB for a static point.
-    static AABB from_point(const VectorMax3d& p, double inflation_radius = 0)
-    {
-        return AABB(p.array() - inflation_radius, p.array() + inflation_radius);
-    }
+    static AABB
+    from_point(const VectorMax3d& p, const double inflation_radius = 0);
 
     /// @brief Compute a AABB for a moving point (i.e. temporal edge).
     static AABB from_point(
         const VectorMax3d& p_t0,
         const VectorMax3d& p_t1,
-        double inflation_radius = 0)
+        const double inflation_radius = 0)
     {
         return AABB(
             from_point(p_t0, inflation_radius),
             from_point(p_t1, inflation_radius));
     }
 
     bool intersects(const AABB& other) const;
 
+    /// @brief Compute a conservative inflation of the AABB.
+    static void conservative_inflation(
+        ArrayMax3d& min, ArrayMax3d& max, const double inflation_radius);
+
+public:
     ArrayMax3d min;
     ArrayMax3d max;
     std::array<long, 3> vertex_ids;
-    // ArrayMax3d half_extent;
-    // ArrayMax3d center;
 };
 
 void build_vertex_boxes(
-    const Eigen::MatrixXd& V,
+    const Eigen::MatrixXd& vertices,
     std::vector<AABB>& vertex_boxes,
-    double inflation_radius = 0);
+    const double inflation_radius = 0);
 
 void build_vertex_boxes(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
     std::vector<AABB>& vertex_boxes,
-    double inflation_radius = 0);
+    const double inflation_radius = 0);
 
 void build_edge_boxes(
     const std::vector<AABB>& vertex_boxes,
-    const Eigen::MatrixXi& E,
+    const Eigen::MatrixXi& edges,
     std::vector<AABB>& edge_boxes);
 
 void build_face_boxes(
     const std::vector<AABB>& vertex_boxes,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXi& faces,
     std::vector<AABB>& face_boxes);
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/broad_phase.cpp` & `ipctk-1.1.0/src/ipc/broad_phase/broad_phase.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #include "broad_phase.hpp"
 
 #include <ipc/broad_phase/brute_force.hpp>
 #include <ipc/broad_phase/spatial_hash.hpp>
 #include <ipc/broad_phase/hash_grid.hpp>
 #include <ipc/broad_phase/sweep_and_tiniest_queue.hpp>
+#include <ipc/candidates/candidates.hpp>
 
 #include <ipc/config.hpp>
 
 namespace ipc {
 
 void BroadPhase::build(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    assert(E.size() == 0 || E.cols() == 2);
-    assert(F.size() == 0 || F.cols() == 3);
+    assert(edges.size() == 0 || edges.cols() == 2);
+    assert(faces.size() == 0 || faces.cols() == 3);
     clear();
-    build_vertex_boxes(V, vertex_boxes, inflation_radius);
-    build_edge_boxes(vertex_boxes, E, edge_boxes);
-    build_face_boxes(vertex_boxes, F, face_boxes);
+    build_vertex_boxes(vertices, vertex_boxes, inflation_radius);
+    build_edge_boxes(vertex_boxes, edges, edge_boxes);
+    build_face_boxes(vertex_boxes, faces, face_boxes);
 }
 
 void BroadPhase::build(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    assert(E.size() == 0 || E.cols() == 2);
-    assert(F.size() == 0 || F.cols() == 3);
+    assert(edges.size() == 0 || edges.cols() == 2);
+    assert(faces.size() == 0 || faces.cols() == 3);
     clear();
-    build_vertex_boxes(V0, V1, vertex_boxes, inflation_radius);
-    build_edge_boxes(vertex_boxes, E, edge_boxes);
-    build_face_boxes(vertex_boxes, F, face_boxes);
+    build_vertex_boxes(
+        vertices_t0, vertices_t1, vertex_boxes, inflation_radius);
+    build_edge_boxes(vertex_boxes, edges, edge_boxes);
+    build_face_boxes(vertex_boxes, faces, face_boxes);
 }
 
 void BroadPhase::clear()
 {
     vertex_boxes.clear();
     edge_boxes.clear();
     face_boxes.clear();
@@ -58,17 +60,17 @@
         detect_face_vertex_candidates(candidates.fv_candidates);
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 
 std::unique_ptr<BroadPhase>
-BroadPhase::make_broad_phase(const BroadPhaseMethod method)
+BroadPhase::make_broad_phase(const BroadPhaseMethod broad_phase_method)
 {
-    switch (method) {
+    switch (broad_phase_method) {
     case BroadPhaseMethod::BRUTE_FORCE:
         return std::make_unique<BruteForce>();
     case BroadPhaseMethod::HASH_GRID:
         return std::make_unique<HashGrid>();
     case BroadPhaseMethod::SPATIAL_HASH:
         return std::make_unique<SpatialHash>();
     case BroadPhaseMethod::SWEEP_AND_TINIEST_QUEUE:
@@ -81,53 +83,14 @@
                                  "because CUDA is disabled!");
 #endif
     default:
         throw std::runtime_error("Invalid BroadPhaseMethod!");
     }
 }
 
-void construct_collision_candidates(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    Candidates& candidates,
-    double inflation_radius,
-    const BroadPhaseMethod method)
-{
-    const int dim = V.cols();
-
-    candidates.clear();
-
-    std::unique_ptr<BroadPhase> broad_phase =
-        BroadPhase::make_broad_phase(method);
-    broad_phase->can_vertices_collide = mesh.can_collide;
-    broad_phase->build(V, mesh.edges(), mesh.faces(), inflation_radius);
-    broad_phase->detect_collision_candidates(dim, candidates);
-    broad_phase->clear();
-}
-
-void construct_collision_candidates(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    Candidates& candidates,
-    double inflation_radius,
-    const BroadPhaseMethod method)
-{
-    const int dim = V0.cols();
-
-    candidates.clear();
-
-    std::unique_ptr<BroadPhase> broad_phase =
-        BroadPhase::make_broad_phase(method);
-    broad_phase->can_vertices_collide = mesh.can_collide;
-    broad_phase->build(V0, V1, mesh.edges(), mesh.faces(), inflation_radius);
-    broad_phase->detect_collision_candidates(dim, candidates);
-    broad_phase->clear();
-}
-
 ////////////////////////////////////////////////////////////////////////////////
 
 bool BroadPhase::can_edge_vertex_collide(size_t ei, size_t vi) const
 {
     const auto& [e0i, e1i, _] = edge_boxes[ei].vertex_ids;
 
     return vi != e0i && vi != e1i
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/broad_phase.hpp` & `ipctk-1.1.0/src/ipc/broad_phase/broad_phase.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #pragma once
 
 #include <ipc/collision_mesh.hpp>
 #include <ipc/broad_phase/aabb.hpp>
-#include <ipc/candidates/candidates.hpp>
+#include <ipc/candidates/edge_vertex.hpp>
+#include <ipc/candidates/edge_edge.hpp>
+#include <ipc/candidates/face_vertex.hpp>
 #include <ipc/candidates/edge_face.hpp>
 
 #include <Eigen/Core>
 
 namespace ipc {
 
 /// Enumeration of implemented broad phase methods.
@@ -15,46 +17,51 @@
     HASH_GRID,
     SPATIAL_HASH,
     SWEEP_AND_TINIEST_QUEUE,
     SWEEP_AND_TINIEST_QUEUE_GPU, // Requires CUDA
     NUM_METHODS
 };
 
+static constexpr BroadPhaseMethod DEFAULT_BROAD_PHASE_METHOD =
+    BroadPhaseMethod::HASH_GRID;
+
+class Candidates; // Forward declaration
+
 class BroadPhase {
 public:
     virtual ~BroadPhase() { clear(); }
 
     /// @brief Construct a registered broad phase object.
-    /// @param method The broad phase method to use.
+    /// @param broad_phase_method The broad phase method to use.
     /// @return The constructed broad phase object.
     static std::unique_ptr<BroadPhase>
-    make_broad_phase(const BroadPhaseMethod method);
+    make_broad_phase(const BroadPhaseMethod broad_phase_method);
 
     /// @brief Build the broad phase for static collision detection.
-    /// @param V0 Positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices Vertex positions
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     virtual void build(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0);
 
     /// @brief Build the broad phase for continuous collision detection.
-    /// @param V0 Starting positions of the vertices.
-    /// @param V1 Ending positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices_t0 Starting vertices of the vertices.
+    /// @param vertices_t1 Ending vertices of the vertices.
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     virtual void build(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0);
 
     /// @brief Clear any built data.
     virtual void clear();
 
     /// @brief Find the candidate edge-vertex collisisons.
     /// @param[out] candidates The candidate edge-vertex collisisons.
@@ -80,50 +87,23 @@
     /// @param dim The dimension of the simulation (i.e., 2 or 3).
     /// @param candidates The detected collision candidates.
     virtual void
     detect_collision_candidates(int dim, Candidates& candidates) const;
 
     /// @brief Function for determining if two vertices can collide.
     std::function<bool(size_t, size_t)> can_vertices_collide =
-        [](size_t, size_t) { return true; };
+        default_can_vertices_collide;
+
+    static bool default_can_vertices_collide(size_t, size_t) { return true; }
 
 protected:
     virtual bool can_edge_vertex_collide(size_t ei, size_t vi) const;
     virtual bool can_edges_collide(size_t eai, size_t ebi) const;
     virtual bool can_face_vertex_collide(size_t fi, size_t vi) const;
     virtual bool can_edge_face_collide(size_t ei, size_t fi) const;
 
     std::vector<AABB> vertex_boxes;
     std::vector<AABB> edge_boxes;
     std::vector<AABB> face_boxes;
 };
 
-/// @brief Construct a set of discrete collision detection candidates.
-/// @param[in] mesh The surface of the contact mesh.
-/// @param[in] V Surface Vertex positions at start as rows of a matrix.
-/// @param[out] candidates The constructed candidate set as output.
-/// @param[in] inflation_radius Amount to inflate the bounding boxes.
-/// @param[in] method Broad phase method to use.
-void construct_collision_candidates(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    Candidates& candidates,
-    double inflation_radius = 0,
-    const BroadPhaseMethod method = BroadPhaseMethod::HASH_GRID);
-
-/// @brief Construct a set of continuous collision detection candidates.
-/// @note Assumes the trajectory is linear.
-/// @param[in] mesh The surface of the contact mesh.
-/// @param[in] V0 Surface vertex positions at start as rows of a matrix.
-/// @param[in] V1 Surface vertex positions at end as rows of a matrix.
-/// @param[out] candidates The constructed candidate set as output.
-/// @param[in] inflation_radius Amount to inflate the bounding boxes.
-/// @param[in] method Broad phase method to use.
-void construct_collision_candidates(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    Candidates& candidates,
-    double inflation_radius = 0,
-    const BroadPhaseMethod method = BroadPhaseMethod::HASH_GRID);
-
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/brute_force.cpp` & `ipctk-1.1.0/src/ipc/broad_phase/brute_force.cpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/brute_force.hpp` & `ipctk-1.1.0/src/ipc/broad_phase/brute_force.hpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/hash_grid.cpp` & `ipctk-1.1.0/src/ipc/broad_phase/hash_grid.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -12,46 +12,55 @@
 #include <algorithm> // std::min/max
 
 #define IPC_TOOLKIT_HASH_GRID_USE_SORT_UNIQUE // else use unordered_set
 
 namespace ipc {
 
 void HashGrid::build(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    BroadPhase::build(V, E, F, inflation_radius); // also calls clear()
+    BroadPhase::build(vertices, edges, faces, inflation_radius);
+    // BroadPhase::build also calls clear()
 
-    ArrayMax3d mesh_min = V.colwise().minCoeff().array() - inflation_radius;
-    ArrayMax3d mesh_max = V.colwise().maxCoeff().array() + inflation_radius;
-    double cell_size = suggest_good_voxel_size(V, E, inflation_radius);
+    ArrayMax3d mesh_min = vertices.colwise().minCoeff().array();
+    ArrayMax3d mesh_max = vertices.colwise().maxCoeff().array();
+    AABB::conservative_inflation(mesh_min, mesh_max, inflation_radius);
+
+    double cell_size =
+        suggest_good_voxel_size(vertices, edges, inflation_radius);
     assert(std::isfinite(cell_size));
     resize(mesh_min, mesh_max, cell_size);
 
     insert_boxes();
 }
 
 void HashGrid::build(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    BroadPhase::build(V0, V1, E, F, inflation_radius); // also calls clear()
+    BroadPhase::build(vertices_t0, vertices_t1, edges, faces, inflation_radius);
+    // BroadPhase::build also calls clear()
+
+    const ArrayMax3d mesh_min_t0 = vertices_t0.colwise().minCoeff();
+    const ArrayMax3d mesh_max_t0 = vertices_t0.colwise().maxCoeff();
+    const ArrayMax3d mesh_min_t1 = vertices_t1.colwise().minCoeff();
+    const ArrayMax3d mesh_max_t1 = vertices_t1.colwise().maxCoeff();
+
+    ArrayMax3d mesh_min = mesh_min_t0.min(mesh_min_t1);
+    ArrayMax3d mesh_max = mesh_max_t0.max(mesh_max_t1);
+    AABB::conservative_inflation(mesh_min, mesh_max, inflation_radius);
 
-    const ArrayMax3d mesh_min_t0 = V0.colwise().minCoeff();
-    const ArrayMax3d mesh_max_t0 = V0.colwise().maxCoeff();
-    const ArrayMax3d mesh_min_t1 = V1.colwise().minCoeff();
-    const ArrayMax3d mesh_max_t1 = V1.colwise().maxCoeff();
-    ArrayMax3d mesh_min = mesh_min_t0.min(mesh_min_t1) - inflation_radius;
-    ArrayMax3d mesh_max = mesh_max_t0.max(mesh_max_t1) + inflation_radius;
-    double cell_size = suggest_good_voxel_size(V0, V1, E, inflation_radius);
+    double cell_size = suggest_good_voxel_size(
+        vertices_t0, vertices_t1, edges, inflation_radius);
     assert(std::isfinite(cell_size));
     resize(mesh_min, mesh_max, cell_size);
 
     insert_boxes();
 }
 
 void HashGrid::resize(
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/hash_grid.hpp` & `ipctk-1.1.0/src/ipc/broad_phase/hash_grid.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -6,54 +6,50 @@
 
 /// @brief An entry into the hash grid as a (key, value) pair.
 struct HashItem {
     long key; /// @brief The key of the item.
     long id;  /// @brief The value of the item.
 
     /// @brief Construct a hash item as a (key, value) pair.
-    HashItem(int key, int id)
-        : key(key)
-        , id(id)
-    {
-    }
+    HashItem(int key, int id) : key(key), id(id) { }
 
     /// @brief Compare HashItems by their keys for sorting.
     bool operator<(const HashItem& other) const
     {
         if (key == other.key) {
             return id < other.id;
         }
         return key < other.key;
     }
 };
 
 class HashGrid : public BroadPhase {
 public:
     /// @brief Build the broad phase for static collision detection.
-    /// @param V0 Positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices Vertex positions
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     void build(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override;
 
     /// @brief Build the broad phase for continuous collision detection.
-    /// @param V0 Starting positions of the vertices.
-    /// @param V1 Ending positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices_t0 Starting vertices of the vertices.
+    /// @param vertices_t1 Ending vertices of the vertices.
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     void build(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override;
 
     /// @brief Clear the hash grid.
     void clear() override
     {
         BroadPhase::clear();
         vertex_items.clear();
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/spatial_hash.cpp` & `ipctk-1.1.0/src/ipc/broad_phase/spatial_hash.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -8,209 +8,162 @@
 
 #include <ipc/config.hpp>
 
 #include <tbb/enumerable_thread_specific.h>
 #include <tbb/parallel_for.h>
 #include <tbb/parallel_sort.h>
 
-// Uncomment this to construct spatial hash in parallel.
-// #define IPC_TOOLKIT_PARALLEL_SH_CONSTRUCT
-
 namespace ipc {
 
 void SpatialHash::build(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius,
     double voxelSize)
 {
-    build(V, V, E, F, inflation_radius, voxelSize);
+    build(vertices, vertices, edges, faces, inflation_radius, voxelSize);
 }
 
 void SpatialHash::build(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius,
     double voxelSize)
 {
-    assert(V0.rows() == V1.rows() && V0.cols() == V1.cols());
+    const size_t num_vertices = vertices_t0.rows();
+    dim = vertices_t0.cols();
+
+    assert(vertices_t1.rows() == num_vertices && vertices_t1.cols() == dim);
 
-    BroadPhase::build(V0, V1, E, F, inflation_radius); // also calls clear()
+    // also calls clear()
+    BroadPhase::build(vertices_t0, vertices_t1, edges, faces, inflation_radius);
 
-    dim = V0.cols();
     builtInRadius = inflation_radius;
 
     if (voxelSize <= 0) {
-        voxelSize = suggest_good_voxel_size(V0, V1, E, inflation_radius);
+        voxelSize = suggest_good_voxel_size(
+            vertices_t0, vertices_t1, edges, inflation_radius);
     }
 
-    leftBottomCorner =
-        V0.colwise().minCoeff().cwiseMin(V1.colwise().minCoeff()).array()
-        - inflation_radius;
-    rightTopCorner =
-        V0.colwise().maxCoeff().cwiseMax(V1.colwise().maxCoeff()).array()
-        + inflation_radius;
+    leftBottomCorner = vertices_t0.colwise().minCoeff().cwiseMin(
+        vertices_t1.colwise().minCoeff());
+    rightTopCorner = vertices_t0.colwise().maxCoeff().cwiseMax(
+        vertices_t1.colwise().maxCoeff());
+
+    AABB::conservative_inflation(
+        leftBottomCorner, rightTopCorner, inflation_radius);
+
     one_div_voxelSize = 1.0 / voxelSize;
     ArrayMax3d range = rightTopCorner - leftBottomCorner;
     voxelCount = (range * one_div_voxelSize).ceil().template cast<int>();
     if (voxelCount.minCoeff() <= 0) {
         // cast overflow due to huge search direction
         one_div_voxelSize = 1.0 / (range.maxCoeff() * 1.01);
         voxelCount.setOnes();
     }
     voxelCount0x1 = voxelCount[0] * voxelCount[1];
 
-    edgeStartInd = V0.rows();
-    triStartInd = edgeStartInd + E.rows();
+    edgeStartInd = num_vertices;
+    triStartInd = edgeStartInd + edges.rows();
 
     // precompute vVAI
-    std::vector<Eigen::Array3i> vertexMinVAI(V0.rows(), Eigen::Array3i::Zero());
-    std::vector<Eigen::Array3i> vertexMaxVAI(V0.rows(), Eigen::Array3i::Zero());
-    tbb::parallel_for(size_t(0), size_t(V0.rows()), [&](size_t vi) {
+    std::vector<Eigen::Array3i> vertexMinVAI(
+        num_vertices, Eigen::Array3i::Zero());
+    std::vector<Eigen::Array3i> vertexMaxVAI(
+        num_vertices, Eigen::Array3i::Zero());
+    tbb::parallel_for(size_t(0), num_vertices, [&](size_t vi) {
+        ArrayMax3d v_min = vertices_t0.row(vi).cwiseMin(vertices_t1.row(vi));
+        ArrayMax3d v_max = vertices_t0.row(vi).cwiseMax(vertices_t1.row(vi));
+        AABB::conservative_inflation(v_min, v_max, inflation_radius);
+
         ArrayMax3i vVAIMin, vVAIMax;
-        locateVoxelAxisIndex(
-            V0.row(vi).cwiseMin(V1.row(vi)).array() - inflation_radius,
-            vVAIMin);
-        locateVoxelAxisIndex(
-            V0.row(vi).cwiseMax(V1.row(vi)).array() + inflation_radius,
-            vVAIMax);
+        locateVoxelAxisIndex(v_min, vVAIMin);
+        locateVoxelAxisIndex(v_max, vVAIMax);
+
         vertexMinVAI[vi].head(dim) = vVAIMin;
         vertexMaxVAI[vi].head(dim) = vVAIMax;
     });
 
-    // #ifdef IPC_TOOLKIT_PARALLEL_SH_CONSTRUCT
-    //     std::vector<std::pair<int, int>> voxel_tmp;
-    //
-    //     for (int vi = 0; vi < V.rows(); vi++) {
-    //         voxel_tmp.emplace_back(locateVoxelIndex(V.row(vi)), vi);
-    //     }
-    // #else
-    //     for (int vi = 0; vi < V.rows(); vi++) {
-    //         voxel[locateVoxelIndex(V.row(vi))].emplace_back(vi);
-    //     }
-    // #endif
-
     pointAndEdgeOccupancy.resize(triStartInd);
 
-    tbb::parallel_for(size_t(0), size_t(V0.rows()), [&](size_t vi) {
+    tbb::parallel_for(size_t(0), num_vertices, [&](size_t vi) {
         const Eigen::Array3i &mins = vertexMinVAI[vi], &maxs = vertexMaxVAI[vi];
         assert((mins <= maxs).all());
         pointAndEdgeOccupancy[vi].reserve((maxs - mins + 1).prod());
         for (int iz = mins[2]; iz <= maxs[2]; iz++) {
             int zOffset = iz * voxelCount0x1;
             for (int iy = mins[1]; iy <= maxs[1]; iy++) {
                 int yzOffset = iy * voxelCount[0] + zOffset;
                 for (int ix = mins[0]; ix <= maxs[0]; ix++) {
                     pointAndEdgeOccupancy[vi].emplace_back(ix + yzOffset);
                 }
             }
         }
     });
 
-    tbb::parallel_for(size_t(0), size_t(E.rows()), [&](size_t ei) {
+    tbb::parallel_for(size_t(0), size_t(edges.rows()), [&](size_t ei) {
         int eiInd = ei + edgeStartInd;
 
         Eigen::Array3i mins =
-            vertexMinVAI[E(ei, 0)].min(vertexMinVAI[E(ei, 1)]);
+            vertexMinVAI[edges(ei, 0)].min(vertexMinVAI[edges(ei, 1)]);
         Eigen::Array3i maxs =
-            vertexMaxVAI[E(ei, 0)].max(vertexMaxVAI[E(ei, 1)]);
+            vertexMaxVAI[edges(ei, 0)].max(vertexMaxVAI[edges(ei, 1)]);
 
         pointAndEdgeOccupancy[eiInd].reserve((maxs - mins + 1).prod());
         for (int iz = mins[2]; iz <= maxs[2]; iz++) {
             int zOffset = iz * voxelCount0x1;
             for (int iy = mins[1]; iy <= maxs[1]; iy++) {
                 int yzOffset = iy * voxelCount[0] + zOffset;
                 for (int ix = mins[0]; ix <= maxs[0]; ix++) {
                     pointAndEdgeOccupancy[eiInd].emplace_back(ix + yzOffset);
                 }
             }
         }
     });
 
-    std::vector<std::vector<int>> voxelLoc_f(F.rows());
-    tbb::parallel_for(size_t(0), size_t(F.rows()), [&](size_t fi) {
-        Eigen::Array3i mins = vertexMinVAI[F(fi, 0)]
-                                  .min(vertexMinVAI[F(fi, 1)])
-                                  .min(vertexMinVAI[F(fi, 2)]);
-        Eigen::Array3i maxs = vertexMaxVAI[F(fi, 0)]
-                                  .max(vertexMaxVAI[F(fi, 1)])
-                                  .max(vertexMaxVAI[F(fi, 2)]);
+    std::vector<std::vector<int>> voxelLoc_f(faces.rows());
+    tbb::parallel_for(size_t(0), size_t(faces.rows()), [&](size_t fi) {
+        Eigen::Array3i mins = vertexMinVAI[faces(fi, 0)]
+                                  .min(vertexMinVAI[faces(fi, 1)])
+                                  .min(vertexMinVAI[faces(fi, 2)]);
+        Eigen::Array3i maxs = vertexMaxVAI[faces(fi, 0)]
+                                  .max(vertexMaxVAI[faces(fi, 1)])
+                                  .max(vertexMaxVAI[faces(fi, 2)]);
 
         for (int iz = mins[2]; iz <= maxs[2]; iz++) {
             int zOffset = iz * voxelCount0x1;
             for (int iy = mins[1]; iy <= maxs[1]; iy++) {
                 int yzOffset = iy * voxelCount[0] + zOffset;
                 for (int ix = mins[0]; ix <= maxs[0]; ix++) {
                     voxelLoc_f[fi].emplace_back(ix + yzOffset);
                 }
             }
         }
     });
 
-    // #ifdef IPC_TOOLKIT_PARALLEL_SH_CONSTRUCT
-    //     for (int ei = 0; ei < voxelLoc_e.size(); ei++) {
-    //         for (const auto& voxelI : voxelLoc_e[ei]) {
-    //             voxel_tmp.emplace_back(voxelI, ei + edgeStartInd);
-    //         }
-    //     }
-    //
-    //     for (int fi = 0; fi < voxelLoc_f.size(); fi++) {
-    //         for (const auto& voxelI : voxelLoc_f[fi]) {
-    //             voxel_tmp.emplace_back(voxelI, fi + triStartInd);
-    //         }
-    //     }
-    //
-    //     // Sort the voxels based on the voxel indices
-    //     tbb::parallel_sort(
-    //         voxel_tmp.begin(), voxel_tmp.end(),
-    //         [](const std::pair<int, int>& f, const std::pair<int, int>& s) {
-    //             return f.first < s.first;
-    //         });
-    //
-    //     std::vector<std::pair<int, std::vector<int>>> voxel_tmp_merged;
-    //     voxel_tmp_merged.reserve(voxel_tmp.size());
-    //     int current_voxel = -1;
-    //     for (const auto& v : voxel_tmp) {
-    //         if (current_voxel != v.first) {
-    //             assert(current_voxel < v.first);
-    //             voxel_tmp_merged.emplace_back();
-    //             voxel_tmp_merged.back().first = v.first;
-    //             current_voxel = v.first;
-    //         }
-    //
-    //         voxel_tmp_merged.back().second.push_back(v.second);
-    //     }
-    //     assert(voxel_tmp_merged.size() <= voxel_tmp.size());
-    //
-    //     voxel.insert(voxel_tmp_merged.begin(), voxel_tmp_merged.end());
-    // #else
     for (int i = 0; i < pointAndEdgeOccupancy.size(); i++) {
         for (const auto& voxelI : pointAndEdgeOccupancy[i]) {
             voxel[voxelI].emplace_back(i);
         }
     }
     for (int fi = 0; fi < voxelLoc_f.size(); fi++) {
         for (const auto& voxelI : voxelLoc_f[fi]) {
             voxel[voxelI].emplace_back(fi + triStartInd);
         }
     }
-    // #endif
 }
 
 void SpatialHash::queryPointForTriangles(
     const VectorMax3d& p, unordered_set<int>& triInds, double radius) const
 {
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(p.array() - radius, mins);
-    locateVoxelAxisIndex(p.array() + radius, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(p, p, mins, maxs, radius);
 
     triInds.clear();
 
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
@@ -233,18 +186,16 @@
 void SpatialHash::queryPointForTriangles(
     const VectorMax3d& p_t0,
     const VectorMax3d& p_t1,
     unordered_set<int>& triInds,
     double radius) const
 {
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(p_t0.array().min((p_t1).array()) - radius, mins);
-    locateVoxelAxisIndex(p_t0.array().max((p_t1).array()) + radius, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(
+        p_t0.cwiseMin(p_t1), p_t0.cwiseMax(p_t1), mins, maxs, radius);
 
     triInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
         for (int iy = mins[1]; iy <= maxs[1]; iy++) {
@@ -268,18 +219,16 @@
     const VectorMax3d& p_t1,
     unordered_set<int>& vertInds,
     unordered_set<int>& edgeInds,
     unordered_set<int>& triInds,
     double radius) const
 {
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(p_t0.array().min((p_t1).array()) - radius, mins);
-    locateVoxelAxisIndex(p_t0.array().max((p_t1).array()) + radius, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(
+        p_t0.cwiseMin(p_t1), p_t0.cwiseMax(p_t1), mins, maxs, radius);
 
     vertInds.clear();
     edgeInds.clear();
     triInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
@@ -307,21 +256,17 @@
 void SpatialHash::queryEdgeForPE(
     const VectorMax3d& e0,
     const VectorMax3d& e1,
     std::vector<int>& vertInds,
     std::vector<int>& edgeInds,
     double radius) const
 {
-    VectorMax3d leftBottom = e0.array().min(e1.array()) - radius;
-    VectorMax3d rightTop = e0.array().max(e1.array()) + radius;
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(leftBottom, mins);
-    locateVoxelAxisIndex(rightTop, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(
+        e0.cwiseMin(e1), e0.cwiseMax(e1), mins, maxs, radius);
 
     vertInds.clear();
     edgeInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
@@ -352,21 +297,17 @@
 void SpatialHash::queryEdgeForEdges(
     const VectorMax3d& e0,
     const VectorMax3d& e1,
     std::vector<int>& edgeInds,
     double radius,
     int eai) const
 {
-    VectorMax3d leftBottom = e0.array().min(e1.array()) - radius;
-    VectorMax3d rightTop = e0.array().max(e1.array()) + radius;
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(leftBottom, mins);
-    locateVoxelAxisIndex(rightTop, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(
+        e0.cwiseMin(e1), e0.cwiseMax(e1), mins, maxs, radius);
 
     edgeInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
         for (int iy = mins[1]; iy <= maxs[1]; iy++) {
@@ -387,24 +328,26 @@
 
     std::sort(edgeInds.begin(), edgeInds.end());
     edgeInds.erase(
         std::unique(edgeInds.begin(), edgeInds.end()), edgeInds.end());
 }
 
 void SpatialHash::queryEdgeForEdgesWithBBoxCheck(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
     const VectorMax3d& ea0,
     const VectorMax3d& ea1,
     std::vector<int>& edgeInds,
     double radius,
     int eai) const
 {
-    VectorMax3d leftBottom = ea0.array().min(ea1.array()) - radius;
-    VectorMax3d rightTop = ea0.array().max(ea1.array()) + radius;
+    ArrayMax3d leftBottom = ea0.cwiseMin(ea1);
+    ArrayMax3d rightTop = ea0.cwiseMax(ea1);
+    AABB::conservative_inflation(leftBottom, rightTop, radius);
+
     ArrayMax3i mins, maxs;
     locateVoxelAxisIndex(leftBottom, mins);
     locateVoxelAxisIndex(rightTop, maxs);
     mins = mins.max(ArrayMax3i::Zero(dim));
     maxs = maxs.min(voxelCount - 1);
 
     edgeInds.clear();
@@ -417,24 +360,22 @@
             for (int ix = mins[0]; ix <= maxs[0]; ix++) {
                 const auto voxelI = voxel.find(ix + yzOffset);
                 if (voxelI != voxel.end()) {
                     for (const auto& indI : voxelI->second) {
                         if (indI >= edgeStartInd && indI < triStartInd
                             && indI - edgeStartInd > eai) {
                             int ebi = indI - edgeStartInd;
-                            const VectorMax3d& eb0 = V.row(E(ebi, 0));
-                            const VectorMax3d& eb1 = V.row(E(ebi, 1));
-                            ArrayMax3d bboxEBTopRight =
-                                eb0.array().max(eb1.array());
-                            ArrayMax3d bboxEBBottomLeft =
-                                eb0.array().min(eb1.array());
-                            if (!((bboxEBBottomLeft - rightTop.array() > 0.0)
-                                      .any()
-                                  || (leftBottom.array() - bboxEBTopRight > 0.0)
-                                         .any())) {
+                            const VectorMax3d& eb0 =
+                                vertices.row(edges(ebi, 0));
+                            const VectorMax3d& eb1 =
+                                vertices.row(edges(ebi, 1));
+                            ArrayMax3d bboxEBBottomLeft = eb0.cwiseMin(eb1);
+                            ArrayMax3d bboxEBTopRight = eb0.cwiseMax(eb1);
+                            if (!((bboxEBBottomLeft > rightTop).any()
+                                  || (leftBottom > bboxEBTopRight).any())) {
                                 edgeInds.emplace_back(indI - edgeStartInd);
                             }
                         }
                     }
                 }
             }
         }
@@ -449,25 +390,21 @@
     const VectorMax3d& ea1_t0,
     const VectorMax3d& ea0_t1,
     const VectorMax3d& ea1_t1,
     std::vector<int>& edgeInds,
     double radius,
     int eai) const
 {
-    VectorMax3d leftBottom = ea0_t0.array()
-                                 .min(ea1_t0.array())
-                                 .min(ea0_t1.array())
-                                 .min(ea1_t1.array());
-    VectorMax3d rightTop = ea0_t0.array()
-                               .max(ea1_t0.array())
-                               .max(ea0_t1.array())
-                               .max(ea1_t1.array());
+    VectorMax3d leftBottom =
+        ea0_t0.cwiseMin(ea1_t0).cwiseMin(ea0_t1).cwiseMin(ea1_t1);
+    VectorMax3d rightTop =
+        ea0_t0.cwiseMax(ea1_t0).cwiseMax(ea0_t1).cwiseMax(ea1_t1);
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(leftBottom.array() - radius, mins);
-    locateVoxelAxisIndex(rightTop.array() + radius, maxs);
+    locateVoxelAxisIndex(leftBottom, mins);
+    locateVoxelAxisIndex(rightTop, maxs);
     mins = mins.max(ArrayMax3i::Zero(dim));
     maxs = maxs.min(voxelCount - 1);
 
     edgeInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
@@ -495,22 +432,18 @@
 void SpatialHash::queryTriangleForPoints(
     const VectorMax3d& t0,
     const VectorMax3d& t1,
     const VectorMax3d& t2,
     unordered_set<int>& pointInds,
     double radius) const
 {
-    VectorMax3d leftBottom =
-        t0.array().min(t1.array()).min(t2.array()) - radius;
-    VectorMax3d rightTop = t0.array().max(t1.array()).max(t2.array()) + radius;
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(leftBottom.array() - radius, mins);
-    locateVoxelAxisIndex(rightTop.array() + radius, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(
+        t0.cwiseMin(t1).cwiseMin(t2), t0.cwiseMax(t1).cwiseMax(t2), mins, maxs,
+        radius);
 
     pointInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
         for (int iy = mins[1]; iy <= maxs[1]; iy++) {
@@ -535,33 +468,21 @@
     const VectorMax3d& t2_t0,
     const VectorMax3d& t0_t1,
     const VectorMax3d& t1_t1,
     const VectorMax3d& t2_t1,
     unordered_set<int>& pointInds,
     double radius) const
 {
-    VectorMax3d leftBottom = t0_t0.array()
-                                 .min(t1_t0.array())
-                                 .min(t2_t0.array())
-                                 .min(t0_t1.array())
-                                 .min(t1_t1.array())
-                                 .min(t2_t1.array())
-        - radius;
-    VectorMax3d rightTop = t0_t0.array()
-                               .max(t1_t0.array())
-                               .max(t2_t0.array())
-                               .max(t0_t1.array())
-                               .max(t1_t1.array())
-                               .max(t2_t1.array())
-        + radius;
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(leftBottom.array(), mins);
-    locateVoxelAxisIndex(rightTop.array(), maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    // clang-format off
+    locateBoxVoxelAxisIndex(
+        t0_t0.cwiseMin(t1_t0).cwiseMin(t2_t0).cwiseMin(t0_t1).cwiseMin(t1_t1).cwiseMin(t2_t1),
+        t0_t0.cwiseMax(t1_t0).cwiseMax(t2_t0).cwiseMax(t0_t1).cwiseMax(t1_t1).cwiseMax(t2_t1),
+        mins, maxs, radius);
+    // clang-format on
 
     pointInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
         for (int iy = mins[1]; iy <= maxs[1]; iy++) {
@@ -583,21 +504,18 @@
 void SpatialHash::queryTriangleForEdges(
     const VectorMax3d& t0,
     const VectorMax3d& t1,
     const VectorMax3d& t2,
     unordered_set<int>& edgeInds,
     double radius) const
 {
-    VectorMax3d leftBottom = t0.array().min(t1.array()).min(t2.array());
-    VectorMax3d rightTop = t0.array().max(t1.array()).max(t2.array());
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(leftBottom.array() - radius, mins);
-    locateVoxelAxisIndex(rightTop.array() + radius, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(
+        t0.cwiseMin(t1).cwiseMin(t2), t0.cwiseMax(t1).cwiseMax(t2), mins, maxs,
+        radius);
 
     edgeInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
         for (int iy = mins[1]; iy <= maxs[1]; iy++) {
@@ -618,21 +536,17 @@
 
 void SpatialHash::queryEdgeForTriangles(
     const VectorMax3d& e0,
     const VectorMax3d& e1,
     unordered_set<int>& triInds,
     double radius) const
 {
-    VectorMax3d leftBottom = e0.array().min(e1.array());
-    VectorMax3d rightTop = e0.array().max(e1.array());
     ArrayMax3i mins, maxs;
-    locateVoxelAxisIndex(leftBottom.array() - radius, mins);
-    locateVoxelAxisIndex(rightTop.array() + radius, maxs);
-    mins = mins.max(ArrayMax3i::Zero(dim));
-    maxs = maxs.min(voxelCount - 1);
+    locateBoxVoxelAxisIndex(
+        e0.cwiseMin(e1), e0.cwiseMax(e1), mins, maxs, radius);
 
     triInds.clear();
     int min_z = mins.size() >= 3 ? mins[2] : 0;
     int max_z = maxs.size() >= 3 ? maxs[2] : 0;
     for (int iz = min_z; iz <= max_z; iz++) {
         int zOffset = iz * voxelCount0x1;
         for (int iy = mins[1]; iy <= maxs[1]; iy++) {
@@ -713,57 +627,49 @@
                 edgeInds.insert(indI - edgeStartInd);
             }
         }
     }
 }
 
 void SpatialHash::queryEdgeForEdgesWithBBoxCheck(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
     int eai,
     unordered_set<int>& edgeInds) const
 {
-    const VectorMax3d& ea0_t0 = V0.row(E(eai, 0));
-    const VectorMax3d& ea1_t0 = V0.row(E(eai, 1));
-    const VectorMax3d& ea0_t1 = V1.row(E(eai, 0));
-    const VectorMax3d& ea1_t1 = V1.row(E(eai, 1));
-
-    ArrayMax3d bboxEATopRight = ea0_t0.array()
-                                    .max(ea1_t0.array())
-                                    .max(ea0_t1.array())
-                                    .max(ea1_t1.array());
-    ArrayMax3d bboxEABottomLeft = ea0_t0.array()
-                                      .min(ea1_t0.array())
-                                      .min(ea0_t1.array())
-                                      .min(ea1_t1.array());
+    const VectorMax3d& ea0_t0 = vertices_t0.row(edges(eai, 0));
+    const VectorMax3d& ea1_t0 = vertices_t0.row(edges(eai, 1));
+    const VectorMax3d& ea0_t1 = vertices_t1.row(edges(eai, 0));
+    const VectorMax3d& ea1_t1 = vertices_t1.row(edges(eai, 1));
+
+    const ArrayMax3d bboxEABottomLeft =
+        ea0_t0.cwiseMin(ea1_t0).cwiseMin(ea0_t1).cwiseMin(ea1_t1);
+    const ArrayMax3d bboxEATopRight =
+        ea0_t0.cwiseMax(ea1_t0).cwiseMax(ea0_t1).cwiseMax(ea1_t1);
 
     edgeInds.clear();
     for (const auto& voxelInd : pointAndEdgeOccupancy[eai + edgeStartInd]) {
         const auto& voxelI = voxel.at(voxelInd);
         for (const auto& indI : voxelI) {
             if (indI >= edgeStartInd && indI < triStartInd
                 && indI - edgeStartInd > eai) {
                 int ebi = indI - edgeStartInd;
-                const VectorMax3d& eb0_t0 = V0.row(E(ebi, 0));
-                const VectorMax3d& eb1_t0 = V0.row(E(ebi, 1));
-                const VectorMax3d& eb0_t1 = V1.row(E(ebi, 0));
-                const VectorMax3d& eb1_t1 = V1.row(E(ebi, 1));
-
-                ArrayMax3d bboxEBTopRight = eb0_t0.array()
-                                                .max(eb1_t0.array())
-                                                .max(eb0_t1.array())
-                                                .max(eb1_t1.array());
-                ArrayMax3d bboxEBBottomLeft = eb0_t0.array()
-                                                  .min(eb1_t0.array())
-                                                  .min(eb0_t1.array())
-                                                  .min(eb1_t1.array());
+                const VectorMax3d& eb0_t0 = vertices_t0.row(edges(ebi, 0));
+                const VectorMax3d& eb1_t0 = vertices_t0.row(edges(ebi, 1));
+                const VectorMax3d& eb0_t1 = vertices_t1.row(edges(ebi, 0));
+                const VectorMax3d& eb1_t1 = vertices_t1.row(edges(ebi, 1));
+
+                const ArrayMax3d bboxEBBottomLeft =
+                    eb0_t0.cwiseMin(eb1_t0).cwiseMin(eb0_t1).cwiseMin(eb1_t1);
+                const ArrayMax3d bboxEBTopRight =
+                    eb0_t0.cwiseMax(eb1_t0).cwiseMax(eb0_t1).cwiseMax(eb1_t1);
 
-                if (!((bboxEBBottomLeft - bboxEATopRight > 0.0).any()
-                      || (bboxEABottomLeft - bboxEBTopRight > 0.0).any())) {
+                if (!((bboxEBBottomLeft > bboxEATopRight).any()
+                      || (bboxEABottomLeft > bboxEBTopRight).any())) {
                     edgeInds.insert(indI - edgeStartInd);
                 }
             }
         }
     }
 }
 
@@ -786,15 +692,15 @@
 
 void SpatialHash::detect_edge_vertex_candidates(
     std::vector<EdgeVertexCandidate>& candidates) const
 {
     tbb::enumerable_thread_specific<std::vector<EdgeVertexCandidate>> storages;
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0ul, vertex_boxes.size()),
+        tbb::blocked_range<size_t>(size_t(0), vertex_boxes.size()),
         [&](const tbb::blocked_range<size_t>& range) {
             auto& local_candidates = storages.local();
 
             for (long vi = range.begin(); vi != range.end(); vi++) {
                 const AABB& vertex_box = vertex_boxes[vi];
 
                 unordered_set<int> edgeInds;
@@ -818,15 +724,15 @@
 
 void SpatialHash::detect_edge_edge_candidates(
     std::vector<EdgeEdgeCandidate>& candidates) const
 {
     tbb::enumerable_thread_specific<std::vector<EdgeEdgeCandidate>> storages;
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0ul, edge_boxes.size()),
+        tbb::blocked_range<size_t>(size_t(0), edge_boxes.size()),
         [&](const tbb::blocked_range<size_t>& range) {
             auto& local_candidates = storages.local();
 
             for (long eai = range.begin(); eai != range.end(); eai++) {
                 const AABB& edge_a_box = edge_boxes[eai];
 
                 unordered_set<int> edgeInds;
@@ -850,15 +756,15 @@
 
 void SpatialHash::detect_face_vertex_candidates(
     std::vector<FaceVertexCandidate>& candidates) const
 {
     tbb::enumerable_thread_specific<std::vector<FaceVertexCandidate>> storages;
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0ul, vertex_boxes.size()),
+        tbb::blocked_range<size_t>(size_t(0), vertex_boxes.size()),
         [&](const tbb::blocked_range<size_t>& range) {
             auto& local_candidates = storages.local();
 
             for (long vi = range.begin(); vi != range.end(); vi++) {
                 const AABB& vertex_box = vertex_boxes[vi];
 
                 unordered_set<int> triInds;
@@ -882,15 +788,15 @@
 
 void SpatialHash::detect_edge_face_candidates(
     std::vector<EdgeFaceCandidate>& candidates) const
 {
     tbb::enumerable_thread_specific<std::vector<EdgeFaceCandidate>> storages;
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0ul, edge_boxes.size()),
+        tbb::blocked_range<size_t>(size_t(0), edge_boxes.size()),
         [&](const tbb::blocked_range<size_t>& range) {
             auto& local_candidates = storages.local();
 
             for (long ei = range.begin(); ei != range.end(); ei++) {
                 const AABB& edge_box = edge_boxes[ei];
 
                 unordered_set<int> triInds;
@@ -920,20 +826,33 @@
     locateVoxelAxisIndex(p, voxelAxisIndex);
     return voxelAxisIndex2VoxelIndex(voxelAxisIndex);
 }
 
 void SpatialHash::SpatialHash::locateVoxelAxisIndex(
     const VectorMax3d& p, ArrayMax3i& voxelAxisIndex) const
 {
-    voxelAxisIndex = ((p - leftBottomCorner) * one_div_voxelSize)
-                         .array()
+    voxelAxisIndex = ((p.array() - leftBottomCorner) * one_div_voxelSize)
                          .floor()
                          .template cast<int>();
 }
 
+void SpatialHash::locateBoxVoxelAxisIndex(
+    ArrayMax3d minCorner,
+    ArrayMax3d maxCorner,
+    ArrayMax3i& minIndex,
+    ArrayMax3i& maxIndex,
+    const double inflation_radius) const
+{
+    AABB::conservative_inflation(minCorner, maxCorner, inflation_radius);
+    locateVoxelAxisIndex(minCorner, minIndex);
+    locateVoxelAxisIndex(maxCorner, maxIndex);
+    minIndex = minIndex.max(ArrayMax3i::Zero(dim));
+    maxIndex = maxIndex.min(voxelCount - 1);
+}
+
 int SpatialHash::voxelAxisIndex2VoxelIndex(
     const ArrayMax3i& voxelAxisIndex) const
 {
     return voxelAxisIndex2VoxelIndex(
         voxelAxisIndex[0], voxelAxisIndex[1],
         voxelAxisIndex.size() >= 3 ? voxelAxisIndex[2] : 0);
 }
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/spatial_hash.hpp` & `ipctk-1.1.0/src/ipc/broad_phase/spatial_hash.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #include <vector>
 
 namespace ipc {
 
 class SpatialHash : public BroadPhase {
 public: // data
-    VectorMax3d leftBottomCorner, rightTopCorner;
+    ArrayMax3d leftBottomCorner, rightTopCorner;
     ArrayMax3i voxelCount;
     double one_div_voxelSize;
     int voxelCount0x1;
 
     int edgeStartInd, triStartInd;
 
     unordered_map<int, std::vector<int>> voxel;
@@ -26,66 +26,70 @@
     int dim;
     double builtInRadius;
 
 public: // constructor
     SpatialHash() { }
 
     SpatialHash(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0,
         double voxelSize = -1)
     {
-        build(V, E, F, inflation_radius, voxelSize);
+        build(vertices, edges, faces, inflation_radius, voxelSize);
     }
 
     SpatialHash(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0,
         double voxelSize = -1)
     {
-        build(V0, V1, E, F, inflation_radius, voxelSize);
+        build(
+            vertices_t0, vertices_t1, edges, faces, inflation_radius,
+            voxelSize);
     }
 
 public: // API
     void build(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override
     {
-        build(V, E, F, inflation_radius, /*voxelSize=*/-1);
+        build(vertices, edges, faces, inflation_radius, /*voxelSize=*/-1);
     }
 
     void build(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override
     {
-        build(V0, V1, E, F, inflation_radius, /*voxelSize=*/-1);
+        build(
+            vertices_t0, vertices_t1, edges, faces, inflation_radius,
+            /*voxelSize=*/-1);
     }
 
     void build(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius,
         double voxelSize);
 
     void build(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius,
         double voxelSize);
 
     void clear() override
     {
         BroadPhase::clear();
         voxel.clear();
@@ -122,16 +126,16 @@
         const VectorMax3d& ea0,
         const VectorMax3d& ea1,
         std::vector<int>& edgeInds,
         double radius = 0,
         int eai = -1) const;
 
     void queryEdgeForEdgesWithBBoxCheck(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
         const VectorMax3d& ea0,
         const VectorMax3d& ea1,
         std::vector<int>& edgeInds,
         double radius = 0,
         int eai = -1) const;
 
     void queryEdgeForEdges(
@@ -183,17 +187,17 @@
 
     void queryPointForTriangles(int vi, unordered_set<int>& triInds) const;
 
     // will only put edges with larger than ei index into edgeInds
     void queryEdgeForEdges(int eai, unordered_set<int>& edgeInds) const;
 
     void queryEdgeForEdgesWithBBoxCheck(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
         int eai,
         unordered_set<int>& edgeInds) const;
 
     void queryEdgeForTriangles(int ei, unordered_set<int>& triInds) const;
 
     ////////////////////////////////////////////////////////////////////////////
     // BroadPhase API
@@ -216,13 +220,20 @@
 
 protected: // helper functions
     int locateVoxelIndex(const VectorMax3d& p) const;
 
     void locateVoxelAxisIndex(
         const VectorMax3d& p, ArrayMax3i& voxelAxisIndex) const;
 
+    void locateBoxVoxelAxisIndex(
+        ArrayMax3d minCorner,
+        ArrayMax3d maxCorner,
+        ArrayMax3i& minIndex,
+        ArrayMax3i& maxIndex,
+        const double inflation_radius = 0) const;
+
     int voxelAxisIndex2VoxelIndex(const ArrayMax3i& voxelAxisIndex) const;
 
     int voxelAxisIndex2VoxelIndex(int ix, int iy, int iz) const;
 };
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/sweep_and_tiniest_queue.cpp` & `ipctk-1.1.0/src/ipc/broad_phase/sweep_and_tiniest_queue.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 #ifdef IPC_TOOLKIT_WITH_CUDA
 #include <ccdgpu/helper.cuh>
 #endif
 
 namespace ipc {
 
 void SweepAndTiniestQueue::build(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    build(V, V, E, F, inflation_radius);
+    build(vertices, vertices, edges, faces, inflation_radius);
 }
 
 void SweepAndTiniestQueue::build(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    CopyMeshBroadPhase::copy_mesh(E, F);
-    num_vertices = V0.rows();
-    stq::cpu::constructBoxes(V0, V1, E, F, boxes, inflation_radius);
+    CopyMeshBroadPhase::copy_mesh(edges, faces);
+    num_vertices = vertices_t0.rows();
+    stq::cpu::constructBoxes(
+        vertices_t0, vertices_t1, edges, faces, boxes, inflation_radius);
     int n = boxes.size();
     stq::cpu::sort_along_xaxis(boxes);
     stq::cpu::run_sweep_cpu(boxes, n, overlaps);
 }
 
 void SweepAndTiniestQueue::clear()
 {
@@ -114,34 +115,35 @@
         && id < num_vertices + this->edges.rows() + this->faces.rows();
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 
 #ifdef IPC_TOOLKIT_WITH_CUDA
 void SweepAndTiniestQueueGPU::build(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    CopyMeshBroadPhase::copy_mesh(E, F);
+    CopyMeshBroadPhase::copy_mesh(edges, faces);
     ccd::gpu::construct_static_collision_candidates(
-        V, E, F, overlaps, boxes, inflation_radius);
+        vertices, edges, faces, overlaps, boxes, inflation_radius);
 }
 
 void SweepAndTiniestQueueGPU::build(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     double inflation_radius)
 {
-    CopyMeshBroadPhase::copy_mesh(E, F);
+    CopyMeshBroadPhase::copy_mesh(edges, faces);
     ccd::gpu::construct_continuous_collision_candidates(
-        V0, V1, E, F, overlaps, boxes, inflation_radius);
+        vertices_t0, vertices_t1, edges, faces, overlaps, boxes,
+        inflation_radius);
 }
 
 void SweepAndTiniestQueueGPU::clear()
 {
     BroadPhase::clear();
     overlaps.clear();
     boxes.clear();
@@ -209,18 +211,18 @@
     throw std::runtime_error("Not implemented!");
 }
 #endif
 
 ////////////////////////////////////////////////////////////////////////////////
 
 void CopyMeshBroadPhase::copy_mesh(
-    const Eigen::MatrixXi& E, const Eigen::MatrixXi& F)
+    const Eigen::MatrixXi& p_edges, const Eigen::MatrixXi& p_faces)
 {
-    edges = E;
-    faces = F;
+    edges = p_edges;
+    faces = p_faces;
 }
 
 bool CopyMeshBroadPhase::can_edge_vertex_collide(size_t ei, size_t vi) const
 {
     const long e0i = edges(ei, 0), e1i = edges(ei, 1);
 
     return vi != e0i && vi != e1i
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/sweep_and_tiniest_queue.hpp` & `ipctk-1.1.0/src/ipc/broad_phase/sweep_and_tiniest_queue.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -13,49 +13,49 @@
 
 namespace ipc {
 
 // A version of the BP that copies the meshes into the class rather than making
 // the AABBs.
 class CopyMeshBroadPhase : public BroadPhase {
 protected:
-    void copy_mesh(const Eigen::MatrixXi& E, const Eigen::MatrixXi& F);
+    void copy_mesh(const Eigen::MatrixXi& edges, const Eigen::MatrixXi& faces);
 
     bool can_edge_vertex_collide(size_t ei, size_t vi) const override;
     bool can_edges_collide(size_t eai, size_t ebi) const override;
     bool can_face_vertex_collide(size_t fi, size_t vi) const override;
     bool can_edge_face_collide(size_t ei, size_t fi) const override;
 
     Eigen::MatrixXi edges;
     Eigen::MatrixXi faces;
 };
 
 class SweepAndTiniestQueue : public CopyMeshBroadPhase {
 public:
     /// @brief Build the broad phase for static collision detection.
-    /// @param V0 Positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices Vertex positions
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     void build(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override;
 
     /// @brief Build the broad phase for continuous collision detection.
-    /// @param V0 Starting positions of the vertices.
-    /// @param V1 Ending positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices_t0 Starting vertex positions
+    /// @param vertices_t1 Ending vertex positions
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     void build(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override;
 
     /// @brief Clear any built data.
     void clear() override;
 
     /// @brief Find the candidate edge-vertex collisisons.
     /// @param[out] candidates The candidate edge-vertex collisisons.
@@ -90,35 +90,35 @@
     long num_vertices;
 };
 
 #ifdef IPC_TOOLKIT_WITH_CUDA
 class SweepAndTiniestQueueGPU : public CopyMeshBroadPhase {
 public:
     /// @brief Build the broad phase for static collision detection.
-    /// @param V0 Positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices Vertex positions
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     void build(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override;
 
     /// @brief Build the broad phase for continuous collision detection.
-    /// @param V0 Starting positions of the vertices.
-    /// @param V1 Ending positions of the vertices.
-    /// @param E Edges of the mesh.
-    /// @param F Faces of the mesh.
+    /// @param vertices_t0 Starting vertex positions
+    /// @param vertices_t1 Ending vertex positions
+    /// @param edges Collision mesh edges
+    /// @param faces Collision mesh faces
     /// @param inflation_radius Radius of inflation around all elements.
     void build(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         double inflation_radius = 0) override;
 
     /// @brief Clear any built data.
     void clear() override;
 
     /// @brief Find the candidate edge-vertex collisisons.
     /// @param[out] candidates The candidate edge-vertex collisisons.
```

### Comparing `ipctk-1.0.0/src/ipc/broad_phase/voxel_size_heuristic.hpp` & `ipctk-1.1.0/src/ipc/broad_phase/voxel_size_heuristic.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 #pragma once
 
 #include <Eigen/Core>
 
 namespace ipc {
 
 double suggest_good_voxel_size(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
     double inflation_radius = 0);
 
 double suggest_good_voxel_size(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
     double inflation_radius = 0);
 
 /// @brief Compute the average edge length of a mesh.
 double mean_edge_length(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E,
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges,
     double& std_deviation);
 
 /// @brief Compute the average displacement length.
-double
-mean_displacement_length(const Eigen::MatrixXd& U, double& std_deviation);
+double mean_displacement_length(
+    const Eigen::MatrixXd& displacements, double& std_deviation);
 
 /// @brief Compute the median edge length of a mesh.
 double median_edge_length(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E);
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges);
 
 /// @brief Compute the median displacement length.
-double median_displacement_length(const Eigen::MatrixXd& U);
+double median_displacement_length(const Eigen::MatrixXd& displacements);
 
 /// @brief Compute the maximum edge length of a mesh.
 double max_edge_length(
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const Eigen::MatrixXi& E);
+    const Eigen::MatrixXd& vertices_t0,
+    const Eigen::MatrixXd& vertices_t1,
+    const Eigen::MatrixXi& edges);
 
 /// @brief Compute the maximum displacement length.
-double max_displacement_length(const Eigen::MatrixXd& U);
+double max_displacement_length(const Eigen::MatrixXd& displacements);
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/candidates/edge_face.hpp` & `ipctk-1.1.0/src/ipc/candidates/edge_face.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 #include <vector>
 
 namespace ipc {
 
 /// @brief Candidate for <b>intersection</b> between edge and face.
 ///
 /// Not included in Candidates because it is not a collision candidate.
-struct EdgeFaceCandidate {
-    EdgeFaceCandidate(long edge_index, long face_index);
+class EdgeFaceCandidate {
+public:
+    EdgeFaceCandidate(long edge_id, long face_id);
 
     bool operator==(const EdgeFaceCandidate& other) const;
     bool operator!=(const EdgeFaceCandidate& other) const;
     /// @brief Compare EdgeFaceCandidate for sorting.
     bool operator<(const EdgeFaceCandidate& other) const;
 
     template <typename H>
     friend H AbslHashValue(H h, const EdgeFaceCandidate& fv)
     {
-        return H::combine(std::move(h), fv.edge_index, fv.face_index);
+        return H::combine(std::move(h), fv.edge_id, fv.face_id);
     }
 
-    long edge_index;
-    long face_index;
+    long edge_id; ///< @brief ID of the edge
+    long face_id; ///< @brief ID of the face
 };
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/candidates/edge_vertex.hpp` & `ipctk-1.1.0/src/ipc/candidates/edge_vertex.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,81 @@
 #pragma once
 
+#include <ipc/candidates/collision_stencil.hpp>
 #include <ipc/candidates/continuous_collision_candidate.hpp>
 #include <ipc/distance/distance_type.hpp>
 
 #include <Eigen/Core>
 
 #include <array>
 
 namespace ipc {
 
-struct EdgeVertexCandidate : ContinuousCollisionCandidate {
-    EdgeVertexCandidate(long edge_index, long vertex_index);
-
-    int num_vertices() const { return 3; };
-
-    std::array<long, 4>
-    vertex_indices(const Eigen::MatrixXi& E, const Eigen::MatrixXi& F) const
+class EdgeVertexCandidate : public ContinuousCollisionCandidate {
+public:
+    EdgeVertexCandidate(long edge_id, long vertex_id);
+
+    int num_vertices() const override { return 3; };
+
+    std::array<long, 4> vertex_ids(
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces) const override
     {
-        return { { vertex_index, E(edge_index, 0), E(edge_index, 1), -1 } };
+        return { { vertex_id, edges(edge_id, 0), edges(edge_id, 1), -1 } };
     }
 
-    double compute_distance(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
-        const PointEdgeDistanceType dtype = PointEdgeDistanceType::AUTO) const;
-
-    VectorMax9d compute_distance_gradient(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
-        const PointEdgeDistanceType dtype = PointEdgeDistanceType::AUTO) const;
-
-    MatrixMax9d compute_distance_hessian(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
-        const PointEdgeDistanceType dtype = PointEdgeDistanceType::AUTO) const;
-
     // ------------------------------------------------------------------------
 
-    /// Perform narrow-phase CCD on the candidate.
-    /// @param[in] V0 Mesh vertex positions at the start of the time step.
-    /// @param[in] V1 Mesh vertex positions at the end of the time step.
-    /// @param[in] E Mesh edges as rows of indicies into V.
-    /// @param[in] F Mesh triangular faces as rows of indicies into V.
-    /// @param[out] toi Computed time of impact (normalized).
-    /// @param[in] tmax Maximum time (normalized) to look for collisions. Should be in [0, 1].
-    /// @param[in] tolerance CCD tolerance used by Tight-Inclusion CCD.
-    /// @param[in] max_iterations Maximum iterations used by Tight-Inclusion CCD.
-    /// @param[in] conservative_rescaling Conservative rescaling value used to avoid taking steps exactly to impact.
-    /// @return If the candidate had a collision over the time interval.
-    bool
-    ccd(const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
-        double& toi,
-        const double min_distance = 0.0,
-        const double tmax = 1.0,
-        const double tolerance = DEFAULT_CCD_TOLERANCE,
-        const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
-        const double conservative_rescaling =
-            DEFAULT_CCD_CONSERVATIVE_RESCALING) const override;
-
     void print_ccd_query(
-        const Eigen::MatrixXd& V0,
-        const Eigen::MatrixXd& V1,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override;
+        const Eigen::MatrixXd& vertices_t0,
+        const Eigen::MatrixXd& vertices_t1,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces) const override;
 
     // ------------------------------------------------------------------------
 
     bool operator==(const EdgeVertexCandidate& other) const;
     bool operator!=(const EdgeVertexCandidate& other) const;
     /// @brief Compare EdgeVertexCandidates for sorting.
     bool operator<(const EdgeVertexCandidate& other) const;
 
     template <typename H>
     friend H AbslHashValue(H h, const EdgeVertexCandidate& ev)
     {
-        return H::combine(std::move(h), ev.edge_index, ev.vertex_index);
+        return H::combine(std::move(h), ev.edge_id, ev.vertex_id);
     }
 
-    long edge_index;
-    long vertex_index;
+    long edge_id;   ///< @brief ID of the edge
+    long vertex_id; ///< @brief ID of the vertex
+
+    using CollisionStencil::compute_distance;
+    using CollisionStencil::compute_distance_gradient;
+    using CollisionStencil::compute_distance_hessian;
+    using ContinuousCollisionCandidate::ccd;
+
+protected:
+    double compute_distance(const VectorMax12d& positions) const override;
+
+    VectorMax12d
+    compute_distance_gradient(const VectorMax12d& positions) const override;
+
+    MatrixMax12d
+    compute_distance_hessian(const VectorMax12d& positions) const override;
+
+    bool
+    ccd(const VectorMax12d& vertices_t0,
+        const VectorMax12d& vertices_t1,
+        double& toi,
+        const double min_distance = 0.0,
+        const double tmax = 1.0,
+        const double tolerance = DEFAULT_CCD_TOLERANCE,
+        const long max_iterations = DEFAULT_CCD_MAX_ITERATIONS,
+        const double conservative_rescaling =
+            DEFAULT_CCD_CONSERVATIVE_RESCALING) const override;
+
+    virtual PointEdgeDistanceType known_dtype() const
+    {
+        return PointEdgeDistanceType::AUTO;
+    }
 };
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/candidates/vertex_vertex.cpp` & `ipctk-1.1.0/src/ipc/candidates/vertex_vertex.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,57 @@
 #include "vertex_vertex.hpp"
 
 #include <ipc/distance/point_point.hpp>
 
 namespace ipc {
 
-VertexVertexCandidate::VertexVertexCandidate(
-    long vertex0_index, long vertex1_index)
-    : vertex0_index(vertex0_index)
-    , vertex1_index(vertex1_index)
+VertexVertexCandidate::VertexVertexCandidate(long vertex0_id, long vertex1_id)
+    : vertex0_id(vertex0_id)
+    , vertex1_id(vertex1_id)
 {
 }
 
-double VertexVertexCandidate::compute_distance(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F) const
+double
+VertexVertexCandidate::compute_distance(const VectorMax12d& positions) const
 {
-    return point_point_distance(V.row(vertex0_index), V.row(vertex1_index));
+    assert(positions.size() == 4 || positions.size() == 6);
+    const int dim = positions.size() / 2;
+    return point_point_distance(positions.head(dim), positions.tail(dim));
 }
 
-VectorMax6d VertexVertexCandidate::compute_distance_gradient(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F) const
+VectorMax12d VertexVertexCandidate::compute_distance_gradient(
+    const VectorMax12d& positions) const
 {
-    VectorMax6d distance_grad;
-    point_point_distance_gradient(
-        V.row(vertex0_index), V.row(vertex1_index), distance_grad);
-    return distance_grad;
+    assert(positions.size() == 4 || positions.size() == 6);
+    const int dim = positions.size() / 2;
+    return point_point_distance_gradient(
+        positions.head(dim), positions.tail(dim));
 }
 
-MatrixMax6d VertexVertexCandidate::compute_distance_hessian(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F) const
+MatrixMax12d VertexVertexCandidate::compute_distance_hessian(
+    const VectorMax12d& positions) const
 {
-    MatrixMax6d distance_hess;
-    point_point_distance_hessian(
-        V.row(vertex0_index), V.row(vertex1_index), distance_hess);
-    return distance_hess;
+    assert(positions.size() == 4 || positions.size() == 6);
+    const int dim = positions.size() / 2;
+    return point_point_distance_hessian(
+        positions.head(dim), positions.tail(dim));
 }
 
 bool VertexVertexCandidate::operator==(const VertexVertexCandidate& other) const
 {
-    return vertex0_index == other.vertex0_index
-        && vertex1_index == other.vertex1_index;
+    return vertex0_id == other.vertex0_id && vertex1_id == other.vertex1_id;
 }
 
 bool VertexVertexCandidate::operator!=(const VertexVertexCandidate& other) const
 {
     return !(*this == other);
 }
 
 bool VertexVertexCandidate::operator<(const VertexVertexCandidate& other) const
 {
-    if (vertex0_index == other.vertex0_index) {
-        return vertex1_index < other.vertex1_index;
+    if (vertex0_id == other.vertex0_id) {
+        return vertex1_id < other.vertex1_id;
     }
-    return vertex0_index < other.vertex0_index;
+    return vertex0_id < other.vertex0_id;
 }
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/ccd/aabb.cpp` & `ipctk-1.1.0/src/ipc/ccd/aabb.cpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/ccd/aabb.hpp` & `ipctk-1.1.0/src/ipc/ccd/aabb.hpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/ccd/ccd.cpp` & `ipctk-1.1.0/src/ipc/ccd/ccd.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 #include "ccd.hpp"
 
+#include <ipc/distance/point_point.hpp>
 #include <ipc/distance/point_edge.hpp>
 #include <ipc/distance/edge_edge.hpp>
 #include <ipc/distance/point_triangle.hpp>
 
 #include <ipc/config.hpp>
 
 #ifdef IPC_TOOLKIT_WITH_CORRECT_CCD
 #include <tight_inclusion/ccd.hpp>
+#include <tight_inclusion/interval_root_finder.hpp>
 #else
+#include <ipc/ccd/inexact_point_edge.hpp>
 #include <CTCD.h>
 #endif
 
 #include <algorithm> // std::min/max
 #include <array>
 
 namespace ipc {
 
-#ifdef IPC_TOOLKIT_WITH_CORRECT_CCD
+/// @brief Scale the distance tolerance to be at most this fraction of the initial distance.
 static constexpr double INITIAL_DISTANCE_TOLERANCE_SCALE = 0.5;
+
+/// @brief Special value for max_iterations to run tight inclusion without a maximum number of iterations.
 static constexpr long TIGHT_INCLUSION_UNLIMITED_ITERATIONS = -1;
-#endif
 
 /// @brief Tolerance for small time of impact which triggers rerunning CCD without a minimum separation.
 static constexpr double SMALL_TOI = 1e-6;
 
 bool ccd_strategy(
     const std::function<bool(
         long /*max_iterations*/,
         double /*min_distance*/,
         bool /*no_zero_toi*/,
         double& /*toi*/)>& ccd,
-    const double max_iterations,
+    const long max_iterations,
     const double min_distance,
     const double initial_distance,
     const double conservative_rescaling,
     double& toi)
 {
-
-    if (initial_distance == 0) {
-        logger().warn("Initial distance is 0, returning toi=0!");
+    if (initial_distance <= min_distance) {
+        logger().warn(
+            "Initial distance {} ≤ d_min={}, returning toi=0!",
+            initial_distance, min_distance);
         toi = 0;
         return true;
     }
 
-    const double min_effective_distance =
-        min_distance + (1.0 - conservative_rescaling) * initial_distance;
-    // #ifdef IPC_TOOLKIT_WITH_CORRECT_CCD
+    double min_effective_distance =
+        (1.0 - conservative_rescaling) * initial_distance;
+#ifdef IPC_TOOLKIT_WITH_CORRECT_CCD
     // Tight Inclusion performs better when the minimum separation is small
-    // min_distance = std::min(min_distance, 1e-4);
-    // #endif
+    min_effective_distance = std::min(min_effective_distance, 1e-4);
+#endif
+    min_effective_distance += min_distance;
 
     assert(min_effective_distance < initial_distance);
 
     // Do not use no_zero_toi because the minimum distance is arbitrary and can
     // be removed if the query is challenging (i.e., produces small ToI).
     bool is_impacting =
         ccd(max_iterations, min_effective_distance, /*no_zero_toi=*/false, toi);
@@ -93,14 +99,18 @@
     const double tmax,
     const double tolerance,
     const long max_iterations,
     const double conservative_rescaling)
 {
     assert(tmax >= 0 && tmax <= 1.0);
 
+    if (p0_t0 == p0_t1 && p1_t0 == p1_t1) {
+        return false; // No motion
+    }
+
     const double initial_distance = sqrt(point_point_distance(p0_t0, p1_t0));
 
     const double adjusted_tolerance = std::min(
         INITIAL_DISTANCE_TOLERANCE_SCALE * initial_distance, tolerance);
 
     const auto ccd = [&](long max_iterations, double min_distance,
                          bool no_zero_toi, double& toi) -> bool {
@@ -144,19 +154,23 @@
     const double min_distance,
     const double tmax,
     const double tolerance,
     const long max_iterations,
     const double conservative_rescaling)
 {
 #ifndef IPC_TOOLKIT_WITH_CORRECT_CCD
-    inexact_point_edge_ccd_2D(
+    return inexact_point_edge_ccd_2D(
         p_t0, e0_t0, e1_t0, p_t1, e0_t1, e1_t1, toi, conservative_rescaling);
 #else
     assert(0 <= tmax && tmax <= 1.0);
 
+    if (p_t0 == p_t1 && e0_t0 == e0_t1 && e1_t0 == e1_t1) {
+        return false; // No motion
+    }
+
     const Eigen::Vector3d p_t0_3D = to_3D(p_t0);
     const Eigen::Vector3d e0_t0_3D = to_3D(e0_t0);
     const Eigen::Vector3d e1_t0_3D = to_3D(e1_t0);
     const Eigen::Vector3d p_t1_3D = to_3D(p_t1);
     const Eigen::Vector3d e0_t1_3D = to_3D(e0_t1);
     const Eigen::Vector3d e1_t1_3D = to_3D(e1_t1);
 
@@ -209,14 +223,18 @@
     const double tmax,
     const double tolerance,
     const long max_iterations,
     const double conservative_rescaling)
 {
     assert(tmax >= 0 && tmax <= 1.0);
 
+    if (p_t0 == p_t1 && e0_t0 == e0_t1 && e1_t0 == e1_t1) {
+        return false; // No motion
+    }
+
     const double initial_distance =
         sqrt(point_edge_distance(p_t0, e0_t0, e1_t0));
 
     const double adjusted_tolerance = std::min(
         INITIAL_DISTANCE_TOLERANCE_SCALE * initial_distance, tolerance);
 
     const auto ccd = [&](long max_iterations, double min_distance,
@@ -300,14 +318,19 @@
     const double tmax,
     const double tolerance,
     const long max_iterations,
     const double conservative_rescaling)
 {
     assert(tmax >= 0 && tmax <= 1.0);
 
+    if (ea0_t0 == ea0_t1 && ea1_t0 == ea1_t1 && eb0_t0 == eb0_t1
+        && eb1_t0 == eb1_t1) {
+        return false; // No motion
+    }
+
     const double initial_distance =
         sqrt(edge_edge_distance(ea0_t0, ea1_t0, eb0_t0, eb1_t0));
 
     const double adjusted_tolerance = std::min(
         INITIAL_DISTANCE_TOLERANCE_SCALE * initial_distance, tolerance);
 
     const auto ccd = [&](long max_iterations, double min_distance,
@@ -358,14 +381,18 @@
     const double tmax,
     const double tolerance,
     const long max_iterations,
     const double conservative_rescaling)
 {
     assert(tmax >= 0 && tmax <= 1.0);
 
+    if (p_t0 == p_t1 && t0_t0 == t0_t1 && t1_t0 == t1_t1 && t2_t0 == t2_t1) {
+        return false; // No motion
+    }
+
     const double initial_distance =
         sqrt(point_triangle_distance(p_t0, t0_t0, t1_t0, t2_t0));
 
     const double adjusted_tolerance = std::min(
         INITIAL_DISTANCE_TOLERANCE_SCALE * initial_distance, tolerance);
 
     const auto ccd = [&](long max_iterations, double min_distance,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipctk-1.0.0/src/ipc/ccd/ccd.hpp` & `ipctk-1.1.0/src/ipc/ccd/ccd.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #include <ipc/utils/eigen_ext.hpp>
 
 namespace ipc {
 
 /// The default tolerance used with Tight-Inclusion CCD.
 static constexpr double DEFAULT_CCD_TOLERANCE = 1e-6;
 /// The default maximum number of iterations used with Tight-Inclusion CCD.
-static constexpr long DEFAULT_CCD_MAX_ITERATIONS = 1e7;
+static constexpr long DEFAULT_CCD_MAX_ITERATIONS = 10'000'000l;
 /// The default conservative rescaling value used to avoid taking steps exactly
 /// to impact.
 static constexpr double DEFAULT_CCD_CONSERVATIVE_RESCALING = 0.8;
 
 // 2D
 
 bool point_edge_ccd_2D(
```

### Comparing `ipctk-1.0.0/src/ipc/ccd/inexact_point_edge.cpp` & `ipctk-1.1.0/src/ipc/ccd/inexact_point_edge.cpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/ccd/point_static_plane.cpp` & `ipctk-1.1.0/src/ipc/ccd/point_static_plane.cpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/collision_mesh.cpp` & `ipctk-1.1.0/src/ipc/collision_mesh.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -5,63 +5,63 @@
 #include <ipc/utils/eigen_ext.hpp>
 #include <ipc/utils/local_to_global.hpp>
 #include <ipc/utils/area_gradient.hpp>
 
 namespace ipc {
 
 CollisionMesh::CollisionMesh(
-    const Eigen::MatrixXd& vertices_at_rest,
+    const Eigen::MatrixXd& rest_positions,
     const Eigen::MatrixXi& edges,
     const Eigen::MatrixXi& faces,
     const Eigen::SparseMatrix<double>& displacement_map)
     : CollisionMesh(
-        std::vector<bool>(vertices_at_rest.rows(), true),
-        vertices_at_rest,
+        std::vector<bool>(rest_positions.rows(), true),
+        rest_positions,
         edges,
         faces)
 {
 }
 
 CollisionMesh::CollisionMesh(
     const std::vector<bool>& include_vertex,
-    const Eigen::MatrixXd& full_vertices_at_rest,
+    const Eigen::MatrixXd& full_rest_positions,
     const Eigen::MatrixXi& edges,
     const Eigen::MatrixXi& faces,
     const Eigen::SparseMatrix<double>& displacement_map)
-    : m_full_vertices_at_rest(full_vertices_at_rest)
+    : m_full_rest_positions(full_rest_positions)
     , m_edges(edges)
     , m_faces(faces)
 {
-    assert(include_vertex.size() == full_vertices_at_rest.rows());
+    assert(include_vertex.size() == full_rest_positions.rows());
     const bool include_all_vertices = std::all_of(
         include_vertex.begin(), include_vertex.end(), [](bool b) { return b; });
 
     if (include_all_vertices) {
         // set full ↔ reduced ≡ identity
         m_full_vertex_to_vertex.setLinSpaced(
-            full_vertices_at_rest.rows(), 0, full_vertices_at_rest.rows() - 1);
+            full_rest_positions.rows(), 0, full_rest_positions.rows() - 1);
         m_vertex_to_full_vertex = m_full_vertex_to_vertex;
     } else {
-        m_full_vertex_to_vertex.setConstant(full_vertices_at_rest.rows(), -1);
+        m_full_vertex_to_vertex.setConstant(full_rest_positions.rows(), -1);
         std::vector<int> dynamic_vertex_to_full_vertex;
-        for (size_t i = 0; i < full_vertices_at_rest.rows(); i++) {
+        for (size_t i = 0; i < full_rest_positions.rows(); i++) {
             if (include_vertex[i]) {
                 m_full_vertex_to_vertex[i] =
                     dynamic_vertex_to_full_vertex.size();
                 dynamic_vertex_to_full_vertex.push_back(i);
             }
         }
         m_vertex_to_full_vertex = Eigen::Map<Eigen::VectorXi>(
             dynamic_vertex_to_full_vertex.data(),
             dynamic_vertex_to_full_vertex.size());
     }
 
     ///////////////////////////////////////////////////////////////////////////
 
-    const int dim = full_vertices_at_rest.cols();
+    const int dim = full_rest_positions.cols();
 
     // Selection matrix S ∈ ℝ^{collision×full}
     init_selection_matrices(dim);
 
     if (displacement_map.size() == 0) {
         m_displacement_map = m_select_vertices;
         m_displacement_dof_map = m_select_dof;
@@ -76,16 +76,16 @@
             m_select_dof * vertex_matrix_to_dof_matrix(displacement_map, dim);
         m_displacement_dof_map.makeCompressed();
     }
 
     ///////////////////////////////////////////////////////////////////////////
 
     // Set vertices at rest using full → reduced map
-    m_vertices_at_rest = m_select_vertices * full_vertices_at_rest;
-    // m_vertices_at_rest = vertices(full_vertices_at_rest);
+    m_rest_positions = m_select_vertices * full_rest_positions;
+    // m_rest_positions = vertices(full_rest_positions);
 
     // Map faces and edges to only included vertices
     if (!include_all_vertices) {
         for (int i = 0; i < m_edges.rows(); i++) {
             for (int j = 0; j < m_edges.cols(); j++) {
                 long new_id = m_full_vertex_to_vertex[m_edges(i, j)];
                 assert(new_id >= 0 && new_id < num_vertices());
@@ -202,16 +202,16 @@
     //     }
     // }
 
     // Compute vertex areas as the sum of ½ the length of connected edges
     Eigen::VectorXd vertex_edge_areas =
         Eigen::VectorXd::Constant(num_vertices(), -1);
     for (int i = 0; i < m_edges.rows(); i++) {
-        const auto& e0 = m_vertices_at_rest.row(m_edges(i, 0));
-        const auto& e1 = m_vertices_at_rest.row(m_edges(i, 1));
+        const VectorMax3d e0 = m_rest_positions.row(m_edges(i, 0));
+        const VectorMax3d e1 = m_rest_positions.row(m_edges(i, 1));
         double edge_len = (e1 - e0).norm();
 
         for (int j = 0; j < m_edges.cols(); j++) {
             if (vertex_edge_areas[m_edges(i, j)] < 0) {
                 vertex_edge_areas[m_edges(i, j)] = 0;
             }
             vertex_edge_areas[m_edges(i, j)] += edge_len / 2;
@@ -220,18 +220,18 @@
 
     // Compute vertex/edge areas as the sum of ⅓ the area of connected face
     Eigen::VectorXd vertex_face_areas =
         Eigen::VectorXd::Constant(num_vertices(), -1);
     m_edge_areas.setConstant(m_edges.rows(), -1);
     if (dim() == 3) {
         for (int i = 0; i < m_faces.rows(); i++) {
-            const auto& f0 = m_vertices_at_rest.row(m_faces(i, 0));
-            const auto& f1 = m_vertices_at_rest.row(m_faces(i, 1));
-            const auto& f2 = m_vertices_at_rest.row(m_faces(i, 2));
-            double face_area = cross(f1 - f0, f2 - f0).norm() / 2;
+            const Eigen::Vector3d f0 = m_rest_positions.row(m_faces(i, 0));
+            const Eigen::Vector3d f1 = m_rest_positions.row(m_faces(i, 1));
+            const Eigen::Vector3d f2 = m_rest_positions.row(m_faces(i, 2));
+            double face_area = (f1 - f0).cross(f2 - f0).norm() / 2;
 
             for (int j = 0; j < m_faces.cols(); ++j) {
                 if (vertex_face_areas[m_faces(i, j)] < 0) {
                     vertex_face_areas[m_faces(i, j)] = 0;
                 }
                 vertex_face_areas[m_faces(i, j)] += face_area / 3;
 
@@ -256,77 +256,76 @@
 
 void CollisionMesh::init_area_jacobians()
 {
     // Compute vertex areas as the sum of ½ the length of connected edges
     m_vertex_area_jacobian.resize(
         num_vertices(), Eigen::SparseVector<double>(ndof()));
     for (int i = 0; i < m_edges.rows(); i++) {
-        const auto& e0 = m_vertices_at_rest.row(m_edges(i, 0));
-        const auto& e1 = m_vertices_at_rest.row(m_edges(i, 1));
+        const VectorMax3d e0 = m_rest_positions.row(m_edges(i, 0));
+        const VectorMax3d e1 = m_rest_positions.row(m_edges(i, 1));
 
-        VectorMax6d edge_len_gradient;
-        edge_length_gradient(e0, e1, edge_len_gradient);
+        const VectorMax6d edge_len_gradient = edge_length_gradient(e0, e1) / 2;
 
         for (int j = 0; j < m_edges.cols(); j++) {
             local_gradient_to_global_gradient(
-                edge_len_gradient / 2, m_edges.row(i), dim(),
+                edge_len_gradient, m_edges.row(i), dim(),
                 m_vertex_area_jacobian[m_edges(i, j)]);
         }
     }
 
     // Compute vertex/edge areas as the sum of ⅓ the area of connected face
     m_edge_area_jacobian.resize(
         m_edges.rows(), Eigen::SparseVector<double>(ndof()));
     if (dim() == 3) {
         std::vector<bool> visited_vertex_before(num_vertices(), false);
         for (int i = 0; i < m_faces.rows(); i++) {
-            const auto& f0 = m_vertices_at_rest.row(m_faces(i, 0));
-            const auto& f1 = m_vertices_at_rest.row(m_faces(i, 1));
-            const auto& f2 = m_vertices_at_rest.row(m_faces(i, 2));
+            const Eigen::Vector3d f0 = m_rest_positions.row(m_faces(i, 0));
+            const Eigen::Vector3d f1 = m_rest_positions.row(m_faces(i, 1));
+            const Eigen::Vector3d f2 = m_rest_positions.row(m_faces(i, 2));
 
-            VectorMax9d face_area_gradient;
-            triangle_area_gradient(f0, f1, f2, face_area_gradient);
+            const Vector9d face_area_gradient =
+                triangle_area_gradient(f0, f1, f2) / 3.0;
 
             for (int j = 0; j < m_faces.cols(); ++j) {
                 if (!visited_vertex_before[m_faces(i, j)]) {
                     // remove the computed value from vertex_edge_areas
                     m_vertex_area_jacobian[m_faces(i, j)].setZero();
                     visited_vertex_before[m_faces(i, j)] = true;
                 }
 
                 // compute gradient of area
 
                 local_gradient_to_global_gradient(
-                    face_area_gradient / 3, m_faces.row(i), dim(),
+                    face_area_gradient, m_faces.row(i), dim(),
                     m_vertex_area_jacobian[m_faces(i, j)]);
 
                 local_gradient_to_global_gradient(
-                    face_area_gradient / 3, m_faces.row(i), dim(),
+                    face_area_gradient, m_faces.row(i), dim(),
                     m_edge_area_jacobian[m_faces_to_edges(i, j)]);
             }
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 
 Eigen::MatrixXd
-CollisionMesh::vertices(const Eigen::MatrixXd& full_vertices) const
+CollisionMesh::vertices(const Eigen::MatrixXd& full_positions) const
 {
     // full_U = full_V - full_V_rest
-    assert(full_vertices.rows() == full_num_vertices());
-    assert(full_vertices.cols() == dim());
-    return displace_vertices(full_vertices - m_full_vertices_at_rest);
+    assert(full_positions.rows() == full_num_vertices());
+    assert(full_positions.cols() == dim());
+    return displace_vertices(full_positions - m_full_rest_positions);
 }
 
 Eigen::MatrixXd CollisionMesh::displace_vertices(
     const Eigen::MatrixXd& full_displacements) const
 {
     // V_rest + S * T * full_U; m_displacement_map = S * T
-    return m_vertices_at_rest + map_displacements(full_displacements);
+    return m_rest_positions + map_displacements(full_displacements);
 }
 
 Eigen::MatrixXd CollisionMesh::map_displacements(
     const Eigen::MatrixXd& full_displacements) const
 {
     assert(m_displacement_map.cols() == full_displacements.rows());
     assert(full_displacements.cols() == dim());
```

### Comparing `ipctk-1.0.0/src/ipc/collision_mesh.hpp` & `ipctk-1.1.0/src/ipc/collision_mesh.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -11,52 +11,52 @@
 class CollisionMesh {
 public:
     /// @brief Construct a new Collision Mesh object.
     /// Collision Mesh objects are immutable, so use the other constructors.
     CollisionMesh() { }
 
     /// @brief Construct a new Collision Mesh object directly from the collision mesh vertices.
-    /// @param vertices_at_rest The vertices of the collision mesh at rest.
-    /// @param edges The edges of the collision mesh.
-    /// @param faces The faces of the collision mesh.
+    /// @param rest_positions The vertices of the collision mesh at rest (#V × dim).
+    /// @param edges The edges of the collision mesh (#E × 2).
+    /// @param faces The faces of the collision mesh (#F × 3).
     /// @param displacement_map The displacement mapping from displacements on the full mesh to the collision mesh.
     CollisionMesh(
-        const Eigen::MatrixXd& vertices_at_rest,
+        const Eigen::MatrixXd& rest_positions,
         const Eigen::MatrixXi& edges,
         const Eigen::MatrixXi& faces,
         const Eigen::SparseMatrix<double>& displacement_map =
             Eigen::SparseMatrix<double>());
 
     /// @brief Construct a new Collision Mesh object from a full mesh vertices.
     /// @param include_vertex Vector of bools indicating whether each vertex should be included in the collision mesh.
-    /// @param full_vertices_at_rest The vertices of the full mesh at rest.
-    /// @param edges The edges of the collision mesh indexed into the full mesh vertices.
-    /// @param faces The faces of the collision mesh indexed into the full mesh vertices.
+    /// @param full_rest_positions The vertices of the full mesh at rest (#V × dim).
+    /// @param edges The edges of the collision mesh indexed into the full mesh vertices (#E × 2).
+    /// @param faces The faces of the collision mesh indexed into the full mesh vertices (#F × 3).
     /// @param displacement_map The displacement mapping from displacements on the full mesh to the collision mesh.
     CollisionMesh(
         const std::vector<bool>& include_vertex,
-        const Eigen::MatrixXd& full_vertices_at_rest,
+        const Eigen::MatrixXd& full_rest_positions,
         const Eigen::MatrixXi& edges,
         const Eigen::MatrixXi& faces,
         const Eigen::SparseMatrix<double>& displacement_map =
             Eigen::SparseMatrix<double>());
 
     /// @brief Helper function that automatically builds include_vertex using construct_is_on_surface.
-    /// @param full_vertices_at_rest The full vertices at rest.
-    /// @param edges The edge matrix of mesh.
-    /// @param faces The face matrix of mesh.
+    /// @param full_rest_positions The full vertices at rest (#FV × dim).
+    /// @param edges The edge matrix of mesh (#E × 2).
+    /// @param faces The face matrix of mesh (#F × 3).
     /// @return Constructed CollisionMesh.
     static CollisionMesh build_from_full_mesh(
-        const Eigen::MatrixXd& full_vertices_at_rest,
+        const Eigen::MatrixXd& full_rest_positions,
         const Eigen::MatrixXi& edges,
         const Eigen::MatrixXi& faces)
     {
         return CollisionMesh(
-            construct_is_on_surface(full_vertices_at_rest.rows(), edges),
-            full_vertices_at_rest, edges, faces);
+            construct_is_on_surface(full_rest_positions.rows(), edges),
+            full_rest_positions, edges, faces);
     }
 
     // The following functions are used to initialize optional data structures.
 
     /// @brief Initialize vertex-vertex and edge-vertex adjacencies.
     void init_adjacencies();
 
@@ -72,38 +72,35 @@
     /// @brief Get the number of edges in the collision mesh.
     size_t num_edges() const { return edges().rows(); }
 
     /// @brief Get the number of faces in the collision mesh.
     size_t num_faces() const { return faces().rows(); }
 
     /// @brief Get the dimension of the mesh.
-    size_t dim() const { return m_vertices_at_rest.cols(); }
+    size_t dim() const { return m_rest_positions.cols(); }
 
     /// @brief Get the number of degrees of freedom in the collision mesh.
     size_t ndof() const { return num_vertices() * dim(); }
 
     /// @brief Get the number of vertices in the full mesh.
     size_t full_num_vertices() const { return m_full_vertex_to_vertex.size(); }
 
     /// @brief Get the number of degrees of freedom in the full mesh.
     size_t full_ndof() const { return full_num_vertices() * dim(); }
 
-    /// @brief Get the vertices of the collision mesh at rest.
-    const Eigen::MatrixXd& vertices_at_rest() const
-    {
-        return m_vertices_at_rest;
-    }
+    /// @brief Get the vertices of the collision mesh at rest (#V × dim).
+    const Eigen::MatrixXd& rest_positions() const { return m_rest_positions; }
 
-    /// @brief Get the edges of the collision mesh.
+    /// @brief Get the edges of the collision mesh (#E × 2).
     const Eigen::MatrixXi& edges() const { return m_edges; }
 
-    /// @brief Get the faces of the collision mesh.
+    /// @brief Get the faces of the collision mesh (#F × 3).
     const Eigen::MatrixXi& faces() const { return m_faces; }
 
-    /// @brief Get the mapping from faces to edges of the collision mesh.
+    /// @brief Get the mapping from faces to edges of the collision mesh (#F × 3).
     const Eigen::MatrixXi& faces_to_edges() const { return m_faces_to_edges; }
 
     // const std::vector<std::vector<int>>& vertices_to_edges() const
     // {
     //     return m_vertices_to_edges;
     // }
 
@@ -111,27 +108,27 @@
     // {
     //     return m_vertices_to_faces;
     // }
 
     // -----------------------------------------------------------------------
 
     /// @brief Compute the vertex positions from the positions of the full mesh.
-    /// @param full_vertices The vertex positions of the full mesh.
-    /// @return The vertex positions of the collision mesh.
-    Eigen::MatrixXd vertices(const Eigen::MatrixXd& full_vertices) const;
+    /// @param full_positions The vertex positions of the full mesh (#FV × dim).
+    /// @return The vertex positions of the collision mesh (#V × dim).
+    Eigen::MatrixXd vertices(const Eigen::MatrixXd& full_positions) const;
 
     /// @brief Compute the vertex positions from vertex displacements on the full mesh.
-    /// @param full_displacements The vertex displacements on the full mesh.
-    /// @return The vertex positions of the collision mesh.
+    /// @param full_displacements The vertex displacements on the full mesh (#FV × dim).
+    /// @return The vertex positions of the collision mesh (#V × dim).
     Eigen::MatrixXd
     displace_vertices(const Eigen::MatrixXd& full_displacements) const;
 
     /// @brief Map vertex displacements on the full mesh to vertex displacements on the collision mesh.
-    /// @param full_displacements The vertex displacements on the full mesh.
-    /// @return The vertex displacements on the collision mesh.
+    /// @param full_displacements The vertex displacements on the full mesh (#FV × dim).
+    /// @return The vertex displacements on the collision mesh (#V × dim).
     Eigen::MatrixXd
     map_displacements(const Eigen::MatrixXd& full_displacements) const;
 
     /// @brief Map a vertex ID to the corresponding vertex ID in the full mesh.
     /// @param id Vertex ID in the collision mesh.
     /// @return Vertex ID in the full mesh.
     size_t to_full_vertex_id(const size_t id) const
@@ -240,57 +237,56 @@
             && m_edge_area_jacobian.size() == num_edges();
     }
 
     // -----------------------------------------------------------------------
 
     /// @brief Construct a vector of bools indicating whether each vertex is on the surface.
     /// @param num_vertices The number of vertices in the mesh.
-    /// @param edges The surface edges of the mesh.
+    /// @param edges The surface edges of the mesh (#E × 2).
     /// @return A vector of bools indicating whether each vertex is on the surface.
     static std::vector<bool> construct_is_on_surface(
         const int num_vertices, const Eigen::MatrixXi& edges);
 
     /// @brief Construct a matrix that maps from the faces' edges to rows in the edges matrix.
-    /// @param faces The face matrix of mesh.
-    /// @param edges The edge matrix of mesh.
+    /// @param faces The face matrix of mesh (#F × 3).
+    /// @param edges The edge matrix of mesh (#E × 2).
     /// @return Matrix that maps from the faces' edges to rows in the edges matrix.
     static Eigen::MatrixXi construct_faces_to_edges(
         const Eigen::MatrixXi& faces, const Eigen::MatrixXi& edges);
 
-    /// A function that takes two vertex IDs (row numbers in V) and returns true
-    /// if the vertices (and faces or edges containing the vertices) can
-    /// collide. By default all primitives can collide with all other
-    /// primitives.
+    /// A function that takes two vertex IDs and returns true if the vertices
+    /// (and faces or edges containing the vertices) can collide. By default all
+    /// primitives can collide with all other primitives.
     std::function<bool(size_t, size_t)> can_collide = default_can_collide;
 
 protected:
     // -----------------------------------------------------------------------
     // Helper initialization functions
 
     /// @brief Initialize the selection matrix from full vertices/DOF to collision vertices/DOF.
     void init_selection_matrices(const int dim);
 
     /// @brief Initialize vertex and edge areas.
     void init_areas();
 
-    /// @brief Convert a matrix meant for M_V * V to M_dof * x by duplicating the entries dim times.
+    /// @brief Convert a matrix meant for M_V * vertices to M_dof * x by duplicating the entries dim times.
     static Eigen::SparseMatrix<double> vertex_matrix_to_dof_matrix(
         const Eigen::SparseMatrix<double>& M_V, int dim);
 
     // -----------------------------------------------------------------------
 
-    /// @brief The full vertex positions at rest.
-    Eigen::MatrixXd m_full_vertices_at_rest;
-    /// @brief The vertex positions at rest.
-    Eigen::MatrixXd m_vertices_at_rest;
-    /// @brief Edges as rows of indicies into V.
+    /// @brief The full vertex positions at rest (#FV × dim).
+    Eigen::MatrixXd m_full_rest_positions;
+    /// @brief The vertex positions at rest (#V × dim).
+    Eigen::MatrixXd m_rest_positions;
+    /// @brief Edges as rows of indicies into vertices (#E × 2).
     Eigen::MatrixXi m_edges;
-    /// @brief Triangular faces as rows of indicies into V.
+    /// @brief Triangular faces as rows of indicies into vertices (#F × 3).
     Eigen::MatrixXi m_faces;
-    /// @brief Map from F edges to rows of E.
+    /// @brief Map from faces edges to rows of edges (#F × 3).
     Eigen::MatrixXi m_faces_to_edges;
 
     /// @brief Map from full vertices to collision vertices.
     /// @note Negative values indicate full vertex is dropped.
     Eigen::VectorXi m_full_vertex_to_vertex;
     /// @brief Map from collision vertices to full vertices.
     Eigen::VectorXi m_vertex_to_full_vertex;
```

### Comparing `ipctk-1.0.0/src/ipc/collisions/collision_constraint.cpp` & `ipctk-1.1.0/src/ipc/collisions/collision_constraint.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 #include "collision_constraint.hpp"
 
 #include <ipc/barrier/barrier.hpp>
 
 namespace ipc {
 
 double CollisionConstraint::compute_potential(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     const double dhat) const
 {
-    const double distance = compute_distance(V, E, F); // Squared distance
+    // Squared distance
+    const double distance = compute_distance(vertices, edges, faces);
     return weight
         * barrier(
                distance - minimum_distance * minimum_distance,
                2 * minimum_distance * dhat + dhat * dhat);
 }
 
 VectorMax12d CollisionConstraint::compute_potential_gradient(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     const double dhat) const
 {
     // ∇b(d(x)) = b'(d(x)) * ∇d(x)
-    const double distance = compute_distance(V, E, F);
-    const VectorMax12d distance_grad = compute_distance_gradient(V, E, F);
+    const VectorMax12d positions = dof(vertices, edges, faces);
+    const double distance = compute_distance(positions);
+    const VectorMax12d distance_grad = compute_distance_gradient(positions);
 
     const double grad_b = barrier_gradient(
         distance - minimum_distance * minimum_distance,
         2 * minimum_distance * dhat + dhat * dhat);
     return weight * grad_b * distance_grad;
 }
 
 MatrixMax12d CollisionConstraint::compute_potential_hessian(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     const double dhat,
     const bool project_hessian_to_psd) const
 {
-    const double dhat_squared = dhat * dhat;
-    const double min_dist_squrared = minimum_distance * minimum_distance;
+    const double adjusted_dhat = 2 * minimum_distance * dhat + dhat * dhat;
+    const double min_dist_squared = minimum_distance * minimum_distance;
 
     // ∇²[b(d(x))] = ∇(b'(d(x)) * ∇d(x))
     //             = b"(d(x)) * ∇d(x) * ∇d(x)ᵀ + b'(d(x)) * ∇²d(x)
 
-    const double distance = compute_distance(V, E, F);
-    const VectorMax12d distance_grad = compute_distance_gradient(V, E, F);
-    const MatrixMax12d distance_hess = compute_distance_hessian(V, E, F);
-
-    const double grad_b = barrier_gradient(
-        distance - min_dist_squrared,
-        2 * minimum_distance * dhat + dhat_squared);
-    const double hess_b = barrier_hessian(
-        distance - min_dist_squrared,
-        2 * minimum_distance * dhat + dhat_squared);
+    const VectorMax12d positions = dof(vertices, edges, faces);
+    const double distance = compute_distance(positions);
+    const VectorMax12d distance_grad = compute_distance_gradient(positions);
+    const MatrixMax12d distance_hess = compute_distance_hessian(positions);
+
+    const double grad_b =
+        barrier_gradient(distance - min_dist_squared, adjusted_dhat);
+    const double hess_b =
+        barrier_hessian(distance - min_dist_squared, adjusted_dhat);
 
     // b"(x) ≥ 0 ⟹ b"(x) * ∇d(x) * ∇d(x)ᵀ is PSD
     assert(hess_b >= 0);
     MatrixMax12d term1 = hess_b * distance_grad * distance_grad.transpose();
     MatrixMax12d term2 = grad_b * distance_hess;
     if (project_hessian_to_psd) {
         term2 = project_to_psd(term2);
```

### Comparing `ipctk-1.0.0/src/ipc/collisions/edge_edge.cpp` & `ipctk-1.1.0/src/ipc/collisions/edge_edge.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -3,127 +3,117 @@
 #include <ipc/barrier/barrier.hpp>
 #include <ipc/distance/edge_edge.hpp>
 #include <ipc/distance/edge_edge_mollifier.hpp>
 
 namespace ipc {
 
 EdgeEdgeConstraint::EdgeEdgeConstraint(
-    long edge0_index, long edge1_index, double eps_x)
-    : EdgeEdgeCandidate(edge0_index, edge1_index)
+    long edge0_id, long edge1_id, double eps_x)
+    : EdgeEdgeCandidate(edge0_id, edge1_id)
     , eps_x(eps_x)
 {
 }
 
 EdgeEdgeConstraint::EdgeEdgeConstraint(
     const EdgeEdgeCandidate& candidate, double eps_x)
     : EdgeEdgeCandidate(candidate)
     , eps_x(eps_x)
 {
 }
 
 double EdgeEdgeConstraint::compute_potential(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     const double dhat) const
 {
     return edge_edge_mollifier(
-               V.row(E(edge0_index, 0)), V.row(E(edge0_index, 1)),
-               V.row(E(edge1_index, 0)), V.row(E(edge1_index, 1)), eps_x)
-        * CollisionConstraint::compute_potential(V, E, F, dhat);
+               vertices.row(edges(edge0_id, 0)),
+               vertices.row(edges(edge0_id, 1)),
+               vertices.row(edges(edge1_id, 0)),
+               vertices.row(edges(edge1_id, 1)), eps_x)
+        * CollisionConstraint::compute_potential(vertices, edges, faces, dhat);
 }
 
 VectorMax12d EdgeEdgeConstraint::compute_potential_gradient(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     const double dhat) const
 {
-    const double dhat_squared = dhat * dhat;
+    const double adjusted_dhat = 2 * minimum_distance * dhat + dhat * dhat;
+    const double min_dist_squared = minimum_distance * minimum_distance;
 
     // ∇[m(x) * b(d(x))] = (∇m(x)) * b(d(x)) + m(x) * b'(d(x)) * ∇d(x)
-    const auto& ea0 = V.row(E(edge0_index, 0));
-    const auto& ea1 = V.row(E(edge0_index, 1));
-    const auto& eb0 = V.row(E(edge1_index, 0));
-    const auto& eb1 = V.row(E(edge1_index, 1));
+    const auto& [ea0, ea1, eb0, eb1] = this->vertices(vertices, edges, faces);
 
     // The distance type is unknown because of mollified PP and PE
     // constraints where also added as EE constraints.
     const EdgeEdgeDistanceType dtype =
         edge_edge_distance_type(ea0, ea1, eb0, eb1);
     const double distance = edge_edge_distance(ea0, ea1, eb0, eb1, dtype);
-    VectorMax12d distance_grad;
-    edge_edge_distance_gradient(ea0, ea1, eb0, eb1, distance_grad, dtype);
+    const Vector12d distance_grad =
+        edge_edge_distance_gradient(ea0, ea1, eb0, eb1, dtype);
 
     // m(x)
     const double mollifier = edge_edge_mollifier(ea0, ea1, eb0, eb1, eps_x);
     // ∇m(x)
-    VectorMax12d mollifier_grad;
-    edge_edge_mollifier_gradient(ea0, ea1, eb0, eb1, eps_x, mollifier_grad);
+    const Vector12d mollifier_grad =
+        edge_edge_mollifier_gradient(ea0, ea1, eb0, eb1, eps_x);
 
     // b(d(x))
-    const double b = barrier(
-        distance - minimum_distance * minimum_distance,
-        2 * minimum_distance * dhat + dhat_squared);
+    const double b = barrier(distance - min_dist_squared, adjusted_dhat);
     // b'(d(x))
-    const double grad_b = barrier_gradient(
-        distance - minimum_distance * minimum_distance,
-        2 * minimum_distance * dhat + dhat_squared);
+    const double grad_b =
+        barrier_gradient(distance - min_dist_squared, adjusted_dhat);
 
     return weight * (mollifier_grad * b + mollifier * grad_b * distance_grad);
 }
 
 MatrixMax12d EdgeEdgeConstraint::compute_potential_hessian(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F,
+    const Eigen::MatrixXd& vertices,
+    const Eigen::MatrixXi& edges,
+    const Eigen::MatrixXi& faces,
     const double dhat,
     const bool project_hessian_to_psd) const
 {
-    const double dhat_squared = dhat * dhat;
-    const double min_dist_squrared = minimum_distance * minimum_distance;
+    const double adjusted_dhat = 2 * minimum_distance * dhat + dhat * dhat;
+    const double min_dist_squared = minimum_distance * minimum_distance;
 
     // ∇²[m(x) * b(d(x))] = ∇[∇m(x) * b(d(x)) + m(x) * b'(d(x)) * ∇d(x)]
     //                    = ∇²m(x) * b(d(x)) + b'(d(x)) * ∇d(x) * ∇m(x)ᵀ
     //                      + ∇m(x) * b'(d(x)) * ∇d(x))ᵀ
     //                      + m(x) * b"(d(x)) * ∇d(x) * ∇d(x)ᵀ
     //                      + m(x) * b'(d(x)) * ∇²d(x)
-    const auto& ea0 = V.row(E(edge0_index, 0));
-    const auto& ea1 = V.row(E(edge0_index, 1));
-    const auto& eb0 = V.row(E(edge1_index, 0));
-    const auto& eb1 = V.row(E(edge1_index, 1));
+    const auto& [ea0, ea1, eb0, eb1] = this->vertices(vertices, edges, faces);
 
     // Compute distance derivatives
     // The distance type is unknown because of mollified PP and PE
     // constraints where also added as EE constraints.
     const EdgeEdgeDistanceType dtype =
         edge_edge_distance_type(ea0, ea1, eb0, eb1);
     const double distance = edge_edge_distance(ea0, ea1, eb0, eb1, dtype);
-    VectorMax12d distance_grad;
-    edge_edge_distance_gradient(ea0, ea1, eb0, eb1, distance_grad, dtype);
-    MatrixMax12d distance_hess;
-    edge_edge_distance_hessian(ea0, ea1, eb0, eb1, distance_hess, dtype);
+    const Vector12d distance_grad =
+        edge_edge_distance_gradient(ea0, ea1, eb0, eb1, dtype);
+    const Matrix12d distance_hess =
+        edge_edge_distance_hessian(ea0, ea1, eb0, eb1, dtype);
 
     // Compute mollifier derivatives
     const double mollifier = edge_edge_mollifier(ea0, ea1, eb0, eb1, eps_x);
-    VectorMax12d mollifier_grad;
-    edge_edge_mollifier_gradient(ea0, ea1, eb0, eb1, eps_x, mollifier_grad);
-    MatrixMax12d mollifier_hess;
-    edge_edge_mollifier_hessian(ea0, ea1, eb0, eb1, eps_x, mollifier_hess);
+    const VectorMax12d mollifier_grad =
+        edge_edge_mollifier_gradient(ea0, ea1, eb0, eb1, eps_x);
+    const MatrixMax12d mollifier_hess =
+        edge_edge_mollifier_hessian(ea0, ea1, eb0, eb1, eps_x);
 
     // Compute barrier derivatives
-    const double b = barrier(
-        distance - min_dist_squrared,
-        2 * minimum_distance * dhat + dhat_squared);
-    const double grad_b = barrier_gradient(
-        distance - min_dist_squrared,
-        2 * minimum_distance * dhat + dhat_squared);
-    const double hess_b = barrier_hessian(
-        distance - min_dist_squrared,
-        2 * minimum_distance * dhat + dhat_squared);
+    const double b = barrier(distance - min_dist_squared, adjusted_dhat);
+    const double grad_b =
+        barrier_gradient(distance - min_dist_squared, adjusted_dhat);
+    const double hess_b =
+        barrier_hessian(distance - min_dist_squared, adjusted_dhat);
 
     MatrixMax12d hess = mollifier_hess * b
         + grad_b
             * (distance_grad * mollifier_grad.transpose()
                + mollifier_grad * distance_grad.transpose())
         + mollifier
             * (hess_b * distance_grad * distance_grad.transpose()
```

### Comparing `ipctk-1.0.0/src/ipc/collisions/edge_edge.hpp` & `ipctk-1.1.0/src/ipc/collisions/edge_edge.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -2,69 +2,36 @@
 
 #include <ipc/candidates/edge_edge.hpp>
 #include <ipc/collisions/collision_constraint.hpp>
 #include <ipc/utils/eigen_ext.hpp>
 
 namespace ipc {
 
-struct EdgeEdgeConstraint : EdgeEdgeCandidate, CollisionConstraint {
-    EdgeEdgeConstraint(long edge0_index, long edge1_index, double eps_x);
+class EdgeEdgeConstraint : public EdgeEdgeCandidate,
+                           public CollisionConstraint {
+public:
+    EdgeEdgeConstraint(long edge0_id, long edge1_id, double eps_x);
     EdgeEdgeConstraint(const EdgeEdgeCandidate& candidate, double eps_x);
 
-    int num_vertices() const override
-    {
-        return EdgeEdgeCandidate::num_vertices();
-    }
-
-    std::array<long, 4> vertex_indices(
-        const Eigen::MatrixXi& E, const Eigen::MatrixXi& F) const override
-    {
-        return EdgeEdgeCandidate::vertex_indices(E, F);
-    }
-
-    double compute_distance(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override
-    {
-        return EdgeEdgeCandidate::compute_distance(V, E, F);
-    }
-
-    VectorMax12d compute_distance_gradient(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override
-    {
-        return EdgeEdgeCandidate::compute_distance_gradient(V, E, F);
-    }
-
-    MatrixMax12d compute_distance_hessian(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override
-    {
-        return EdgeEdgeCandidate::compute_distance_hessian(V, E, F);
-    }
-
     double compute_potential(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         const double dhat) const override;
 
     VectorMax12d compute_potential_gradient(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         const double dhat) const override;
 
     MatrixMax12d compute_potential_hessian(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
         const double dhat,
         const bool project_hessian_to_psd) const override;
 
     template <typename H>
     friend H AbslHashValue(H h, const EdgeEdgeConstraint& ee)
     {
         return AbslHashValue(
```

### Comparing `ipctk-1.0.0/src/ipc/collisions/edge_vertex.hpp` & `ipctk-1.1.0/src/ipc/friction/constraints/edge_vertex.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,49 @@
 #pragma once
 
+#include <ipc/friction/constraints/friction_constraint.hpp>
 #include <ipc/candidates/edge_vertex.hpp>
-#include <ipc/collisions/collision_constraint.hpp>
 #include <ipc/utils/eigen_ext.hpp>
 
 namespace ipc {
 
-struct EdgeVertexConstraint : EdgeVertexCandidate, CollisionConstraint {
+class EdgeVertexFrictionConstraint : public EdgeVertexCandidate,
+                                     public FrictionConstraint {
+public:
     using EdgeVertexCandidate::EdgeVertexCandidate;
 
-    EdgeVertexConstraint(const EdgeVertexCandidate& candidate)
-        : EdgeVertexCandidate(candidate)
-    {
-    }
-
-    int num_vertices() const override { return 3; };
-    std::array<long, 4> vertex_indices(
-        const Eigen::MatrixXi& E, const Eigen::MatrixXi& F) const override
-    {
-        return { { vertex_index, E(edge_index, 0), E(edge_index, 1), -1 } };
-    }
-
-    double compute_distance(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override
-    {
-        // The distance type is known because of Constraints::build()
-        return EdgeVertexCandidate::compute_distance(
-            V, E, F, PointEdgeDistanceType::P_E);
-    }
-
-    VectorMax12d compute_distance_gradient(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override
-    {
-        // The distance type is known because of Constraints::build()
-        return EdgeVertexCandidate::compute_distance_gradient(
-            V, E, F, PointEdgeDistanceType::P_E);
-    }
-
-    MatrixMax12d compute_distance_hessian(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override
-    {
-        // The distance type is known because of Constraints::build()
-        return EdgeVertexCandidate::compute_distance_hessian(
-            V, E, F, PointEdgeDistanceType::P_E);
-    }
-
-    template <typename H>
-    friend H AbslHashValue(H h, const EdgeVertexConstraint& ev)
-    {
-        return AbslHashValue(
-            std::move(h), static_cast<const EdgeVertexCandidate&>(ev));
-    }
+    EdgeVertexFrictionConstraint(const EdgeVertexConstraint& constraint);
+
+    EdgeVertexFrictionConstraint(
+        const EdgeVertexConstraint& constraint,
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
+        const double dhat,
+        const double barrier_stiffness);
+
+protected:
+    MatrixMax<double, 3, 2>
+    compute_tangent_basis(const VectorMax12d& positions) const override;
+
+    MatrixMax<double, 36, 2> compute_tangent_basis_jacobian(
+        const VectorMax12d& positions) const override;
+
+    VectorMax2d
+    compute_closest_point(const VectorMax12d& positions) const override;
+
+    MatrixMax<double, 2, 12> compute_closest_point_jacobian(
+        const VectorMax12d& positions) const override;
+
+    VectorMax3d
+    relative_velocity(const VectorMax12d& velocities) const override;
+
+    using FrictionConstraint::relative_velocity_matrix;
+
+    MatrixMax<double, 3, 12>
+    relative_velocity_matrix(const VectorMax2d& closest_point) const override;
+
+    MatrixMax<double, 6, 12> relative_velocity_matrix_jacobian(
+        const VectorMax2d& closest_point) const override;
 };
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/collisions/plane_vertex.cpp` & `ipctk-1.1.0/src/ipc/collisions/plane_vertex.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,38 @@
-#include "plane_vertex.hpp"
+#pragma once
 
-#include <ipc/distance/point_plane.hpp>
+#include <ipc/collisions/collision_constraint.hpp>
+#include <ipc/utils/eigen_ext.hpp>
 
 namespace ipc {
 
-PlaneVertexConstraint::PlaneVertexConstraint(
-    const VectorMax3d& plane_origin,
-    const VectorMax3d& plane_normal,
-    const long vertex_index)
-    : plane_origin(plane_origin)
-    , plane_normal(plane_normal)
-    , vertex_index(vertex_index)
-{
-}
-
-double PlaneVertexConstraint::compute_distance(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F) const
-{
-    return point_plane_distance(
-        V.row(vertex_index).transpose(), plane_origin, plane_normal);
-}
-
-VectorMax12d PlaneVertexConstraint::compute_distance_gradient(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F) const
-{
-    VectorMax3d distance_grad;
-    point_plane_distance_gradient(
-        V.row(vertex_index).transpose(), plane_origin, plane_normal,
-        distance_grad);
-    return distance_grad;
-}
-
-MatrixMax12d PlaneVertexConstraint::compute_distance_hessian(
-    const Eigen::MatrixXd& V,
-    const Eigen::MatrixXi& E,
-    const Eigen::MatrixXi& F) const
-{
-    MatrixMax3d distance_hess;
-    point_plane_distance_hessian(
-        V.row(vertex_index).transpose(), plane_origin, plane_normal,
-        distance_hess);
-    return distance_hess;
-}
+class PlaneVertexConstraint : public CollisionConstraint {
+public:
+    PlaneVertexConstraint(
+        const VectorMax3d& plane_origin,
+        const VectorMax3d& plane_normal,
+        const long vertex_id);
+
+    int num_vertices() const override { return 1; };
+
+    std::array<long, 4> vertex_ids(
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces) const override
+    {
+        return { { vertex_id, -1, -1, -1 } };
+    }
+
+    VectorMax3d plane_origin;
+    VectorMax3d plane_normal;
+    long vertex_id;
+
+protected:
+    double compute_distance(const VectorMax12d& point) const override;
+
+    VectorMax12d
+    compute_distance_gradient(const VectorMax12d& point) const override;
+
+    MatrixMax12d
+    compute_distance_hessian(const VectorMax12d& point) const override;
+};
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/collisions/plane_vertex.hpp` & `ipctk-1.1.0/src/ipc/collisions/collision_constraint.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 #pragma once
 
-#include <ipc/collisions/collision_constraint.hpp>
+#include <ipc/candidates/collision_stencil.hpp>
 #include <ipc/utils/eigen_ext.hpp>
 
+#include <Eigen/Core>
+
+#include <array>
+
 namespace ipc {
 
-struct PlaneVertexConstraint : CollisionConstraint {
-    PlaneVertexConstraint(
-        const VectorMax3d& plane_origin,
-        const VectorMax3d& plane_normal,
-        const long vertex_index);
-
-    int num_vertices() const override { return 1; };
-    std::array<long, 4> vertex_indices(
-        const Eigen::MatrixXi& E, const Eigen::MatrixXi& F) const override
-    {
-        return { { vertex_index, -1, -1, -1 } };
-    }
-
-    double compute_distance(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override;
-
-    VectorMax12d compute_distance_gradient(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override;
-
-    MatrixMax12d compute_distance_hessian(
-        const Eigen::MatrixXd& V,
-        const Eigen::MatrixXi& E,
-        const Eigen::MatrixXi& F) const override;
-
-    VectorMax3d plane_origin;
-    VectorMax3d plane_normal;
-    long vertex_index;
+class CollisionConstraint : virtual public CollisionStencil {
+public:
+    virtual ~CollisionConstraint() { }
+
+    virtual double compute_potential(
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
+        const double dhat) const;
+
+    virtual VectorMax12d compute_potential_gradient(
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
+        const double dhat) const;
+
+    virtual MatrixMax12d compute_potential_hessian(
+        const Eigen::MatrixXd& vertices,
+        const Eigen::MatrixXi& edges,
+        const Eigen::MatrixXi& faces,
+        const double dhat,
+        const bool project_hessian_to_psd) const;
+
+    double minimum_distance = 0;
+    double weight = 1;
+    Eigen::SparseVector<double> weight_gradient;
 };
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/distance/distance_type.hpp` & `ipctk-1.1.0/src/ipc/distance/distance_type.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #pragma once
 
-#include <Eigen/Core>
+#include <ipc/utils/eigen_ext.hpp>
 
 namespace ipc {
 
 /// @brief Closest pair between a point and edge.
 enum class PointEdgeDistanceType {
     P_E0, ///< The point is closest to edge vertex zero.
     P_E1, ///< The point is closest to edge vertex one.
@@ -43,50 +43,49 @@
 };
 
 /// @brief Determine the closest pair between a point and edge.
 /// @param p The point.
 /// @param e0 The first vertex of the edge.
 /// @param e1 The second vertex of the edge.
 /// @return The distance type of the point-edge pair.
-template <typename DerivedP, typename DerivedE0, typename DerivedE1>
 PointEdgeDistanceType point_edge_distance_type(
-    const Eigen::MatrixBase<DerivedP>& p,
-    const Eigen::MatrixBase<DerivedE0>& e0,
-    const Eigen::MatrixBase<DerivedE1>& e1);
+    const Eigen::Ref<const VectorMax3d>& p,
+    const Eigen::Ref<const VectorMax3d>& e0,
+    const Eigen::Ref<const VectorMax3d>& e1);
 
 /// @brief Determine the closest pair between a point and triangle.
 /// @param p The point.
 /// @param t0 The first vertex of the triangle.
 /// @param t1 The second vertex of the triangle.
 /// @param t2 The third vertex of the triangle.
 /// @return The distance type of the point-triangle pair.
-template <
-    typename DerivedP,
-    typename DerivedT0,
-    typename DerivedT1,
-    typename DerivedT2>
 PointTriangleDistanceType point_triangle_distance_type(
-    const Eigen::MatrixBase<DerivedP>& p,
-    const Eigen::MatrixBase<DerivedT0>& t0,
-    const Eigen::MatrixBase<DerivedT1>& t1,
-    const Eigen::MatrixBase<DerivedT2>& t2);
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& t0,
+    const Eigen::Ref<const Eigen::Vector3d>& t1,
+    const Eigen::Ref<const Eigen::Vector3d>& t2);
 
 /// @brief Determine the closest pair between two edges.
 /// @param ea0 The first vertex of the first edge.
 /// @param ea1 The second vertex of the first edge.
 /// @param eb0 The first vertex of the second edge.
 /// @param eb1 The second vertex of the second edge.
 /// @return The distance type of the edge-edge pair.
-template <
-    typename DerivedEA0,
-    typename DerivedEA1,
-    typename DerivedEB0,
-    typename DerivedEB1>
 EdgeEdgeDistanceType edge_edge_distance_type(
-    const Eigen::MatrixBase<DerivedEA0>& ea0,
-    const Eigen::MatrixBase<DerivedEA1>& ea1,
-    const Eigen::MatrixBase<DerivedEB0>& eb0,
-    const Eigen::MatrixBase<DerivedEB1>& eb1);
+    const Eigen::Ref<const Eigen::Vector3d>& ea0,
+    const Eigen::Ref<const Eigen::Vector3d>& ea1,
+    const Eigen::Ref<const Eigen::Vector3d>& eb0,
+    const Eigen::Ref<const Eigen::Vector3d>& eb1);
 
-} // namespace ipc
+/// @brief Determine the closest pair between two parallel edges.
+/// @param ea0 The first vertex of the first edge.
+/// @param ea1 The second vertex of the first edge.
+/// @param eb0 The first vertex of the second edge.
+/// @param eb1 The second vertex of the second edge.
+/// @return The distance type of the edge-edge pair.
+EdgeEdgeDistanceType edge_edge_parallel_distance_type(
+    const Eigen::Ref<const Eigen::Vector3d>& ea0,
+    const Eigen::Ref<const Eigen::Vector3d>& ea1,
+    const Eigen::Ref<const Eigen::Vector3d>& eb0,
+    const Eigen::Ref<const Eigen::Vector3d>& eb1);
 
-#include <ipc/distance/distance_type.tpp>
+} // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/distance/line_line.cpp` & `ipctk-1.1.0/src/ipc/distance/line_line.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,50 @@
 #include "line_line.hpp"
 
+#include <Eigen/Geometry>
+
 namespace ipc {
+
+double line_line_distance(
+    const Eigen::Ref<const Eigen::Vector3d>& ea0,
+    const Eigen::Ref<const Eigen::Vector3d>& ea1,
+    const Eigen::Ref<const Eigen::Vector3d>& eb0,
+    const Eigen::Ref<const Eigen::Vector3d>& eb1)
+{
+    const Eigen::Vector3d normal = (ea1 - ea0).cross(eb1 - eb0);
+    const double line_to_line = (eb0 - ea0).dot(normal);
+    return line_to_line * line_to_line / normal.squaredNorm();
+}
+
+Vector12d line_line_distance_gradient(
+    const Eigen::Ref<const Eigen::Vector3d>& ea0,
+    const Eigen::Ref<const Eigen::Vector3d>& ea1,
+    const Eigen::Ref<const Eigen::Vector3d>& eb0,
+    const Eigen::Ref<const Eigen::Vector3d>& eb1)
+{
+    Vector12d grad;
+    autogen::line_line_distance_gradient(
+        ea0[0], ea0[1], ea0[2], ea1[0], ea1[1], ea1[2], eb0[0], eb0[1], eb0[2],
+        eb1[0], eb1[1], eb1[2], grad.data());
+    return grad;
+}
+
+Matrix12d line_line_distance_hessian(
+    const Eigen::Ref<const Eigen::Vector3d>& ea0,
+    const Eigen::Ref<const Eigen::Vector3d>& ea1,
+    const Eigen::Ref<const Eigen::Vector3d>& eb0,
+    const Eigen::Ref<const Eigen::Vector3d>& eb1)
+{
+    Matrix12d hess;
+    autogen::line_line_distance_hessian(
+        ea0[0], ea0[1], ea0[2], ea1[0], ea1[1], ea1[2], eb0[0], eb0[1], eb0[2],
+        eb1[0], eb1[1], eb1[2], hess.data());
+    return hess;
+}
+
 namespace autogen {
 
     // This function was generated by the Symbolic Math Toolbox version 8.3.
     // 14-Jun-2019 13:58:25
     void line_line_distance_gradient(
         double v01,
         double v02,
```

### Comparing `ipctk-1.0.0/src/ipc/distance/point_line.cpp` & `ipctk-1.1.0/src/ipc/distance/point_line.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,73 @@
 #include "point_line.hpp"
 
 namespace ipc {
+
+double point_line_distance(
+    const Eigen::Ref<const VectorMax3d>& p,
+    const Eigen::Ref<const VectorMax3d>& e0,
+    const Eigen::Ref<const VectorMax3d>& e1)
+{
+    assert(p.size() == 2 || p.size() == 3);
+    assert(e0.size() == 2 || e0.size() == 3);
+    assert(e1.size() == 2 || e1.size() == 3);
+
+    if (p.size() == 2) {
+        const Eigen::Vector2d e = e1 - e0;
+        const double numerator =
+            (e[1] * p[0] - e[0] * p[1] + e1[0] * e0[1] - e1[1] * e0[0]);
+        return numerator * numerator / e.squaredNorm();
+    } else {
+        return (e0 - p).head<3>().cross((e1 - p).head<3>()).squaredNorm()
+            / (e1 - e0).squaredNorm();
+    }
+}
+
+VectorMax9d point_line_distance_gradient(
+    const Eigen::Ref<const VectorMax3d>& p,
+    const Eigen::Ref<const VectorMax3d>& e0,
+    const Eigen::Ref<const VectorMax3d>& e1)
+{
+    const int dim = p.size();
+    assert(e0.size() == dim);
+    assert(e1.size() == dim);
+
+    VectorMax9d grad(3 * dim);
+    if (dim == 2) {
+        autogen::point_line_distance_gradient_2D(
+            p[0], p[1], e0[0], e0[1], e1[0], e1[1], grad.data());
+    } else {
+        autogen::point_line_distance_gradient_3D(
+            p[0], p[1], p[2], e0[0], e0[1], e0[2], e1[0], e1[1], e1[2],
+            grad.data());
+    }
+    return grad;
+}
+
+MatrixMax9d point_line_distance_hessian(
+    const Eigen::Ref<const VectorMax3d>& p,
+    const Eigen::Ref<const VectorMax3d>& e0,
+    const Eigen::Ref<const VectorMax3d>& e1)
+{
+    const int dim = p.size();
+    assert(e0.size() == dim);
+    assert(e1.size() == dim);
+
+    MatrixMax9d hess(3 * dim, 3 * dim);
+    if (dim == 2) {
+        autogen::point_line_distance_hessian_2D(
+            p[0], p[1], e0[0], e0[1], e1[0], e1[1], hess.data());
+    } else {
+        autogen::point_line_distance_hessian_3D(
+            p[0], p[1], p[2], e0[0], e0[1], e0[2], e1[0], e1[1], e1[2],
+            hess.data());
+    }
+    return hess;
+}
+
 namespace autogen {
 
     // This function was generated by the Symbolic Math Toolbox version 8.3.
     // 16-Mar-2020 15:56:29
     void point_line_distance_gradient_2D(
         double v01,
         double v02,
```

### Comparing `ipctk-1.0.0/src/ipc/distance/point_plane.cpp` & `ipctk-1.1.0/src/ipc/distance/point_plane.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,74 @@
 #include "point_plane.hpp"
 
+#include <ipc/utils/eigen_ext.hpp>
+#include <Eigen/Geometry>
+
 namespace ipc {
+
+double point_plane_distance(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& origin,
+    const Eigen::Ref<const Eigen::Vector3d>& normal)
+{
+    const double point_to_plane = (p - origin).dot(normal);
+    return point_to_plane * point_to_plane / normal.squaredNorm();
+}
+
+double point_plane_distance(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& t0,
+    const Eigen::Ref<const Eigen::Vector3d>& t1,
+    const Eigen::Ref<const Eigen::Vector3d>& t2)
+{
+    return point_plane_distance(p, t0, (t1 - t0).cross(t2 - t0));
+}
+
+Eigen::Vector3d point_plane_distance_gradient(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& origin,
+    const Eigen::Ref<const Eigen::Vector3d>& normal)
+{
+    return (2 / normal.squaredNorm()) * (p - origin).dot(normal) * normal;
+}
+
+Vector12d point_plane_distance_gradient(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& t0,
+    const Eigen::Ref<const Eigen::Vector3d>& t1,
+    const Eigen::Ref<const Eigen::Vector3d>& t2)
+{
+    Vector12d grad;
+    autogen::point_plane_distance_gradient(
+        p[0], p[1], p[2], t0[0], t0[1], t0[2], t1[0], t1[1], t1[2], t2[0],
+        t2[1], t2[2], grad.data());
+    return grad;
+}
+
+Eigen::Matrix3d point_plane_distance_hessian(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& origin,
+    const Eigen::Ref<const Eigen::Vector3d>& normal)
+{
+    return 2 / normal.squaredNorm() * normal * normal.transpose();
+}
+
+Matrix12d point_plane_distance_hessian(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& t0,
+    const Eigen::Ref<const Eigen::Vector3d>& t1,
+    const Eigen::Ref<const Eigen::Vector3d>& t2)
+{
+    Matrix12d hess;
+    autogen::point_plane_distance_hessian(
+        p[0], p[1], p[2], t0[0], t0[1], t0[2], t1[0], t1[1], t1[2], t2[0],
+        t2[1], t2[2], hess.data());
+    return hess;
+}
+
 namespace autogen {
 
     // This function was generated by the Symbolic Math Toolbox version 8.3.
     // 10-Jun-2019 17:42:16
     void point_plane_distance_gradient(
         double v01,
         double v02,
```

### Comparing `ipctk-1.0.0/src/ipc/friction/closest_point.cpp` & `ipctk-1.1.0/src/ipc/friction/closest_point.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,123 @@
 #include "closest_point.hpp"
 
+#include <Eigen/Core>
+#include <Eigen/Cholesky>
+
 namespace ipc {
+
+// ============================================================================
+// Point - Edge
+
+double point_edge_closest_point(
+    const Eigen::Ref<const VectorMax3d>& p,
+    const Eigen::Ref<const VectorMax3d>& e0,
+    const Eigen::Ref<const VectorMax3d>& e1)
+{
+    const VectorMax3d e = e1 - e0;
+    return (p - e0).dot(e) / e.squaredNorm();
+}
+
+VectorMax9d point_edge_closest_point_jacobian(
+    const Eigen::Ref<const VectorMax3d>& p,
+    const Eigen::Ref<const VectorMax3d>& e0,
+    const Eigen::Ref<const VectorMax3d>& e1)
+{
+    const int dim = p.size();
+    assert(dim == 2 || dim == 3);
+    assert(e0.size() == dim && e1.size() == dim);
+
+    const VectorMax3d e = e1 - e0;
+    const VectorMax3d e2p = p - e0;
+    const double e_sqnorm = e.squaredNorm();
+
+    VectorMax9d J(3 * dim);
+    J.head(dim) = e / e_sqnorm;
+    J.segment(dim, dim) = (2 / e_sqnorm * e.dot(e2p) * e - e - e2p) / e_sqnorm;
+    J.tail(dim) = (e2p - 2 / e_sqnorm * e.dot(e2p) * e) / e_sqnorm;
+    return J;
+}
+
+// ============================================================================
+// Edge - Edge
+
+Vector2<double> edge_edge_closest_point(
+    const Eigen::Ref<const Eigen::Vector3d>& ea0,
+    const Eigen::Ref<const Eigen::Vector3d>& ea1,
+    const Eigen::Ref<const Eigen::Vector3d>& eb0,
+    const Eigen::Ref<const Eigen::Vector3d>& eb1)
+{
+    const Eigen::Vector3d eb_to_ea = ea0 - eb0;
+    const Eigen::Vector3d ea = ea1 - ea0;
+    const Eigen::Vector3d eb = eb1 - eb0;
+
+    Eigen::Matrix<double, 2, 2> coefMtr;
+    coefMtr(0, 0) = ea.squaredNorm();
+    coefMtr(0, 1) = coefMtr(1, 0) = -eb.dot(ea);
+    coefMtr(1, 1) = eb.squaredNorm();
+
+    Vector2<double> rhs;
+    rhs[0] = -eb_to_ea.dot(ea);
+    rhs[1] = eb_to_ea.dot(eb);
+
+    const Eigen::Vector2d x = coefMtr.ldlt().solve(rhs);
+    assert((coefMtr * x - rhs).norm() < 1e-10);
+    return x;
+}
+
+Eigen::Matrix<double, 2, 12> edge_edge_closest_point_jacobian(
+    const Eigen::Ref<const Eigen::Vector3d>& ea0,
+    const Eigen::Ref<const Eigen::Vector3d>& ea1,
+    const Eigen::Ref<const Eigen::Vector3d>& eb0,
+    const Eigen::Ref<const Eigen::Vector3d>& eb1)
+{
+    Eigen::Matrix<double, 2, 12> J;
+
+    autogen::edge_edge_closest_point_jacobian(
+        ea0[0], ea0[1], ea0[2], ea1[0], ea1[1], ea1[2], eb0[0], eb0[1], eb0[2],
+        eb1[0], eb1[1], eb1[2], J.data());
+
+    return J;
+}
+
+// ============================================================================
+// Point - Triangle
+
+Vector2<double> point_triangle_closest_point(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& t0,
+    const Eigen::Ref<const Eigen::Vector3d>& t1,
+    const Eigen::Ref<const Eigen::Vector3d>& t2)
+{
+    Eigen::Matrix<double, 2, 3> basis;
+    basis.row(0) = RowVector3<double>(t1 - t0); // edge 0
+    basis.row(1) = RowVector3<double>(t2 - t0); // edge 1
+    const Eigen::Matrix2d A = basis * basis.transpose();
+    const Eigen::Vector2d b = basis * (p - t0);
+    const Eigen::Vector2d x = A.ldlt().solve(b);
+    assert((A * x - b).norm() < 1e-10);
+    return x;
+}
+
+Eigen::Matrix<double, 2, 12> point_triangle_closest_point_jacobian(
+    const Eigen::Ref<const Eigen::Vector3d>& p,
+    const Eigen::Ref<const Eigen::Vector3d>& t0,
+    const Eigen::Ref<const Eigen::Vector3d>& t1,
+    const Eigen::Ref<const Eigen::Vector3d>& t2)
+{
+    Eigen::Matrix<double, 2, 12> J;
+    autogen::point_triangle_closest_point_jacobian(
+        p[0], p[1], p[2], t0[0], t0[1], t0[2], t1[0], t1[1], t1[2], t2[0],
+        t2[1], t2[2], J.data());
+
+    return J;
+}
+
+// ============================================================================
+
 namespace autogen {
     // J is (6×1) flattened in column-major order
     void point_edge_closest_point_2D_jacobian(
         double p_x,
         double p_y,
         double e0_x,
         double e0_y,
```

### Comparing `ipctk-1.0.0/src/ipc/friction/friction.cpp` & `ipctk-1.1.0/src/ipc/friction/friction_constraints.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,342 +1,402 @@
-#include "friction.hpp"
+#include "friction_constraints.hpp"
 
-#include <ipc/barrier/barrier.hpp>
-#include <ipc/distance/edge_edge.hpp>
 #include <ipc/distance/edge_edge_mollifier.hpp>
-#include <ipc/distance/point_edge.hpp>
-#include <ipc/distance/point_triangle.hpp>
-#include <ipc/friction/closest_point.hpp>
-#include <ipc/friction/normal_force_magnitude.hpp>
-#include <ipc/friction/relative_displacement.hpp>
-#include <ipc/friction/tangent_basis.hpp>
-#include <ipc/utils/eigen_ext.hpp>
 #include <ipc/utils/local_to_global.hpp>
 
-#include <ipc/config.hpp>
-
 #include <tbb/parallel_for.h>
 #include <tbb/blocked_range.h>
 #include <tbb/enumerable_thread_specific.h>
 
-namespace ipc {
-
-void construct_friction_constraint_set(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& contact_constraint_set,
-    double dhat,
-    double barrier_stiffness,
-    double mu,
-    FrictionConstraints& friction_constraint_set)
-{
-    return construct_friction_constraint_set(
-        mesh, V, contact_constraint_set, dhat, barrier_stiffness,
-        Eigen::VectorXd::Constant(V.rows(), mu), friction_constraint_set);
-}
+#include <stdexcept> // std::out_of_range
 
-void construct_friction_constraint_set(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& contact_constraint_set,
-    double dhat,
-    double barrier_stiffness,
-    const Eigen::VectorXd& mus,
-    FrictionConstraints& friction_constraint_set)
-{
-    return construct_friction_constraint_set(
-        mesh, V, contact_constraint_set, dhat, barrier_stiffness, mus,
-        [](double mu0, double mu1) { return (mu0 + mu1) / 2; },
-        // [](double mu0, double mu1) { return mu0 * mu1; },
-        // [](double mu0, double mu1) { return std::min(mu0, mu1); },
-        // [](double mu0, double mu1) { return std::max(mu0, mu1); },
-        friction_constraint_set);
-}
+namespace ipc {
 
-void construct_friction_constraint_set(
+void FrictionConstraints::build(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& contact_constraint_set,
-    double dhat,
-    double barrier_stiffness,
+    const Eigen::MatrixXd& vertices,
+    const CollisionConstraints& contact_constraint_set,
+    const double dhat,
+    const double barrier_stiffness,
     const Eigen::VectorXd& mus,
-    const std::function<double(double, double)>& blend_mu,
-    FrictionConstraints& friction_constraint_set)
+    const std::function<double(double, double)>& blend_mu)
 {
-    assert(mus.size() == V.rows());
+    assert(mus.size() == vertices.rows());
 
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    const Eigen::MatrixXi& edges = mesh.edges();
+    const Eigen::MatrixXi& faces = mesh.faces();
 
-    friction_constraint_set.clear();
+    clear();
 
-    const auto& [C_vv, C_ev, C_ee, C_fv, _, __, ___] = contact_constraint_set;
-    auto& [FC_vv, FC_ev, FC_ee, FC_fv] = friction_constraint_set;
+    const auto& C_vv = contact_constraint_set.vv_constraints;
+    const auto& C_ev = contact_constraint_set.ev_constraints;
+    const auto& C_ee = contact_constraint_set.ee_constraints;
+    const auto& C_fv = contact_constraint_set.fv_constraints;
+    auto& [FC_vv, FC_ev, FC_ee, FC_fv] = *this;
 
     FC_vv.reserve(C_vv.size());
     for (const auto& c_vv : C_vv) {
-        FC_vv.emplace_back(c_vv, V, E, F, dhat, barrier_stiffness);
-        const auto& [v0i, v1i, _, __] = FC_vv.back().vertex_indices(E, F);
+        FC_vv.emplace_back(
+            c_vv, vertices, edges, faces, dhat, barrier_stiffness);
+        const auto& [v0i, v1i, _, __] = FC_vv.back().vertex_ids(edges, faces);
 
         FC_vv.back().mu = blend_mu(mus(v0i), mus(v1i));
     }
 
     FC_ev.reserve(C_ev.size());
     for (const auto& c_ev : C_ev) {
-        FC_ev.emplace_back(c_ev, V, E, F, dhat, barrier_stiffness);
-        const auto& [vi, e0i, e1i, _] = FC_ev.back().vertex_indices(E, F);
+        FC_ev.emplace_back(
+            c_ev, vertices, edges, faces, dhat, barrier_stiffness);
+        const auto& [vi, e0i, e1i, _] = FC_ev.back().vertex_ids(edges, faces);
 
         const double edge_mu =
             (mus(e1i) - mus(e0i)) * FC_ev.back().closest_point[0] + mus(e0i);
         FC_ev.back().mu = blend_mu(edge_mu, mus(vi));
     }
 
     FC_ee.reserve(C_ee.size());
     for (const auto& c_ee : C_ee) {
-        const auto& [ea0i, ea1i, eb0i, eb1i] = c_ee.vertex_indices(E, F);
-        const Eigen::Vector3d ea0 = V.row(ea0i), ea1 = V.row(ea1i),
-                              eb0 = V.row(eb0i), eb1 = V.row(eb1i);
+        const auto& [ea0i, ea1i, eb0i, eb1i] = c_ee.vertex_ids(edges, faces);
+        const Eigen::Vector3d ea0 = vertices.row(ea0i);
+        const Eigen::Vector3d ea1 = vertices.row(ea1i);
+        const Eigen::Vector3d eb0 = vertices.row(eb0i);
+        const Eigen::Vector3d eb1 = vertices.row(eb1i);
 
         // Skip EE constraints that are close to parallel
         if (edge_edge_cross_squarednorm(ea0, ea1, eb0, eb1) < c_ee.eps_x) {
             continue;
         }
 
-        FC_ee.emplace_back(c_ee, V, E, F, dhat, barrier_stiffness);
+        FC_ee.emplace_back(
+            c_ee, vertices, edges, faces, dhat, barrier_stiffness);
 
         double ea_mu =
             (mus(ea1i) - mus(ea0i)) * FC_ee.back().closest_point[0] + mus(ea0i);
         double eb_mu =
             (mus(eb1i) - mus(eb0i)) * FC_ee.back().closest_point[1] + mus(eb0i);
         FC_ee.back().mu = blend_mu(ea_mu, eb_mu);
     }
 
     FC_fv.reserve(C_fv.size());
     for (const auto& c_fv : C_fv) {
-        FC_fv.emplace_back(c_fv, V, E, F, dhat, barrier_stiffness);
-        const auto& [vi, f0i, f1i, f2i] = FC_fv.back().vertex_indices(E, F);
+        FC_fv.emplace_back(
+            c_fv, vertices, edges, faces, dhat, barrier_stiffness);
+        const auto& [vi, f0i, f1i, f2i] = FC_fv.back().vertex_ids(edges, faces);
 
         double face_mu = mus(f0i)
             + FC_fv.back().closest_point[0] * (mus(f1i) - mus(f0i))
             + FC_fv.back().closest_point[1] * (mus(f2i) - mus(f0i));
         FC_fv.back().mu = blend_mu(face_mu, mus(vi));
     }
 }
 
-///////////////////////////////////////////////////////////////////////////////
-//
-// compute_friction_potential() in friction.tpp
-//
-///////////////////////////////////////////////////////////////////////////////
-
-Eigen::VectorXd compute_friction_potential_gradient(
+double FrictionConstraints::compute_potential(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const FrictionConstraints& friction_constraint_set,
-    double epsv_times_h)
+    const Eigen::MatrixXd& velocity,
+    const double epsv) const
 {
-    if (friction_constraint_set.empty()) {
-        return Eigen::VectorXd::Zero(V0.size());
+    assert(velocity.rows() == mesh.num_vertices());
+    assert(epsv > 0);
+
+    if (empty()) {
+        return 0;
     }
-    assert(epsv_times_h > 0);
 
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    tbb::enumerable_thread_specific<double> storage(0);
+
+    tbb::parallel_for(
+        tbb::blocked_range<size_t>(size_t(0), size()),
+        [&](tbb::blocked_range<size_t> r) {
+            auto& local_potential = storage.local();
+            for (size_t i = r.begin(); i < r.end(); i++) {
+                // Quadrature weight is premultiplied by compute_potential
+                local_potential += (*this)[i].compute_potential(
+                    velocity, mesh.edges(), mesh.faces(), epsv);
+            }
+        });
+
+    return storage.combine([](double a, double b) { return a + b; });
+}
 
-    auto U = V1 - V0; // absolute linear dislacement of each point
-    int dim = U.cols();
+Eigen::VectorXd FrictionConstraints::compute_potential_gradient(
+    const CollisionMesh& mesh,
+    const Eigen::MatrixXd& velocity,
+    const double epsv) const
+{
+    const int dim = velocity.cols();
+    const int ndof = velocity.size();
+
+    if (empty()) {
+        return Eigen::VectorXd::Zero(ndof);
+    }
+    assert(epsv > 0);
 
     tbb::enumerable_thread_specific<Eigen::VectorXd> storage(
-        Eigen::VectorXd::Zero(U.size()));
+        Eigen::VectorXd::Zero(ndof));
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), friction_constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
-            auto& local_grad = storage.local();
+            auto& global_grad = storage.local();
+
             for (size_t i = r.begin(); i < r.end(); i++) {
+                const auto& constraint = (*this)[i];
+
+                const VectorMax12d local_grad =
+                    constraint.compute_potential_gradient(
+                        velocity, mesh.edges(), mesh.faces(), epsv);
+
+                const std::array<long, 4> vis =
+                    constraint.vertex_ids(mesh.edges(), mesh.faces());
+
                 local_gradient_to_global_gradient(
-                    friction_constraint_set[i].compute_potential_gradient(
-                        U, E, F, epsv_times_h),
-                    friction_constraint_set[i].vertex_indices(E, F), dim,
-                    local_grad);
+                    local_grad, vis, dim, global_grad);
             }
         });
 
-    Eigen::VectorXd grad = Eigen::VectorXd::Zero(U.size());
-    for (const auto& local_grad : storage) {
-        grad += local_grad;
-    }
-    return grad;
+    return storage.combine([](const Eigen::VectorXd& a,
+                              const Eigen::VectorXd& b) { return a + b; });
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
-Eigen::SparseMatrix<double> compute_friction_potential_hessian(
+Eigen::SparseMatrix<double> FrictionConstraints::compute_potential_hessian(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const FrictionConstraints& friction_constraint_set,
-    double epsv_times_h,
-    bool project_hessian_to_psd)
-{
-    if (friction_constraint_set.empty()) {
-        return Eigen::SparseMatrix<double>(V0.size(), V0.size());
-    }
-    assert(epsv_times_h > 0);
-
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    const Eigen::MatrixXd& velocity,
+    const double epsv,
+    const bool project_hessian_to_psd) const
+{
+    const int dim = velocity.cols();
+    const int ndof = velocity.size();
 
-    auto U = V1 - V0; // absolute linear dislacement of each point
-    int dim = U.cols();
+    if (empty()) {
+        return Eigen::SparseMatrix<double>(ndof, ndof);
+    }
+    assert(epsv > 0);
 
     tbb::enumerable_thread_specific<std::vector<Eigen::Triplet<double>>>
         storage;
+
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), friction_constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
-            auto& local_hess_triplets = storage.local();
+            auto& hess_triplets = storage.local();
 
             for (size_t i = r.begin(); i < r.end(); i++) {
+                const auto& constraint = (*this)[i];
+
+                const MatrixMax12d local_hess =
+                    constraint.compute_potential_hessian(
+                        velocity, mesh.edges(), mesh.faces(), epsv,
+                        project_hessian_to_psd);
+
+                const std::array<long, 4> vis =
+                    constraint.vertex_ids(mesh.edges(), mesh.faces());
+
                 local_hessian_to_global_triplets(
-                    friction_constraint_set[i].compute_potential_hessian(
-                        U, E, F, epsv_times_h, project_hessian_to_psd),
-                    friction_constraint_set[i].vertex_indices(E, F), dim,
-                    local_hess_triplets);
+                    local_hess, vis, dim, hess_triplets);
             }
         });
 
-    Eigen::SparseMatrix<double> hess(U.size(), U.size());
+    Eigen::SparseMatrix<double> hess(ndof, ndof);
     for (const auto& local_hess_triplets : storage) {
-        Eigen::SparseMatrix<double> local_hess(U.size(), U.size());
+        Eigen::SparseMatrix<double> local_hess(ndof, ndof);
         local_hess.setFromTriplets(
             local_hess_triplets.begin(), local_hess_triplets.end());
         hess += local_hess;
     }
     return hess;
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
-Eigen::VectorXd compute_friction_force(
+Eigen::VectorXd FrictionConstraints::compute_force(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& X,
-    const Eigen::MatrixXd& Ut,
-    const Eigen::MatrixXd& U,
-    const FrictionConstraints& friction_constraint_set,
+    const Eigen::MatrixXd& rest_positions,
+    const Eigen::MatrixXd& lagged_displacements,
+    const Eigen::MatrixXd& velocities,
     const double dhat,
     const double barrier_stiffness,
-    const double epsv_times_h,
+    const double epsv,
     const double dmin,
-    const bool no_mu)
+    const bool no_mu) const
 {
-    if (friction_constraint_set.empty()) {
-        return Eigen::VectorXd::Zero(U.size());
+    if (empty()) {
+        return Eigen::VectorXd::Zero(velocities.size());
     }
-    assert(epsv_times_h > 0);
+    assert(epsv > 0);
 
-    int dim = U.cols();
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    int dim = velocities.cols();
 
     tbb::enumerable_thread_specific<Eigen::VectorXd> storage(
-        Eigen::VectorXd::Zero(U.size()));
+        Eigen::VectorXd::Zero(velocities.size()));
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), friction_constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
-            auto& local_force = storage.local();
+            Eigen::VectorXd& force = storage.local();
             for (size_t i = r.begin(); i < r.end(); i++) {
-                local_gradient_to_global_gradient(
-                    friction_constraint_set[i].compute_force(
-                        X, Ut, U, E, F, dhat, barrier_stiffness, epsv_times_h,
-                        dmin, no_mu),
-                    friction_constraint_set[i].vertex_indices(E, F), dim,
-                    local_force);
+                const auto& constraint = (*this)[i];
+
+                const VectorMax12d local_force = constraint.compute_force(
+                    rest_positions, lagged_displacements, velocities,
+                    mesh.edges(), mesh.faces(), dhat, barrier_stiffness, epsv,
+                    dmin, no_mu);
+
+                const std::array<long, 4> vis =
+                    constraint.vertex_ids(mesh.edges(), mesh.faces());
+
+                local_gradient_to_global_gradient(local_force, vis, dim, force);
             }
         });
 
-    Eigen::VectorXd force = Eigen::VectorXd::Zero(U.size());
-    for (const auto& local_force : storage) {
-        force += local_force;
-    }
-    return force;
+    return storage.combine([](const Eigen::VectorXd& a,
+                              const Eigen::VectorXd& b) { return a + b; });
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
-Eigen::SparseMatrix<double> compute_friction_force_jacobian(
+Eigen::SparseMatrix<double> FrictionConstraints::compute_force_jacobian(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& X,
-    const Eigen::MatrixXd& Ut,
-    const Eigen::MatrixXd& U,
-    const FrictionConstraints& friction_constraint_set,
+    const Eigen::MatrixXd& rest_positions,
+    const Eigen::MatrixXd& lagged_displacements,
+    const Eigen::MatrixXd& velocities,
     const double dhat,
     const double barrier_stiffness,
-    const double epsv_times_h,
+    const double epsv,
     const FrictionConstraint::DiffWRT wrt,
-    const double dmin)
+    const double dmin) const
 {
-    if (friction_constraint_set.empty()) {
-        return Eigen::SparseMatrix<double>(U.size(), U.size());
-    }
-    assert(epsv_times_h > 0);
-
-    int dim = U.cols();
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    if (empty()) {
+        return Eigen::SparseMatrix<double>(
+            velocities.size(), velocities.size());
+    }
+    assert(epsv > 0);
+
+    int dim = velocities.cols();
+    const Eigen::MatrixXi& edges = mesh.edges();
+    const Eigen::MatrixXi& faces = mesh.faces();
 
     tbb::enumerable_thread_specific<std::vector<Eigen::Triplet<double>>>
         storage;
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), friction_constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
-            auto& local_jac_triplets = storage.local();
+            auto& jac_triplets = storage.local();
 
             for (size_t i = r.begin(); i < r.end(); i++) {
+                const FrictionConstraint& constraint = (*this)[i];
+
+                const MatrixMax12d local_force_jacobian =
+                    constraint.compute_force_jacobian(
+                        rest_positions, lagged_displacements, velocities, edges,
+                        faces, dhat, barrier_stiffness, epsv, wrt, dmin);
+
+                const std::array<long, 4> vis =
+                    constraint.vertex_ids(mesh.edges(), mesh.faces());
+
                 local_hessian_to_global_triplets(
-                    friction_constraint_set[i].compute_force_jacobian(
-                        X, Ut, U, E, F, dhat, barrier_stiffness, epsv_times_h,
-                        wrt, dmin),
-                    friction_constraint_set[i].vertex_indices(E, F), dim,
-                    local_jac_triplets);
+                    local_force_jacobian, vis, dim, jac_triplets);
             }
         });
 
-    Eigen::SparseMatrix<double> jacobian(U.size(), U.size());
+    Eigen::SparseMatrix<double> jacobian(velocities.size(), velocities.size());
     for (const auto& local_jac_triplets : storage) {
-        Eigen::SparseMatrix<double> local_jacobian(U.size(), U.size());
+        Eigen::SparseMatrix<double> local_jacobian(
+            velocities.size(), velocities.size());
         local_jacobian.setFromTriplets(
             local_jac_triplets.begin(), local_jac_triplets.end());
         jacobian += local_jacobian;
     }
 
     // if wrt == X then compute ∇ₓ w(x)
-    if (wrt == FrictionConstraint::DiffWRT::X) {
-        for (int i = 0; i < friction_constraint_set.size(); i++) {
-            const FrictionConstraint& constraint = friction_constraint_set[i];
-            assert(constraint.weight_gradient.size() == X.size());
-            if (constraint.weight_gradient.size() != X.size()) {
+    if (wrt == FrictionConstraint::DiffWRT::REST_POSITIONS) {
+        for (int i = 0; i < this->size(); i++) {
+            const FrictionConstraint& constraint = (*this)[i];
+            assert(constraint.weight_gradient.size() == rest_positions.size());
+            if (constraint.weight_gradient.size() != rest_positions.size()) {
                 throw std::runtime_error(
                     "Shape derivative is not computed for friction constraint!");
             }
 
             VectorMax12d local_force = constraint.compute_force(
-                X, Ut, U, E, F, dhat, barrier_stiffness, epsv_times_h, dmin);
+                rest_positions, lagged_displacements, velocities, edges, faces,
+                dhat, barrier_stiffness, epsv, dmin);
             assert(constraint.weight != 0);
-            local_force.array() /= constraint.weight;
+            local_force /= constraint.weight;
 
-            Eigen::SparseVector<double> force(X.size());
+            Eigen::SparseVector<double> force(rest_positions.size());
             force.reserve(local_force.size());
             local_gradient_to_global_gradient(
-                local_force, constraint.vertex_indices(E, F), dim, force);
+                local_force, constraint.vertex_ids(edges, faces), dim, force);
 
             jacobian += force * constraint.weight_gradient.transpose();
         }
     }
 
     return jacobian;
 }
 
+///////////////////////////////////////////////////////////////////////////////
+
+size_t FrictionConstraints::size() const
+{
+    return vv_constraints.size() + ev_constraints.size() + ee_constraints.size()
+        + fv_constraints.size();
+}
+
+bool FrictionConstraints::empty() const
+{
+    return vv_constraints.empty() && ev_constraints.empty()
+        && ee_constraints.empty() && fv_constraints.empty();
+}
+
+void FrictionConstraints::clear()
+{
+    vv_constraints.clear();
+    ev_constraints.clear();
+    ee_constraints.clear();
+    fv_constraints.clear();
+}
+
+FrictionConstraint& FrictionConstraints::operator[](size_t idx)
+{
+    if (idx < vv_constraints.size()) {
+        return vv_constraints[idx];
+    }
+    idx -= vv_constraints.size();
+    if (idx < ev_constraints.size()) {
+        return ev_constraints[idx];
+    }
+    idx -= ev_constraints.size();
+    if (idx < ee_constraints.size()) {
+        return ee_constraints[idx];
+    }
+    idx -= ee_constraints.size();
+    if (idx < fv_constraints.size()) {
+        return fv_constraints[idx];
+    }
+    throw std::out_of_range("Friction constraint index is out of range!");
+}
+
+const FrictionConstraint& FrictionConstraints::operator[](size_t idx) const
+{
+    if (idx < vv_constraints.size()) {
+        return vv_constraints[idx];
+    }
+    idx -= vv_constraints.size();
+    if (idx < ev_constraints.size()) {
+        return ev_constraints[idx];
+    }
+    idx -= ev_constraints.size();
+    if (idx < ee_constraints.size()) {
+        return ee_constraints[idx];
+    }
+    idx -= ee_constraints.size();
+    if (idx < fv_constraints.size()) {
+        return fv_constraints[idx];
+    }
+    throw std::out_of_range("Friction constraint index is out of range!");
+}
+
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/friction/normal_force_magnitude.cpp` & `ipctk-1.1.0/src/ipc/friction/normal_force_magnitude.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 namespace ipc {
 
 double compute_normal_force_magnitude(
     double distance_squared, double dhat, double barrier_stiffness, double dmin)
 {
     double grad_b = barrier_gradient(
         distance_squared - dmin * dmin, 2 * dmin * dhat + dhat * dhat);
-    return -barrier_stiffness * grad_b * 2
-        * sqrt(distance_squared); // / (h * h) eliminated here
+    return -barrier_stiffness * grad_b * 2 * sqrt(distance_squared);
 }
 
 VectorMax12d compute_normal_force_magnitude_gradient(
     double distance_squared,
     const Eigen::VectorXd& distance_squared_gradient,
     double dhat,
     double barrier_stiffness,
```

### Comparing `ipctk-1.0.0/src/ipc/ipc.cpp` & `ipctk-1.1.0/src/ipc/collisions/collision_constraints.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,189 +1,287 @@
-#include "ipc.hpp"
+#include "collision_constraints.hpp"
 
-#include <ipc/ccd/ccd.hpp>
-#include <ipc/broad_phase/hash_grid.hpp>
+#include <ipc/collisions/collision_constraints_builder.hpp>
+// #include <ipc/utils/unordered_map_and_set.hpp>
 #include <ipc/utils/local_to_global.hpp>
-#include <ipc/utils/intersection.hpp>
-#include <ipc/utils/world_bbox_diagonal_length.hpp>
-
-#include <ipc/config.hpp>
-
-#ifdef IPC_TOOLKIT_WITH_CUDA
-#include <ccdgpu/helper.cuh>
-#endif
-
-#include <igl/predicates/segment_segment_intersect.h>
 
 #include <tbb/parallel_for.h>
 #include <tbb/blocked_range.h>
 #include <tbb/enumerable_thread_specific.h>
-#include <shared_mutex>
 
-#include <algorithm> // std::min/max
+#include <stdexcept> // std::out_of_range
 
 namespace ipc {
 
-double compute_barrier_potential(
+void CollisionConstraints::build(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
-    const double dhat)
+    const Eigen::MatrixXd& vertices,
+    const double dhat,
+    const double dmin,
+    const BroadPhaseMethod broad_phase_method)
 {
-    assert(V.rows() == mesh.num_vertices());
+    assert(vertices.rows() == mesh.num_vertices());
 
-    if (constraint_set.empty()) {
-        return 0;
+    double inflation_radius = (dhat + dmin) / 2;
+
+    Candidates candidates;
+    candidates.build(mesh, vertices, inflation_radius, broad_phase_method);
+
+    this->build(candidates, mesh, vertices, dhat, dmin);
+}
+
+void CollisionConstraints::build(
+    const Candidates& candidates,
+    const CollisionMesh& mesh,
+    const Eigen::MatrixXd& vertices,
+    const double dhat,
+    const double dmin)
+{
+    assert(vertices.rows() == mesh.num_vertices());
+
+    clear();
+
+    // Cull the candidates by measuring the distance and dropping those that are
+    // greater than dhat.
+    const double offset_sqr = (dmin + dhat) * (dmin + dhat);
+    auto is_active = [&](double distance_sqr) {
+        return distance_sqr < offset_sqr;
+    };
+
+    tbb::enumerable_thread_specific<CollisionConstraintsBuilder> storage(
+        CollisionConstraintsBuilder(*this));
+
+    tbb::parallel_for(
+        tbb::blocked_range<size_t>(size_t(0), candidates.ev_candidates.size()),
+        [&](const tbb::blocked_range<size_t>& r) {
+            storage.local().add_edge_vertex_constraints(
+                mesh, vertices, candidates.ev_candidates, is_active, r.begin(),
+                r.end());
+        });
+
+    tbb::parallel_for(
+        tbb::blocked_range<size_t>(size_t(0), candidates.ee_candidates.size()),
+        [&](const tbb::blocked_range<size_t>& r) {
+            storage.local().add_edge_edge_constraints(
+                mesh, vertices, candidates.ee_candidates, is_active, r.begin(),
+                r.end());
+        });
+
+    tbb::parallel_for(
+        tbb::blocked_range<size_t>(size_t(0), candidates.fv_candidates.size()),
+        [&](const tbb::blocked_range<size_t>& r) {
+            storage.local().add_face_vertex_constraints(
+                mesh, vertices, candidates.fv_candidates, is_active, r.begin(),
+                r.end());
+        });
+
+    CollisionConstraintsBuilder::merge(storage, *this);
+
+    for (size_t ci = 0; ci < size(); ci++) {
+        CollisionConstraint& constraint = (*this)[ci];
+        constraint.minimum_distance = dmin;
+    }
+
+    if (use_convergent_formulation()) {
+        // NOTE: When using the convergent formulation we want the barrier to
+        // have units of Pa⋅m, so κ gets units of Pa and the barrier function
+        // should have units of m. See notebooks/physical_barrier.ipynb for more
+        // details.
+        const double barrier_to_physical_barrier_divisor =
+            dhat * std::pow(dhat + 2 * dmin, 2);
+
+        for (size_t ci = 0; ci < size(); ci++) {
+            CollisionConstraint& constraint = (*this)[ci];
+            constraint.weight /= barrier_to_physical_barrier_divisor;
+            if (are_shape_derivatives_enabled()) {
+                constraint.weight_gradient /=
+                    barrier_to_physical_barrier_divisor;
+            }
+        }
+    }
+}
+
+void CollisionConstraints::set_use_convergent_formulation(
+    const bool use_convergent_formulation)
+{
+    if (!empty()
+        && use_convergent_formulation != m_use_convergent_formulation) {
+        logger().warn(
+            "Setting use_convergent_formulation after building constraints. "
+            "Re-build constraints for this to have an effect.");
     }
 
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    m_use_convergent_formulation = use_convergent_formulation;
+}
+
+void CollisionConstraints::set_are_shape_derivatives_enabled(
+    const bool are_shape_derivatives_enabled)
+{
+    if (!empty()
+        && are_shape_derivatives_enabled != m_are_shape_derivatives_enabled) {
+        logger().warn(
+            "Setting enable_shape_derivatives after building constraints. "
+            "Re-build constraints for this to have an effect.");
+    }
+
+    m_are_shape_derivatives_enabled = are_shape_derivatives_enabled;
+}
+
+// ============================================================================
+
+double CollisionConstraints::compute_potential(
+    const CollisionMesh& mesh,
+    const Eigen::MatrixXd& vertices,
+    const double dhat) const
+{
+    assert(vertices.rows() == mesh.num_vertices());
+    assert(dhat > 0);
+
+    if (empty()) {
+        return 0;
+    }
 
     tbb::enumerable_thread_specific<double> storage(0);
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
             auto& local_potential = storage.local();
             for (size_t i = r.begin(); i < r.end(); i++) {
                 // Quadrature weight is premultiplied by compute_potential
-                local_potential +=
-                    constraint_set[i].compute_potential(V, E, F, dhat);
+                local_potential += (*this)[i].compute_potential(
+                    vertices, mesh.edges(), mesh.faces(), dhat);
             }
         });
 
-    double potential = 0;
-    for (const auto& local_potential : storage) {
-        potential += local_potential;
-    }
-    return potential;
+    return storage.combine([](double a, double b) { return a + b; });
 }
 
-Eigen::VectorXd compute_barrier_potential_gradient(
+Eigen::VectorXd CollisionConstraints::compute_potential_gradient(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
-    const double dhat)
+    const Eigen::MatrixXd& vertices,
+    const double dhat) const
 {
-    assert(V.rows() == mesh.num_vertices());
+    assert(vertices.rows() == mesh.num_vertices());
 
-    if (constraint_set.empty()) {
-        return Eigen::VectorXd::Zero(V.size());
+    if (empty()) {
+        return Eigen::VectorXd::Zero(vertices.size());
     }
 
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    const Eigen::MatrixXi& edges = mesh.edges();
+    const Eigen::MatrixXi& faces = mesh.faces();
 
-    int dim = V.cols();
+    int dim = vertices.cols();
 
     tbb::enumerable_thread_specific<Eigen::VectorXd> storage(
-        Eigen::VectorXd::Zero(V.size()));
+        Eigen::VectorXd::Zero(vertices.size()));
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
             auto& local_grad = storage.local();
             for (size_t i = r.begin(); i < r.end(); i++) {
                 local_gradient_to_global_gradient(
-                    constraint_set[i].compute_potential_gradient(V, E, F, dhat),
-                    constraint_set[i].vertex_indices(E, F), dim, local_grad);
+                    (*this)[i].compute_potential_gradient(
+                        vertices, edges, faces, dhat),
+                    (*this)[i].vertex_ids(edges, faces), dim, local_grad);
             }
         });
 
-    Eigen::VectorXd grad = Eigen::VectorXd::Zero(V.size());
-    for (const auto& local_grad : storage) {
-        grad += local_grad;
-    }
-    return grad;
+    return storage.combine([](const Eigen::VectorXd& a,
+                              const Eigen::VectorXd& b) { return a + b; });
 }
 
-Eigen::SparseMatrix<double> compute_barrier_potential_hessian(
+Eigen::SparseMatrix<double> CollisionConstraints::compute_potential_hessian(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
+    const Eigen::MatrixXd& vertices,
     const double dhat,
-    const bool project_hessian_to_psd)
+    const bool project_hessian_to_psd) const
 {
-    assert(V.rows() == mesh.num_vertices());
+    assert(vertices.rows() == mesh.num_vertices());
 
-    if (constraint_set.empty()) {
-        return Eigen::SparseMatrix<double>(V.size(), V.size());
+    if (empty()) {
+        return Eigen::SparseMatrix<double>(vertices.size(), vertices.size());
     }
 
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    const Eigen::MatrixXi& edges = mesh.edges();
+    const Eigen::MatrixXi& faces = mesh.faces();
 
-    const int dim = V.cols();
+    const int dim = vertices.cols();
 
     tbb::enumerable_thread_specific<std::vector<Eigen::Triplet<double>>>
         storage;
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
             auto& local_hess_triplets = storage.local();
 
             for (size_t i = r.begin(); i < r.end(); i++) {
                 local_hessian_to_global_triplets(
-                    constraint_set[i].compute_potential_hessian(
-                        V, E, F, dhat, project_hessian_to_psd),
-                    constraint_set[i].vertex_indices(E, F), dim,
+                    (*this)[i].compute_potential_hessian(
+                        vertices, edges, faces, dhat, project_hessian_to_psd),
+                    (*this)[i].vertex_ids(edges, faces), dim,
                     local_hess_triplets);
             }
         });
 
-    Eigen::SparseMatrix<double> hess(V.size(), V.size());
+    Eigen::SparseMatrix<double> hess(vertices.size(), vertices.size());
     for (const auto& local_hess_triplets : storage) {
-        Eigen::SparseMatrix<double> local_hess(V.size(), V.size());
+        Eigen::SparseMatrix<double> local_hess(
+            vertices.size(), vertices.size());
         local_hess.setFromTriplets(
             local_hess_triplets.begin(), local_hess_triplets.end());
         hess += local_hess;
     }
     return hess;
 }
 
-Eigen::SparseMatrix<double> compute_barrier_shape_derivative(
+// ============================================================================
+
+Eigen::SparseMatrix<double> CollisionConstraints::compute_shape_derivative(
     const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
-    const double dhat)
+    const Eigen::MatrixXd& vertices,
+    const double dhat) const
 {
     Eigen::SparseMatrix<double> shape_derivative =
-        compute_barrier_potential_hessian(mesh, V, constraint_set, dhat, false);
+        compute_potential_hessian(mesh, vertices, dhat, false);
 
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    const Eigen::MatrixXi& edges = mesh.edges();
+    const Eigen::MatrixXi& faces = mesh.faces();
 
-    const int dim = V.cols();
+    const int dim = vertices.cols();
 
     tbb::enumerable_thread_specific<std::vector<Eigen::Triplet<double>>>
         storage;
 
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(size_t(0), constraint_set.size()),
+        tbb::blocked_range<size_t>(size_t(0), size()),
         [&](const tbb::blocked_range<size_t>& r) {
             auto& local_triplets = storage.local();
 
             // for (size_t ci = 0; ci < constraint_set.size(); ci++) {
             for (size_t ci = r.begin(); ci < r.end(); ci++) {
 
-                const CollisionConstraint& constraint = constraint_set[ci];
+                const CollisionConstraint& constraint = (*this)[ci];
                 const Eigen::SparseVector<double>& weight_gradient =
                     constraint.weight_gradient;
-                if (weight_gradient.size() != V.size()) {
+                if (weight_gradient.size() != vertices.size()) {
                     throw std::runtime_error(
                         "Shape derivative is not computed for contact constraint!");
                 }
 
                 VectorMax12d local_barrier_grad =
-                    constraint.compute_potential_gradient(V, E, F, dhat);
+                    constraint.compute_potential_gradient(
+                        vertices, edges, faces, dhat);
                 assert(constraint.weight != 0);
                 local_barrier_grad.array() /= constraint.weight;
 
-                const std::array<long, 4> ids = constraint.vertex_indices(E, F);
+                const std::array<long, 4> ids =
+                    constraint.vertex_ids(edges, faces);
                 assert(local_barrier_grad.size() % dim == 0);
                 const int n_verts = local_barrier_grad.size() / dim;
                 assert(ids.size() >= n_verts); // Can be extra ids
 
                 for (int i = 0; i < n_verts; i++) {
                     for (int d = 0; d < dim; d++) {
                         using Itr = Eigen::SparseVector<double>::InnerIterator;
@@ -194,268 +292,127 @@
                         }
                     }
                 }
             }
         });
 
     for (const auto& local_triplets : storage) {
-        Eigen::SparseMatrix<double> local_shape_derivative(V.size(), V.size());
+        Eigen::SparseMatrix<double> local_shape_derivative(
+            vertices.size(), vertices.size());
         local_shape_derivative.setFromTriplets(
             local_triplets.begin(), local_triplets.end());
         shape_derivative += local_shape_derivative;
     }
 
     return shape_derivative;
 }
 
-///////////////////////////////////////////////////////////////////////////////
-
-bool is_step_collision_free(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const BroadPhaseMethod method,
-    const double min_distance,
-    const double tolerance,
-    const long max_iterations)
-{
-    assert(V0.rows() == mesh.num_vertices());
-    assert(V1.rows() == mesh.num_vertices());
-
-    // Broad phase
-    Candidates candidates;
-    construct_collision_candidates(
-        mesh, V0, V1, candidates, /*inflation_radius=*/min_distance / 1.99,
-        method);
-
-    // Narrow phase
-    return is_step_collision_free(
-        candidates, mesh, V0, V1, min_distance, tolerance, max_iterations);
-}
-
-bool is_step_collision_free(
-    const Candidates& candidates,
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const double min_distance,
-    const double tolerance,
-    const long max_iterations)
-{
-    assert(V0.rows() == mesh.num_vertices());
-    assert(V1.rows() == mesh.num_vertices());
-
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
-
-    // Narrow phase
-    for (size_t i = 0; i < candidates.size(); i++) {
-        double toi;
-        bool is_collision = candidates[i].ccd(
-            V0, V1, E, F, toi, min_distance, /*tmax=*/1.0, tolerance,
-            max_iterations);
-
-        if (is_collision) {
-            return false;
-        }
-    }
-
-    return true;
-}
-
-///////////////////////////////////////////////////////////////////////////////
-
-double compute_collision_free_stepsize(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const BroadPhaseMethod method,
-    const double min_distance,
-    const double tolerance,
-    const long max_iterations)
-{
-    assert(V0.rows() == mesh.num_vertices());
-    assert(V1.rows() == mesh.num_vertices());
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
-
-    if (method == BroadPhaseMethod::SWEEP_AND_TINIEST_QUEUE_GPU) {
-#ifdef IPC_TOOLKIT_WITH_CUDA
-        double min_distance = 0; // TODO
-        const double step_size = ccd::gpu::compute_toi_strategy(
-            V0, V1, E, F, max_iterations, min_distance, tolerance);
-        if (step_size < 1.0) {
-            return 0.8 * step_size;
-        }
-        return 1.0;
-#else
-        throw std::runtime_error("GPU Sweep and Tiniest Queue is disabled "
-                                 "because CUDA is disabled!");
-#endif
-    }
-
-    // Broad phase
-    Candidates candidates;
-    construct_collision_candidates(
-        mesh, V0, V1, candidates, /*inflation_radius=*/min_distance / 1.99,
-        method);
-
-    // Narrow phase
-    double step_size = compute_collision_free_stepsize(
-        candidates, mesh, V0, V1, min_distance, tolerance, max_iterations);
-
-    return step_size;
-}
-
-double compute_collision_free_stepsize(
-    const Candidates& candidates,
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const double min_distance,
-    const double tolerance,
-    const long max_iterations)
-{
-    assert(V0.rows() == mesh.num_vertices());
-    assert(V1.rows() == mesh.num_vertices());
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
-
-    if (candidates.empty()) {
-        return 1; // No possible collisions, so can take full step.
-    }
-
-    double earliest_toi = 1;
-    std::shared_mutex earliest_toi_mutex;
-
-    tbb::parallel_for(
-        tbb::blocked_range<size_t>(0, candidates.size()),
-        [&](tbb::blocked_range<size_t> r) {
-            for (size_t i = r.begin(); i < r.end(); i++) {
-                // Use the mutex to read as well in case writing double takes
-                // more than one clock cycle.
-                double tmax;
-                {
-                    std::shared_lock lock(earliest_toi_mutex);
-                    tmax = earliest_toi;
-                }
-
-                double toi = std::numeric_limits<double>::infinity(); // output
-                bool are_colliding = candidates[i].ccd(
-                    V0, V1, E, F, toi, min_distance, tmax, tolerance,
-                    max_iterations);
-
-                if (are_colliding) {
-                    std::unique_lock lock(earliest_toi_mutex);
-                    if (toi < earliest_toi) {
-                        earliest_toi = toi;
-                    }
-                }
-            }
-        });
-
-    assert(earliest_toi >= 0 && earliest_toi <= 1.0);
-    return earliest_toi;
-}
-
-///////////////////////////////////////////////////////////////////////////////
+// ============================================================================
 
 // NOTE: Actually distance squared
-double compute_minimum_distance(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set)
+double CollisionConstraints::compute_minimum_distance(
+    const CollisionMesh& mesh, const Eigen::MatrixXd& vertices) const
 {
-    assert(V.rows() == mesh.num_vertices());
+    assert(vertices.rows() == mesh.num_vertices());
 
-    if (constraint_set.empty()) {
+    if (empty()) {
         return std::numeric_limits<double>::infinity();
     }
 
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
+    const Eigen::MatrixXi& edges = mesh.edges();
+    const Eigen::MatrixXi& faces = mesh.faces();
 
     tbb::enumerable_thread_specific<double> storage(
         std::numeric_limits<double>::infinity());
 
     // Do a single block range over all constraint vectors
     tbb::parallel_for(
-        tbb::blocked_range<size_t>(0, constraint_set.size()),
+        tbb::blocked_range<size_t>(0, size()),
         [&](tbb::blocked_range<size_t> r) {
             double& local_min_dist = storage.local();
 
             for (size_t i = r.begin(); i < r.end(); i++) {
-                const double dist = constraint_set[i].compute_distance(V, E, F);
+                const double dist =
+                    (*this)[i].compute_distance(vertices, edges, faces);
 
                 if (dist < local_min_dist) {
                     local_min_dist = dist;
                 }
             }
         });
 
-    double min_dist = std::numeric_limits<double>::infinity();
-    for (const auto& local_min_dist : storage) {
-        min_dist = std::min(min_dist, local_min_dist);
-    }
-    return min_dist;
+    return storage.combine([](double a, double b) { return std::min(a, b); });
 }
 
-///////////////////////////////////////////////////////////////////////////////
+// ============================================================================
 
-bool has_intersections(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const BroadPhaseMethod method)
+size_t CollisionConstraints::size() const
 {
-    assert(V.rows() == mesh.num_vertices());
-    const Eigen::MatrixXi& E = mesh.edges();
-    const Eigen::MatrixXi& F = mesh.faces();
-
-    const double conservative_inflation_radius =
-        1e-6 * world_bbox_diagonal_length(V);
-
-    // TODO: Expose the broad-phase method
-    std::unique_ptr<BroadPhase> broad_phase =
-        BroadPhase::make_broad_phase(method);
-    broad_phase->can_vertices_collide = mesh.can_collide;
-
-    broad_phase->build(V, E, F, conservative_inflation_radius);
-
-    if (V.cols() == 2) { // Need to check segment-segment intersections in 2D
-        std::vector<EdgeEdgeCandidate> ee_candidates;
-
-        broad_phase->detect_edge_edge_candidates(ee_candidates);
-        broad_phase->clear();
-
-        // narrow-phase using igl
-        igl::predicates::exactinit();
-        for (const EdgeEdgeCandidate& ee_candidate : ee_candidates) {
-            if (igl::predicates::segment_segment_intersect(
-                    V.row(E(ee_candidate.edge0_index, 0)).head<2>(),
-                    V.row(E(ee_candidate.edge0_index, 1)).head<2>(),
-                    V.row(E(ee_candidate.edge1_index, 0)).head<2>(),
-                    V.row(E(ee_candidate.edge1_index, 1)).head<2>())) {
-                return true;
-            }
-        }
-    } else { // Need to check segment-triangle intersections in 3D
-        assert(V.cols() == 3);
+    return vv_constraints.size() + ev_constraints.size() + ee_constraints.size()
+        + fv_constraints.size() + pv_constraints.size();
+}
 
-        std::vector<EdgeFaceCandidate> ef_candidates;
-        broad_phase->detect_edge_face_candidates(ef_candidates);
-        broad_phase->clear();
-
-        for (const EdgeFaceCandidate& ef_candidate : ef_candidates) {
-            if (is_edge_intersecting_triangle(
-                    V.row(E(ef_candidate.edge_index, 0)),
-                    V.row(E(ef_candidate.edge_index, 1)),
-                    V.row(F(ef_candidate.face_index, 0)),
-                    V.row(F(ef_candidate.face_index, 1)),
-                    V.row(F(ef_candidate.face_index, 2)))) {
-                return true;
-            }
-        }
+bool CollisionConstraints::empty() const
+{
+    return vv_constraints.empty() && ev_constraints.empty()
+        && ee_constraints.empty() && fv_constraints.empty()
+        && pv_constraints.empty();
+}
+
+void CollisionConstraints::clear()
+{
+    vv_constraints.clear();
+    ev_constraints.clear();
+    ee_constraints.clear();
+    fv_constraints.clear();
+    pv_constraints.clear();
+}
+
+CollisionConstraint& CollisionConstraints::operator[](size_t idx)
+{
+    if (idx < vv_constraints.size()) {
+        return vv_constraints[idx];
+    }
+    idx -= vv_constraints.size();
+    if (idx < ev_constraints.size()) {
+        return ev_constraints[idx];
+    }
+    idx -= ev_constraints.size();
+    if (idx < ee_constraints.size()) {
+        return ee_constraints[idx];
+    }
+    idx -= ee_constraints.size();
+    if (idx < fv_constraints.size()) {
+        return fv_constraints[idx];
+    }
+    idx -= fv_constraints.size();
+    if (idx < pv_constraints.size()) {
+        return pv_constraints[idx];
     }
+    throw std::out_of_range("Constraint index is out of range!");
+}
 
-    return false;
+const CollisionConstraint& CollisionConstraints::operator[](size_t idx) const
+{
+    if (idx < vv_constraints.size()) {
+        return vv_constraints[idx];
+    }
+    idx -= vv_constraints.size();
+    if (idx < ev_constraints.size()) {
+        return ev_constraints[idx];
+    }
+    idx -= ev_constraints.size();
+    if (idx < ee_constraints.size()) {
+        return ee_constraints[idx];
+    }
+    idx -= ee_constraints.size();
+    if (idx < fv_constraints.size()) {
+        return fv_constraints[idx];
+    }
+    idx -= fv_constraints.size();
+    if (idx < pv_constraints.size()) {
+        return pv_constraints[idx];
+    }
+    throw std::out_of_range("Constraint index is out of range!");
 }
+
 } // namespace ipc
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ipctk-1.0.0/src/ipc/ipc.hpp` & `ipctk-1.1.0/src/ipc/friction/friction_constraints.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,161 @@
 #pragma once
 
-// NOTE: Include this so the user can just include ipc.hpp
-#include <ipc/collisions/constraints.hpp>
-#include <ipc/friction/friction.hpp>
-#include <ipc/broad_phase/broad_phase.hpp>
+#include <ipc/friction/constraints/friction_constraint.hpp>
+#include <ipc/friction/constraints/vertex_vertex.hpp>
+#include <ipc/friction/constraints/edge_vertex.hpp>
+#include <ipc/friction/constraints/edge_edge.hpp>
+#include <ipc/friction/constraints/face_vertex.hpp>
+
 #include <ipc/collision_mesh.hpp>
+#include <ipc/collisions/collision_constraints.hpp>
+#include <ipc/utils/eigen_ext.hpp>
 
 #include <Eigen/Core>
 #include <Eigen/Sparse>
 
-/// Incremental Potential Contact functions
 namespace ipc {
 
-/// @brief Compute the barrier potential for a given constraint set.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V Vertices of the collision mesh.
-/// @param[in] constraint_set The set of constraints.
-/// @param[in] dhat The activation distance of the barrier.
-/// @returns The sum of all barrier potentials (not scaled by the barrier stiffness).
-double compute_barrier_potential(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
-    const double dhat);
-
-/// @brief Compute the gradient of the barrier potential.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V Vertices of the collision mesh.
-/// @param[in] constraint_set The set of constraints.
-/// @param[in] dhat The activation distance of the barrier.
-/// @returns The gradient of all barrier potentials (not scaled by the barrier stiffness). This will have a size of |V|.
-Eigen::VectorXd compute_barrier_potential_gradient(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
-    const double dhat);
-
-/// @brief Compute the hessian of the barrier potential.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V Vertices of the collision mesh.
-/// @param[in] constraint_set The set of constraints.
-/// @param[in] dhat The activation distance of the barrier.
-/// @param[in] project_hessian_to_psd Make sure the hessian is positive semi-definite.
-/// @returns The hessian of all barrier potentials (not scaled by the barrier stiffness). This will have a size of |V|x|V|.
-Eigen::SparseMatrix<double> compute_barrier_potential_hessian(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
-    const double dhat,
-    const bool project_hessian_to_psd = true);
-
-/// @brief Compute the barrier shape derivative.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V Vertices of the collision mesh.
-/// @param[in] constraint_set The set of constraints.
-/// @param[in] dhat The activation distance of the barrier.
-/// @returns The derivative of the force with respect to X, the rest positions.
-Eigen::SparseMatrix<double> compute_barrier_shape_derivative(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set,
-    const double dhat);
-
-///////////////////////////////////////////////////////////////////////////////
-// Collision detection
-
-/// @brief Determine if the step is collision free.
-/// @note Assumes the trajectory is linear.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V0 Surface vertex positions at start as rows of a matrix.
-/// @param[in] V1 Surface vertex positions at end as rows of a matrix.
-/// @returns True if <b>any</b> collisions occur.
-bool is_step_collision_free(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const BroadPhaseMethod method = BroadPhaseMethod::HASH_GRID,
-    const double min_distance = 0.0,
-    const double tolerance = 1e-6,
-    const long max_iterations = 1e7);
-
-/// @brief Determine if the step is collision free from a set of candidates.
-/// @note Assumes the trajectory is linear.
-/// @param[in] candidates Set of candidates to check for collisions.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V0 Surface vertex positions at start as rows of a matrix.
-/// @param[in] V1 Surface vertex positions at end as rows of a matrix.
-/// @returns True if <b>any</b> collisions occur.
-bool is_step_collision_free(
-    const Candidates& candidates,
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const double min_distance = 0.0,
-    const double tolerance = 1e-6,
-    const long max_iterations = 1e7);
-
-/// @brief Computes a maximal step size that is collision free.
-/// @note Assumes the trajectory is linear.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V0 Vertex positions at start as rows of a matrix. Assumes V0 is intersection free.
-/// @param[in] V1 Surface vertex positions at end as rows of a matrix.
-/// @returns A step-size \f$\in [0, 1]\f$ that is collision free. A value of 1.0 if a full step and 0.0 is no step.
-double compute_collision_free_stepsize(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const BroadPhaseMethod method = BroadPhaseMethod::HASH_GRID,
-    const double min_distance = 0.0,
-    const double tolerance = 1e-6,
-    const long max_iterations = 1e7);
-
-/// @brief Computes a maximal step size that is collision free using a set of collision candidates.
-/// @note Assumes the trajectory is linear.
-/// @param[in] candidates Set of candidates to check for collisions.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V0 Vertex positions at start as rows of a matrix. Assumes V0 is intersection free.
-/// @param[in] V1 Surface vertex positions at end as rows of a matrix.
-/// @returns A step-size \f$\in [0, 1]\f$ that is collision free. A value of 1.0 if a full step and 0.0 is no step.
-double compute_collision_free_stepsize(
-    const Candidates& candidates,
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V0,
-    const Eigen::MatrixXd& V1,
-    const double min_distance = 0.0,
-    const double tolerance = 1e-6,
-    const long max_iterations = 1e7);
-
-///////////////////////////////////////////////////////////////////////////////
-// Utilities
-
-/// @brief Computes the minimum distance between any non-adjacent elements.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V Vertices of the collision mesh.
-/// @returns The minimum distance between any non-adjacent elements.
-double compute_minimum_distance(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const Constraints& constraint_set);
-
-/// @brief Determine if the mesh has self intersections.
-/// @param[in] mesh The collision mesh.
-/// @param[in] V Vertices of the collision mesh.
-/// @return A boolean for if the mesh has intersections.
-bool has_intersections(
-    const CollisionMesh& mesh,
-    const Eigen::MatrixXd& V,
-    const BroadPhaseMethod method = BroadPhaseMethod::HASH_GRID);
+class FrictionConstraints {
+public:
+    FrictionConstraints() { }
+
+    void build(
+        const CollisionMesh& mesh,
+        const Eigen::MatrixXd& vertices,
+        const CollisionConstraints& contact_constraints,
+        double dhat,
+        double barrier_stiffness,
+        double mu)
+    {
+        this->build(
+            mesh, vertices, contact_constraints, dhat, barrier_stiffness,
+            Eigen::VectorXd::Constant(vertices.rows(), mu));
+    }
+
+    void build(
+        const CollisionMesh& mesh,
+        const Eigen::MatrixXd& vertices,
+        const CollisionConstraints& contact_constraints,
+        const double dhat,
+        const double barrier_stiffness,
+        const Eigen::VectorXd& mus,
+        const std::function<double(double, double)>& blend_mu =
+            default_blend_mu);
+
+    // ------------------------------------------------------------------------
+
+    /// @brief Compute the friction dissapative potential from the given velocity.
+    /// @param mesh The collision mesh.
+    /// @param velocity Current vertex velocity (rowwise).
+    /// @param epsv Mollifier parameter \f$\epsilon_v\f$.
+    /// @return The friction dissapative potential.
+    double compute_potential(
+        const CollisionMesh& mesh,
+        const Eigen::MatrixXd& velocity,
+        const double epsv) const;
+
+    /// @brief Compute the gradient of the friction dissapative potential wrt the velocity.
+    /// @param mesh The collision mesh.
+    /// @param velocity Current vertex velocity (rowwise).
+    /// @param epsv Mollifier parameter \f$\epsilon_v\f$.
+    /// @return The gradient of the friction dissapative potential wrt the velocity.
+    Eigen::VectorXd compute_potential_gradient(
+        const CollisionMesh& mesh,
+        const Eigen::MatrixXd& velocity,
+        const double epsv) const;
+
+    /// @brief Compute the Hessian of the friction dissapative potential wrt the velocity.
+    /// @param mesh The collision mesh.
+    /// @param velocity Current vertex velocity (rowwise).
+    /// @param epsv Mollifier parameter \f$\epsilon_v\f$.
+    /// @param project_hessian_to_psd If true, project the Hessian to be positive semi-definite.
+    /// @return The Hessian of the friction dissapative potential wrt the velocity.
+    Eigen::SparseMatrix<double> compute_potential_hessian(
+        const CollisionMesh& mesh,
+        const Eigen::MatrixXd& velocity,
+        const double epsv,
+        const bool project_hessian_to_psd = false) const;
+
+    // ------------------------------------------------------------------------
+
+    /// @brief Compute the friction force from the given velocity.
+    /// @param mesh The collision mesh.
+    /// @param rest_positions Rest positions of the vertices (rowwise)
+    /// @param lagged_displacements Previous displacements of the vertices (rowwise)
+    /// @param velocities Current displacements of the vertices (rowwise)
+    /// @param dhat Barrier activation distance.
+    /// @param barrier_stiffness Barrier stiffness.
+    /// @param epsv Mollifier parameter \f$\epsilon_v\f$.
+    /// @param dmin Minimum distance to use for the barrier.
+    /// @param no_mu whether to not multiply by mu
+    /// @return The friction force.
+    Eigen::VectorXd compute_force(
+        const CollisionMesh& mesh,
+        const Eigen::MatrixXd& rest_positions,
+        const Eigen::MatrixXd& lagged_displacements,
+        const Eigen::MatrixXd& velocities,
+        const double dhat,
+        const double barrier_stiffness,
+        const double epsv,
+        const double dmin = 0,
+        const bool no_mu = false) const;
+
+    /// @brief Compute the Jacobian of the friction force wrt the velocity.
+    /// @param mesh The collision mesh.
+    /// @param rest_positions Rest positions of the vertices (rowwise)
+    /// @param lagged_displacements Previous displacements of the vertices (rowwise)
+    /// @param velocities Current displacements of the vertices (rowwise)
+    /// @param dhat Barrier activation distance.
+    /// @param barrier_stiffness Barrier stiffness.
+    /// @param epsv Mollifier parameter \f$\epsilon_v\f$.
+    /// @param wrt The variable to take the derivative with respect to.
+    /// @param dmin Minimum distance to use for the barrier.
+    /// @return The Jacobian of the friction force wrt the velocity.
+    Eigen::SparseMatrix<double> compute_force_jacobian(
+        const CollisionMesh& mesh,
+        const Eigen::MatrixXd& rest_positions,
+        const Eigen::MatrixXd& lagged_displacements,
+        const Eigen::MatrixXd& velocities,
+        const double dhat,
+        const double barrier_stiffness,
+        const double epsv,
+        const FrictionConstraint::DiffWRT wrt,
+        const double dmin = 0) const;
+
+    // ------------------------------------------------------------------------
+
+    /// @brief Get the number of friction constraints.
+    size_t size() const;
+
+    /// @brief Get if the friction constraints are empty.
+    bool empty() const;
+
+    /// @brief Clear the friction constraints.
+    void clear();
+
+    /// @brief Get a reference to constriant idx.
+    /// @param idx The index of the constraint.
+    /// @return A reference to the constraint.
+    FrictionConstraint& operator[](const size_t idx);
+
+    /// @brief Get a const reference to constriant idx.
+    /// @param idx The index of the constraint.
+    /// @return A const reference to the constraint.
+    const FrictionConstraint& operator[](const size_t idx) const;
+
+    static double default_blend_mu(double mu0, double mu1)
+    {
+        // return mu0 * mu1;
+        // return std::min(mu0, mu1);
+        // return std::max(mu0, mu1);
+        return (mu0 + mu1) / 2;
+    }
+
+public:
+    std::vector<VertexVertexFrictionConstraint> vv_constraints;
+    std::vector<EdgeVertexFrictionConstraint> ev_constraints;
+    std::vector<EdgeEdgeFrictionConstraint> ee_constraints;
+    std::vector<FaceVertexFrictionConstraint> fv_constraints;
+};
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/utils/area_gradient.cpp` & `ipctk-1.1.0/src/ipc/utils/area_gradient.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,40 @@
 #include "area_gradient.hpp"
 
 #include <cmath>
 
 namespace ipc {
+
+VectorMax6d edge_length_gradient(
+    const Eigen::Ref<const VectorMax3d>& e0,
+    const Eigen::Ref<const VectorMax3d>& e1)
+{
+    assert(e0.size() == 2 || e0.size() == 3);
+    assert(e1.size() == 2 || e1.size() == 3);
+    assert((e1 - e0).norm() != 0);
+
+    // ∇ ‖e₁ - e₀‖
+    VectorMax6d grad(e0.size() + e1.size());
+    grad.head(e0.size()) = (e0 - e1) / (e1 - e0).norm();
+    grad.tail(e1.size()) = -grad.head(e0.size());
+    return grad;
+}
+
+Vector9d triangle_area_gradient(
+    const Eigen::Ref<const Eigen::Vector3d>& t0,
+    const Eigen::Ref<const Eigen::Vector3d>& t1,
+    const Eigen::Ref<const Eigen::Vector3d>& t2)
+{
+    Vector9d grad;
+    autogen::triangle_area_gradient(
+        t0[0], t0[1], t0[2], t1[0], t1[1], t1[2], t2[0], t2[1], t2[2],
+        grad.data());
+    return grad;
+}
+
 namespace autogen {
 
     // dA is (9×1) flattened in column-major order
     void triangle_area_gradient(
         double t0_x,
         double t0_y,
         double t0_z,
```

### Comparing `ipctk-1.0.0/src/ipc/utils/eigen_ext.hpp` & `ipctk-1.1.0/src/ipc/utils/eigen_ext.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 template <typename T> using RowVectorX = RowVector<T, Eigen::Dynamic>;
 template <typename T> using Matrix2 = Eigen::Matrix<T, 2, 2>;
 template <typename T> using Matrix3 = Eigen::Matrix<T, 3, 3>;
 template <typename T>
 using MatrixX = Eigen::Matrix<T, Eigen::Dynamic, Eigen::Dynamic>;
 
 using Vector1d = Vector1<double>;
+using Vector6d = Vector<double, 6>;
+using Vector9d = Vector<double, 9>;
+using Vector12d = Vector<double, 12>;
+using Matrix6d = Eigen::Matrix<double, 6, 6>;
+using Matrix9d = Eigen::Matrix<double, 9, 9>;
+using Matrix12d = Eigen::Matrix<double, 12, 12>;
+
 /// @brief A dynamic size matrix with a fixed maximum size of 3×1
 template <typename T> using VectorMax2 = Vector<T, Eigen::Dynamic, 2>;
 /// @brief A dynamic size matrix with a fixed maximum size of 3×1
 template <typename T> using VectorMax3 = Vector<T, Eigen::Dynamic, 3>;
 /// @brief A dynamic size matrix with a fixed maximum size of 2×1
 using VectorMax2d = VectorMax2<double>;
 /// @brief A dynamic size matrix with a fixed maximum size of 3×1
@@ -135,25 +142,14 @@
     int _MaxRows,
     int _MaxCols>
 Eigen::Matrix<_Scalar, _Rows, _Cols, _Options, _MaxRows, _MaxCols>
 project_to_psd(
     const Eigen::Matrix<_Scalar, _Rows, _Cols, _Options, _MaxRows, _MaxCols>&
         A);
 
-/// Cross product for dynamically sized matrices.
-template <
-    typename DerivedA,
-    typename DerivedB,
-    typename Result = Eigen::Matrix<
-        typename DerivedA::Scalar,
-        DerivedA::RowsAtCompileTime,
-        DerivedA::ColsAtCompileTime>>
-Result cross(
-    const Eigen::MatrixBase<DerivedA>& a, const Eigen::MatrixBase<DerivedB>& b);
-
 /// Eigen IO Format to format vectors like vertex rows in an OBJ file.
 static const Eigen::IOFormat OBJ_VERTEX_FORMAT = Eigen::IOFormat(
     Eigen::FullPrecision, Eigen::DontAlignCols, " ", "", "v ", "\n", "", "");
 
 } // namespace ipc
 
 #include "eigen_ext.tpp"
```

### Comparing `ipctk-1.0.0/src/ipc/utils/eigen_ext.tpp` & `ipctk-1.1.0/src/ipc/utils/eigen_ext.tpp`

 * *Files 5% similar despite different names*

```diff
@@ -86,20 +86,8 @@
             break;
         }
     }
     return eigensolver.eigenvectors() * D
         * eigensolver.eigenvectors().transpose();
 }
 
-template <typename DerivedA, typename DerivedB, typename Result>
-Result cross(
-    const Eigen::MatrixBase<DerivedA>& a, const Eigen::MatrixBase<DerivedB>& b)
-{
-    assert(a.size() == 3 && b.size() == 3);
-    Result c(a.rows(), a.cols());
-    c(0) = a(1) * b(2) - a(2) * b(1);
-    c(1) = a(2) * b(0) - a(0) * b(2);
-    c(2) = a(0) * b(1) - a(1) * b(0);
-    return c;
-}
-
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/utils/intersection.cpp` & `ipctk-1.1.0/src/ipc/utils/intersection.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     if (ori1 != igl::predicates::Orientation::COPLANAR
         && ori2 != igl::predicates::Orientation::COPLANAR && ori1 == ori2) {
         // edge is completly on one side of the plane that triangle is in
         return false;
     }
 
-#ifdef IPC_TOOLKIT_USE_RATIONAL_INTERSECTION
+#ifdef IPC_TOOLKIT_WITH_RATIONAL_INTERSECTION
     return is_edge_intersecting_triangle_rational(e0, e1, t0, t1, t2);
 #else
     Eigen::Matrix3d M;
     M.col(0) = t1 - t0;
     M.col(1) = t2 - t0;
     M.col(2) = e0 - e1;
     Eigen::Vector3d uvt = M.fullPivLu().solve(e0 - t0);
```

### Comparing `ipctk-1.0.0/src/ipc/utils/local_to_global.hpp` & `ipctk-1.1.0/src/ipc/utils/local_to_global.hpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/utils/logger.cpp` & `ipctk-1.1.0/src/ipc/utils/logger.cpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/utils/merge_thread_local.hpp` & `ipctk-1.1.0/src/ipc/utils/merge_thread_local.hpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/utils/rational.hpp` & `ipctk-1.1.0/src/ipc/utils/rational.hpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipc/utils/save_obj.cpp` & `ipctk-1.1.0/src/ipc/utils/save_obj.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     const Eigen::MatrixXi& F,
     const std::vector<EdgeVertexCandidate>& ev_candidates,
     const int v_offset)
 {
     out << "o EV\n";
     int i = v_offset + 1;
     for (const auto& ev_candidate : ev_candidates) {
-        out << V.row(E(ev_candidate.edge_index, 0)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(E(ev_candidate.edge_index, 1)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(ev_candidate.vertex_index).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ev_candidate.edge_id, 0)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ev_candidate.edge_id, 1)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(ev_candidate.vertex_id).format(OBJ_VERTEX_FORMAT);
         out << fmt::format("l {:d} {:d}\n", i, i + 1);
         i += 3;
     }
 }
 
 template <>
 void save_obj(
@@ -36,18 +36,18 @@
     const Eigen::MatrixXi& F,
     const std::vector<EdgeEdgeCandidate>& ee_candidates,
     const int v_offset)
 {
     out << "o EE\n";
     int i = v_offset + 1;
     for (const auto& ee_candidate : ee_candidates) {
-        out << V.row(E(ee_candidate.edge0_index, 0)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(E(ee_candidate.edge0_index, 1)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(E(ee_candidate.edge1_index, 0)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(E(ee_candidate.edge1_index, 1)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ee_candidate.edge0_id, 0)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ee_candidate.edge0_id, 1)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ee_candidate.edge1_id, 0)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ee_candidate.edge1_id, 1)).format(OBJ_VERTEX_FORMAT);
         out << fmt::format("l {:d} {:d}\n", i + 0, i + 1);
         out << fmt::format("l {:d} {:d}\n", i + 2, i + 3);
         i += 4;
     }
 }
 
 template <>
@@ -58,18 +58,18 @@
     const Eigen::MatrixXi& F,
     const std::vector<FaceVertexCandidate>& fv_candidates,
     const int v_offset)
 {
     out << "o FV\n";
     int i = v_offset + 1;
     for (const auto& fv_candidate : fv_candidates) {
-        out << V.row(F(fv_candidate.face_index, 0)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(F(fv_candidate.face_index, 1)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(F(fv_candidate.face_index, 2)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(fv_candidate.vertex_index).format(OBJ_VERTEX_FORMAT);
+        out << V.row(F(fv_candidate.face_id, 0)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(F(fv_candidate.face_id, 1)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(F(fv_candidate.face_id, 2)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(fv_candidate.vertex_id).format(OBJ_VERTEX_FORMAT);
         out << fmt::format("f {:d} {:d} {:d}\n", i, i + 1, i + 2);
         i += 4;
     }
 }
 
 template <>
 void save_obj(
@@ -79,19 +79,19 @@
     const Eigen::MatrixXi& F,
     const std::vector<EdgeFaceCandidate>& ef_candidates,
     const int v_offset)
 {
     out << "o EF\n";
     int i = v_offset + 1;
     for (const auto& ef_candidate : ef_candidates) {
-        out << V.row(E(ef_candidate.edge_index, 0)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(E(ef_candidate.edge_index, 1)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(F(ef_candidate.face_index, 0)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(F(ef_candidate.face_index, 1)).format(OBJ_VERTEX_FORMAT);
-        out << V.row(F(ef_candidate.face_index, 2)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ef_candidate.edge_id, 0)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(E(ef_candidate.edge_id, 1)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(F(ef_candidate.face_id, 0)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(F(ef_candidate.face_id, 1)).format(OBJ_VERTEX_FORMAT);
+        out << V.row(F(ef_candidate.face_id, 2)).format(OBJ_VERTEX_FORMAT);
         out << fmt::format("l {:d} {:d}\n", i, i + 1);
         out << fmt::format("f {:d} {:d} {:d}\n", i + 2, i + 3, i + 4);
         i += 5;
     }
 }
 
 } // namespace ipc
```

### Comparing `ipctk-1.0.0/src/ipc/utils/save_obj.hpp` & `ipctk-1.1.0/src/ipc/utils/save_obj.hpp`

 * *Files identical despite different names*

### Comparing `ipctk-1.0.0/src/ipctk.egg-info/PKG-INFO` & `ipctk-1.1.0/src/ipctk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipctk
-Version: 1.0.0
+Version: 1.1.0
 Summary: A set of reusable functions to integrate Incremental Potential Contact (IPC) into a simulation.
 Author-email: Zachary Ferguson <zfergus@nyu.edu>
 License: MIT License
         
         Copyright (c) 2020 IPC-Sim
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ipctk-1.0.0/src/ipctk.egg-info/SOURCES.txt` & `ipctk-1.1.0/src/ipctk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 README.md
 pyproject.toml
 setup.py
 cmake/find/FindAVX.cmake
 cmake/find/FindFMA.cmake
 cmake/find/FindGMP.cmake
 cmake/find/FindSSE.cmake
-cmake/ipc_toolkit/ipc_toolkit_prepend_current_path.cmake
-cmake/ipc_toolkit/ipc_toolkit_set_source_group.cmake
-cmake/ipc_toolkit/ipc_toolkit_target_link_system_libraries.cmake
+cmake/ipc_toolkit/ipc_toolkit_cpm_cache.cmake
+cmake/ipc_toolkit/ipc_toolkit_filter_flags.cmake
 cmake/ipc_toolkit/ipc_toolkit_use_colors.cmake
 cmake/ipc_toolkit/ipc_toolkit_warnings.cmake
+cmake/recipes/CPM.cmake
 cmake/recipes/abseil.cmake
 cmake/recipes/catch2.cmake
 cmake/recipes/eigen.cmake
 cmake/recipes/evouga_ccd.cmake
 cmake/recipes/finite_diff.cmake
 cmake/recipes/gmp.cmake
 cmake/recipes/gpu_ccd.cmake
@@ -27,70 +27,94 @@
 cmake/recipes/robin_map.cmake
 cmake/recipes/spdlog.cmake
 cmake/recipes/sweep_and_tiniest_queue.cmake
 cmake/recipes/tight_inclusion.cmake
 docs/PYPI_README.md
 python/CMakeLists.txt
 python/src/bindings.cpp
-python/src/collision_constraint.cpp
+python/src/bindings.hpp
 python/src/collision_mesh.cpp
 python/src/common.hpp
 python/src/ipc.cpp
 python/src/barrier/adaptive_stiffness.cpp
 python/src/barrier/barrier.cpp
+python/src/barrier/bindings.hpp
 python/src/broad_phase/aabb.cpp
+python/src/broad_phase/bindings.hpp
 python/src/broad_phase/broad_phase.cpp
 python/src/broad_phase/brute_force.cpp
 python/src/broad_phase/hash_grid.cpp
 python/src/broad_phase/spatial_hash.cpp
 python/src/broad_phase/sweep_and_tiniest_queue.cpp
 python/src/broad_phase/voxel_size_heuristic.cpp
+python/src/candidates/bindings.hpp
 python/src/candidates/candidates.cpp
+python/src/candidates/collision_stencil.cpp
 python/src/candidates/continuous_collision_candidate.cpp
 python/src/candidates/edge_edge.cpp
 python/src/candidates/edge_face.cpp
 python/src/candidates/edge_vertex.cpp
 python/src/candidates/face_vertex.cpp
 python/src/candidates/vertex_vertex.cpp
 python/src/ccd/aabb.cpp
+python/src/ccd/bindings.hpp
 python/src/ccd/ccd.cpp
 python/src/ccd/inexact_point_edge.cpp
 python/src/ccd/point_static_plane.cpp
+python/src/collisions/bindings.hpp
+python/src/collisions/collision_constraint.cpp
+python/src/collisions/collision_constraints.cpp
+python/src/collisions/edge_edge.cpp
+python/src/collisions/edge_vertex.cpp
+python/src/collisions/face_vertex.cpp
+python/src/collisions/plane_vertex.cpp
+python/src/collisions/vertex_vertex.cpp
+python/src/distance/bindings.hpp
 python/src/distance/distance_type.cpp
 python/src/distance/edge_edge.cpp
 python/src/distance/edge_edge_mollifier.cpp
 python/src/distance/line_line.cpp
 python/src/distance/point_edge.cpp
 python/src/distance/point_line.cpp
 python/src/distance/point_plane.cpp
 python/src/distance/point_point.cpp
 python/src/distance/point_triangle.cpp
+python/src/friction/bindings.hpp
 python/src/friction/closest_point.cpp
-python/src/friction/friction.cpp
-python/src/friction/friction_constraint.cpp
+python/src/friction/friction_constraints.cpp
 python/src/friction/normal_force_magnitude.cpp
-python/src/friction/relative_displacement.cpp
+python/src/friction/relative_velocity.cpp
 python/src/friction/smooth_friction_mollifier.cpp
 python/src/friction/tangent_basis.cpp
+python/src/friction/constraints/bindings.hpp
+python/src/friction/constraints/edge_edge.cpp
+python/src/friction/constraints/edge_vertex.cpp
+python/src/friction/constraints/face_vertex.cpp
+python/src/friction/constraints/friction_constraint.cpp
+python/src/friction/constraints/vertex_vertex.cpp
+python/src/implicits/bindings.hpp
+python/src/implicits/plane.cpp
+python/src/utils/area_gradient.cpp
+python/src/utils/bindings.hpp
 python/src/utils/eigen_ext.cpp
 python/src/utils/intersection.cpp
 python/src/utils/logger.cpp
 python/src/utils/thread_limiter.cpp
+python/src/utils/vertex_to_min_edge.cpp
 python/src/utils/world_bbox_diagonal_length.cpp
 src/ipc/CMakeLists.txt
 src/ipc/collision_mesh.cpp
 src/ipc/collision_mesh.hpp
 src/ipc/ipc.cpp
 src/ipc/ipc.hpp
 src/ipc/barrier/CMakeLists.txt
 src/ipc/barrier/adaptive_stiffness.cpp
 src/ipc/barrier/adaptive_stiffness.hpp
 src/ipc/barrier/barrier.cpp
 src/ipc/barrier/barrier.hpp
-src/ipc/barrier/barrier.tpp
 src/ipc/broad_phase/CMakeLists.txt
 src/ipc/broad_phase/aabb.cpp
 src/ipc/broad_phase/aabb.hpp
 src/ipc/broad_phase/broad_phase.cpp
 src/ipc/broad_phase/broad_phase.hpp
 src/ipc/broad_phase/brute_force.cpp
 src/ipc/broad_phase/brute_force.hpp
@@ -101,14 +125,17 @@
 src/ipc/broad_phase/sweep_and_tiniest_queue.cpp
 src/ipc/broad_phase/sweep_and_tiniest_queue.hpp
 src/ipc/broad_phase/voxel_size_heuristic.cpp
 src/ipc/broad_phase/voxel_size_heuristic.hpp
 src/ipc/candidates/CMakeLists.txt
 src/ipc/candidates/candidates.cpp
 src/ipc/candidates/candidates.hpp
+src/ipc/candidates/collision_stencil.cpp
+src/ipc/candidates/collision_stencil.hpp
+src/ipc/candidates/continuous_collision_candidate.cpp
 src/ipc/candidates/continuous_collision_candidate.hpp
 src/ipc/candidates/edge_edge.cpp
 src/ipc/candidates/edge_edge.hpp
 src/ipc/candidates/edge_face.cpp
 src/ipc/candidates/edge_face.hpp
 src/ipc/candidates/edge_vertex.cpp
 src/ipc/candidates/edge_vertex.hpp
@@ -124,53 +151,68 @@
 src/ipc/ccd/inexact_point_edge.cpp
 src/ipc/ccd/inexact_point_edge.hpp
 src/ipc/ccd/point_static_plane.cpp
 src/ipc/ccd/point_static_plane.hpp
 src/ipc/collisions/CMakeLists.txt
 src/ipc/collisions/collision_constraint.cpp
 src/ipc/collisions/collision_constraint.hpp
-src/ipc/collisions/constraints.cpp
-src/ipc/collisions/constraints.hpp
+src/ipc/collisions/collision_constraints.cpp
+src/ipc/collisions/collision_constraints.hpp
+src/ipc/collisions/collision_constraints_builder.cpp
+src/ipc/collisions/collision_constraints_builder.hpp
 src/ipc/collisions/edge_edge.cpp
 src/ipc/collisions/edge_edge.hpp
 src/ipc/collisions/edge_vertex.hpp
 src/ipc/collisions/face_vertex.hpp
 src/ipc/collisions/plane_vertex.cpp
 src/ipc/collisions/plane_vertex.hpp
 src/ipc/collisions/vertex_vertex.hpp
 src/ipc/distance/CMakeLists.txt
+src/ipc/distance/distance_type.cpp
 src/ipc/distance/distance_type.hpp
-src/ipc/distance/distance_type.tpp
+src/ipc/distance/edge_edge.cpp
 src/ipc/distance/edge_edge.hpp
 src/ipc/distance/edge_edge_mollifier.cpp
 src/ipc/distance/edge_edge_mollifier.hpp
 src/ipc/distance/line_line.cpp
 src/ipc/distance/line_line.hpp
+src/ipc/distance/point_edge.cpp
 src/ipc/distance/point_edge.hpp
 src/ipc/distance/point_line.cpp
 src/ipc/distance/point_line.hpp
 src/ipc/distance/point_plane.cpp
 src/ipc/distance/point_plane.hpp
+src/ipc/distance/point_point.cpp
 src/ipc/distance/point_point.hpp
+src/ipc/distance/point_triangle.cpp
 src/ipc/distance/point_triangle.hpp
 src/ipc/friction/CMakeLists.txt
 src/ipc/friction/closest_point.cpp
 src/ipc/friction/closest_point.hpp
-src/ipc/friction/friction.cpp
-src/ipc/friction/friction.hpp
-src/ipc/friction/friction.tpp
-src/ipc/friction/friction_constraint.cpp
-src/ipc/friction/friction_constraint.hpp
+src/ipc/friction/friction_constraints.cpp
+src/ipc/friction/friction_constraints.hpp
 src/ipc/friction/normal_force_magnitude.cpp
 src/ipc/friction/normal_force_magnitude.hpp
-src/ipc/friction/relative_displacement.hpp
+src/ipc/friction/relative_velocity.cpp
+src/ipc/friction/relative_velocity.hpp
+src/ipc/friction/smooth_friction_mollifier.cpp
 src/ipc/friction/smooth_friction_mollifier.hpp
-src/ipc/friction/smooth_friction_mollifier.tpp
 src/ipc/friction/tangent_basis.cpp
 src/ipc/friction/tangent_basis.hpp
+src/ipc/friction/constraints/CMakeLists.txt
+src/ipc/friction/constraints/edge_edge.cpp
+src/ipc/friction/constraints/edge_edge.hpp
+src/ipc/friction/constraints/edge_vertex.cpp
+src/ipc/friction/constraints/edge_vertex.hpp
+src/ipc/friction/constraints/face_vertex.cpp
+src/ipc/friction/constraints/face_vertex.hpp
+src/ipc/friction/constraints/friction_constraint.cpp
+src/ipc/friction/constraints/friction_constraint.hpp
+src/ipc/friction/constraints/vertex_vertex.cpp
+src/ipc/friction/constraints/vertex_vertex.hpp
 src/ipc/implicits/CMakeLists.txt
 src/ipc/implicits/plane.cpp
 src/ipc/implicits/plane.hpp
 src/ipc/utils/CMakeLists.txt
 src/ipc/utils/area_gradient.cpp
 src/ipc/utils/area_gradient.hpp
 src/ipc/utils/eigen_ext.hpp
@@ -180,14 +222,15 @@
 src/ipc/utils/local_to_global.hpp
 src/ipc/utils/logger.cpp
 src/ipc/utils/logger.hpp
 src/ipc/utils/merge_thread_local.hpp
 src/ipc/utils/rational.hpp
 src/ipc/utils/save_obj.cpp
 src/ipc/utils/save_obj.hpp
+src/ipc/utils/unordered_map_and_set.cpp
 src/ipc/utils/unordered_map_and_set.hpp
 src/ipc/utils/vertex_to_min_edge.cpp
 src/ipc/utils/vertex_to_min_edge.hpp
 src/ipc/utils/world_bbox_diagonal_length.hpp
 src/ipctk.egg-info/PKG-INFO
 src/ipctk.egg-info/SOURCES.txt
 src/ipctk.egg-info/dependency_links.txt
```

