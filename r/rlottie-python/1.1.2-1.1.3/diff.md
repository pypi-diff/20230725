# Comparing `tmp/rlottie_python-1.1.2.tar.gz` & `tmp/rlottie_python-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlottie_python-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rlottie_python-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rlottie_python-1.1.2.tar` & `rlottie_python-1.1.3.tar`

### file list

```diff
@@ -1,315 +1,315 @@
--rw-r--r--   0        0        0      447 2023-07-24 15:51:48.275659 rlottie_python-1.1.2/CMakeLists.txt
--rw-r--r--   0        0        0    18092 2023-07-24 15:51:48.275659 rlottie_python-1.1.2/LICENSE
--rw-r--r--   0        0        0     4107 2023-07-24 15:51:48.275659 rlottie_python-1.1.2/README.md
--rw-r--r--   0        0        0     1629 2023-07-24 15:51:48.275659 rlottie_python-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      709 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/AUTHORS
--rw-r--r--   0        0        0     6246 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/CMakeLists.txt
--rw-r--r--   0        0        0      690 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/COPYING
--rw-r--r--   0        0        0    10977 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/README.md
--rwxr-xr-x   0        0        0      317 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/arm_build.sh
--rw-r--r--   0        0        0      320 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/arm_cross.txt
--rw-r--r--   0        0        0      322 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/cmake/config.h.in
--rw-r--r--   0        0        0      546 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/cmake/rlottieConfig.cmake.in
--rw-r--r--   0        0        0      474 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/CMakeLists.txt
--rw-r--r--   0        0        0     9226 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/demo.cpp
--rw-r--r--   0        0        0     2650 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/demo_marker.cpp
--rw-r--r--   0        0        0     4158 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/evasapp.cpp
--rw-r--r--   0        0        0     2957 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/evasapp.h
--rw-r--r--   0        0        0    27371 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/gif.h
--rw-r--r--   0        0        0     4908 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/lottie2gif.cpp
--rw-r--r--   0        0        0     4938 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/lottieperf.cpp
--rw-r--r--   0        0        0     5676 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/lottieview.cpp
--rw-r--r--   0        0        0    14747 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/lottieview.h
--rw-r--r--   0        0        0     7405 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/lottieviewer.cpp
--rw-r--r--   0        0        0     5437 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/lottieviewtest.cpp
--rw-r--r--   0        0        0     2107 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/meson.build
--rw-r--r--   0        0        0     3620 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/pathtest.cpp
--rw-r--r--   0        0        0    27806 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/resource/1643-exploding-star.json
--rw-r--r--   0        0        0    11654 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/resource/1667-firework.json
--rw-r--r--   0        0        0    43105 2023-07-24 15:51:50.547685 rlottie_python-1.1.2/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json
--rw-r--r--   0        0        0   154297 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/29056-nepenthe-illustration.json
--rw-r--r--   0        0        0    10221 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/360º_degree.json
--rw-r--r--   0        0        0     2536 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/3d.json
--rw-r--r--   0        0        0    19081 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/4479-fireworks.json
--rw-r--r--   0        0        0     9299 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/5317-fireworkds.json
--rw-r--r--   0        0        0   138526 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/5344-honey-sack-hud.json
--rw-r--r--   0        0        0    16809 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/Indicators1.json
--rw-r--r--   0        0        0    16155 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json
--rw-r--r--   0        0        0     5361 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/StickAndBall.json
--rw-r--r--   0        0        0    54592 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json
--rw-r--r--   0        0        0    40558 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json
--rw-r--r--   0        0        0    52068 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json
--rw-r--r--   0        0        0    53471 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json
--rw-r--r--   0        0        0   246148 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json
--rw-r--r--   0        0        0    48292 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json
--rw-r--r--   0        0        0    35702 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json
--rw-r--r--   0        0        0     6341 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/_alarm.json
--rw-r--r--   0        0        0     9845 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/a_cup_of_coffee.json
--rw-r--r--   0        0        0    34000 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/a_mountain.json
--rw-r--r--   0        0        0     2248 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/abstract_circle.json
--rw-r--r--   0        0        0    76171 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/acrobatics.json
--rw-r--r--   0        0        0    42273 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/anubis.json
--rw-r--r--   0        0        0     2643 2023-07-24 15:51:50.551684 rlottie_python-1.1.2/rlottie/example/resource/ao.json
--rw-r--r--   0        0        0    32268 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/balloons_with_string.json
--rw-r--r--   0        0        0     5107 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/bell.json
--rw-r--r--   0        0        0     4382 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/birth_stone_logo.json
--rw-r--r--   0        0        0     8543 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/bounching_ball.json
--rw-r--r--   0        0        0    14809 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/browser.json
--rw-r--r--   0        0        0    30454 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/confetti.json
--rw-r--r--   0        0        0    14323 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/cooking.json
--rw-r--r--   0        0        0    18611 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/dna.json
--rw-r--r--   0        0        0     3790 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/done.json
--rw-r--r--   0        0        0     2352 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/dynamic_path_test.json
--rw-r--r--   0        0        0    13891 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/dynamic_property.json
--rw-r--r--   0        0        0    30573 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/eid_mubarak.json
--rw-r--r--   0        0        0    18230 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/emoji_shock.json
--rw-r--r--   0        0        0     8800 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/emoji_wink.json
--rw-r--r--   0        0        0    11372 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/file_transfer.json
--rw-r--r--   0        0        0    34388 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/fingerprint_success.json
--rw-r--r--   0        0        0    86448 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/funky_chicken.json
--rw-r--r--   0        0        0     9040 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/gears.json
--rw-r--r--   0        0        0    10251 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/gears_or_settings.json
--rw-r--r--   0        0        0    15143 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/glow_loading.json
--rw-r--r--   0        0        0     4056 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/gradient_animated_background.json
--rw-r--r--   0        0        0     4531 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/gradient_sleepy_loader.json
--rw-r--r--   0        0        0    10981 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/happy.json
--rw-r--r--   0        0        0    11403 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/heart.json
--rw-r--r--   0        0        0    16888 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/hourglass.json
--rw-r--r--   0        0        0   142760 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/image_embedded.json
--rw-r--r--   0        0        0      815 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/image_test.json
--rw-r--r--   0        0        0   101560 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/images/img_0.png
--rw-r--r--   0        0        0    28898 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/imprint.json
--rw-r--r--   0        0        0    62909 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/insta_camera.json
--rw-r--r--   0        0        0    57591 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/intelia_logo_animation.json
--rw-r--r--   0        0        0    10119 2023-07-24 15:51:50.555685 rlottie_python-1.1.2/rlottie/example/resource/it's_lunch_time!.json
--rw-r--r--   0        0        0    76453 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/jolly_walker.json
--rw-r--r--   0        0        0     2531 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/layout.edc
--rw-r--r--   0        0        0     9106 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/layout.edj
--rw-r--r--   0        0        0    12532 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/leap_frog_loader.json
--rw-r--r--   0        0        0     8074 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/like.json
--rw-r--r--   0        0        0    13208 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/loader.json
--rw-r--r--   0        0        0     3337 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/loader_4.json
--rw-r--r--   0        0        0    27260 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/loader_animation.json
--rw-r--r--   0        0        0   526177 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/loading.json
--rw-r--r--   0        0        0     5306 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/loading_.json
--rw-r--r--   0        0        0     7512 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/loading_animation.json
--rw-r--r--   0        0        0    22205 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/loading_rectangles.json
--rw-r--r--   0        0        0    57073 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json
--rw-r--r--   0        0        0    36565 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/maps.json
--rw-r--r--   0        0        0    32154 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/marker.json
--rw-r--r--   0        0        0      933 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/mask.json
--rw-r--r--   0        0        0     5944 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/material_wave_loading.json
--rw-r--r--   0        0        0     3847 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/matte_two_item_with_lowerlayer.json
--rw-r--r--   0        0        0    20602 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/mnemonics.json
--rw-r--r--   0        0        0    10147 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/movie_loading.json
--rw-r--r--   0        0        0   103828 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/mughead.json
--rw-r--r--   0        0        0    56069 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/night_own.json
--rw-r--r--   0        0        0    33525 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/ondas.json
--rw-r--r--   0        0        0    42417 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/party_penguin.json
--rw-r--r--   0        0        0   105667 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/peli-canon.json
--rw-r--r--   0        0        0    78362 2023-07-24 15:51:50.559685 rlottie_python-1.1.2/rlottie/example/resource/personal_character.json
--rw-r--r--   0        0        0     1808 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/polystar_anim.json
--rw-r--r--   0        0        0     1849 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/polystar_line_clockwise_trim.json
--rw-r--r--   0        0        0   248836 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/pumped_up.json
--rw-r--r--   0        0        0    13581 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/red_box.json
--rw-r--r--   0        0        0     9020 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/ripple_loading_animation.json
--rw-r--r--   0        0        0    12681 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/settings.json
--rw-r--r--   0        0        0    10510 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/spin,_lil_loader_v2.json
--rw-r--r--   0        0        0    28044 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/square_wheel.json
--rw-r--r--   0        0        0   180889 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/starts_transparent.json
--rw-r--r--   0        0        0     2859 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/static_dynamic_dash.json
--rw-r--r--   0        0        0     9738 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/telegram.json
--rw-r--r--   0        0        0     2192 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/test/repro_infinite_loop.json
--rw-r--r--   0        0        0     7283 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json
--rw-r--r--   0        0        0     7278 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json
--rw-r--r--   0        0        0     4427 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/test/repro_sbof.json
--rw-r--r--   0        0        0   197687 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json
--rw-r--r--   0        0        0    49302 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/tile_grid_loading_animation.json
--rw-r--r--   0        0        0   348342 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/tractor.json
--rw-r--r--   0        0        0     8099 2023-07-24 15:51:50.563685 rlottie_python-1.1.2/rlottie/example/resource/triib_manage.json
--rw-r--r--   0        0        0     7755 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/resource/waves_.json
--rw-r--r--   0        0        0    27850 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/resource/windmill.json
--rw-r--r--   0        0        0    70089 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/resource/world_locations.json
--rw-r--r--   0        0        0    24031 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/resource/worm.json
--rw-r--r--   0        0        0   202304 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/resource/you're_in!.json
--rw-r--r--   0        0        0     3952 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/uxsampletest.cpp
--rw-r--r--   0        0        0     1176 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/win32Player/Source.cpp
--rw-r--r--   0        0        0      320 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/win32Player/animation.h
--rw-r--r--   0        0        0      380 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/win32Player/framework.h
--rw-r--r--   0        0        0     1508 2023-07-24 15:51:50.567685 rlottie_python-1.1.2/rlottie/example/win32Player/resource.h
--rw-r--r--   0        0        0  2035712 2023-07-24 15:51:50.575685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottie.dll
--rw-r--r--   0        0        0    27826 2023-07-24 15:51:50.575685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottie.lib
--rw-r--r--   0        0        0    15904 2023-07-24 15:51:50.575685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.cpp
--rw-r--r--   0        0        0   244224 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.exe
--rw-r--r--   0        0        0      710 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.h
--rw-r--r--   0        0        0    46227 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.ico
--rw-r--r--   0        0        0     7298 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.rc
--rw-r--r--   0        0        0     1415 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.sln
--rw-r--r--   0        0        0     8120 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.vcxproj
--rw-r--r--   0        0        0     1884 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters
--rw-r--r--   0        0        0      165 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.vcxproj.user
--rw-r--r--   0        0        0    46227 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/small.ico
--rw-r--r--   0        0        0      307 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/example/win32Player/targetver.h
--rwxr-xr-x   0        0        0       56 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/format
--rw-r--r--   0        0        0       89 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/inc/CMakeLists.txt
--rw-r--r--   0        0        0      138 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/inc/meson.build
--rw-r--r--   0        0        0    17630 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/inc/rlottie.h
--rw-r--r--   0        0        0    11630 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/inc/rlottie_capi.h
--rw-r--r--   0        0        0     5193 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/inc/rlottiecommon.h
--rw-r--r--   0        0        0     6718 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/licenses/COPYING.FTL
--rw-r--r--   0        0        0     1053 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/licenses/COPYING.MIT
--rw-r--r--   0        0        0    16726 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/licenses/COPYING.MPL
--rw-r--r--   0        0        0     2086 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/licenses/COPYING.PIX
--rw-r--r--   0        0        0     5152 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/licenses/COPYING.RPD
--rw-r--r--   0        0        0     1507 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/licenses/COPYING.SKIA
--rw-r--r--   0        0        0     1073 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/licenses/COPYING.STB
--rw-r--r--   0        0        0     2984 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/meson.build
--rw-r--r--   0        0        0      920 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/meson_options.txt
--rw-r--r--   0        0        0       69 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/packaging/rlottie.manifest
--rw-r--r--   0        0        0     3024 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/packaging/rlottie.spec
--rw-r--r--   0        0        0      141 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/rlottie.expmap
--rw-r--r--   0        0        0      127 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/rlottie.pc.in
--rw-r--r--   0        0        0       79 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/CMakeLists.txt
--rw-r--r--   0        0        0       20 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/binding/CMakeLists.txt
--rw-r--r--   0        0        0      192 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/binding/c/CMakeLists.txt
--rw-r--r--   0        0        0    10348 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/binding/c/lottieanimation_capi.cpp
--rw-r--r--   0        0        0      267 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/binding/c/meson.build
--rw-r--r--   0        0        0       40 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/binding/meson.build
--rw-r--r--   0        0        0      564 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/CMakeLists.txt
--rw-r--r--   0        0        0    14622 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottieanimation.cpp
--rw-r--r--   0        0        0    12847 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottiefiltermodel.h
--rw-r--r--   0        0        0    45197 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottieitem.cpp
--rw-r--r--   0        0        0    19784 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottieitem.h
--rw-r--r--   0        0        0    11381 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottieitem_capi.cpp
--rw-r--r--   0        0        0     2216 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottiekeypath.cpp
--rw-r--r--   0        0        0     2097 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottiekeypath.h
--rw-r--r--   0        0        0     4889 2023-07-24 15:51:50.583685 rlottie_python-1.1.2/rlottie/src/lottie/lottieloader.cpp
--rw-r--r--   0        0        0    12452 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/lottiemodel.cpp
--rw-r--r--   0        0        0    35941 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/lottiemodel.h
--rw-r--r--   0        0        0    71912 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/lottieparser.cpp
--rw-r--r--   0        0        0        0 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/lottieproxymodel.cpp
--rw-r--r--   0        0        0      423 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/meson.build
--rw-r--r--   0        0        0    10695 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/allocators.h
--rw-r--r--   0        0        0     2281 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h
--rw-r--r--   0        0        0   121069 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/document.h
--rw-r--r--   0        0        0    10681 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/encodedstream.h
--rw-r--r--   0        0        0    29281 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/encodings.h
--rw-r--r--   0        0        0     3870 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/error/en.h
--rw-r--r--   0        0        0     6213 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/error/error.h
--rw-r--r--   0        0        0     3001 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/filereadstream.h
--rw-r--r--   0        0        0     3146 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/filewritestream.h
--rw-r--r--   0        0        0     4034 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/fwd.h
--rw-r--r--   0        0        0     9143 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/biginteger.h
--rw-r--r--   0        0        0     2066 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/clzll.h
--rw-r--r--   0        0        0    11509 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/diyfp.h
--rw-r--r--   0        0        0     8125 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/dtoa.h
--rw-r--r--   0        0        0     2994 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/ieee754.h
--rw-r--r--   0        0        0    10131 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/itoa.h
--rw-r--r--   0        0        0     6641 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/meta.h
--rw-r--r--   0        0        0     3595 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/pow10.h
--rw-r--r--   0        0        0    26141 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/regex.h
--rw-r--r--   0        0        0     7184 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/stack.h
--rw-r--r--   0        0        0     2199 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/strfunc.h
--rw-r--r--   0        0        0     8994 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/strtod.h
--rw-r--r--   0        0        0     1419 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/swap.h
--rw-r--r--   0        0        0     4082 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/istreamwrapper.h
--rw-r--r--   0        0        0     2560 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/memorybuffer.h
--rw-r--r--   0        0        0     2667 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/memorystream.h
--rw-r--r--   0        0        0     8372 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h
--rw-r--r--   0        0        0     9386 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/msinttypes/stdint.h
--rw-r--r--   0        0        0     2331 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/ostreamwrapper.h
--rw-r--r--   0        0        0    60889 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/pointer.h
--rw-r--r--   0        0        0    10539 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/prettywriter.h
--rw-r--r--   0        0        0    24161 2023-07-24 15:51:50.587685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/rapidjson.h
--rw-r--r--   0        0        0    93838 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/reader.h
--rw-r--r--   0        0        0   103633 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/schema.h
--rw-r--r--   0        0        0     6753 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/stream.h
--rw-r--r--   0        0        0     3993 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/stringbuffer.h
--rw-r--r--   0        0        0    26877 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/writer.h
--rw-r--r--   0        0        0     1862 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/meson.build
--rw-r--r--   0        0        0     1267 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/CMakeLists.txt
--rw-r--r--   0        0        0      286 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/CMakeLists.txt
--rw-r--r--   0        0        0      304 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/meson.build
--rw-r--r--   0        0        0    12132 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_math.cpp
--rw-r--r--   0        0        0    14680 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_math.h
--rw-r--r--   0        0        0    46945 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_raster.cpp
--rw-r--r--   0        0        0    39675 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_raster.h
--rw-r--r--   0        0        0    62535 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_stroker.cpp
--rw-r--r--   0        0        0    10128 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_stroker.h
--rw-r--r--   0        0        0     8325 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_types.h
--rw-r--r--   0        0        0      801 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/meson.build
--rw-r--r--   0        0        0      306 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/pixman/CMakeLists.txt
--rw-r--r--   0        0        0      310 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/pixman/meson.build
--rw-r--r--   0        0        0    19930 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/pixman/pixman-arm-neon-asm.S
--rw-r--r--   0        0        0    37637 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/pixman/pixman-arm-neon-asm.h
--rw-r--r--   0        0        0     1036 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/stb/CMakeLists.txt
--rw-r--r--   0        0        0     1028 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/stb/meson.build
--rw-r--r--   0        0        0     1355 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/stb/stb_image.cpp
--rw-r--r--   0        0        0   261660 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/stb/stb_image.h
--rw-r--r--   0        0        0     5584 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/varenaalloc.cpp
--rw-r--r--   0        0        0     8807 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/varenaalloc.h
--rw-r--r--   0        0        0     3658 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/vbezier.cpp
--rw-r--r--   0        0        0     4584 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/vbezier.h
--rw-r--r--   0        0        0     5772 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/vbitmap.cpp
--rw-r--r--   0        0        0     3630 2023-07-24 15:51:50.591685 rlottie_python-1.1.2/rlottie/src/vector/vbitmap.h
--rw-r--r--   0        0        0     2168 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vbrush.cpp
--rw-r--r--   0        0        0     2981 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vbrush.h
--rw-r--r--   0        0        0     3215 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vcowptr.h
--rw-r--r--   0        0        0     7123 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdasher.cpp
--rw-r--r--   0        0        0     2352 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdasher.h
--rw-r--r--   0        0        0    22094 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdebug.cpp
--rw-r--r--   0        0        0     5749 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdebug.h
--rw-r--r--   0        0        0     3895 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdrawable.cpp
--rw-r--r--   0        0        0     3014 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdrawable.h
--rw-r--r--   0        0        0    25053 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper.cpp
--rw-r--r--   0        0        0     7837 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper.h
--rw-r--r--   0        0        0     5615 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper_common.cpp
--rw-r--r--   0        0        0      615 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper_neon.cpp
--rw-r--r--   0        0        0     8117 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper_sse2.cpp
--rw-r--r--   0        0        0     1749 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/velapsedtimer.cpp
--rw-r--r--   0        0        0     1615 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/velapsedtimer.h
--rw-r--r--   0        0        0     8411 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vglobal.h
--rw-r--r--   0        0        0     6375 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vimageloader.cpp
--rw-r--r--   0        0        0      450 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vimageloader.h
--rw-r--r--   0        0        0     3730 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vinterpolator.cpp
--rw-r--r--   0        0        0     2680 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vinterpolator.h
--rw-r--r--   0        0        0     2996 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vline.h
--rw-r--r--   0        0        0    18367 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vmatrix.cpp
--rw-r--r--   0        0        0     4041 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vmatrix.h
--rw-r--r--   0        0        0     4841 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vpainter.cpp
--rw-r--r--   0        0        0     2422 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vpainter.h
--rw-r--r--   0        0        0    22546 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vpath.cpp
--rw-r--r--   0        0        0     9067 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vpath.h
--rw-r--r--   0        0        0     2413 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vpathmesure.cpp
--rw-r--r--   0        0        0     1586 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vpathmesure.h
--rw-r--r--   0        0        0     6289 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vpoint.h
--rw-r--r--   0        0        0    15023 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vraster.cpp
--rw-r--r--   0        0        0     1746 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vraster.h
--rw-r--r--   0        0        0     1955 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vrect.cpp
--rw-r--r--   0        0        0     5642 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vrect.h
--rw-r--r--   0        0        0    20545 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vrle.cpp
--rw-r--r--   0        0        0     4252 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vrle.h
--rw-r--r--   0        0        0     2396 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vsharedptr.h
--rw-r--r--   0        0        0     5031 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vstackallocator.h
--rw-r--r--   0        0        0     2494 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/vector/vtaskqueue.h
--rw-r--r--   0        0        0      236 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/wasm/meson.build
--rw-r--r--   0        0        0    55577 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/src/wasm/rlottiewasm.cpp
--rw-r--r--   0        0        0      904 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/CMakeLists.txt
--rw-r--r--   0        0        0     1113 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/meson.build
--rw-r--r--   0        0        0      822 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/test_lottieanimation.cpp
--rw-r--r--   0        0        0      889 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/test_lottieanimation_capi.cpp
--rw-r--r--   0        0        0     7171 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/test_vpath.cpp
--rw-r--r--   0        0        0     1149 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/test_vrect.cpp
--rw-r--r--   0        0        0      132 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/testsuite.cpp
--rw-r--r--   0        0        0     1131 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/test/wasm_test.html
--rw-r--r--   0        0        0      173 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/vs2019/config.h
--rw-r--r--   0        0        0     1434 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/vs2019/rlottie.sln
--rw-r--r--   0        0        0    13672 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/vs2019/rlottie.vcxproj
--rw-r--r--   0        0        0    15217 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/vs2019/rlottie.vcxproj.filters
--rw-r--r--   0        0        0      168 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/vs2019/rlottie.vcxproj.user
--rwxr-xr-x   0        0        0      625 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/wasm_build.sh
--rw-r--r--   0        0        0      588 2023-07-24 15:51:50.595685 rlottie_python-1.1.2/rlottie/wasm_cross.txt
--rw-r--r--   0        0        0       89 2023-07-24 15:51:48.279659 rlottie_python-1.1.2/rlottie_python/__init__.py
--rw-r--r--   0        0        0    23384 2023-07-24 15:51:48.279659 rlottie_python-1.1.2/rlottie_python/rlottie_wrapper.py
--rw-r--r--   0        0        0     4004 2023-07-24 15:51:48.279659 rlottie_python-1.1.2/rlottie_python/rlottiecommon.py
--rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 rlottie_python-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      447 2023-07-25 04:24:02.129842 rlottie_python-1.1.3/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2023-07-25 04:24:02.129842 rlottie_python-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4107 2023-07-25 04:24:02.129842 rlottie_python-1.1.3/README.md
+-rw-r--r--   0        0        0     1538 2023-07-25 04:24:02.129842 rlottie_python-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/AUTHORS
+-rw-r--r--   0        0        0     6246 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/CMakeLists.txt
+-rw-r--r--   0        0        0      690 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/COPYING
+-rw-r--r--   0        0        0    10977 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/README.md
+-rwxr-xr-x   0        0        0      317 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/arm_build.sh
+-rw-r--r--   0        0        0      320 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/arm_cross.txt
+-rw-r--r--   0        0        0      322 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/cmake/config.h.in
+-rw-r--r--   0        0        0      546 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/cmake/rlottieConfig.cmake.in
+-rw-r--r--   0        0        0      474 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/CMakeLists.txt
+-rw-r--r--   0        0        0     9226 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/demo.cpp
+-rw-r--r--   0        0        0     2650 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/demo_marker.cpp
+-rw-r--r--   0        0        0     4158 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/evasapp.cpp
+-rw-r--r--   0        0        0     2957 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/evasapp.h
+-rw-r--r--   0        0        0    27371 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/gif.h
+-rw-r--r--   0        0        0     4908 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/lottie2gif.cpp
+-rw-r--r--   0        0        0     4938 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/lottieperf.cpp
+-rw-r--r--   0        0        0     5676 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/lottieview.cpp
+-rw-r--r--   0        0        0    14747 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/lottieview.h
+-rw-r--r--   0        0        0     7405 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/lottieviewer.cpp
+-rw-r--r--   0        0        0     5437 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/lottieviewtest.cpp
+-rw-r--r--   0        0        0     2107 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/meson.build
+-rw-r--r--   0        0        0     3620 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/pathtest.cpp
+-rw-r--r--   0        0        0    27806 2023-07-25 04:24:04.441877 rlottie_python-1.1.3/rlottie/example/resource/1643-exploding-star.json
+-rw-r--r--   0        0        0    11654 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/1667-firework.json
+-rw-r--r--   0        0        0    43105 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json
+-rw-r--r--   0        0        0   154297 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/29056-nepenthe-illustration.json
+-rw-r--r--   0        0        0    10221 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/360º_degree.json
+-rw-r--r--   0        0        0     2536 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/3d.json
+-rw-r--r--   0        0        0    19081 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/4479-fireworks.json
+-rw-r--r--   0        0        0     9299 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/5317-fireworkds.json
+-rw-r--r--   0        0        0   138526 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/5344-honey-sack-hud.json
+-rw-r--r--   0        0        0    16809 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/Indicators1.json
+-rw-r--r--   0        0        0    16155 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json
+-rw-r--r--   0        0        0     5361 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/StickAndBall.json
+-rw-r--r--   0        0        0    54592 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json
+-rw-r--r--   0        0        0    40558 2023-07-25 04:24:04.445877 rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json
+-rw-r--r--   0        0        0    52068 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json
+-rw-r--r--   0        0        0    53471 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json
+-rw-r--r--   0        0        0   246148 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json
+-rw-r--r--   0        0        0    48292 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json
+-rw-r--r--   0        0        0    35702 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json
+-rw-r--r--   0        0        0     6341 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/_alarm.json
+-rw-r--r--   0        0        0     9845 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/a_cup_of_coffee.json
+-rw-r--r--   0        0        0    34000 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/a_mountain.json
+-rw-r--r--   0        0        0     2248 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/abstract_circle.json
+-rw-r--r--   0        0        0    76171 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/acrobatics.json
+-rw-r--r--   0        0        0    42273 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/anubis.json
+-rw-r--r--   0        0        0     2643 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/ao.json
+-rw-r--r--   0        0        0    32268 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/balloons_with_string.json
+-rw-r--r--   0        0        0     5107 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/bell.json
+-rw-r--r--   0        0        0     4382 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/birth_stone_logo.json
+-rw-r--r--   0        0        0     8543 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/bounching_ball.json
+-rw-r--r--   0        0        0    14809 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/browser.json
+-rw-r--r--   0        0        0    30454 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/confetti.json
+-rw-r--r--   0        0        0    14323 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/cooking.json
+-rw-r--r--   0        0        0    18611 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/dna.json
+-rw-r--r--   0        0        0     3790 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/done.json
+-rw-r--r--   0        0        0     2352 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/dynamic_path_test.json
+-rw-r--r--   0        0        0    13891 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/dynamic_property.json
+-rw-r--r--   0        0        0    30573 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/eid_mubarak.json
+-rw-r--r--   0        0        0    18230 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/emoji_shock.json
+-rw-r--r--   0        0        0     8800 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/emoji_wink.json
+-rw-r--r--   0        0        0    11372 2023-07-25 04:24:04.449877 rlottie_python-1.1.3/rlottie/example/resource/file_transfer.json
+-rw-r--r--   0        0        0    34388 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/fingerprint_success.json
+-rw-r--r--   0        0        0    86448 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/funky_chicken.json
+-rw-r--r--   0        0        0     9040 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/gears.json
+-rw-r--r--   0        0        0    10251 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/gears_or_settings.json
+-rw-r--r--   0        0        0    15143 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/glow_loading.json
+-rw-r--r--   0        0        0     4056 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/gradient_animated_background.json
+-rw-r--r--   0        0        0     4531 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/gradient_sleepy_loader.json
+-rw-r--r--   0        0        0    10981 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/happy.json
+-rw-r--r--   0        0        0    11403 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/heart.json
+-rw-r--r--   0        0        0    16888 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/hourglass.json
+-rw-r--r--   0        0        0   142760 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/image_embedded.json
+-rw-r--r--   0        0        0      815 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/image_test.json
+-rw-r--r--   0        0        0   101560 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/images/img_0.png
+-rw-r--r--   0        0        0    28898 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/imprint.json
+-rw-r--r--   0        0        0    62909 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/insta_camera.json
+-rw-r--r--   0        0        0    57591 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/intelia_logo_animation.json
+-rw-r--r--   0        0        0    10119 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/it's_lunch_time!.json
+-rw-r--r--   0        0        0    76453 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/jolly_walker.json
+-rw-r--r--   0        0        0     2531 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/layout.edc
+-rw-r--r--   0        0        0     9106 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/layout.edj
+-rw-r--r--   0        0        0    12532 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/leap_frog_loader.json
+-rw-r--r--   0        0        0     8074 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/like.json
+-rw-r--r--   0        0        0    13208 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/loader.json
+-rw-r--r--   0        0        0     3337 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/loader_4.json
+-rw-r--r--   0        0        0    27260 2023-07-25 04:24:04.453877 rlottie_python-1.1.3/rlottie/example/resource/loader_animation.json
+-rw-r--r--   0        0        0   526177 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/loading.json
+-rw-r--r--   0        0        0     5306 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/loading_.json
+-rw-r--r--   0        0        0     7512 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/loading_animation.json
+-rw-r--r--   0        0        0    22205 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/loading_rectangles.json
+-rw-r--r--   0        0        0    57073 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json
+-rw-r--r--   0        0        0    36565 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/maps.json
+-rw-r--r--   0        0        0    32154 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/marker.json
+-rw-r--r--   0        0        0      933 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/mask.json
+-rw-r--r--   0        0        0     5944 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/material_wave_loading.json
+-rw-r--r--   0        0        0     3847 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/matte_two_item_with_lowerlayer.json
+-rw-r--r--   0        0        0    20602 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/mnemonics.json
+-rw-r--r--   0        0        0    10147 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/movie_loading.json
+-rw-r--r--   0        0        0   103828 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/mughead.json
+-rw-r--r--   0        0        0    56069 2023-07-25 04:24:04.457877 rlottie_python-1.1.3/rlottie/example/resource/night_own.json
+-rw-r--r--   0        0        0    33525 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/ondas.json
+-rw-r--r--   0        0        0    42417 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/party_penguin.json
+-rw-r--r--   0        0        0   105667 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/peli-canon.json
+-rw-r--r--   0        0        0    78362 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/personal_character.json
+-rw-r--r--   0        0        0     1808 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/polystar_anim.json
+-rw-r--r--   0        0        0     1849 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/polystar_line_clockwise_trim.json
+-rw-r--r--   0        0        0   248836 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/pumped_up.json
+-rw-r--r--   0        0        0    13581 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/red_box.json
+-rw-r--r--   0        0        0     9020 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/ripple_loading_animation.json
+-rw-r--r--   0        0        0    12681 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/settings.json
+-rw-r--r--   0        0        0    10510 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/spin,_lil_loader_v2.json
+-rw-r--r--   0        0        0    28044 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/square_wheel.json
+-rw-r--r--   0        0        0   180889 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/starts_transparent.json
+-rw-r--r--   0        0        0     2859 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/static_dynamic_dash.json
+-rw-r--r--   0        0        0     9738 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/telegram.json
+-rw-r--r--   0        0        0     2192 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/test/repro_infinite_loop.json
+-rw-r--r--   0        0        0     7283 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json
+-rw-r--r--   0        0        0     7278 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json
+-rw-r--r--   0        0        0     4427 2023-07-25 04:24:04.461877 rlottie_python-1.1.3/rlottie/example/resource/test/repro_sbof.json
+-rw-r--r--   0        0        0   197687 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json
+-rw-r--r--   0        0        0    49302 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/tile_grid_loading_animation.json
+-rw-r--r--   0        0        0   348342 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/tractor.json
+-rw-r--r--   0        0        0     8099 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/triib_manage.json
+-rw-r--r--   0        0        0     7755 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/waves_.json
+-rw-r--r--   0        0        0    27850 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/windmill.json
+-rw-r--r--   0        0        0    70089 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/world_locations.json
+-rw-r--r--   0        0        0    24031 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/worm.json
+-rw-r--r--   0        0        0   202304 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/resource/you're_in!.json
+-rw-r--r--   0        0        0     3952 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/uxsampletest.cpp
+-rw-r--r--   0        0        0     1176 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/win32Player/Source.cpp
+-rw-r--r--   0        0        0      320 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/win32Player/animation.h
+-rw-r--r--   0        0        0      380 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/win32Player/framework.h
+-rw-r--r--   0        0        0     1508 2023-07-25 04:24:04.465877 rlottie_python-1.1.3/rlottie/example/win32Player/resource.h
+-rw-r--r--   0        0        0  2035712 2023-07-25 04:24:04.477877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottie.dll
+-rw-r--r--   0        0        0    27826 2023-07-25 04:24:04.477877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottie.lib
+-rw-r--r--   0        0        0    15904 2023-07-25 04:24:04.477877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.cpp
+-rw-r--r--   0        0        0   244224 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.exe
+-rw-r--r--   0        0        0      710 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.h
+-rw-r--r--   0        0        0    46227 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.ico
+-rw-r--r--   0        0        0     7298 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.rc
+-rw-r--r--   0        0        0     1415 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.sln
+-rw-r--r--   0        0        0     8120 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.vcxproj
+-rw-r--r--   0        0        0     1884 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters
+-rw-r--r--   0        0        0      165 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.vcxproj.user
+-rw-r--r--   0        0        0    46227 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/small.ico
+-rw-r--r--   0        0        0      307 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/example/win32Player/targetver.h
+-rwxr-xr-x   0        0        0       56 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/format
+-rw-r--r--   0        0        0       89 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/inc/CMakeLists.txt
+-rw-r--r--   0        0        0      138 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/inc/meson.build
+-rw-r--r--   0        0        0    17630 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/inc/rlottie.h
+-rw-r--r--   0        0        0    11630 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/inc/rlottie_capi.h
+-rw-r--r--   0        0        0     5193 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/inc/rlottiecommon.h
+-rw-r--r--   0        0        0     6718 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/licenses/COPYING.FTL
+-rw-r--r--   0        0        0     1053 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/licenses/COPYING.MIT
+-rw-r--r--   0        0        0    16726 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/licenses/COPYING.MPL
+-rw-r--r--   0        0        0     2086 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/licenses/COPYING.PIX
+-rw-r--r--   0        0        0     5152 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/licenses/COPYING.RPD
+-rw-r--r--   0        0        0     1507 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/licenses/COPYING.SKIA
+-rw-r--r--   0        0        0     1073 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/licenses/COPYING.STB
+-rw-r--r--   0        0        0     2984 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/meson.build
+-rw-r--r--   0        0        0      920 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/meson_options.txt
+-rw-r--r--   0        0        0       69 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/packaging/rlottie.manifest
+-rw-r--r--   0        0        0     3024 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/packaging/rlottie.spec
+-rw-r--r--   0        0        0      141 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/rlottie.expmap
+-rw-r--r--   0        0        0      127 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/rlottie.pc.in
+-rw-r--r--   0        0        0       79 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/CMakeLists.txt
+-rw-r--r--   0        0        0       20 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/binding/CMakeLists.txt
+-rw-r--r--   0        0        0      192 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/binding/c/CMakeLists.txt
+-rw-r--r--   0        0        0    10348 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/binding/c/lottieanimation_capi.cpp
+-rw-r--r--   0        0        0      267 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/binding/c/meson.build
+-rw-r--r--   0        0        0       40 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/binding/meson.build
+-rw-r--r--   0        0        0      564 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/CMakeLists.txt
+-rw-r--r--   0        0        0    14622 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottieanimation.cpp
+-rw-r--r--   0        0        0    12847 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottiefiltermodel.h
+-rw-r--r--   0        0        0    45197 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottieitem.cpp
+-rw-r--r--   0        0        0    19784 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottieitem.h
+-rw-r--r--   0        0        0    11381 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottieitem_capi.cpp
+-rw-r--r--   0        0        0     2216 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottiekeypath.cpp
+-rw-r--r--   0        0        0     2097 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottiekeypath.h
+-rw-r--r--   0        0        0     4889 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottieloader.cpp
+-rw-r--r--   0        0        0    12452 2023-07-25 04:24:04.489877 rlottie_python-1.1.3/rlottie/src/lottie/lottiemodel.cpp
+-rw-r--r--   0        0        0    35941 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/lottiemodel.h
+-rw-r--r--   0        0        0    71912 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/lottieparser.cpp
+-rw-r--r--   0        0        0        0 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/lottieproxymodel.cpp
+-rw-r--r--   0        0        0      423 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/meson.build
+-rw-r--r--   0        0        0    10695 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/allocators.h
+-rw-r--r--   0        0        0     2281 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h
+-rw-r--r--   0        0        0   121069 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/document.h
+-rw-r--r--   0        0        0    10681 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/encodedstream.h
+-rw-r--r--   0        0        0    29281 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/encodings.h
+-rw-r--r--   0        0        0     3870 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/error/en.h
+-rw-r--r--   0        0        0     6213 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/error/error.h
+-rw-r--r--   0        0        0     3001 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/filereadstream.h
+-rw-r--r--   0        0        0     3146 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/filewritestream.h
+-rw-r--r--   0        0        0     4034 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/fwd.h
+-rw-r--r--   0        0        0     9143 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/biginteger.h
+-rw-r--r--   0        0        0     2066 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/clzll.h
+-rw-r--r--   0        0        0    11509 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/diyfp.h
+-rw-r--r--   0        0        0     8125 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/dtoa.h
+-rw-r--r--   0        0        0     2994 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/ieee754.h
+-rw-r--r--   0        0        0    10131 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/itoa.h
+-rw-r--r--   0        0        0     6641 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/meta.h
+-rw-r--r--   0        0        0     3595 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/pow10.h
+-rw-r--r--   0        0        0    26141 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/regex.h
+-rw-r--r--   0        0        0     7184 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/stack.h
+-rw-r--r--   0        0        0     2199 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/strfunc.h
+-rw-r--r--   0        0        0     8994 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/strtod.h
+-rw-r--r--   0        0        0     1419 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/swap.h
+-rw-r--r--   0        0        0     4082 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/istreamwrapper.h
+-rw-r--r--   0        0        0     2560 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/memorybuffer.h
+-rw-r--r--   0        0        0     2667 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/memorystream.h
+-rw-r--r--   0        0        0     8372 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h
+-rw-r--r--   0        0        0     9386 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/msinttypes/stdint.h
+-rw-r--r--   0        0        0     2331 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/ostreamwrapper.h
+-rw-r--r--   0        0        0    60889 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/pointer.h
+-rw-r--r--   0        0        0    10539 2023-07-25 04:24:04.493878 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/prettywriter.h
+-rw-r--r--   0        0        0    24161 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/rapidjson.h
+-rw-r--r--   0        0        0    93838 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/reader.h
+-rw-r--r--   0        0        0   103633 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/schema.h
+-rw-r--r--   0        0        0     6753 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/stream.h
+-rw-r--r--   0        0        0     3993 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/stringbuffer.h
+-rw-r--r--   0        0        0    26877 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/writer.h
+-rw-r--r--   0        0        0     1862 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/meson.build
+-rw-r--r--   0        0        0     1267 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/CMakeLists.txt
+-rw-r--r--   0        0        0      286 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/CMakeLists.txt
+-rw-r--r--   0        0        0      304 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/meson.build
+-rw-r--r--   0        0        0    12132 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_math.cpp
+-rw-r--r--   0        0        0    14680 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_math.h
+-rw-r--r--   0        0        0    46945 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_raster.cpp
+-rw-r--r--   0        0        0    39675 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_raster.h
+-rw-r--r--   0        0        0    62535 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_stroker.cpp
+-rw-r--r--   0        0        0    10128 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_stroker.h
+-rw-r--r--   0        0        0     8325 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_types.h
+-rw-r--r--   0        0        0      801 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/meson.build
+-rw-r--r--   0        0        0      306 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/pixman/CMakeLists.txt
+-rw-r--r--   0        0        0      310 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/pixman/meson.build
+-rw-r--r--   0        0        0    19930 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.S
+-rw-r--r--   0        0        0    37637 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.h
+-rw-r--r--   0        0        0     1036 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/stb/CMakeLists.txt
+-rw-r--r--   0        0        0     1028 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/stb/meson.build
+-rw-r--r--   0        0        0     1355 2023-07-25 04:24:04.497877 rlottie_python-1.1.3/rlottie/src/vector/stb/stb_image.cpp
+-rw-r--r--   0        0        0   261660 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/stb/stb_image.h
+-rw-r--r--   0        0        0     5584 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/varenaalloc.cpp
+-rw-r--r--   0        0        0     8807 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/varenaalloc.h
+-rw-r--r--   0        0        0     3658 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vbezier.cpp
+-rw-r--r--   0        0        0     4584 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vbezier.h
+-rw-r--r--   0        0        0     5772 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vbitmap.cpp
+-rw-r--r--   0        0        0     3630 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vbitmap.h
+-rw-r--r--   0        0        0     2168 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vbrush.cpp
+-rw-r--r--   0        0        0     2981 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vbrush.h
+-rw-r--r--   0        0        0     3215 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vcowptr.h
+-rw-r--r--   0        0        0     7123 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdasher.cpp
+-rw-r--r--   0        0        0     2352 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdasher.h
+-rw-r--r--   0        0        0    22094 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdebug.cpp
+-rw-r--r--   0        0        0     5749 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdebug.h
+-rw-r--r--   0        0        0     3895 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdrawable.cpp
+-rw-r--r--   0        0        0     3014 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdrawable.h
+-rw-r--r--   0        0        0    25053 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper.cpp
+-rw-r--r--   0        0        0     7837 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper.h
+-rw-r--r--   0        0        0     5615 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper_common.cpp
+-rw-r--r--   0        0        0      615 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper_neon.cpp
+-rw-r--r--   0        0        0     8117 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper_sse2.cpp
+-rw-r--r--   0        0        0     1749 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/velapsedtimer.cpp
+-rw-r--r--   0        0        0     1615 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/velapsedtimer.h
+-rw-r--r--   0        0        0     8411 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vglobal.h
+-rw-r--r--   0        0        0     6375 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vimageloader.cpp
+-rw-r--r--   0        0        0      450 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vimageloader.h
+-rw-r--r--   0        0        0     3730 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vinterpolator.cpp
+-rw-r--r--   0        0        0     2680 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vinterpolator.h
+-rw-r--r--   0        0        0     2996 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vline.h
+-rw-r--r--   0        0        0    18367 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vmatrix.cpp
+-rw-r--r--   0        0        0     4041 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vmatrix.h
+-rw-r--r--   0        0        0     4841 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vpainter.cpp
+-rw-r--r--   0        0        0     2422 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vpainter.h
+-rw-r--r--   0        0        0    22546 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vpath.cpp
+-rw-r--r--   0        0        0     9067 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vpath.h
+-rw-r--r--   0        0        0     2413 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vpathmesure.cpp
+-rw-r--r--   0        0        0     1586 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vpathmesure.h
+-rw-r--r--   0        0        0     6289 2023-07-25 04:24:04.501878 rlottie_python-1.1.3/rlottie/src/vector/vpoint.h
+-rw-r--r--   0        0        0    15023 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vraster.cpp
+-rw-r--r--   0        0        0     1746 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vraster.h
+-rw-r--r--   0        0        0     1955 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vrect.cpp
+-rw-r--r--   0        0        0     5642 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vrect.h
+-rw-r--r--   0        0        0    20545 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vrle.cpp
+-rw-r--r--   0        0        0     4252 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vrle.h
+-rw-r--r--   0        0        0     2396 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vsharedptr.h
+-rw-r--r--   0        0        0     5031 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vstackallocator.h
+-rw-r--r--   0        0        0     2494 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/vector/vtaskqueue.h
+-rw-r--r--   0        0        0      236 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/wasm/meson.build
+-rw-r--r--   0        0        0    55577 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/src/wasm/rlottiewasm.cpp
+-rw-r--r--   0        0        0      904 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/CMakeLists.txt
+-rw-r--r--   0        0        0     1113 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/meson.build
+-rw-r--r--   0        0        0      822 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/test_lottieanimation.cpp
+-rw-r--r--   0        0        0      889 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/test_lottieanimation_capi.cpp
+-rw-r--r--   0        0        0     7171 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/test_vpath.cpp
+-rw-r--r--   0        0        0     1149 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/test_vrect.cpp
+-rw-r--r--   0        0        0      132 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/testsuite.cpp
+-rw-r--r--   0        0        0     1131 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/test/wasm_test.html
+-rw-r--r--   0        0        0      173 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/vs2019/config.h
+-rw-r--r--   0        0        0     1434 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/vs2019/rlottie.sln
+-rw-r--r--   0        0        0    13672 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/vs2019/rlottie.vcxproj
+-rw-r--r--   0        0        0    15217 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/vs2019/rlottie.vcxproj.filters
+-rw-r--r--   0        0        0      168 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/vs2019/rlottie.vcxproj.user
+-rwxr-xr-x   0        0        0      625 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/wasm_build.sh
+-rw-r--r--   0        0        0      588 2023-07-25 04:24:04.505878 rlottie_python-1.1.3/rlottie/wasm_cross.txt
+-rw-r--r--   0        0        0       89 2023-07-25 04:24:02.129842 rlottie_python-1.1.3/rlottie_python/__init__.py
+-rw-r--r--   0        0        0    23384 2023-07-25 04:24:02.129842 rlottie_python-1.1.3/rlottie_python/rlottie_wrapper.py
+-rw-r--r--   0        0        0     4004 2023-07-25 04:24:02.129842 rlottie_python-1.1.3/rlottie_python/rlottiecommon.py
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 rlottie_python-1.1.3/PKG-INFO
```

### Comparing `rlottie_python-1.1.2/LICENSE` & `rlottie_python-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/README.md` & `rlottie_python-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/AUTHORS` & `rlottie_python-1.1.3/rlottie/AUTHORS`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/CMakeLists.txt` & `rlottie_python-1.1.3/rlottie/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/COPYING` & `rlottie_python-1.1.3/rlottie/COPYING`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/README.md` & `rlottie_python-1.1.3/rlottie/README.md`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/cmake/rlottieConfig.cmake.in` & `rlottie_python-1.1.3/rlottie/cmake/rlottieConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/demo.cpp` & `rlottie_python-1.1.3/rlottie/example/demo.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/demo_marker.cpp` & `rlottie_python-1.1.3/rlottie/example/demo_marker.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/evasapp.cpp` & `rlottie_python-1.1.3/rlottie/example/evasapp.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/evasapp.h` & `rlottie_python-1.1.3/rlottie/example/evasapp.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/gif.h` & `rlottie_python-1.1.3/rlottie/example/gif.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/lottie2gif.cpp` & `rlottie_python-1.1.3/rlottie/example/lottie2gif.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/lottieperf.cpp` & `rlottie_python-1.1.3/rlottie/example/lottieperf.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/lottieview.cpp` & `rlottie_python-1.1.3/rlottie/example/lottieview.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/lottieview.h` & `rlottie_python-1.1.3/rlottie/example/lottieview.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/lottieviewer.cpp` & `rlottie_python-1.1.3/rlottie/example/lottieviewer.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/lottieviewtest.cpp` & `rlottie_python-1.1.3/rlottie/example/lottieviewtest.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/meson.build` & `rlottie_python-1.1.3/rlottie/example/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/pathtest.cpp` & `rlottie_python-1.1.3/rlottie/example/pathtest.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/1643-exploding-star.json` & `rlottie_python-1.1.3/rlottie/example/resource/1643-exploding-star.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/1667-firework.json` & `rlottie_python-1.1.3/rlottie/example/resource/1667-firework.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json` & `rlottie_python-1.1.3/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/29056-nepenthe-illustration.json` & `rlottie_python-1.1.3/rlottie/example/resource/29056-nepenthe-illustration.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/360º_degree.json` & `rlottie_python-1.1.3/rlottie/example/resource/360º_degree.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/3d.json` & `rlottie_python-1.1.3/rlottie/example/resource/3d.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/4479-fireworks.json` & `rlottie_python-1.1.3/rlottie/example/resource/4479-fireworks.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/5317-fireworkds.json` & `rlottie_python-1.1.3/rlottie/example/resource/5317-fireworkds.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/5344-honey-sack-hud.json` & `rlottie_python-1.1.3/rlottie/example/resource/5344-honey-sack-hud.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/Indicators1.json` & `rlottie_python-1.1.3/rlottie/example/resource/Indicators1.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json` & `rlottie_python-1.1.3/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/StickAndBall.json` & `rlottie_python-1.1.3/rlottie/example/resource/StickAndBall.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json` & `rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json` & `rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json` & `rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json` & `rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json` & `rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json` & `rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json` & `rlottie_python-1.1.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/_alarm.json` & `rlottie_python-1.1.3/rlottie/example/resource/_alarm.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/a_cup_of_coffee.json` & `rlottie_python-1.1.3/rlottie/example/resource/a_cup_of_coffee.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/a_mountain.json` & `rlottie_python-1.1.3/rlottie/example/resource/a_mountain.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/abstract_circle.json` & `rlottie_python-1.1.3/rlottie/example/resource/abstract_circle.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/acrobatics.json` & `rlottie_python-1.1.3/rlottie/example/resource/acrobatics.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/anubis.json` & `rlottie_python-1.1.3/rlottie/example/resource/anubis.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/ao.json` & `rlottie_python-1.1.3/rlottie/example/resource/ao.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/balloons_with_string.json` & `rlottie_python-1.1.3/rlottie/example/resource/balloons_with_string.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/bell.json` & `rlottie_python-1.1.3/rlottie/example/resource/bell.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/birth_stone_logo.json` & `rlottie_python-1.1.3/rlottie/example/resource/birth_stone_logo.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/bounching_ball.json` & `rlottie_python-1.1.3/rlottie/example/resource/bounching_ball.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/browser.json` & `rlottie_python-1.1.3/rlottie/example/resource/browser.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/confetti.json` & `rlottie_python-1.1.3/rlottie/example/resource/confetti.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/cooking.json` & `rlottie_python-1.1.3/rlottie/example/resource/cooking.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/dna.json` & `rlottie_python-1.1.3/rlottie/example/resource/dna.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/done.json` & `rlottie_python-1.1.3/rlottie/example/resource/done.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/dynamic_path_test.json` & `rlottie_python-1.1.3/rlottie/example/resource/dynamic_path_test.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/dynamic_property.json` & `rlottie_python-1.1.3/rlottie/example/resource/dynamic_property.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/eid_mubarak.json` & `rlottie_python-1.1.3/rlottie/example/resource/eid_mubarak.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/emoji_shock.json` & `rlottie_python-1.1.3/rlottie/example/resource/emoji_shock.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/emoji_wink.json` & `rlottie_python-1.1.3/rlottie/example/resource/emoji_wink.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/file_transfer.json` & `rlottie_python-1.1.3/rlottie/example/resource/file_transfer.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/fingerprint_success.json` & `rlottie_python-1.1.3/rlottie/example/resource/fingerprint_success.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/funky_chicken.json` & `rlottie_python-1.1.3/rlottie/example/resource/funky_chicken.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/gears.json` & `rlottie_python-1.1.3/rlottie/example/resource/gears.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/gears_or_settings.json` & `rlottie_python-1.1.3/rlottie/example/resource/gears_or_settings.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/glow_loading.json` & `rlottie_python-1.1.3/rlottie/example/resource/glow_loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/gradient_animated_background.json` & `rlottie_python-1.1.3/rlottie/example/resource/gradient_animated_background.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/gradient_sleepy_loader.json` & `rlottie_python-1.1.3/rlottie/example/resource/gradient_sleepy_loader.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/happy.json` & `rlottie_python-1.1.3/rlottie/example/resource/happy.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/heart.json` & `rlottie_python-1.1.3/rlottie/example/resource/heart.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/hourglass.json` & `rlottie_python-1.1.3/rlottie/example/resource/hourglass.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/image_embedded.json` & `rlottie_python-1.1.3/rlottie/example/resource/image_embedded.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/image_test.json` & `rlottie_python-1.1.3/rlottie/example/resource/image_test.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/images/img_0.png` & `rlottie_python-1.1.3/rlottie/example/resource/images/img_0.png`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/imprint.json` & `rlottie_python-1.1.3/rlottie/example/resource/imprint.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/insta_camera.json` & `rlottie_python-1.1.3/rlottie/example/resource/insta_camera.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/intelia_logo_animation.json` & `rlottie_python-1.1.3/rlottie/example/resource/intelia_logo_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/it's_lunch_time!.json` & `rlottie_python-1.1.3/rlottie/example/resource/it's_lunch_time!.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/jolly_walker.json` & `rlottie_python-1.1.3/rlottie/example/resource/jolly_walker.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/layout.edc` & `rlottie_python-1.1.3/rlottie/example/resource/layout.edc`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/layout.edj` & `rlottie_python-1.1.3/rlottie/example/resource/layout.edj`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/leap_frog_loader.json` & `rlottie_python-1.1.3/rlottie/example/resource/leap_frog_loader.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/like.json` & `rlottie_python-1.1.3/rlottie/example/resource/like.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/loader.json` & `rlottie_python-1.1.3/rlottie/example/resource/loader.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/loader_4.json` & `rlottie_python-1.1.3/rlottie/example/resource/loader_4.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/loader_animation.json` & `rlottie_python-1.1.3/rlottie/example/resource/loader_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/loading.json` & `rlottie_python-1.1.3/rlottie/example/resource/loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/loading_.json` & `rlottie_python-1.1.3/rlottie/example/resource/loading_.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/loading_animation.json` & `rlottie_python-1.1.3/rlottie/example/resource/loading_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/loading_rectangles.json` & `rlottie_python-1.1.3/rlottie/example/resource/loading_rectangles.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json` & `rlottie_python-1.1.3/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/maps.json` & `rlottie_python-1.1.3/rlottie/example/resource/maps.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/marker.json` & `rlottie_python-1.1.3/rlottie/example/resource/marker.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/mask.json` & `rlottie_python-1.1.3/rlottie/example/resource/mask.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/material_wave_loading.json` & `rlottie_python-1.1.3/rlottie/example/resource/material_wave_loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/matte_two_item_with_lowerlayer.json` & `rlottie_python-1.1.3/rlottie/example/resource/matte_two_item_with_lowerlayer.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/mnemonics.json` & `rlottie_python-1.1.3/rlottie/example/resource/mnemonics.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/movie_loading.json` & `rlottie_python-1.1.3/rlottie/example/resource/movie_loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/mughead.json` & `rlottie_python-1.1.3/rlottie/example/resource/mughead.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/night_own.json` & `rlottie_python-1.1.3/rlottie/example/resource/night_own.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/ondas.json` & `rlottie_python-1.1.3/rlottie/example/resource/ondas.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/party_penguin.json` & `rlottie_python-1.1.3/rlottie/example/resource/party_penguin.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/peli-canon.json` & `rlottie_python-1.1.3/rlottie/example/resource/peli-canon.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/personal_character.json` & `rlottie_python-1.1.3/rlottie/example/resource/personal_character.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/polystar_anim.json` & `rlottie_python-1.1.3/rlottie/example/resource/polystar_anim.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/polystar_line_clockwise_trim.json` & `rlottie_python-1.1.3/rlottie/example/resource/polystar_line_clockwise_trim.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/pumped_up.json` & `rlottie_python-1.1.3/rlottie/example/resource/pumped_up.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/red_box.json` & `rlottie_python-1.1.3/rlottie/example/resource/red_box.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/ripple_loading_animation.json` & `rlottie_python-1.1.3/rlottie/example/resource/ripple_loading_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/settings.json` & `rlottie_python-1.1.3/rlottie/example/resource/settings.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/spin,_lil_loader_v2.json` & `rlottie_python-1.1.3/rlottie/example/resource/spin,_lil_loader_v2.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/square_wheel.json` & `rlottie_python-1.1.3/rlottie/example/resource/square_wheel.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/starts_transparent.json` & `rlottie_python-1.1.3/rlottie/example/resource/starts_transparent.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/static_dynamic_dash.json` & `rlottie_python-1.1.3/rlottie/example/resource/static_dynamic_dash.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/telegram.json` & `rlottie_python-1.1.3/rlottie/example/resource/telegram.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/test/repro_infinite_loop.json` & `rlottie_python-1.1.3/rlottie/example/resource/test/repro_infinite_loop.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json` & `rlottie_python-1.1.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json` & `rlottie_python-1.1.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/test/repro_sbof.json` & `rlottie_python-1.1.3/rlottie/example/resource/test/repro_sbof.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json` & `rlottie_python-1.1.3/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/tile_grid_loading_animation.json` & `rlottie_python-1.1.3/rlottie/example/resource/tile_grid_loading_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/tractor.json` & `rlottie_python-1.1.3/rlottie/example/resource/tractor.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/triib_manage.json` & `rlottie_python-1.1.3/rlottie/example/resource/triib_manage.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/waves_.json` & `rlottie_python-1.1.3/rlottie/example/resource/waves_.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/windmill.json` & `rlottie_python-1.1.3/rlottie/example/resource/windmill.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/world_locations.json` & `rlottie_python-1.1.3/rlottie/example/resource/world_locations.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/worm.json` & `rlottie_python-1.1.3/rlottie/example/resource/worm.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/resource/you're_in!.json` & `rlottie_python-1.1.3/rlottie/example/resource/you're_in!.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/uxsampletest.cpp` & `rlottie_python-1.1.3/rlottie/example/uxsampletest.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/Source.cpp` & `rlottie_python-1.1.3/rlottie/example/win32Player/Source.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/resource.h` & `rlottie_python-1.1.3/rlottie/example/win32Player/resource.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottie.dll` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottie.dll`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottie.lib` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottie.lib`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.cpp` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.exe` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.exe`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.h` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.ico` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.ico`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.rc` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.rc`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.sln` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.sln`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.vcxproj` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.vcxproj`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters` & `rlottie_python-1.1.3/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/example/win32Player/small.ico` & `rlottie_python-1.1.3/rlottie/example/win32Player/small.ico`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/inc/rlottie.h` & `rlottie_python-1.1.3/rlottie/inc/rlottie.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/inc/rlottie_capi.h` & `rlottie_python-1.1.3/rlottie/inc/rlottie_capi.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/inc/rlottiecommon.h` & `rlottie_python-1.1.3/rlottie/inc/rlottiecommon.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/licenses/COPYING.FTL` & `rlottie_python-1.1.3/rlottie/licenses/COPYING.FTL`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/licenses/COPYING.MIT` & `rlottie_python-1.1.3/rlottie/licenses/COPYING.MIT`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/licenses/COPYING.MPL` & `rlottie_python-1.1.3/rlottie/licenses/COPYING.MPL`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/licenses/COPYING.PIX` & `rlottie_python-1.1.3/rlottie/licenses/COPYING.PIX`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/licenses/COPYING.RPD` & `rlottie_python-1.1.3/rlottie/licenses/COPYING.RPD`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/licenses/COPYING.SKIA` & `rlottie_python-1.1.3/rlottie/licenses/COPYING.SKIA`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/licenses/COPYING.STB` & `rlottie_python-1.1.3/rlottie/licenses/COPYING.STB`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/meson.build` & `rlottie_python-1.1.3/rlottie/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/meson_options.txt` & `rlottie_python-1.1.3/rlottie/meson_options.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/packaging/rlottie.spec` & `rlottie_python-1.1.3/rlottie/packaging/rlottie.spec`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/binding/c/lottieanimation_capi.cpp` & `rlottie_python-1.1.3/rlottie/src/binding/c/lottieanimation_capi.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/CMakeLists.txt` & `rlottie_python-1.1.3/rlottie/src/lottie/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottieanimation.cpp` & `rlottie_python-1.1.3/rlottie/src/lottie/lottieanimation.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottiefiltermodel.h` & `rlottie_python-1.1.3/rlottie/src/lottie/lottiefiltermodel.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottieitem.cpp` & `rlottie_python-1.1.3/rlottie/src/lottie/lottieitem.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottieitem.h` & `rlottie_python-1.1.3/rlottie/src/lottie/lottieitem.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottieitem_capi.cpp` & `rlottie_python-1.1.3/rlottie/src/lottie/lottieitem_capi.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottiekeypath.cpp` & `rlottie_python-1.1.3/rlottie/src/lottie/lottiekeypath.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottiekeypath.h` & `rlottie_python-1.1.3/rlottie/src/lottie/lottiekeypath.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottieloader.cpp` & `rlottie_python-1.1.3/rlottie/src/lottie/lottieloader.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottiemodel.cpp` & `rlottie_python-1.1.3/rlottie/src/lottie/lottiemodel.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottiemodel.h` & `rlottie_python-1.1.3/rlottie/src/lottie/lottiemodel.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/lottieparser.cpp` & `rlottie_python-1.1.3/rlottie/src/lottie/lottieparser.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/allocators.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/allocators.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/document.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/document.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/encodedstream.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/encodedstream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/encodings.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/encodings.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/error/en.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/error/en.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/error/error.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/error/error.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/filereadstream.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/filereadstream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/filewritestream.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/filewritestream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/fwd.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/fwd.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/biginteger.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/biginteger.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/clzll.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/clzll.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/diyfp.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/diyfp.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/dtoa.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/dtoa.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/ieee754.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/ieee754.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/itoa.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/itoa.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/meta.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/meta.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/pow10.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/pow10.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/regex.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/regex.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/stack.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/stack.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/strfunc.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/strfunc.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/strtod.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/strtod.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/internal/swap.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/internal/swap.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/istreamwrapper.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/istreamwrapper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/memorybuffer.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/memorybuffer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/memorystream.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/memorystream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/msinttypes/stdint.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/msinttypes/stdint.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/ostreamwrapper.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/ostreamwrapper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/pointer.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/pointer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/prettywriter.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/prettywriter.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/rapidjson.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/rapidjson.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/reader.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/reader.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/schema.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/schema.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/stream.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/stream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/stringbuffer.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/stringbuffer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/lottie/rapidjson/writer.h` & `rlottie_python-1.1.3/rlottie/src/lottie/rapidjson/writer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/meson.build` & `rlottie_python-1.1.3/rlottie/src/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/CMakeLists.txt` & `rlottie_python-1.1.3/rlottie/src/vector/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_math.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_math.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_math.h` & `rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_math.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_raster.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_raster.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_raster.h` & `rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_raster.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_stroker.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_stroker.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_stroker.h` & `rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_stroker.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/freetype/v_ft_types.h` & `rlottie_python-1.1.3/rlottie/src/vector/freetype/v_ft_types.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/meson.build` & `rlottie_python-1.1.3/rlottie/src/vector/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/pixman/pixman-arm-neon-asm.S` & `rlottie_python-1.1.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.S`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/pixman/pixman-arm-neon-asm.h` & `rlottie_python-1.1.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/stb/CMakeLists.txt` & `rlottie_python-1.1.3/rlottie/src/vector/stb/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/stb/meson.build` & `rlottie_python-1.1.3/rlottie/src/vector/stb/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/stb/stb_image.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/stb/stb_image.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/stb/stb_image.h` & `rlottie_python-1.1.3/rlottie/src/vector/stb/stb_image.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/varenaalloc.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/varenaalloc.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/varenaalloc.h` & `rlottie_python-1.1.3/rlottie/src/vector/varenaalloc.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vbezier.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vbezier.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vbezier.h` & `rlottie_python-1.1.3/rlottie/src/vector/vbezier.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vbitmap.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vbitmap.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vbitmap.h` & `rlottie_python-1.1.3/rlottie/src/vector/vbitmap.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vbrush.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vbrush.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vbrush.h` & `rlottie_python-1.1.3/rlottie/src/vector/vbrush.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vcowptr.h` & `rlottie_python-1.1.3/rlottie/src/vector/vcowptr.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdasher.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vdasher.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdasher.h` & `rlottie_python-1.1.3/rlottie/src/vector/vdasher.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdebug.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vdebug.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdebug.h` & `rlottie_python-1.1.3/rlottie/src/vector/vdebug.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdrawable.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vdrawable.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdrawable.h` & `rlottie_python-1.1.3/rlottie/src/vector/vdrawable.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper.h` & `rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper_common.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper_common.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper_neon.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper_neon.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vdrawhelper_sse2.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vdrawhelper_sse2.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/velapsedtimer.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/velapsedtimer.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/velapsedtimer.h` & `rlottie_python-1.1.3/rlottie/src/vector/velapsedtimer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vglobal.h` & `rlottie_python-1.1.3/rlottie/src/vector/vglobal.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vimageloader.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vimageloader.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vinterpolator.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vinterpolator.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vinterpolator.h` & `rlottie_python-1.1.3/rlottie/src/vector/vinterpolator.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vline.h` & `rlottie_python-1.1.3/rlottie/src/vector/vline.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vmatrix.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vmatrix.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vmatrix.h` & `rlottie_python-1.1.3/rlottie/src/vector/vmatrix.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vpainter.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vpainter.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vpainter.h` & `rlottie_python-1.1.3/rlottie/src/vector/vpainter.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vpath.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vpath.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vpath.h` & `rlottie_python-1.1.3/rlottie/src/vector/vpath.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vpathmesure.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vpathmesure.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vpathmesure.h` & `rlottie_python-1.1.3/rlottie/src/vector/vpathmesure.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vpoint.h` & `rlottie_python-1.1.3/rlottie/src/vector/vpoint.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vraster.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vraster.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vraster.h` & `rlottie_python-1.1.3/rlottie/src/vector/vraster.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vrect.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vrect.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vrect.h` & `rlottie_python-1.1.3/rlottie/src/vector/vrect.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vrle.cpp` & `rlottie_python-1.1.3/rlottie/src/vector/vrle.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vrle.h` & `rlottie_python-1.1.3/rlottie/src/vector/vrle.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vsharedptr.h` & `rlottie_python-1.1.3/rlottie/src/vector/vsharedptr.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vstackallocator.h` & `rlottie_python-1.1.3/rlottie/src/vector/vstackallocator.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/vector/vtaskqueue.h` & `rlottie_python-1.1.3/rlottie/src/vector/vtaskqueue.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/src/wasm/rlottiewasm.cpp` & `rlottie_python-1.1.3/rlottie/src/wasm/rlottiewasm.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/test/CMakeLists.txt` & `rlottie_python-1.1.3/rlottie/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/test/meson.build` & `rlottie_python-1.1.3/rlottie/test/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/test/test_lottieanimation.cpp` & `rlottie_python-1.1.3/rlottie/test/test_lottieanimation.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/test/test_lottieanimation_capi.cpp` & `rlottie_python-1.1.3/rlottie/test/test_lottieanimation_capi.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/test/test_vpath.cpp` & `rlottie_python-1.1.3/rlottie/test/test_vpath.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/test/test_vrect.cpp` & `rlottie_python-1.1.3/rlottie/test/test_vrect.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/test/wasm_test.html` & `rlottie_python-1.1.3/rlottie/test/wasm_test.html`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/vs2019/rlottie.sln` & `rlottie_python-1.1.3/rlottie/vs2019/rlottie.sln`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/vs2019/rlottie.vcxproj` & `rlottie_python-1.1.3/rlottie/vs2019/rlottie.vcxproj`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/vs2019/rlottie.vcxproj.filters` & `rlottie_python-1.1.3/rlottie/vs2019/rlottie.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/wasm_build.sh` & `rlottie_python-1.1.3/rlottie/wasm_build.sh`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie/wasm_cross.txt` & `rlottie_python-1.1.3/rlottie/wasm_cross.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie_python/rlottie_wrapper.py` & `rlottie_python-1.1.3/rlottie_python/rlottie_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/rlottie_python/rlottiecommon.py` & `rlottie_python-1.1.3/rlottie_python/rlottiecommon.py`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.1.2/PKG-INFO` & `rlottie_python-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlottie-python
-Version: 1.1.2
+Version: 1.1.3
 Summary: A ctypes API for rlottie, with additional functions for getting Pillow Image.
 Keywords: rlottie,lottie,tgs,ctypes
 Author-email: chaudominic <chaudominic2@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Dist: Pillow
```

