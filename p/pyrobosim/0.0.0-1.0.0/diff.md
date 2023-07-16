# Comparing `tmp/pyrobosim-0.0.0.tar.gz` & `tmp/pyrobosim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrobosim-0.0.0.tar", last modified: Sun Jul 16 11:50:52 2023, max compression
+gzip compressed data, was "pyrobosim-1.0.0.tar", last modified: Sun Jul 16 11:57:20 2023, max compression
```

## Comparing `pyrobosim-0.0.0.tar` & `pyrobosim-1.0.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      282 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/PKG-INFO
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       74 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/__init__.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/core/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      453 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12018 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/gazebo.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8245 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/hallway.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10758 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/locations.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6546 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/objects.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    16611 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/robot.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5021 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/room.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    47789 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/world.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7452 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/core/yaml_utils.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1632 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/example_location_data.yaml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      566 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/example_object_data.yaml
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/pddlstream/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/01_simple/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2685 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/01_simple/domain.pddl
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      466 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/01_simple/streams.pddl
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/02_derived/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7465 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/02_derived/domain.pddl
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      479 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/02_derived/streams.pddl
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8188 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/domain.pddl
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      919 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/streams.pddl
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9554 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/domain.pddl
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1516 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/streams.pddl
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9892 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/domain.pddl
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1965 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/streams.pddl
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2703 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/pddlstream_simple_world.yaml
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/sample_models/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/materials/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/materials/textures/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)  1189011 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/materials/textures/coke_can.png
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/meshes/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)   640785 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/meshes/coke_can.dae
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      862 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model-1_2.sdf
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      856 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model-1_3.sdf
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1284 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model-1_4.sdf
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      393 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model.config
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1284 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model.sdf
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/data/sample_models/first_2015_trash_can/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/data/sample_models/first_2015_trash_can/meshes/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)   882628 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/first_2015_trash_can/meshes/trash_can.dae
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      284 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/first_2015_trash_can/model.config
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      836 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/sample_models/first_2015_trash_can/model.sdf
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/data/templates/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      892 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/templates/link_template_polyline.sdf
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      230 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/templates/model_template.config
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      235 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/templates/model_template.sdf
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2056 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/templates/world_template_gazebo.sdf
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2515 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/templates/world_template_ignition.sdf
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3085 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/test_world.yaml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3452 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/data/test_world_multirobot.yaml
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/gui/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      379 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/gui/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9798 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/gui/main.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    16818 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/gui/world_canvas.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/manipulation/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      200 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/manipulation/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    25763 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/manipulation/grasping.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/navigation/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      298 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6469 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/a_star.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2822 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/execution.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9745 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/occupancy_grid.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2800 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/path_planner.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4676 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/planner_base.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5686 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/prm.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14480 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/rrt.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3873 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/trajectory.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5392 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/navigation/world_graph.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/planning/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      473 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/planning/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5267 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/planning/actions.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/planning/pddlstream/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      388 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/planning/pddlstream/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2800 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/planning/pddlstream/default_mappings.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4649 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/planning/pddlstream/planner.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7450 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/planning/pddlstream/primitives.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6837 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/planning/pddlstream/utils.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/pyrobosim/utils/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      209 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/utils/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2711 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/utils/general.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11921 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/utils/knowledge.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3610 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/utils/motion.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10605 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/utils/polygon.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8419 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/utils/pose.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6617 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/pyrobosim/utils/search_graph.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:50:52.528448 pyrobosim-0.0.0/pyrobosim.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      282 2023-07-16 11:50:52.000000 pyrobosim-0.0.0/pyrobosim.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3048 2023-07-16 11:50:52.000000 pyrobosim-0.0.0/pyrobosim.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-16 11:50:52.000000 pyrobosim-0.0.0/pyrobosim.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       99 2023-07-16 11:50:52.000000 pyrobosim-0.0.0/pyrobosim.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       10 2023-07-16 11:50:52.000000 pyrobosim-0.0.0/pyrobosim.egg-info/top_level.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-06 16:52:33.000000 pyrobosim-0.0.0/pyrobosim.egg-info/zip-safe
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-16 11:50:52.532448 pyrobosim-0.0.0/setup.cfg
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1083 2023-07-06 16:46:54.000000 pyrobosim-0.0.0/setup.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.368270 pyrobosim-1.0.0/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      282 2023-07-16 11:57:20.368270 pyrobosim-1.0.0/PKG-INFO
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       74 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/__init__.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/core/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      453 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12018 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/gazebo.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8245 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/hallway.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10758 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/locations.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6546 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/objects.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    16611 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/robot.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5021 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/room.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    47789 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/world.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7452 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/core/yaml_utils.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1632 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/example_location_data.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      566 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/example_object_data.yaml
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.360269 pyrobosim-1.0.0/pyrobosim/data/pddlstream/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.360269 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/01_simple/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2685 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/01_simple/domain.pddl
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      466 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/01_simple/streams.pddl
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/02_derived/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7465 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/02_derived/domain.pddl
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      479 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/02_derived/streams.pddl
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8188 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/domain.pddl
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      919 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/streams.pddl
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9554 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/domain.pddl
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1516 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/streams.pddl
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9892 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/domain.pddl
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1965 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/streams.pddl
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2703 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/pddlstream_simple_world.yaml
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.360269 pyrobosim-1.0.0/pyrobosim/data/sample_models/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.360269 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/materials/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/materials/textures/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)  1189011 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/materials/textures/coke_can.png
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/meshes/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)   640785 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/meshes/coke_can.dae
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      862 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model-1_2.sdf
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      856 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model-1_3.sdf
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1284 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model-1_4.sdf
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      393 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model.config
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1284 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model.sdf
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/sample_models/first_2015_trash_can/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/sample_models/first_2015_trash_can/meshes/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)   882628 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/first_2015_trash_can/meshes/trash_can.dae
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      284 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/first_2015_trash_can/model.config
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      836 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/sample_models/first_2015_trash_can/model.sdf
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/data/templates/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      892 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/templates/link_template_polyline.sdf
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      230 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/templates/model_template.config
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      235 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/templates/model_template.sdf
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2056 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/templates/world_template_gazebo.sdf
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2515 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/templates/world_template_ignition.sdf
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3085 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/test_world.yaml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3452 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/data/test_world_multirobot.yaml
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/gui/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      379 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/gui/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9798 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/gui/main.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    16818 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/gui/world_canvas.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/manipulation/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      200 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/manipulation/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    25763 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/manipulation/grasping.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim/navigation/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      298 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6469 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/a_star.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2822 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/execution.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9745 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/occupancy_grid.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2800 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/path_planner.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4676 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/planner_base.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5686 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/prm.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14480 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/rrt.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3873 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/trajectory.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5392 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/navigation/world_graph.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.368270 pyrobosim-1.0.0/pyrobosim/planning/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      473 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/planning/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5267 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/planning/actions.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.368270 pyrobosim-1.0.0/pyrobosim/planning/pddlstream/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      388 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/planning/pddlstream/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2800 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/planning/pddlstream/default_mappings.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4649 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/planning/pddlstream/planner.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7450 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/planning/pddlstream/primitives.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6837 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/planning/pddlstream/utils.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.368270 pyrobosim-1.0.0/pyrobosim/utils/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      209 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/utils/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2711 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/utils/general.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11921 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/utils/knowledge.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3610 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/utils/motion.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10605 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/utils/polygon.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8419 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/utils/pose.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6617 2023-07-06 16:46:54.000000 pyrobosim-1.0.0/pyrobosim/utils/search_graph.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-16 11:57:20.364269 pyrobosim-1.0.0/pyrobosim.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      282 2023-07-16 11:57:20.000000 pyrobosim-1.0.0/pyrobosim.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3048 2023-07-16 11:57:20.000000 pyrobosim-1.0.0/pyrobosim.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-16 11:57:20.000000 pyrobosim-1.0.0/pyrobosim.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       99 2023-07-16 11:57:20.000000 pyrobosim-1.0.0/pyrobosim.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       10 2023-07-16 11:57:20.000000 pyrobosim-1.0.0/pyrobosim.egg-info/top_level.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-06 16:52:33.000000 pyrobosim-1.0.0/pyrobosim.egg-info/zip-safe
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-16 11:57:20.368270 pyrobosim-1.0.0/setup.cfg
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1083 2023-07-16 11:55:05.000000 pyrobosim-1.0.0/setup.py
```

### Comparing `pyrobosim-0.0.0/pyrobosim/core/gazebo.py` & `pyrobosim-1.0.0/pyrobosim/core/gazebo.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/core/hallway.py` & `pyrobosim-1.0.0/pyrobosim/core/hallway.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/core/locations.py` & `pyrobosim-1.0.0/pyrobosim/core/locations.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/core/objects.py` & `pyrobosim-1.0.0/pyrobosim/core/objects.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/core/robot.py` & `pyrobosim-1.0.0/pyrobosim/core/robot.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/core/room.py` & `pyrobosim-1.0.0/pyrobosim/core/room.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/core/world.py` & `pyrobosim-1.0.0/pyrobosim/core/world.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/core/yaml_utils.py` & `pyrobosim-1.0.0/pyrobosim/core/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/example_location_data.yaml` & `pyrobosim-1.0.0/pyrobosim/data/example_location_data.yaml`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/example_object_data.yaml` & `pyrobosim-1.0.0/pyrobosim/data/example_object_data.yaml`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/01_simple/domain.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/01_simple/domain.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/02_derived/domain.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/02_derived/domain.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/domain.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/domain.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/streams.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/03_nav_stream/streams.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/domain.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/domain.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/streams.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/04_nav_manip_stream/streams.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/domain.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/domain.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/streams.pddl` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream/domains/05_nav_grasp_stream/streams.pddl`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/pddlstream_simple_world.yaml` & `pyrobosim-1.0.0/pyrobosim/data/pddlstream_simple_world.yaml`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/materials/textures/coke_can.png` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/materials/textures/coke_can.png`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/meshes/coke_can.dae` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/meshes/coke_can.dae`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model-1_2.sdf` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model-1_2.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model-1_3.sdf` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model-1_3.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model-1_4.sdf` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model-1_4.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/coke_can/model.sdf` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/coke_can/model.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/first_2015_trash_can/meshes/trash_can.dae` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/first_2015_trash_can/meshes/trash_can.dae`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/sample_models/first_2015_trash_can/model.sdf` & `pyrobosim-1.0.0/pyrobosim/data/sample_models/first_2015_trash_can/model.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/templates/link_template_polyline.sdf` & `pyrobosim-1.0.0/pyrobosim/data/templates/link_template_polyline.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/templates/world_template_gazebo.sdf` & `pyrobosim-1.0.0/pyrobosim/data/templates/world_template_gazebo.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/templates/world_template_ignition.sdf` & `pyrobosim-1.0.0/pyrobosim/data/templates/world_template_ignition.sdf`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/test_world.yaml` & `pyrobosim-1.0.0/pyrobosim/data/test_world.yaml`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/data/test_world_multirobot.yaml` & `pyrobosim-1.0.0/pyrobosim/data/test_world_multirobot.yaml`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/gui/main.py` & `pyrobosim-1.0.0/pyrobosim/gui/main.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/gui/world_canvas.py` & `pyrobosim-1.0.0/pyrobosim/gui/world_canvas.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/manipulation/grasping.py` & `pyrobosim-1.0.0/pyrobosim/manipulation/grasping.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/a_star.py` & `pyrobosim-1.0.0/pyrobosim/navigation/a_star.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/execution.py` & `pyrobosim-1.0.0/pyrobosim/navigation/execution.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/occupancy_grid.py` & `pyrobosim-1.0.0/pyrobosim/navigation/occupancy_grid.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/path_planner.py` & `pyrobosim-1.0.0/pyrobosim/navigation/path_planner.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/planner_base.py` & `pyrobosim-1.0.0/pyrobosim/navigation/planner_base.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/prm.py` & `pyrobosim-1.0.0/pyrobosim/navigation/prm.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/rrt.py` & `pyrobosim-1.0.0/pyrobosim/navigation/rrt.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/trajectory.py` & `pyrobosim-1.0.0/pyrobosim/navigation/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/navigation/world_graph.py` & `pyrobosim-1.0.0/pyrobosim/navigation/world_graph.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/planning/actions.py` & `pyrobosim-1.0.0/pyrobosim/planning/actions.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/planning/pddlstream/default_mappings.py` & `pyrobosim-1.0.0/pyrobosim/planning/pddlstream/default_mappings.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/planning/pddlstream/planner.py` & `pyrobosim-1.0.0/pyrobosim/planning/pddlstream/planner.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/planning/pddlstream/primitives.py` & `pyrobosim-1.0.0/pyrobosim/planning/pddlstream/primitives.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/planning/pddlstream/utils.py` & `pyrobosim-1.0.0/pyrobosim/planning/pddlstream/utils.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/utils/general.py` & `pyrobosim-1.0.0/pyrobosim/utils/general.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/utils/knowledge.py` & `pyrobosim-1.0.0/pyrobosim/utils/knowledge.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/utils/motion.py` & `pyrobosim-1.0.0/pyrobosim/utils/motion.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/utils/polygon.py` & `pyrobosim-1.0.0/pyrobosim/utils/polygon.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/utils/pose.py` & `pyrobosim-1.0.0/pyrobosim/utils/pose.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim/utils/search_graph.py` & `pyrobosim-1.0.0/pyrobosim/utils/search_graph.py`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/pyrobosim.egg-info/SOURCES.txt` & `pyrobosim-1.0.0/pyrobosim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrobosim-0.0.0/setup.py` & `pyrobosim-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "transforms3d",
     "trimesh",
 ]
 
 project_name = "pyrobosim"
 setup(
     name=project_name,
-    version="0.0.0",
+    version="1.0.0",
     url="https://github.com/sea-bass/pyrobosim",
     author="Sebastian Castro",
     author_email="sebas.a.castro@gmail.com",
     description="ROS 2 enabled 2D mobile robot simulator for behavior prototyping.",
     license="MIT",
     install_requires=install_requires,
     packages=find_packages(),
```

