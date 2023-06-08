# Comparing `tmp/magnebot-2.2.5.tar.gz` & `tmp/magnebot-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\magnebot-2.2.5.tar", last modified: Mon Feb 27 13:49:34 2023, max compression
+gzip compressed data, was "dist\magnebot-2.2.6.tar", last modified: Thu Jun  8 19:46:46 2023, max compression
```

## Comparing `magnebot-2.2.5.tar` & `magnebot-2.2.6.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/
--rw-rw-rw-   0        0        0     1067 2021-01-19 21:11:44.000000 magnebot-2.2.5/LICENSE
--rw-rw-rw-   0        0        0       30 2021-02-10 14:04:58.000000 magnebot-2.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0    10042 2023-02-27 13:49:34.000000 magnebot-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     7464 2022-10-12 13:19:44.000000 magnebot-2.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/
--rw-rw-rw-   0        0        0      244 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/__pycache__/
--rw-rw-rw-   0        0        0      451 2022-01-12 13:39:00.000000 magnebot-2.2.5/magnebot/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1990 2022-01-12 13:39:00.000000 magnebot-2.2.5/magnebot/__pycache__/action_status.cpython-37.pyc
--rw-rw-rw-   0        0        0     3315 2022-07-27 15:43:59.000000 magnebot-2.2.5/magnebot/__pycache__/add_on.cpython-37.pyc
--rw-rw-rw-   0        0        0      535 2021-05-04 13:48:56.000000 magnebot-2.2.5/magnebot/__pycache__/arm.cpython-37.pyc
--rw-rw-rw-   0        0        0      557 2021-05-04 13:48:56.000000 magnebot-2.2.5/magnebot/__pycache__/arm_joint.cpython-37.pyc
--rw-rw-rw-   0        0        0      549 2021-11-09 16:01:25.000000 magnebot-2.2.5/magnebot/__pycache__/collision_action.cpython-37.pyc
--rw-rw-rw-   0        0        0     1711 2022-01-12 13:39:00.000000 magnebot-2.2.5/magnebot/__pycache__/collision_detection.cpython-37.pyc
--rw-rw-rw-   0        0        0     4654 2021-08-10 14:20:28.000000 magnebot-2.2.5/magnebot/__pycache__/collisions.cpython-37.pyc
--rw-rw-rw-   0        0        0      945 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/__pycache__/constants.cpython-37.pyc
--rw-rw-rw-   0        0        0    21136 2022-07-27 15:59:38.000000 magnebot-2.2.5/magnebot/__pycache__/controller.cpython-37.pyc
--rw-rw-rw-   0        0        0     1129 2021-11-09 16:01:25.000000 magnebot-2.2.5/magnebot/__pycache__/drive.cpython-37.pyc
--rw-rw-rw-   0        0        0      455 2022-01-12 13:39:00.000000 magnebot-2.2.5/magnebot/__pycache__/image_frequency.cpython-37.pyc
--rw-rw-rw-   0        0        0     1196 2021-11-09 16:01:25.000000 magnebot-2.2.5/magnebot/__pycache__/joint_static.cpython-37.pyc
--rw-rw-rw-   0        0        0      443 2021-11-09 16:01:25.000000 magnebot-2.2.5/magnebot/__pycache__/joint_type.cpython-37.pyc
--rw-rw-rw-   0        0        0    24085 2023-02-14 14:00:21.000000 magnebot-2.2.5/magnebot/__pycache__/magnebot.cpython-37.pyc
--rw-rw-rw-   0        0        0    23183 2022-10-12 17:05:45.000000 magnebot-2.2.5/magnebot/__pycache__/magnebot_controller.cpython-37.pyc
--rw-rw-rw-   0        0        0     5367 2022-07-27 17:20:12.000000 magnebot-2.2.5/magnebot/__pycache__/magnebot_dynamic.cpython-37.pyc
--rw-rw-rw-   0        0        0     2033 2022-01-12 13:39:00.000000 magnebot-2.2.5/magnebot/__pycache__/magnebot_static.cpython-37.pyc
--rw-rw-rw-   0        0        0     2531 2021-11-09 16:01:25.000000 magnebot-2.2.5/magnebot/__pycache__/object_static.cpython-37.pyc
--rw-rw-rw-   0        0        0      916 2021-10-12 13:04:14.000000 magnebot-2.2.5/magnebot/__pycache__/paths.cpython-37.pyc
--rw-rw-rw-   0        0        0     7401 2022-07-27 15:59:38.000000 magnebot-2.2.5/magnebot/__pycache__/robot.cpython-37.pyc
--rw-rw-rw-   0        0        0     5149 2022-06-21 19:47:16.000000 magnebot-2.2.5/magnebot/__pycache__/robot_base.cpython-37.pyc
--rw-rw-rw-   0        0        0     2681 2022-12-09 14:43:14.000000 magnebot-2.2.5/magnebot/__pycache__/robot_dynamic.cpython-37.pyc
--rw-rw-rw-   0        0        0     1892 2022-12-09 14:43:14.000000 magnebot-2.2.5/magnebot/__pycache__/robot_static.cpython-37.pyc
--rw-rw-rw-   0        0        0     2430 2021-08-10 14:20:28.000000 magnebot-2.2.5/magnebot/__pycache__/scene_environment.cpython-37.pyc
--rw-rw-rw-   0        0        0     5638 2021-11-09 18:09:08.000000 magnebot-2.2.5/magnebot/__pycache__/scene_state.cpython-37.pyc
--rw-rw-rw-   0        0        0     1155 2021-09-03 19:03:55.000000 magnebot-2.2.5/magnebot/__pycache__/skip_frames.cpython-37.pyc
--rw-rw-rw-   0        0        0     1993 2021-10-11 15:50:03.000000 magnebot-2.2.5/magnebot/__pycache__/test_controller.cpython-37.pyc
--rw-rw-rw-   0        0        0      872 2021-11-09 16:01:25.000000 magnebot-2.2.5/magnebot/__pycache__/transform.cpython-37.pyc
--rw-rw-rw-   0        0        0     1068 2021-08-12 13:26:54.000000 magnebot-2.2.5/magnebot/__pycache__/turn_constants.cpython-37.pyc
--rw-rw-rw-   0        0        0     2881 2022-11-08 19:46:52.000000 magnebot-2.2.5/magnebot/__pycache__/util.cpython-37.pyc
--rw-rw-rw-   0        0        0      496 2021-05-04 13:48:56.000000 magnebot-2.2.5/magnebot/__pycache__/wheel.cpython-37.pyc
--rw-rw-rw-   0        0        0     2638 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/action_status.py
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/actions/
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/actions/__pycache__/
--rw-rw-rw-   0        0        0     8978 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/action.cpython-37.pyc
--rw-rw-rw-   0        0        0     4352 2021-08-10 14:20:28.000000 magnebot-2.2.5/magnebot/actions/__pycache__/arm_action.cpython-37.pyc
--rw-rw-rw-   0        0        0     2480 2023-02-14 13:55:33.000000 magnebot-2.2.5/magnebot/actions/__pycache__/arm_motion.cpython-37.pyc
--rw-rw-rw-   0        0        0     1126 2022-01-12 13:39:02.000000 magnebot-2.2.5/magnebot/actions/__pycache__/camera_action.cpython-37.pyc
--rw-rw-rw-   0        0        0     3544 2023-02-14 13:55:33.000000 magnebot-2.2.5/magnebot/actions/__pycache__/drop.cpython-37.pyc
--rw-rw-rw-   0        0        0     7268 2023-02-14 13:55:33.000000 magnebot-2.2.5/magnebot/actions/__pycache__/grasp.cpython-37.pyc
--rw-rw-rw-   0        0        0    11414 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/ik_motion.cpython-37.pyc
--rw-rw-rw-   0        0        0     2564 2022-10-12 17:06:49.000000 magnebot-2.2.5/magnebot/actions/__pycache__/look_at.cpython-37.pyc
--rw-rw-rw-   0        0        0     4575 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/move_by.cpython-37.pyc
--rw-rw-rw-   0        0        0     2130 2022-10-12 17:06:49.000000 magnebot-2.2.5/magnebot/actions/__pycache__/move_camera.cpython-37.pyc
--rw-rw-rw-   0        0        0     4123 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/move_to.cpython-37.pyc
--rw-rw-rw-   0        0        0     4372 2021-05-13 15:30:39.000000 magnebot-2.2.5/magnebot/actions/__pycache__/navigate.cpython-37.pyc
--rw-rw-rw-   0        0        0     3771 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/reach_for.cpython-37.pyc
--rw-rw-rw-   0        0        0     1432 2022-01-12 13:39:02.000000 magnebot-2.2.5/magnebot/actions/__pycache__/reset_arm.cpython-37.pyc
--rw-rw-rw-   0        0        0     2244 2022-10-12 17:06:49.000000 magnebot-2.2.5/magnebot/actions/__pycache__/reset_camera.cpython-37.pyc
--rw-rw-rw-   0        0        0     4802 2023-02-14 13:55:33.000000 magnebot-2.2.5/magnebot/actions/__pycache__/reset_position.cpython-37.pyc
--rw-rw-rw-   0        0        0     2633 2022-10-12 17:06:49.000000 magnebot-2.2.5/magnebot/actions/__pycache__/rotate_camera.cpython-37.pyc
--rw-rw-rw-   0        0        0     2112 2023-02-14 13:55:33.000000 magnebot-2.2.5/magnebot/actions/__pycache__/slide_torso.cpython-37.pyc
--rw-rw-rw-   0        0        0     1813 2023-02-14 13:55:33.000000 magnebot-2.2.5/magnebot/actions/__pycache__/stop.cpython-37.pyc
--rw-rw-rw-   0        0        0     6169 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/turn.cpython-37.pyc
--rw-rw-rw-   0        0        0     2313 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/turn_by.cpython-37.pyc
--rw-rw-rw-   0        0        0     3159 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/turn_to.cpython-37.pyc
--rw-rw-rw-   0        0        0     1540 2022-01-12 13:39:02.000000 magnebot-2.2.5/magnebot/actions/__pycache__/wait.cpython-37.pyc
--rw-rw-rw-   0        0        0     1090 2021-08-10 14:20:28.000000 magnebot-2.2.5/magnebot/actions/__pycache__/wait_for_joints.cpython-37.pyc
--rw-rw-rw-   0        0        0      503 2021-05-07 20:15:19.000000 magnebot-2.2.5/magnebot/actions/__pycache__/wheel_action_state.cpython-37.pyc
--rw-rw-rw-   0        0        0     9700 2023-02-14 13:55:31.000000 magnebot-2.2.5/magnebot/actions/__pycache__/wheel_motion.cpython-37.pyc
--rw-rw-rw-   0        0        0    12701 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/action.py
--rw-rw-rw-   0        0        0     2423 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/arm_motion.py
--rw-rw-rw-   0        0        0      577 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/actions/camera_action.py
--rw-rw-rw-   0        0        0     3892 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/drop.py
--rw-rw-rw-   0        0        0    13060 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/grasp.py
--rw-rw-rw-   0        0        0    19121 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/ik_motion.py
--rw-rw-rw-   0        0        0     2636 2022-10-12 13:19:44.000000 magnebot-2.2.5/magnebot/actions/look_at.py
--rw-rw-rw-   0        0        0     7500 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/move_by.py
--rw-rw-rw-   0        0        0     1738 2022-10-12 13:19:44.000000 magnebot-2.2.5/magnebot/actions/move_camera.py
--rw-rw-rw-   0        0        0     5808 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/move_to.py
--rw-rw-rw-   0        0        0     3483 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/reach_for.py
--rw-rw-rw-   0        0        0     1114 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/actions/reset_arm.py
--rw-rw-rw-   0        0        0     2054 2022-10-12 13:19:44.000000 magnebot-2.2.5/magnebot/actions/reset_camera.py
--rw-rw-rw-   0        0        0     8158 2023-02-10 19:24:46.000000 magnebot-2.2.5/magnebot/actions/reset_position.py
--rw-rw-rw-   0        0        0     3006 2022-10-12 13:19:44.000000 magnebot-2.2.5/magnebot/actions/rotate_camera.py
--rw-rw-rw-   0        0        0     2058 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/slide_torso.py
--rw-rw-rw-   0        0        0     1526 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/stop.py
--rw-rw-rw-   0        0        0     8847 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/turn.py
--rw-rw-rw-   0        0        0     1951 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/turn_by.py
--rw-rw-rw-   0        0        0     3507 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/turn_to.py
--rw-rw-rw-   0        0        0     1377 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/actions/wait.py
--rw-rw-rw-   0        0        0    12937 2023-01-24 15:05:03.000000 magnebot-2.2.5/magnebot/actions/wheel_motion.py
--rw-rw-rw-   0        0        0      306 2020-11-25 16:20:23.000000 magnebot-2.2.5/magnebot/arm.py
--rw-rw-rw-   0        0        0      261 2020-12-02 18:33:37.000000 magnebot-2.2.5/magnebot/arm_joint.py
--rw-rw-rw-   0        0        0     2720 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/collision_detection.py
--rw-rw-rw-   0        0        0     1460 2023-02-27 13:49:23.000000 magnebot-2.2.5/magnebot/constants.py
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/data/
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/data/magnebot/
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/data/magnebot/ik/
--rw-rw-rw-   0        0        0    20352 2021-10-12 12:54:07.000000 magnebot-2.2.5/magnebot/data/magnebot/ik/orientations_left.npy
--rw-rw-rw-   0        0        0    20352 2021-10-12 12:54:07.000000 magnebot-2.2.5/magnebot/data/magnebot/ik/orientations_right.npy
--rw-rw-rw-   0        0        0   121472 2021-10-12 12:54:07.000000 magnebot-2.2.5/magnebot/data/magnebot/ik/positions.npy
--rw-rw-rw-   0        0        0      143 2021-08-11 14:32:23.000000 magnebot-2.2.5/magnebot/data/magnebot/turn_constants.csv
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/data/objects/
--rw-rw-rw-   0        0        0    10044 2020-11-25 14:56:13.000000 magnebot-2.2.5/magnebot/data/objects/categories.json
--rw-rw-rw-   0        0        0    89636 2021-10-12 12:54:07.000000 magnebot-2.2.5/magnebot/data/objects/convex.json
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/data/scenes/
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/
--rw-rw-rw-   0        0        0     4968 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/1_0.npy
--rw-rw-rw-   0        0        0     4968 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/1_1.npy
--rw-rw-rw-   0        0        0     4968 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/1_2.npy
--rw-rw-rw-   0        0        0     3488 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/2_0.npy
--rw-rw-rw-   0        0        0     3488 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/2_1.npy
--rw-rw-rw-   0        0        0     3488 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/2_2.npy
--rw-rw-rw-   0        0        0     3072 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/4_0.npy
--rw-rw-rw-   0        0        0     3072 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/4_1.npy
--rw-rw-rw-   0        0        0     3072 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/4_2.npy
--rw-rw-rw-   0        0        0     4176 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/5_0.npy
--rw-rw-rw-   0        0        0     4176 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/5_1.npy
--rw-rw-rw-   0        0        0     4176 2021-04-30 14:53:42.000000 magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/5_2.npy
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/data/scenes/room_maps/
--rw-rw-rw-   0        0        0     4968 2021-01-06 17:43:53.000000 magnebot-2.2.5/magnebot/data/scenes/room_maps/1.npy
--rw-rw-rw-   0        0        0     3488 2021-01-06 17:44:56.000000 magnebot-2.2.5/magnebot/data/scenes/room_maps/2.npy
--rw-rw-rw-   0        0        0     3072 2021-01-06 17:45:28.000000 magnebot-2.2.5/magnebot/data/scenes/room_maps/4.npy
--rw-rw-rw-   0        0        0     4176 2021-01-06 17:45:59.000000 magnebot-2.2.5/magnebot/data/scenes/room_maps/5.npy
--rw-rw-rw-   0        0        0     8775 2021-01-07 18:05:52.000000 magnebot-2.2.5/magnebot/data/scenes/spawn_positions.json
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/ik/
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/ik/__pycache__/
--rw-rw-rw-   0        0        0     1506 2022-01-12 13:39:02.000000 magnebot-2.2.5/magnebot/ik/__pycache__/orientation.cpython-37.pyc
--rw-rw-rw-   0        0        0      465 2022-01-12 13:39:00.000000 magnebot-2.2.5/magnebot/ik/__pycache__/orientation_mode.cpython-37.pyc
--rw-rw-rw-   0        0        0      507 2022-01-12 13:39:00.000000 magnebot-2.2.5/magnebot/ik/__pycache__/target_orientation.cpython-37.pyc
--rw-rw-rw-   0        0        0     2972 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/ik/orientation.py
--rw-rw-rw-   0        0        0      299 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/ik/orientation_mode.py
--rw-rw-rw-   0        0        0      387 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/ik/target_orientation.py
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/ikpy/
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot/ikpy/__pycache__/
--rw-rw-rw-   0        0        0     7177 2021-10-12 13:04:14.000000 magnebot-2.2.5/magnebot/ikpy/__pycache__/link.cpython-37.pyc
--rw-rw-rw-   0        0        0     7957 2021-10-12 12:54:07.000000 magnebot-2.2.5/magnebot/ikpy/link.py
--rw-rw-rw-   0        0        0       40 2021-10-12 12:54:07.000000 magnebot-2.2.5/magnebot/ikpy/source.txt
--rw-rw-rw-   0        0        0      272 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/image_frequency.py
--rw-rw-rw-   0        0        0    30148 2023-02-27 13:49:23.000000 magnebot-2.2.5/magnebot/magnebot.py
--rw-rw-rw-   0        0        0    27562 2022-10-12 13:19:44.000000 magnebot-2.2.5/magnebot/magnebot_controller.py
--rw-rw-rw-   0        0        0     8235 2022-07-27 16:03:57.000000 magnebot-2.2.5/magnebot/magnebot_dynamic.py
--rw-rw-rw-   0        0        0     2423 2021-12-14 15:49:38.000000 magnebot-2.2.5/magnebot/magnebot_static.py
--rw-rw-rw-   0        0        0     1636 2021-10-12 12:54:07.000000 magnebot-2.2.5/magnebot/paths.py
--rw-rw-rw-   0        0        0     1100 2021-08-11 14:32:23.000000 magnebot-2.2.5/magnebot/turn_constants.py
--rw-rw-rw-   0        0        0     3432 2022-11-08 19:40:07.000000 magnebot-2.2.5/magnebot/util.py
--rw-rw-rw-   0        0        0      216 2020-12-03 19:23:54.000000 magnebot-2.2.5/magnebot/wheel.py
-drwxrwxrwx   0        0        0        0 2023-02-27 13:49:34.000000 magnebot-2.2.5/magnebot.egg-info/
--rw-rw-rw-   0        0        0    10042 2023-02-27 13:49:33.000000 magnebot-2.2.5/magnebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5458 2023-02-27 13:49:33.000000 magnebot-2.2.5/magnebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 13:49:33.000000 magnebot-2.2.5/magnebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-02-27 13:49:33.000000 magnebot-2.2.5/magnebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-27 13:49:33.000000 magnebot-2.2.5/magnebot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-27 13:49:34.000000 magnebot-2.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1467 2023-02-27 13:49:23.000000 magnebot-2.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/
+-rw-rw-rw-   0        0        0     1067 2021-01-19 21:11:44.000000 magnebot-2.2.6/LICENSE
+-rw-rw-rw-   0        0        0       30 2021-02-10 14:04:58.000000 magnebot-2.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    10042 2023-06-08 19:46:46.000000 magnebot-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7464 2022-10-12 13:19:44.000000 magnebot-2.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot/
+-rw-rw-rw-   0        0        0      244 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot/__pycache__/
+-rw-rw-rw-   0        0        0      451 2022-01-12 13:39:00.000000 magnebot-2.2.6/magnebot/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1990 2022-01-12 13:39:00.000000 magnebot-2.2.6/magnebot/__pycache__/action_status.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3315 2022-07-27 15:43:59.000000 magnebot-2.2.6/magnebot/__pycache__/add_on.cpython-37.pyc
+-rw-rw-rw-   0        0        0      535 2021-05-04 13:48:56.000000 magnebot-2.2.6/magnebot/__pycache__/arm.cpython-37.pyc
+-rw-rw-rw-   0        0        0      557 2021-05-04 13:48:56.000000 magnebot-2.2.6/magnebot/__pycache__/arm_joint.cpython-37.pyc
+-rw-rw-rw-   0        0        0      549 2021-11-09 16:01:25.000000 magnebot-2.2.6/magnebot/__pycache__/collision_action.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1711 2022-01-12 13:39:00.000000 magnebot-2.2.6/magnebot/__pycache__/collision_detection.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4654 2021-08-10 14:20:28.000000 magnebot-2.2.6/magnebot/__pycache__/collisions.cpython-37.pyc
+-rw-rw-rw-   0        0        0      945 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/__pycache__/constants.cpython-37.pyc
+-rw-rw-rw-   0        0        0    21136 2022-07-27 15:59:38.000000 magnebot-2.2.6/magnebot/__pycache__/controller.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1129 2021-11-09 16:01:25.000000 magnebot-2.2.6/magnebot/__pycache__/drive.cpython-37.pyc
+-rw-rw-rw-   0        0        0      455 2022-01-12 13:39:00.000000 magnebot-2.2.6/magnebot/__pycache__/image_frequency.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1196 2021-11-09 16:01:25.000000 magnebot-2.2.6/magnebot/__pycache__/joint_static.cpython-37.pyc
+-rw-rw-rw-   0        0        0      443 2021-11-09 16:01:25.000000 magnebot-2.2.6/magnebot/__pycache__/joint_type.cpython-37.pyc
+-rw-rw-rw-   0        0        0    24085 2023-02-14 14:00:21.000000 magnebot-2.2.6/magnebot/__pycache__/magnebot.cpython-37.pyc
+-rw-rw-rw-   0        0        0    23183 2022-10-12 17:05:45.000000 magnebot-2.2.6/magnebot/__pycache__/magnebot_controller.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5367 2022-07-27 17:20:12.000000 magnebot-2.2.6/magnebot/__pycache__/magnebot_dynamic.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2033 2022-01-12 13:39:00.000000 magnebot-2.2.6/magnebot/__pycache__/magnebot_static.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2531 2021-11-09 16:01:25.000000 magnebot-2.2.6/magnebot/__pycache__/object_static.cpython-37.pyc
+-rw-rw-rw-   0        0        0      916 2021-10-12 13:04:14.000000 magnebot-2.2.6/magnebot/__pycache__/paths.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7401 2022-07-27 15:59:38.000000 magnebot-2.2.6/magnebot/__pycache__/robot.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5149 2022-06-21 19:47:16.000000 magnebot-2.2.6/magnebot/__pycache__/robot_base.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2681 2022-12-09 14:43:14.000000 magnebot-2.2.6/magnebot/__pycache__/robot_dynamic.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1892 2022-12-09 14:43:14.000000 magnebot-2.2.6/magnebot/__pycache__/robot_static.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2430 2021-08-10 14:20:28.000000 magnebot-2.2.6/magnebot/__pycache__/scene_environment.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5638 2021-11-09 18:09:08.000000 magnebot-2.2.6/magnebot/__pycache__/scene_state.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1155 2021-09-03 19:03:55.000000 magnebot-2.2.6/magnebot/__pycache__/skip_frames.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1993 2021-10-11 15:50:03.000000 magnebot-2.2.6/magnebot/__pycache__/test_controller.cpython-37.pyc
+-rw-rw-rw-   0        0        0      872 2021-11-09 16:01:25.000000 magnebot-2.2.6/magnebot/__pycache__/transform.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1068 2021-08-12 13:26:54.000000 magnebot-2.2.6/magnebot/__pycache__/turn_constants.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2881 2022-11-08 19:46:52.000000 magnebot-2.2.6/magnebot/__pycache__/util.cpython-37.pyc
+-rw-rw-rw-   0        0        0      496 2021-05-04 13:48:56.000000 magnebot-2.2.6/magnebot/__pycache__/wheel.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2638 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/action_status.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/actions/
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/actions/__pycache__/
+-rw-rw-rw-   0        0        0     8978 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/action.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4352 2021-08-10 14:20:28.000000 magnebot-2.2.6/magnebot/actions/__pycache__/arm_action.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2480 2023-02-14 13:55:33.000000 magnebot-2.2.6/magnebot/actions/__pycache__/arm_motion.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1126 2022-01-12 13:39:02.000000 magnebot-2.2.6/magnebot/actions/__pycache__/camera_action.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3544 2023-02-14 13:55:33.000000 magnebot-2.2.6/magnebot/actions/__pycache__/drop.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7268 2023-02-14 13:55:33.000000 magnebot-2.2.6/magnebot/actions/__pycache__/grasp.cpython-37.pyc
+-rw-rw-rw-   0        0        0    11414 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/ik_motion.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2564 2022-10-12 17:06:49.000000 magnebot-2.2.6/magnebot/actions/__pycache__/look_at.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4575 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/move_by.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2130 2022-10-12 17:06:49.000000 magnebot-2.2.6/magnebot/actions/__pycache__/move_camera.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4123 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/move_to.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4372 2021-05-13 15:30:39.000000 magnebot-2.2.6/magnebot/actions/__pycache__/navigate.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3771 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/reach_for.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1432 2022-01-12 13:39:02.000000 magnebot-2.2.6/magnebot/actions/__pycache__/reset_arm.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2244 2022-10-12 17:06:49.000000 magnebot-2.2.6/magnebot/actions/__pycache__/reset_camera.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4802 2023-02-14 13:55:33.000000 magnebot-2.2.6/magnebot/actions/__pycache__/reset_position.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2633 2022-10-12 17:06:49.000000 magnebot-2.2.6/magnebot/actions/__pycache__/rotate_camera.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2112 2023-02-14 13:55:33.000000 magnebot-2.2.6/magnebot/actions/__pycache__/slide_torso.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1813 2023-02-14 13:55:33.000000 magnebot-2.2.6/magnebot/actions/__pycache__/stop.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6169 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/turn.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2313 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/turn_by.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3159 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/turn_to.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1540 2022-01-12 13:39:02.000000 magnebot-2.2.6/magnebot/actions/__pycache__/wait.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1090 2021-08-10 14:20:28.000000 magnebot-2.2.6/magnebot/actions/__pycache__/wait_for_joints.cpython-37.pyc
+-rw-rw-rw-   0        0        0      503 2021-05-07 20:15:19.000000 magnebot-2.2.6/magnebot/actions/__pycache__/wheel_action_state.cpython-37.pyc
+-rw-rw-rw-   0        0        0     9700 2023-02-14 13:55:31.000000 magnebot-2.2.6/magnebot/actions/__pycache__/wheel_motion.cpython-37.pyc
+-rw-rw-rw-   0        0        0    12701 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/action.py
+-rw-rw-rw-   0        0        0     2423 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/arm_motion.py
+-rw-rw-rw-   0        0        0      577 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/actions/camera_action.py
+-rw-rw-rw-   0        0        0     3892 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/drop.py
+-rw-rw-rw-   0        0        0    13060 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/grasp.py
+-rw-rw-rw-   0        0        0    19121 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/ik_motion.py
+-rw-rw-rw-   0        0        0     2636 2022-10-12 13:19:44.000000 magnebot-2.2.6/magnebot/actions/look_at.py
+-rw-rw-rw-   0        0        0     7500 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/move_by.py
+-rw-rw-rw-   0        0        0     1738 2022-10-12 13:19:44.000000 magnebot-2.2.6/magnebot/actions/move_camera.py
+-rw-rw-rw-   0        0        0     5808 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/move_to.py
+-rw-rw-rw-   0        0        0     3483 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/reach_for.py
+-rw-rw-rw-   0        0        0     1114 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/actions/reset_arm.py
+-rw-rw-rw-   0        0        0     2054 2022-10-12 13:19:44.000000 magnebot-2.2.6/magnebot/actions/reset_camera.py
+-rw-rw-rw-   0        0        0     8158 2023-02-10 19:24:46.000000 magnebot-2.2.6/magnebot/actions/reset_position.py
+-rw-rw-rw-   0        0        0     3006 2022-10-12 13:19:44.000000 magnebot-2.2.6/magnebot/actions/rotate_camera.py
+-rw-rw-rw-   0        0        0     2058 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/slide_torso.py
+-rw-rw-rw-   0        0        0     1526 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/stop.py
+-rw-rw-rw-   0        0        0     8847 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/turn.py
+-rw-rw-rw-   0        0        0     1951 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/turn_by.py
+-rw-rw-rw-   0        0        0     3507 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/turn_to.py
+-rw-rw-rw-   0        0        0     1377 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/actions/wait.py
+-rw-rw-rw-   0        0        0    12937 2023-01-24 15:05:03.000000 magnebot-2.2.6/magnebot/actions/wheel_motion.py
+-rw-rw-rw-   0        0        0      306 2020-11-25 16:20:23.000000 magnebot-2.2.6/magnebot/arm.py
+-rw-rw-rw-   0        0        0      261 2020-12-02 18:33:37.000000 magnebot-2.2.6/magnebot/arm_joint.py
+-rw-rw-rw-   0        0        0     2720 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/collision_detection.py
+-rw-rw-rw-   0        0        0     1461 2023-06-08 13:20:55.000000 magnebot-2.2.6/magnebot/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot/data/
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/data/magnebot/
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/data/magnebot/ik/
+-rw-rw-rw-   0        0        0    20352 2021-10-12 12:54:07.000000 magnebot-2.2.6/magnebot/data/magnebot/ik/orientations_left.npy
+-rw-rw-rw-   0        0        0    20352 2021-10-12 12:54:07.000000 magnebot-2.2.6/magnebot/data/magnebot/ik/orientations_right.npy
+-rw-rw-rw-   0        0        0   121472 2021-10-12 12:54:07.000000 magnebot-2.2.6/magnebot/data/magnebot/ik/positions.npy
+-rw-rw-rw-   0        0        0      143 2021-08-11 14:32:23.000000 magnebot-2.2.6/magnebot/data/magnebot/turn_constants.csv
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/data/objects/
+-rw-rw-rw-   0        0        0    10044 2020-11-25 14:56:13.000000 magnebot-2.2.6/magnebot/data/objects/categories.json
+-rw-rw-rw-   0        0        0    89636 2021-10-12 12:54:07.000000 magnebot-2.2.6/magnebot/data/objects/convex.json
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/data/scenes/
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/
+-rw-rw-rw-   0        0        0     4968 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/1_0.npy
+-rw-rw-rw-   0        0        0     4968 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/1_1.npy
+-rw-rw-rw-   0        0        0     4968 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/1_2.npy
+-rw-rw-rw-   0        0        0     3488 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/2_0.npy
+-rw-rw-rw-   0        0        0     3488 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/2_1.npy
+-rw-rw-rw-   0        0        0     3488 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/2_2.npy
+-rw-rw-rw-   0        0        0     3072 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/4_0.npy
+-rw-rw-rw-   0        0        0     3072 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/4_1.npy
+-rw-rw-rw-   0        0        0     3072 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/4_2.npy
+-rw-rw-rw-   0        0        0     4176 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/5_0.npy
+-rw-rw-rw-   0        0        0     4176 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/5_1.npy
+-rw-rw-rw-   0        0        0     4176 2021-04-30 14:53:42.000000 magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/5_2.npy
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/data/scenes/room_maps/
+-rw-rw-rw-   0        0        0     4968 2021-01-06 17:43:53.000000 magnebot-2.2.6/magnebot/data/scenes/room_maps/1.npy
+-rw-rw-rw-   0        0        0     3488 2021-01-06 17:44:56.000000 magnebot-2.2.6/magnebot/data/scenes/room_maps/2.npy
+-rw-rw-rw-   0        0        0     3072 2021-01-06 17:45:28.000000 magnebot-2.2.6/magnebot/data/scenes/room_maps/4.npy
+-rw-rw-rw-   0        0        0     4176 2021-01-06 17:45:59.000000 magnebot-2.2.6/magnebot/data/scenes/room_maps/5.npy
+-rw-rw-rw-   0        0        0     8775 2021-01-07 18:05:52.000000 magnebot-2.2.6/magnebot/data/scenes/spawn_positions.json
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/ik/
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/ik/__pycache__/
+-rw-rw-rw-   0        0        0     1506 2022-01-12 13:39:02.000000 magnebot-2.2.6/magnebot/ik/__pycache__/orientation.cpython-37.pyc
+-rw-rw-rw-   0        0        0      465 2022-01-12 13:39:00.000000 magnebot-2.2.6/magnebot/ik/__pycache__/orientation_mode.cpython-37.pyc
+-rw-rw-rw-   0        0        0      507 2022-01-12 13:39:00.000000 magnebot-2.2.6/magnebot/ik/__pycache__/target_orientation.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2972 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/ik/orientation.py
+-rw-rw-rw-   0        0        0      299 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/ik/orientation_mode.py
+-rw-rw-rw-   0        0        0      387 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/ik/target_orientation.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/ikpy/
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:46.000000 magnebot-2.2.6/magnebot/ikpy/__pycache__/
+-rw-rw-rw-   0        0        0     7177 2021-10-12 13:04:14.000000 magnebot-2.2.6/magnebot/ikpy/__pycache__/link.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7957 2021-10-12 12:54:07.000000 magnebot-2.2.6/magnebot/ikpy/link.py
+-rw-rw-rw-   0        0        0       40 2021-10-12 12:54:07.000000 magnebot-2.2.6/magnebot/ikpy/source.txt
+-rw-rw-rw-   0        0        0      272 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/image_frequency.py
+-rw-rw-rw-   0        0        0    30112 2023-06-08 13:19:14.000000 magnebot-2.2.6/magnebot/magnebot.py
+-rw-rw-rw-   0        0        0    27562 2022-10-12 13:19:44.000000 magnebot-2.2.6/magnebot/magnebot_controller.py
+-rw-rw-rw-   0        0        0     8235 2022-07-27 16:03:57.000000 magnebot-2.2.6/magnebot/magnebot_dynamic.py
+-rw-rw-rw-   0        0        0     2423 2021-12-14 15:49:38.000000 magnebot-2.2.6/magnebot/magnebot_static.py
+-rw-rw-rw-   0        0        0     1636 2021-10-12 12:54:07.000000 magnebot-2.2.6/magnebot/paths.py
+-rw-rw-rw-   0        0        0     1100 2021-08-11 14:32:23.000000 magnebot-2.2.6/magnebot/turn_constants.py
+-rw-rw-rw-   0        0        0     3432 2022-11-08 19:40:07.000000 magnebot-2.2.6/magnebot/util.py
+-rw-rw-rw-   0        0        0      216 2020-12-03 19:23:54.000000 magnebot-2.2.6/magnebot/wheel.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot.egg-info/
+-rw-rw-rw-   0        0        0    10042 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5458 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 19:46:45.000000 magnebot-2.2.6/magnebot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 19:46:46.000000 magnebot-2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-06-08 13:20:55.000000 magnebot-2.2.6/setup.py
```

### Comparing `magnebot-2.2.5/LICENSE` & `magnebot-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/PKG-INFO` & `magnebot-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnebot
-Version: 2.2.5
+Version: 2.2.6
 Summary: High-level API for the Magnebot in TDW.
 Home-page: https://github.com/alters-mit/magnebot
 Author: Esther Alter
 Author-email: alters@mit.edu
 License: MIT
 Keywords: unity simulation tdw robotics
 Platform: UNKNOWN
```

### Comparing `magnebot-2.2.5/README.md` & `magnebot-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/action_status.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/action_status.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/add_on.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/add_on.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/arm.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/arm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/arm_joint.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/arm_joint.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/collision_action.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/collision_action.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/collision_detection.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/collision_detection.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/collisions.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/collisions.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/constants.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/constants.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/controller.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/controller.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/drive.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/drive.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/joint_static.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/joint_static.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/magnebot.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/magnebot.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/magnebot_controller.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/magnebot_controller.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/magnebot_dynamic.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/magnebot_dynamic.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/magnebot_static.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/magnebot_static.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/object_static.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/object_static.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/paths.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/paths.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/robot.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/robot.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/robot_base.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/robot_base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/robot_dynamic.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/robot_dynamic.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/robot_static.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/robot_static.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/scene_environment.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/scene_environment.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/scene_state.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/scene_state.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/skip_frames.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/skip_frames.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/test_controller.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/test_controller.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/transform.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/transform.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/turn_constants.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/turn_constants.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/__pycache__/util.cpython-37.pyc` & `magnebot-2.2.6/magnebot/__pycache__/util.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/action_status.py` & `magnebot-2.2.6/magnebot/action_status.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/action.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/action.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/arm_action.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/arm_action.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/arm_motion.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/arm_motion.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/camera_action.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/camera_action.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/drop.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/drop.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/grasp.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/grasp.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/ik_motion.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/ik_motion.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/look_at.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/look_at.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/move_by.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/move_by.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/move_camera.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/move_camera.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/move_to.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/move_to.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/navigate.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/navigate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/reach_for.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/reach_for.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/reset_arm.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/reset_arm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/reset_camera.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/reset_camera.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/reset_position.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/reset_position.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/rotate_camera.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/rotate_camera.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/slide_torso.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/slide_torso.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/stop.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/stop.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/turn.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/turn.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/turn_by.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/turn_by.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/turn_to.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/turn_to.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/wait.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/wait.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/wait_for_joints.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/wait_for_joints.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/__pycache__/wheel_motion.cpython-37.pyc` & `magnebot-2.2.6/magnebot/actions/__pycache__/wheel_motion.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/action.py` & `magnebot-2.2.6/magnebot/actions/action.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/arm_motion.py` & `magnebot-2.2.6/magnebot/actions/arm_motion.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/camera_action.py` & `magnebot-2.2.6/magnebot/actions/camera_action.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/drop.py` & `magnebot-2.2.6/magnebot/actions/drop.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/grasp.py` & `magnebot-2.2.6/magnebot/actions/grasp.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/ik_motion.py` & `magnebot-2.2.6/magnebot/actions/ik_motion.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/look_at.py` & `magnebot-2.2.6/magnebot/actions/look_at.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/move_by.py` & `magnebot-2.2.6/magnebot/actions/move_by.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/move_camera.py` & `magnebot-2.2.6/magnebot/actions/move_camera.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/move_to.py` & `magnebot-2.2.6/magnebot/actions/move_to.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/reach_for.py` & `magnebot-2.2.6/magnebot/actions/reach_for.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/reset_arm.py` & `magnebot-2.2.6/magnebot/actions/reset_arm.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/reset_camera.py` & `magnebot-2.2.6/magnebot/actions/reset_camera.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/reset_position.py` & `magnebot-2.2.6/magnebot/actions/reset_position.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/rotate_camera.py` & `magnebot-2.2.6/magnebot/actions/rotate_camera.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/slide_torso.py` & `magnebot-2.2.6/magnebot/actions/slide_torso.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/stop.py` & `magnebot-2.2.6/magnebot/actions/stop.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/turn.py` & `magnebot-2.2.6/magnebot/actions/turn.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/turn_by.py` & `magnebot-2.2.6/magnebot/actions/turn_by.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/turn_to.py` & `magnebot-2.2.6/magnebot/actions/turn_to.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/wait.py` & `magnebot-2.2.6/magnebot/actions/wait.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/actions/wheel_motion.py` & `magnebot-2.2.6/magnebot/actions/wheel_motion.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/collision_detection.py` & `magnebot-2.2.6/magnebot/collision_detection.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/constants.py` & `magnebot-2.2.6/magnebot/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # The wheel friction coefficient when braking during a move action.
 BRAKE_FRICTION: float = 0.95
 # The default camera position if the camera is parented to the torso.
 DEFAULT_CAMERA_POSITION_TORSO: Dict[str, float] = {"x": 0, "y": 0.053, "z": 0.1838}
 # The default camera position if the camera is parented to the column.
 DEFAULT_CAMERA_POSITION_COLUMN: Dict[str, float] = {"x": 0, "y": 0.6324, "z": 0.1838}
 # The required TDW version.
-TDW_VERSION: str = "1.11.6"
+TDW_VERSION: str = "1.11.22"
```

### Comparing `magnebot-2.2.5/magnebot/data/magnebot/ik/orientations_left.npy` & `magnebot-2.2.6/magnebot/data/magnebot/ik/orientations_left.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/magnebot/ik/orientations_right.npy` & `magnebot-2.2.6/magnebot/data/magnebot/ik/orientations_right.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/magnebot/ik/positions.npy` & `magnebot-2.2.6/magnebot/data/magnebot/ik/positions.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/objects/categories.json` & `magnebot-2.2.6/magnebot/data/objects/categories.json`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/objects/convex.json` & `magnebot-2.2.6/magnebot/data/objects/convex.json`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/1_0.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/1_0.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/1_1.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/1_1.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/1_2.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/1_2.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/2_0.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/2_0.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/2_1.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/2_1.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/2_2.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/2_2.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/4_0.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/4_0.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/4_1.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/4_1.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/4_2.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/4_2.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/5_0.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/5_0.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/5_1.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/5_1.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/occupancy_maps/5_2.npy` & `magnebot-2.2.6/magnebot/data/scenes/occupancy_maps/5_2.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/room_maps/1.npy` & `magnebot-2.2.6/magnebot/data/scenes/room_maps/1.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/room_maps/2.npy` & `magnebot-2.2.6/magnebot/data/scenes/room_maps/2.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/room_maps/4.npy` & `magnebot-2.2.6/magnebot/data/scenes/room_maps/4.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/room_maps/5.npy` & `magnebot-2.2.6/magnebot/data/scenes/room_maps/5.npy`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/data/scenes/spawn_positions.json` & `magnebot-2.2.6/magnebot/data/scenes/spawn_positions.json`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/ik/__pycache__/orientation.cpython-37.pyc` & `magnebot-2.2.6/magnebot/ik/__pycache__/orientation.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/ik/orientation.py` & `magnebot-2.2.6/magnebot/ik/orientation.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/ikpy/__pycache__/link.cpython-37.pyc` & `magnebot-2.2.6/magnebot/ikpy/__pycache__/link.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/ikpy/link.py` & `magnebot-2.2.6/magnebot/ikpy/link.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/magnebot.py` & `magnebot-2.2.6/magnebot/magnebot.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,15 +550,14 @@
             Magnebot._CHECKED_VERSION = True
             check_version()
             version_data = get_data(resp=resp, d_type=Version)
             build_version = version_data.get_tdw_version()
             PyPi.required_tdw_version_is_installed(required_version=TDW_VERSION, build_version=build_version,
                                                    comparison=">=")
         self.static = MagnebotStatic(robot_id=self.robot_id, resp=resp)
-        self._set_robot_joint_ids()
         # Wait for the joints to finish moving.
         self.action = Wait()
         # Add an avatar and set up its camera.
         self.commands.extend([{"$type": "create_avatar",
                                "type": "A_Img_Caps_Kinematic",
                                "id": self.static.avatar_id},
                               {"$type": "set_pass_masks",
```

### Comparing `magnebot-2.2.5/magnebot/magnebot_controller.py` & `magnebot-2.2.6/magnebot/magnebot_controller.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/magnebot_dynamic.py` & `magnebot-2.2.6/magnebot/magnebot_dynamic.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/magnebot_static.py` & `magnebot-2.2.6/magnebot/magnebot_static.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/paths.py` & `magnebot-2.2.6/magnebot/paths.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/turn_constants.py` & `magnebot-2.2.6/magnebot/turn_constants.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot/util.py` & `magnebot-2.2.6/magnebot/util.py`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/magnebot.egg-info/PKG-INFO` & `magnebot-2.2.6/magnebot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnebot
-Version: 2.2.5
+Version: 2.2.6
 Summary: High-level API for the Magnebot in TDW.
 Home-page: https://github.com/alters-mit/magnebot
 Author: Esther Alter
 Author-email: alters@mit.edu
 License: MIT
 Keywords: unity simulation tdw robotics
 Platform: UNKNOWN
```

### Comparing `magnebot-2.2.5/magnebot.egg-info/SOURCES.txt` & `magnebot-2.2.6/magnebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnebot-2.2.5/setup.py` & `magnebot-2.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 readme = readme.replace('"https://raw.githubusercontent.com/alters-mit/magnebot/main/doc/images/reach_high.gif"',
                         '"https://github.com/alters-mit/magnebot/raw/main/social.jpg"')
 # Replace relative markdown links with absolute https links.
 readme = re.sub(r'\[(.*?)\]\(doc/(.*?)\)', r'[\1][https://github.com/alters-mit/magnebot/blob/main/doc/\2]', readme)
 
 setup(
     name='magnebot',
-    version="2.2.5",
+    version="2.2.6",
     description='High-level API for the Magnebot in TDW.',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/alters-mit/magnebot',
     author='Esther Alter',
     author_email="alters@mit.edu",
     license='MIT',
@@ -26,10 +26,10 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8'
     ],
     keywords='unity simulation tdw robotics',
     packages=find_packages(),
     include_package_data=True,
-    install_requires=['tdw>=1.11.3.0', 'numpy', 'requests', 'matplotlib', 'pillow', "py_md_doc", "tqdm", "scipy", "ikpy==3.1",
+    install_requires=['tdw>=1.11.22.0', 'numpy', 'requests', 'matplotlib', 'pillow', "py_md_doc", "tqdm", "scipy", "ikpy==3.1",
                       "overrides"],
 )
```

