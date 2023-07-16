# Comparing `tmp/freemocap-1.0.8rc0.tar.gz` & `tmp/freemocap-1.0.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freemocap-1.0.8rc0.tar", last modified: Thu Apr 20 13:49:00 2023, max compression
+gzip compressed data, was "freemocap-1.0.9rc0.tar", last modified: Thu Apr 20 15:27:23 2023, max compression
```

## Comparing `freemocap-1.0.8rc0.tar` & `freemocap-1.0.9rc0.tar`

### file list

```diff
@@ -1,194 +1,194 @@
--rwxr-xr-x   0        0        0      492 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/.github/dependabot.yml
--rw-r--r--   0        0        0      423 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1083 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rwxr-xr-x   0        0        0     1094 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2215 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/.gitignore
--rw-r--r--   0        0        0      229 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      418 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/CITATION.cff
--rw-r--r--   0        0        0      327 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/CODEOWNERS
--rw-r--r--   0        0        0     3348 2023-04-20 13:48:55.060538 freemocap-1.0.8rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/LICENSE
--rw-r--r--   0        0        0      234 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/MANIFEST.in
--rw-r--r--   0        0        0     4868 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/README.md
--rw-r--r--   0        0        0    44734 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/assets/charuco/charuco_board_image.png
--rw-r--r--   0        0        0   332173 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/assets/charuco/charuco_board_image_highRes.png
--rw-r--r--   0        0        0    26366 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/assets/logo/freemocap-logo-black-border.svg
--rw-r--r--   0        0        0   124841 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
--rw-r--r--   0        0        0    99678 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/assets/logo/freemocap_skelly_logo.ico
--rwxr-xr-x   0        0        0      607 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/builds/install_packages
--rwxr-xr-x   0        0        0      288 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/installer.sh
--rwxr-xr-x   0        0        0      278 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/linux/build.sh
--rwxr-xr-x   0        0        0      161 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/linux/run_uvicorn_server.sh
--rwxr-xr-x   0        0        0      381 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/linux/run_web_server.sh
--rwxr-xr-x   0        0        0      118 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/linux/shell.sh
--rwxr-xr-x   0        0        0      104 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/linux/test.sh
--rwxr-xr-x   0        0        0       71 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/linux/up.sh
--rw-r--r--   0        0        0      410 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/windows/installChocolatey.cmd
--rw-r--r--   0        0        0      112 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/bin/windows/run_web_server.cmd
--rw-r--r--   0        0        0      331 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/experimental/freemocap-ui/.gitignore
--rw-r--r--   0        0        0     2359 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/experimental/freemocap-ui/README.md
--rw-r--r--   0        0        0      734 2023-04-20 13:48:55.064538 freemocap-1.0.8rc0/experimental/freemocap-ui/config-overrides.js
--rw-r--r--   0        0        0  1263565 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/package-lock.json
--rw-r--r--   0        0        0     2548 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/package.json
--rw-r--r--   0        0        0     3585 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/public/favicon.ico
--rw-r--r--   0        0        0     1963 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/public/index.html
--rw-r--r--   0        0        0     4153 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/public/logo192.png
--rw-r--r--   0        0        0    12066 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/public/logo512.png
--rw-r--r--   0        0        0      492 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/public/manifest.json
--rw-r--r--   0        0        0       67 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/public/robots.txt
--rw-r--r--   0        0        0       33 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/scripts/cert.sh
--rw-r--r--   0        0        0      582 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/App.css
--rw-r--r--   0        0        0      366 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/App.test.tsx
--rw-r--r--   0        0        0      193 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/App.tsx
--rw-r--r--   0        0        0      346 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/app/hooks.ts
--rw-r--r--   0        0        0      445 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/app/store.ts
--rw-r--r--   0        0        0      941 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx
--rw-r--r--   0        0        0      475 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
--rw-r--r--   0        0        0     1057 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
--rw-r--r--   0        0        0      104 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/components/webcam/webcam.tsx
--rw-r--r--   0        0        0      610 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
--rw-r--r--   0        0        0     1291 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css
--rw-r--r--   0        0        0     1758 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx
--rw-r--r--   0        0        0      214 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/counterAPI.ts
--rw-r--r--   0        0        0      842 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
--rw-r--r--   0        0        0     2983 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts
--rw-r--r--   0        0        0      291 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/hooks/use-device-stream.ts
--rw-r--r--   0        0        0      791 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
--rw-r--r--   0        0        0      366 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/index.css
--rw-r--r--   0        0        0      623 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/index.tsx
--rw-r--r--   0        0        0      417 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/Copyright.tsx
--rw-r--r--   0        0        0     1625 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/Header.tsx
--rw-r--r--   0        0        0     2353 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/Navigator.tsx
--rw-r--r--   0        0        0     4303 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx
--rw-r--r--   0        0        0      394 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
--rw-r--r--   0        0        0      273 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
--rw-r--r--   0        0        0     1943 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/content/Content.tsx
--rw-r--r--   0        0        0      737 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/routing/router.tsx
--rw-r--r--   0        0        0     1122 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/logo.svg
--rw-r--r--   0        0        0       40 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/react-app-env.d.ts
--rw-r--r--   0        0        0     5290 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/serviceWorker.ts
--rw-r--r--   0        0        0      629 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/Capture.tsx
--rw-r--r--   0        0        0      370 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/Record.ts
--rw-r--r--   0        0        0      198 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/cam.ts
--rw-r--r--   0        0        0      325 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/download.ts
--rw-r--r--   0        0        0     1717 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/frame-capture.tsx
--rw-r--r--   0        0        0      497 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/image_send_worker.ts
--rw-r--r--   0        0        0     2044 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/recorder.ts
--rw-r--r--   0        0        0     1560 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/supported_recorder.ts
--rw-r--r--   0        0        0      254 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/setupTests.ts
--rw-r--r--   0        0        0     1384 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/Capture.tsx
--rw-r--r--   0        0        0      733 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/Config.tsx
--rw-r--r--   0        0        0     1153 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
--rw-r--r--   0        0        0      109 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/ShowCameras.tsx
--rw-r--r--   0        0        0      124 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/UserConfig.tsx
--rw-r--r--   0        0        0      965 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
--rw-r--r--   0        0        0      792 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
--rw-r--r--   0        0        0     1023 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
--rw-r--r--   0        0        0     1976 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
--rw-r--r--   0        0        0      599 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/freemocap-ui/tsconfig.json
--rw-r--r--   0        0        0      789 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/python_scratch/qt_drag_and_drop.py
--rw-r--r--   0        0        0     1609 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/experimental/tool_bar.py
--rw-r--r--   0        0        0     1821 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/__init__.py
--rw-r--r--   0        0        0      888 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/__main__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
--rw-r--r--   0        0        0     6700 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
--rw-r--r--   0        0        0    60000 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
--rw-r--r--   0        0        0     2613 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
--rw-r--r--   0        0        0     1504 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
--rw-r--r--   0        0        0       36 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/default_charuco_square_size.py
--rw-r--r--   0        0        0     1177 2023-04-20 13:48:55.072538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
--rw-r--r--   0        0        0     9539 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
--rw-r--r--   0        0        0    14641 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
--rw-r--r--   0        0        0    24623 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
--rw-r--r--   0        0        0     1752 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/__init__.py
--rw-r--r--   0        0        0    57980 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py
--rw-r--r--   0        0        0     1091 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py
--rw-r--r--   0        0        0    37868 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py
--rw-r--r--   0        0        0     5843 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py
--rw-r--r--   0        0        0     1876 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py
--rw-r--r--   0        0        0     1445 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/post_process_skeleton_data/__init__.py
--rw-r--r--   0        0        0     6228 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py
--rw-r--r--   0        0        0    44609 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py
--rw-r--r--   0        0        0     1389 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/process_motion_capture_videos/__init__.py
--rw-r--r--   0        0        0     8240 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/actions_and_menus/__init__.py
--rw-r--r--   0        0        0     4270 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/actions_and_menus/actions.py
--rw-r--r--   0        0        0     2379 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py
--rw-r--r--   0        0        0     1630 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/freemocap_main.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/main_window/__init__.py
--rw-r--r--   0        0        0    23348 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/main_window/freemocap_main_window.py
--rw-r--r--   0        0        0    13143 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/AMOLED.qss
--rw-r--r--   0        0        0     7364 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/ElegantDark.qss
--rw-r--r--   0        0        0     7431 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/FunkyTown.qss
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/__init__.py
--rw-r--r--   0        0        0      360 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
--rw-r--r--   0        0        0     1329 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py
--rw-r--r--   0        0        0     2403 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.css
--rw-r--r--   0        0        0     3225 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
--rw-r--r--   0        0        0     1479 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py
--rw-r--r--   0        0        0      303 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
--rw-r--r--   0        0        0      136 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/stylesheet-branch-more.png
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/utilities/__init__.py
--rw-r--r--   0        0        0      192 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/utilities/get_qt_app.py
--rw-r--r--   0        0        0      856 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0     6852 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/active_recording_widget.py
--rw-r--r--   0        0        0     6901 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py
--rw-r--r--   0        0        0     3265 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/central_tab_widget.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/__init__.py
--rw-r--r--   0        0        0    13441 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
--rw-r--r--   0        0        0     2328 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
--rw-r--r--   0        0        0        2 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
--rw-r--r--   0        0        0     7510 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
--rw-r--r--   0        0        0     9808 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
--rw-r--r--   0        0        0     4435 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py
--rw-r--r--   0        0        0     2312 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py
--rw-r--r--   0        0        0     6631 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/directory_view_widget.py
--rw-r--r--   0        0        0     4427 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/home_widget.py
--rw-r--r--   0        0        0     4736 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/import_videos_window.py
--rw-r--r--   0        0        0     3085 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py
--rw-r--r--   0        0        0     2684 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/widgets/log_view_widget.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/workers/__init__.py
--rw-r--r--   0        0        0     2272 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
--rw-r--r--   0        0        0     1489 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/parameter_info_models/__init__.py
--rw-r--r--   0        0        0     9779 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/parameter_info_models/recording_info_model.py
--rw-r--r--   0        0        0     1308 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/system/__init__.py
--rw-r--r--   0        0        0     1477 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/system/logging/configure_logging.py
--rw-r--r--   0        0        0     8232 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/system/paths_and_files_names.py
--rw-r--r--   0        0        0      251 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/system/start_file.py
--rw-r--r--   0        0        0        0 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/system/user_data/__init__.py
--rw-r--r--   0        0        0      863 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/system/user_data/pipedream_pings.py
--rw-r--r--   0        0        0     1817 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/tests/test_mediapipe_2d_data_shape.py
--rw-r--r--   0        0        0     2363 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/tests/test_mediapipe_3d_data_shape.py
--rw-r--r--   0        0        0      809 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/tests/test_synchronized_video_frame_counts.py
--rw-r--r--   0        0        0      130 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/tests/test_test.py
--rw-r--r--   0        0        0     1276 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py
--rw-r--r--   0        0        0      743 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0      645 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/utilities/get_video_paths.py
--rw-r--r--   0        0        0      447 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/utilities/project_3d_data_to_z_plane.py
--rw-r--r--   0        0        0      497 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/utilities/rotate_by_90_degrees_around_x_axis.py
--rw-r--r--   0        0        0      513 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/freemocap/utilities/save_dictionary_to_json.py
--rw-r--r--   0        0        0     5252 2023-04-20 13:48:55.076538 freemocap-1.0.8rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
--rw-r--r--   0        0        0    21821 2023-04-20 13:48:55.080538 freemocap-1.0.8rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
--rw-r--r--   0        0        0    13464 2023-04-20 13:48:55.080538 freemocap-1.0.8rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
--rw-r--r--   0        0        0     3594 2023-04-20 13:48:55.080538 freemocap-1.0.8rc0/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-20 13:48:55.080538 freemocap-1.0.8rc0/requirements.txt
--rw-r--r--   0        0        0       50 2023-04-20 13:48:55.080538 freemocap-1.0.8rc0/setup.py
--rw-r--r--   0        0        0     1045 2023-04-20 13:48:55.080538 freemocap-1.0.8rc0/src/gui/main/main.py
--rw-r--r--   0        0        0     7614 1970-01-01 00:00:00.000000 freemocap-1.0.8rc0/PKG-INFO
+-rwxr-xr-x   0        0        0      492 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/.github/dependabot.yml
+-rw-r--r--   0        0        0      423 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1083 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rwxr-xr-x   0        0        0     1094 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2215 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/.gitignore
+-rw-r--r--   0        0        0      229 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      418 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/CITATION.cff
+-rw-r--r--   0        0        0      327 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/CODEOWNERS
+-rw-r--r--   0        0        0     3348 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/LICENSE
+-rw-r--r--   0        0        0      234 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/MANIFEST.in
+-rw-r--r--   0        0        0     4868 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/README.md
+-rw-r--r--   0        0        0    44734 2023-04-20 15:27:16.813684 freemocap-1.0.9rc0/assets/charuco/charuco_board_image.png
+-rw-r--r--   0        0        0   332173 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/assets/charuco/charuco_board_image_highRes.png
+-rw-r--r--   0        0        0    26366 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/assets/logo/freemocap-logo-black-border.svg
+-rw-r--r--   0        0        0   124841 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
+-rw-r--r--   0        0        0    99678 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/assets/logo/freemocap_skelly_logo.ico
+-rwxr-xr-x   0        0        0      607 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/builds/install_packages
+-rwxr-xr-x   0        0        0      288 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/installer.sh
+-rwxr-xr-x   0        0        0      278 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/linux/build.sh
+-rwxr-xr-x   0        0        0      161 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/linux/run_uvicorn_server.sh
+-rwxr-xr-x   0        0        0      381 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/linux/run_web_server.sh
+-rwxr-xr-x   0        0        0      118 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/linux/shell.sh
+-rwxr-xr-x   0        0        0      104 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/linux/test.sh
+-rwxr-xr-x   0        0        0       71 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/linux/up.sh
+-rw-r--r--   0        0        0      410 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/windows/installChocolatey.cmd
+-rw-r--r--   0        0        0      112 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/bin/windows/run_web_server.cmd
+-rw-r--r--   0        0        0      331 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/experimental/freemocap-ui/.gitignore
+-rw-r--r--   0        0        0     2359 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/experimental/freemocap-ui/README.md
+-rw-r--r--   0        0        0      734 2023-04-20 15:27:16.817684 freemocap-1.0.9rc0/experimental/freemocap-ui/config-overrides.js
+-rw-r--r--   0        0        0  1263565 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/package-lock.json
+-rw-r--r--   0        0        0     2548 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/package.json
+-rw-r--r--   0        0        0     3585 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/public/favicon.ico
+-rw-r--r--   0        0        0     1963 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/public/index.html
+-rw-r--r--   0        0        0     4153 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/public/logo192.png
+-rw-r--r--   0        0        0    12066 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/public/logo512.png
+-rw-r--r--   0        0        0      492 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/public/robots.txt
+-rw-r--r--   0        0        0       33 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/scripts/cert.sh
+-rw-r--r--   0        0        0      582 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/App.css
+-rw-r--r--   0        0        0      366 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/App.test.tsx
+-rw-r--r--   0        0        0      193 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/App.tsx
+-rw-r--r--   0        0        0      346 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/app/hooks.ts
+-rw-r--r--   0        0        0      445 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/app/store.ts
+-rw-r--r--   0        0        0      941 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx
+-rw-r--r--   0        0        0      475 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
+-rw-r--r--   0        0        0     1057 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
+-rw-r--r--   0        0        0      104 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/components/webcam/webcam.tsx
+-rw-r--r--   0        0        0      610 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
+-rw-r--r--   0        0        0     1291 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css
+-rw-r--r--   0        0        0     1758 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx
+-rw-r--r--   0        0        0      214 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/counterAPI.ts
+-rw-r--r--   0        0        0      842 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
+-rw-r--r--   0        0        0     2983 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts
+-rw-r--r--   0        0        0      291 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/hooks/use-device-stream.ts
+-rw-r--r--   0        0        0      791 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
+-rw-r--r--   0        0        0      366 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/index.css
+-rw-r--r--   0        0        0      623 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/index.tsx
+-rw-r--r--   0        0        0      417 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/Copyright.tsx
+-rw-r--r--   0        0        0     1625 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/Header.tsx
+-rw-r--r--   0        0        0     2353 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/Navigator.tsx
+-rw-r--r--   0        0        0     4303 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx
+-rw-r--r--   0        0        0      394 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
+-rw-r--r--   0        0        0      273 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
+-rw-r--r--   0        0        0     1943 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/content/Content.tsx
+-rw-r--r--   0        0        0      737 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/routing/router.tsx
+-rw-r--r--   0        0        0     1122 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/logo.svg
+-rw-r--r--   0        0        0       40 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/react-app-env.d.ts
+-rw-r--r--   0        0        0     5290 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/serviceWorker.ts
+-rw-r--r--   0        0        0      629 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/Capture.tsx
+-rw-r--r--   0        0        0      370 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/Record.ts
+-rw-r--r--   0        0        0      198 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/cam.ts
+-rw-r--r--   0        0        0      325 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/download.ts
+-rw-r--r--   0        0        0     1717 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/frame-capture.tsx
+-rw-r--r--   0        0        0      497 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/image_send_worker.ts
+-rw-r--r--   0        0        0     2044 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/recorder.ts
+-rw-r--r--   0        0        0     1560 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/supported_recorder.ts
+-rw-r--r--   0        0        0      254 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/setupTests.ts
+-rw-r--r--   0        0        0     1384 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/Capture.tsx
+-rw-r--r--   0        0        0      733 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/Config.tsx
+-rw-r--r--   0        0        0     1153 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
+-rw-r--r--   0        0        0      109 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/ShowCameras.tsx
+-rw-r--r--   0        0        0      124 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/UserConfig.tsx
+-rw-r--r--   0        0        0      965 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
+-rw-r--r--   0        0        0      792 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
+-rw-r--r--   0        0        0     1023 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
+-rw-r--r--   0        0        0     1976 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
+-rw-r--r--   0        0        0      599 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/freemocap-ui/tsconfig.json
+-rw-r--r--   0        0        0      789 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/python_scratch/qt_drag_and_drop.py
+-rw-r--r--   0        0        0     1609 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/experimental/tool_bar.py
+-rw-r--r--   0        0        0     1821 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/__init__.py
+-rw-r--r--   0        0        0      888 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
+-rw-r--r--   0        0        0     6700 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
+-rw-r--r--   0        0        0    60000 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
+-rw-r--r--   0        0        0     2613 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
+-rw-r--r--   0        0        0     1504 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
+-rw-r--r--   0        0        0       36 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/default_charuco_square_size.py
+-rw-r--r--   0        0        0     1177 2023-04-20 15:27:16.825684 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
+-rw-r--r--   0        0        0     9539 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
+-rw-r--r--   0        0        0    14641 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
+-rw-r--r--   0        0        0    24623 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
+-rw-r--r--   0        0        0     1752 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/__init__.py
+-rw-r--r--   0        0        0    57980 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py
+-rw-r--r--   0        0        0     1091 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py
+-rw-r--r--   0        0        0    37868 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py
+-rw-r--r--   0        0        0     5843 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py
+-rw-r--r--   0        0        0     1876 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py
+-rw-r--r--   0        0        0     1445 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/post_process_skeleton_data/__init__.py
+-rw-r--r--   0        0        0     6228 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py
+-rw-r--r--   0        0        0    44609 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py
+-rw-r--r--   0        0        0     1389 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/process_motion_capture_videos/__init__.py
+-rw-r--r--   0        0        0     8240 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/actions_and_menus/__init__.py
+-rw-r--r--   0        0        0     4270 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/actions_and_menus/actions.py
+-rw-r--r--   0        0        0     2379 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py
+-rw-r--r--   0        0        0     1630 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/freemocap_main.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/main_window/__init__.py
+-rw-r--r--   0        0        0    23348 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/main_window/freemocap_main_window.py
+-rw-r--r--   0        0        0    13143 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/AMOLED.qss
+-rw-r--r--   0        0        0     7364 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/ElegantDark.qss
+-rw-r--r--   0        0        0     7431 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/FunkyTown.qss
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/__init__.py
+-rw-r--r--   0        0        0      360 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
+-rw-r--r--   0        0        0     1329 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py
+-rw-r--r--   0        0        0     2403 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.css
+-rw-r--r--   0        0        0     3225 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
+-rw-r--r--   0        0        0     1479 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py
+-rw-r--r--   0        0        0      303 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
+-rw-r--r--   0        0        0      136 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/stylesheet-branch-more.png
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/utilities/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/utilities/get_qt_app.py
+-rw-r--r--   0        0        0      856 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0     6852 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/active_recording_widget.py
+-rw-r--r--   0        0        0     6901 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py
+-rw-r--r--   0        0        0     3265 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/central_tab_widget.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/__init__.py
+-rw-r--r--   0        0        0    13441 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
+-rw-r--r--   0        0        0     2328 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
+-rw-r--r--   0        0        0        2 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
+-rw-r--r--   0        0        0     7510 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
+-rw-r--r--   0        0        0     9808 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
+-rw-r--r--   0        0        0     4435 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py
+-rw-r--r--   0        0        0     2312 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py
+-rw-r--r--   0        0        0     6631 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/directory_view_widget.py
+-rw-r--r--   0        0        0     4427 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/home_widget.py
+-rw-r--r--   0        0        0     4736 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/import_videos_window.py
+-rw-r--r--   0        0        0     3085 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py
+-rw-r--r--   0        0        0     2684 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/widgets/log_view_widget.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/workers/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
+-rw-r--r--   0        0        0     1489 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/parameter_info_models/__init__.py
+-rw-r--r--   0        0        0     9779 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/parameter_info_models/recording_info_model.py
+-rw-r--r--   0        0        0     1308 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/system/__init__.py
+-rw-r--r--   0        0        0     1477 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/system/logging/configure_logging.py
+-rw-r--r--   0        0        0     8232 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/system/paths_and_files_names.py
+-rw-r--r--   0        0        0      251 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/system/start_file.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/system/user_data/__init__.py
+-rw-r--r--   0        0        0      863 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/system/user_data/pipedream_pings.py
+-rw-r--r--   0        0        0     1817 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/tests/test_mediapipe_2d_data_shape.py
+-rw-r--r--   0        0        0     2363 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/tests/test_mediapipe_3d_data_shape.py
+-rw-r--r--   0        0        0      809 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/tests/test_synchronized_video_frame_counts.py
+-rw-r--r--   0        0        0      130 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/tests/test_test.py
+-rw-r--r--   0        0        0     1276 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py
+-rw-r--r--   0        0        0      743 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0      645 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/utilities/get_video_paths.py
+-rw-r--r--   0        0        0      447 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/utilities/project_3d_data_to_z_plane.py
+-rw-r--r--   0        0        0      497 2023-04-20 15:27:16.829685 freemocap-1.0.9rc0/freemocap/utilities/rotate_by_90_degrees_around_x_axis.py
+-rw-r--r--   0        0        0      513 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/freemocap/utilities/save_dictionary_to_json.py
+-rw-r--r--   0        0        0     5252 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
+-rw-r--r--   0        0        0    21821 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
+-rw-r--r--   0        0        0    13464 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
+-rw-r--r--   0        0        0     3581 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/requirements.txt
+-rw-r--r--   0        0        0       50 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/setup.py
+-rw-r--r--   0        0        0     1045 2023-04-20 15:27:16.833685 freemocap-1.0.9rc0/src/gui/main/main.py
+-rw-r--r--   0        0        0     7601 1970-01-01 00:00:00.000000 freemocap-1.0.9rc0/PKG-INFO
```

### Comparing `freemocap-1.0.8rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `freemocap-1.0.9rc0/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/.github/workflows/python-testing.yml` & `freemocap-1.0.9rc0/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/.gitignore` & `freemocap-1.0.9rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/CONTRIBUTING.md` & `freemocap-1.0.9rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/LICENSE` & `freemocap-1.0.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/README.md` & `freemocap-1.0.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/assets/charuco/charuco_board_image.png` & `freemocap-1.0.9rc0/assets/charuco/charuco_board_image.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/assets/charuco/charuco_board_image_highRes.png` & `freemocap-1.0.9rc0/assets/charuco/charuco_board_image_highRes.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/assets/logo/freemocap-logo-black-border.svg` & `freemocap-1.0.9rc0/assets/logo/freemocap-logo-black-border.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png` & `freemocap-1.0.9rc0/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/assets/logo/freemocap_skelly_logo.ico` & `freemocap-1.0.9rc0/assets/logo/freemocap_skelly_logo.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/bin/builds/install_packages` & `freemocap-1.0.9rc0/bin/builds/install_packages`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/README.md` & `freemocap-1.0.9rc0/experimental/freemocap-ui/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/config-overrides.js` & `freemocap-1.0.9rc0/experimental/freemocap-ui/config-overrides.js`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/package-lock.json` & `freemocap-1.0.9rc0/experimental/freemocap-ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/package.json` & `freemocap-1.0.9rc0/experimental/freemocap-ui/package.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/public/favicon.ico` & `freemocap-1.0.9rc0/experimental/freemocap-ui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/public/index.html` & `freemocap-1.0.9rc0/experimental/freemocap-ui/public/index.html`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/public/logo192.png` & `freemocap-1.0.9rc0/experimental/freemocap-ui/public/logo192.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/public/logo512.png` & `freemocap-1.0.9rc0/experimental/freemocap-ui/public/logo512.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/App.css` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/App.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/components/start-stop-process.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/Counter.module.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/Counter.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/features/counter/counterSlice.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/index.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/Header.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/Header.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/Navigator.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/Navigator.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/Paperbase.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/content/Content.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/content/Content.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/layout/routing/router.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/layout/routing/router.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/logo.svg` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/serviceWorker.ts` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/serviceWorker.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/Capture.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/frame-capture.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/recorder.ts` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/services/supported_recorder.ts` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/services/supported_recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/Capture.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/Config.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/Config.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx` & `freemocap-1.0.9rc0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/freemocap-ui/tsconfig.json` & `freemocap-1.0.9rc0/experimental/freemocap-ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/python_scratch/qt_drag_and_drop.py` & `freemocap-1.0.9rc0/experimental/python_scratch/qt_drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/experimental/tool_bar.py` & `freemocap-1.0.9rc0/experimental/tool_bar.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/__init__.py` & `freemocap-1.0.9rc0/freemocap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for freemocap"""
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
-__version__ = "v1.0.8-rc"
+__version__ = "v1.0.9-rc"
 __description__ = "A free and open source markerless motion capture system for everyone 💀✨"
 
 __package_name__ = "freemocap"
 __repo_url__ = f"https://github.com/freemocap/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
 
 import sys
```

### Comparing `freemocap-1.0.8rc0/freemocap/__main__.py` & `freemocap-1.0.9rc0/freemocap/__main__.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py` & `freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py` & `freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py` & `freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py` & `freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py` & `freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py` & `freemocap-1.0.9rc0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py` & `freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py` & `freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py` & `freemocap-1.0.9rc0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_names_and_connections.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py` & `freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/alpha_freemocap_blender_megascript.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py` & `freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/cgtinker_blendarmocap_load.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py` & `freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/blender_bpy_export_scripts/freemocap_blender_megascript_take2.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py` & `freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/call_blender_subprocess_methods.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py` & `freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/export_to_blender.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py` & `freemocap-1.0.9rc0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py` & `freemocap-1.0.9rc0/freemocap/core_processes/post_process_skeleton_data/estimate_skeleton_segment_lengths.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py` & `freemocap-1.0.9rc0/freemocap/core_processes/post_process_skeleton_data/gap_fill_filter_and_origin_align_skeleton_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py` & `freemocap-1.0.9rc0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py` & `freemocap-1.0.9rc0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/actions_and_menus/actions.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/actions_and_menus/actions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/actions_and_menus/menu_bar.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/freemocap_main.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/freemocap_main.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/main_window/freemocap_main_window.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/main_window/freemocap_main_window.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/AMOLED.qss` & `freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/AMOLED.qss`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/ElegantDark.qss` & `freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/ElegantDark.qss`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/FunkyTown.qss` & `freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/FunkyTown.qss`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/css_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.css` & `freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss` & `freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/style_sheet/scss_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/active_recording_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/active_recording_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/camera_controller_group_box.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/central_tab_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/central_tab_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel/visualization_control_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/directory_view_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/directory_view_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/home_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/home_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/import_videos_window.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/import_videos_window.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/jupyter_console_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/widgets/log_view_widget.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/widgets/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py` & `freemocap-1.0.9rc0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/parameter_info_models/recording_info_model.py` & `freemocap-1.0.9rc0/freemocap/parameter_info_models/recording_info_model.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py` & `freemocap-1.0.9rc0/freemocap/parameter_info_models/recording_processing_parameter_models.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/system/logging/configure_logging.py` & `freemocap-1.0.9rc0/freemocap/system/logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/system/paths_and_files_names.py` & `freemocap-1.0.9rc0/freemocap/system/paths_and_files_names.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/system/user_data/pipedream_pings.py` & `freemocap-1.0.9rc0/freemocap/system/user_data/pipedream_pings.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/tests/test_mediapipe_2d_data_shape.py` & `freemocap-1.0.9rc0/freemocap/tests/test_mediapipe_2d_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/tests/test_mediapipe_3d_data_shape.py` & `freemocap-1.0.9rc0/freemocap/tests/test_mediapipe_3d_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/tests/test_synchronized_video_frame_counts.py` & `freemocap-1.0.9rc0/freemocap/tests/test_synchronized_video_frame_counts.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py` & `freemocap-1.0.9rc0/freemocap/tests/test_total_body_center_of_mass_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `freemocap-1.0.9rc0/freemocap/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/utilities/get_video_paths.py` & `freemocap-1.0.9rc0/freemocap/utilities/get_video_paths.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/freemocap/utilities/save_dictionary_to_json.py` & `freemocap-1.0.9rc0/freemocap/utilities/save_dictionary_to_json.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb` & `freemocap-1.0.9rc0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb` & `freemocap-1.0.9rc0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb` & `freemocap-1.0.9rc0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/pyproject.toml` & `freemocap-1.0.9rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     "Blender3d",
     "synchronization",
     "computer vision"
 ]
 
 #dynamic = ["dependencies"]
 dependencies = [
-    "skellycam==2023.4.1080",
+    "skellycam",
     "skelly_viewer",
     'mediapipe; platform_system != "Darwin" or platform_machine != "arm64"',
     'mediapipe-silicon; platform_system == "Darwin" and platform_machine == "arm64"',
     "opencv-contrib-python==4.6.0.66",
     "toml",
     "aniposelib",
     "libsass",
@@ -86,15 +86,15 @@
 
 [project.urls]
 Homepage = "https://freemocap.org"
 Documentation = "https://freemocap.readthedocs.io/en/latest/"
 Github = "https://github.com/freemocap/freemocap"
 
 [tool.bumpver]
-current_version = "v1.0.8-rc"
+current_version = "v1.0.9-rc"
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `freemocap-1.0.8rc0/src/gui/main/main.py` & `freemocap-1.0.9rc0/src/gui/main/main.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.0.8rc0/PKG-INFO` & `freemocap-1.0.9rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freemocap
-Version: 1.0.8rc0
+Version: 1.0.9rc0
 Summary: Top-level package for freemocap
 Keywords: camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d animation,Blender,Blender3d,synchronization,computer vision
 Author: Endurance Idehen, Aaron Cherian, Jonathan Samir Matthis
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -30,15 +30,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Video (UVC)
-Requires-Dist: skellycam==2023.4.1080
+Requires-Dist: skellycam
 Requires-Dist: skelly_viewer
 Requires-Dist: mediapipe; platform_system != "Darwin" or platform_machine != "arm64"
 Requires-Dist: mediapipe-silicon; platform_system == "Darwin" and platform_machine == "arm64"
 Requires-Dist: opencv-contrib-python==4.6.0.66
 Requires-Dist: toml
 Requires-Dist: aniposelib
 Requires-Dist: libsass
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freemocap Version: 1.0.8rc0 Summary: Top-level
+Metadata-Version: 2.1 Name: freemocap Version: 1.0.9rc0 Summary: Top-level
 package for freemocap Keywords:
 camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless
 motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d
 animation,Blender,Blender3d,synchronization,computer vision Author: Endurance
 Idehen, Aaron Cherian, Jonathan Samir Matthis Author-email: Skelly FreeMoCap
 freemocap.org> Requires-Python: >=3.8, <3.11 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI
@@ -20,17 +20,17 @@
 Classifier: Topic :: Multimedia :: Video :: Capture Classifier: Topic ::
 Multimedia :: Video :: Display Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing Classifier:
 Topic :: Scientific/Engineering :: Visualization Classifier: Topic ::
 Scientific/Engineering :: Human Machine Interfaces Classifier: Topic :: System
 :: Hardware Classifier: Topic :: System :: Hardware :: Universal Serial Bus
 (USB) Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) ::
-Video (UVC) Requires-Dist: skellycam==2023.4.1080 Requires-Dist: skelly_viewer
-Requires-Dist: mediapipe; platform_system != "Darwin" or platform_machine !=
-"arm64" Requires-Dist: mediapipe-silicon; platform_system == "Darwin" and
+Video (UVC) Requires-Dist: skellycam Requires-Dist: skelly_viewer Requires-
+Dist: mediapipe; platform_system != "Darwin" or platform_machine != "arm64"
+Requires-Dist: mediapipe-silicon; platform_system == "Darwin" and
 platform_machine == "arm64" Requires-Dist: opencv-contrib-python==4.6.0.66
 Requires-Dist: toml Requires-Dist: aniposelib Requires-Dist: libsass Requires-
 Dist: black ; extra == "dev" Requires-Dist: bumpver ; extra == "dev" Requires-
 Dist: isort ; extra == "dev" Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev" Requires-Dist: flit ; extra == "dev"
 Project-URL: Documentation, https://freemocap.readthedocs.io/en/latest/
 Project-URL: Github, https://github.com/freemocap/freemocap Project-URL:
```

