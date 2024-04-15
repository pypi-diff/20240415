# Comparing `tmp/spacerescue-0.2.8.tar.gz` & `tmp/spacerescue-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacerescue-0.2.8.tar", max compression
+gzip compressed data, was "spacerescue-0.2.9.tar", max compression
```

## Comparing `spacerescue-0.2.8.tar` & `spacerescue-0.2.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    35145 2024-03-25 08:32:03.538805 spacerescue-0.2.8/LICENSE
--rw-r--r--   0        0        0     2230 2024-03-25 08:32:03.538805 spacerescue-0.2.8/README.md
--rw-r--r--   0        0        0      643 2024-03-25 08:32:03.539805 spacerescue-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 08:32:03.568805 spacerescue-0.2.8/spacerescue/__init__.py
--rw-r--r--   0        0        0     1309 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/__main__.py
--rw-r--r--   0        0        0      390 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/constants.py
--rw-r--r--   0        0        0     1338 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/core/math.py
--rw-r--r--   0        0        0      399 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/core/pyray.py
--rw-r--r--   0        0        0     2206 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/core/types.py
--rw-r--r--   0        0        0     3149 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/challenge.py
--rw-r--r--   0        0        0     2570 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/challenges/challenge1.py
--rw-r--r--   0        0        0      915 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/challenges/challenge2.py
--rw-r--r--   0        0        0     2481 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/challenges/challenge3.py
--rw-r--r--   0        0        0     4341 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/databases/database.py
--rw-r--r--   0        0        0      579 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/game_board.py
--rw-r--r--   0        0        0     1187 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/game_scene.py
--rw-r--r--   0        0        0     1667 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/game_state.py
--rw-r--r--   0        0        0     2489 2024-03-25 08:32:03.539805 spacerescue-0.2.8/spacerescue/gameplay/game_states/game_states.py
--rw-r--r--   0        0        0     1103 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/game_states/main_state.py
--rw-r--r--   0        0        0     6177 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/computer_console.py
--rw-r--r--   0        0        0     7798 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/computer_room.py
--rw-r--r--   0        0        0     3080 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/game_over.py
--rw-r--r--   0        0        0     3397 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/logo_scene.py
--rw-r--r--   0        0        0     4531 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/menu_scene.py
--rw-r--r--   0        0        0     5377 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/quizz_console.py
--rw-r--r--   0        0        0     8532 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/simulator_console.py
--rw-r--r--   0        0        0     1946 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/title.py
--rw-r--r--   0        0        0     3062 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_in_space.py
--rw-r--r--   0        0        0     1189 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_to_home.py
--rw-r--r--   0        0        0     2789 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_to_hyperspace.py
--rw-r--r--   0        0        0      936 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_to_portal.py
--rw-r--r--   0        0        0     2004 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/physic/entity.py
--rw-r--r--   0        0        0     1341 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/physic/galaxy/asteroid.py
--rw-r--r--   0        0        0     1628 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/physic/galaxy/dust.py
--rw-r--r--   0        0        0     6286 2024-03-25 08:32:03.540805 spacerescue-0.2.8/spacerescue/physic/galaxy/galaxy.py
--rw-r--r--   0        0        0     5431 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/galaxy/galaxy_generator.py
--rw-r--r--   0        0        0     1985 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/galaxy/hyperspace_portal.py
--rw-r--r--   0        0        0     1654 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/galaxy/physic/physical_laws.py
--rw-r--r--   0        0        0     3050 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/galaxy/physic/physical_mapper.py
--rw-r--r--   0        0        0     1933 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/galaxy/planet.py
--rw-r--r--   0        0        0     3835 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/galaxy/spaceship.py
--rw-r--r--   0        0        0     1918 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/galaxy/star.py
--rw-r--r--   0        0        0      524 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/laws.py
--rw-r--r--   0        0        0      869 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/mapper.py
--rw-r--r--   0        0        0     1374 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/simulation/drone.py
--rw-r--r--   0        0        0      363 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/simulation/physic/physical_laws.py
--rw-r--r--   0        0        0     1736 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/simulation/physic/physical_mapper.py
--rw-r--r--   0        0        0     4291 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/simulation/world.py
--rw-r--r--   0        0        0      591 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/physic/universe.py
--rw-r--r--   0        0        0     2134 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/render/aabb.py
--rw-r--r--   0        0        0      422 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/render/animator.py
--rw-r--r--   0        0        0     1083 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/render/animators/open_horizontal.py
--rw-r--r--   0        0        0     1087 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/render/animators/open_vertical.py
--rw-r--r--   0        0        0      794 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/render/camera.py
--rw-r--r--   0        0        0     1301 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/render/cameras/camera_entity.py
--rw-r--r--   0        0        0     1983 2024-03-25 08:32:03.541805 spacerescue-0.2.8/spacerescue/render/cameras/camera_follower.py
--rw-r--r--   0        0        0      697 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/effects/fade_inout.py
--rw-r--r--   0        0        0      937 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/effects/fade_scr.py
--rw-r--r--   0        0        0     1446 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/effects/star_field.py
--rw-r--r--   0        0        0     1480 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/frustrum.py
--rw-r--r--   0        0        0     2635 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/light.py
--rw-r--r--   0        0        0     4192 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/quadtree.py
--rw-r--r--   0        0        0      228 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widget.py
--rw-r--r--   0        0        0     3212 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/blueprint_box.py
--rw-r--r--   0        0        0     2622 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/button.py
--rw-r--r--   0        0        0     1796 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/checkbox.py
--rw-r--r--   0        0        0     5725 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/markdown_box.py
--rw-r--r--   0        0        0     2838 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/message_box.py
--rw-r--r--   0        0        0     1858 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/progress_box.py
--rw-r--r--   0        0        0     3279 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/quizz_box.py
--rw-r--r--   0        0        0      781 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/render/widgets/screen.py
--rw-r--r--   0        0        0     1387 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/resources/__init__.py
--rw-r--r--   0        0        0     1099 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/resources/data/missions.yml
--rw-r--r--   0        0        0     5652 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/resources/data/planet_names.txt
--rw-r--r--   0        0        0     3503 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/resources/data/questions.yml
--rw-r--r--   0        0        0     5111 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/resources/resource_manager.py
--rw-r--r--   0        0        0     1875 2024-03-25 08:32:03.542805 spacerescue-0.2.8/spacerescue/resources/resource_manager.yml
--rw-r--r--   0        0        0     1741 2024-03-25 08:32:03.543805 spacerescue-0.2.8/spacerescue/sketch.py
--rw-r--r--   0        0        0     3716 2024-03-25 08:32:03.543805 spacerescue-0.2.8/spacerescue/tools/dynamic_code.py
--rw-r--r--   0        0        0     1660 2024-03-25 08:32:03.543805 spacerescue-0.2.8/spacerescue/tools/markdown_parser.py
--rw-r--r--   0        0        0      619 2024-03-25 08:32:03.543805 spacerescue-0.2.8/spacerescue/tools/name_generator.py
--rw-r--r--   0        0        0      470 2024-03-25 08:32:03.543805 spacerescue-0.2.8/spacerescue/tools/simple_allocator.py
--rw-r--r--   0        0        0     1541 2024-03-25 08:32:03.543805 spacerescue-0.2.8/spacerescue/tools/util.py
--rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 spacerescue-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35145 2024-03-25 08:38:42.278670 spacerescue-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2230 2024-03-25 08:38:42.278670 spacerescue-0.2.9/README.md
+-rw-r--r--   0        0        0      643 2024-03-25 08:38:42.278670 spacerescue-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-25 08:38:42.307670 spacerescue-0.2.9/spacerescue/__init__.py
+-rw-r--r--   0        0        0     1309 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/__main__.py
+-rw-r--r--   0        0        0      390 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/constants.py
+-rw-r--r--   0        0        0     1338 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/core/math.py
+-rw-r--r--   0        0        0      399 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/core/pyray.py
+-rw-r--r--   0        0        0     2206 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/core/types.py
+-rw-r--r--   0        0        0     3149 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/challenge.py
+-rw-r--r--   0        0        0     2570 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/challenges/challenge1.py
+-rw-r--r--   0        0        0      915 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/challenges/challenge2.py
+-rw-r--r--   0        0        0     2481 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/challenges/challenge3.py
+-rw-r--r--   0        0        0     4341 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/databases/database.py
+-rw-r--r--   0        0        0      579 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/game_board.py
+-rw-r--r--   0        0        0     1187 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/game_scene.py
+-rw-r--r--   0        0        0     1667 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/game_state.py
+-rw-r--r--   0        0        0     2489 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/game_states/game_states.py
+-rw-r--r--   0        0        0     1103 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/game_states/main_state.py
+-rw-r--r--   0        0        0     6177 2024-03-25 08:38:42.279670 spacerescue-0.2.9/spacerescue/gameplay/scenes/computer_console.py
+-rw-r--r--   0        0        0     7798 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/computer_room.py
+-rw-r--r--   0        0        0     3080 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/game_over.py
+-rw-r--r--   0        0        0     3397 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/logo_scene.py
+-rw-r--r--   0        0        0     4531 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/menu_scene.py
+-rw-r--r--   0        0        0     5377 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/quizz_console.py
+-rw-r--r--   0        0        0     8532 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/simulator_console.py
+-rw-r--r--   0        0        0     1946 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/title.py
+-rw-r--r--   0        0        0     3062 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_in_space.py
+-rw-r--r--   0        0        0     1189 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_to_home.py
+-rw-r--r--   0        0        0     2789 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_to_hyperspace.py
+-rw-r--r--   0        0        0      936 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_to_portal.py
+-rw-r--r--   0        0        0     2004 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/physic/entity.py
+-rw-r--r--   0        0        0     1341 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/physic/galaxy/asteroid.py
+-rw-r--r--   0        0        0     1628 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/physic/galaxy/dust.py
+-rw-r--r--   0        0        0     6286 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/physic/galaxy/galaxy.py
+-rw-r--r--   0        0        0     5431 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/physic/galaxy/galaxy_generator.py
+-rw-r--r--   0        0        0     1985 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/physic/galaxy/hyperspace_portal.py
+-rw-r--r--   0        0        0     1654 2024-03-25 08:38:42.280670 spacerescue-0.2.9/spacerescue/physic/galaxy/physic/physical_laws.py
+-rw-r--r--   0        0        0     3050 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/galaxy/physic/physical_mapper.py
+-rw-r--r--   0        0        0     1933 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/galaxy/planet.py
+-rw-r--r--   0        0        0     3835 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/galaxy/spaceship.py
+-rw-r--r--   0        0        0     1918 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/galaxy/star.py
+-rw-r--r--   0        0        0      524 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/laws.py
+-rw-r--r--   0        0        0      869 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/mapper.py
+-rw-r--r--   0        0        0     1374 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/simulation/drone.py
+-rw-r--r--   0        0        0      363 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/simulation/physic/physical_laws.py
+-rw-r--r--   0        0        0     1736 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/simulation/physic/physical_mapper.py
+-rw-r--r--   0        0        0     4291 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/simulation/world.py
+-rw-r--r--   0        0        0      591 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/physic/universe.py
+-rw-r--r--   0        0        0     2134 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/aabb.py
+-rw-r--r--   0        0        0      422 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/animator.py
+-rw-r--r--   0        0        0     1083 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/animators/open_horizontal.py
+-rw-r--r--   0        0        0     1087 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/animators/open_vertical.py
+-rw-r--r--   0        0        0      794 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/camera.py
+-rw-r--r--   0        0        0     1301 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/cameras/camera_entity.py
+-rw-r--r--   0        0        0     1983 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/cameras/camera_follower.py
+-rw-r--r--   0        0        0      697 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/effects/fade_inout.py
+-rw-r--r--   0        0        0      937 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/effects/fade_scr.py
+-rw-r--r--   0        0        0     1446 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/effects/star_field.py
+-rw-r--r--   0        0        0     1480 2024-03-25 08:38:42.281670 spacerescue-0.2.9/spacerescue/render/frustrum.py
+-rw-r--r--   0        0        0     2635 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/light.py
+-rw-r--r--   0        0        0     4192 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/quadtree.py
+-rw-r--r--   0        0        0      228 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widget.py
+-rw-r--r--   0        0        0     3212 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/blueprint_box.py
+-rw-r--r--   0        0        0     2622 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/button.py
+-rw-r--r--   0        0        0     1796 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/checkbox.py
+-rw-r--r--   0        0        0     5725 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/markdown_box.py
+-rw-r--r--   0        0        0     2838 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/message_box.py
+-rw-r--r--   0        0        0     1858 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/progress_box.py
+-rw-r--r--   0        0        0     3279 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/quizz_box.py
+-rw-r--r--   0        0        0      781 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/render/widgets/screen.py
+-rw-r--r--   0        0        0     1387 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/resources/__init__.py
+-rw-r--r--   0        0        0     1099 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/resources/data/missions.yml
+-rw-r--r--   0        0        0     5652 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/resources/data/planet_names.txt
+-rw-r--r--   0        0        0     3503 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/resources/data/questions.yml
+-rw-r--r--   0        0        0     5111 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/resources/resource_manager.py
+-rw-r--r--   0        0        0     1875 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/resources/resource_manager.yml
+-rw-r--r--   0        0        0     1741 2024-03-25 08:38:42.282670 spacerescue-0.2.9/spacerescue/sketch.py
+-rw-r--r--   0        0        0     3716 2024-03-25 08:38:42.283670 spacerescue-0.2.9/spacerescue/tools/dynamic_code.py
+-rw-r--r--   0        0        0     1660 2024-03-25 08:38:42.283670 spacerescue-0.2.9/spacerescue/tools/markdown_parser.py
+-rw-r--r--   0        0        0      619 2024-03-25 08:38:42.283670 spacerescue-0.2.9/spacerescue/tools/name_generator.py
+-rw-r--r--   0        0        0      470 2024-03-25 08:38:42.283670 spacerescue-0.2.9/spacerescue/tools/simple_allocator.py
+-rw-r--r--   0        0        0     1541 2024-03-25 08:38:42.283670 spacerescue-0.2.9/spacerescue/tools/util.py
+-rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 spacerescue-0.2.9/PKG-INFO
```

### Comparing `spacerescue-0.2.8/LICENSE` & `spacerescue-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/README.md` & `spacerescue-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/pyproject.toml` & `spacerescue-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacerescue"
-version = "0.2.8"
+version = "0.2.9"
 description = "Space Rescue - A Escape Coding Adventure"
 authors = ["Romuald Rousseau <romuald.rousseau@servier.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.26.4"
```

### Comparing `spacerescue-0.2.8/spacerescue/__main__.py` & `spacerescue-0.2.9/spacerescue/__main__.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/core/math.py` & `spacerescue-0.2.9/spacerescue/core/math.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/core/types.py` & `spacerescue-0.2.9/spacerescue/core/types.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/challenge.py` & `spacerescue-0.2.9/spacerescue/gameplay/challenge.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/challenges/challenge1.py` & `spacerescue-0.2.9/spacerescue/gameplay/challenges/challenge1.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/challenges/challenge2.py` & `spacerescue-0.2.9/spacerescue/gameplay/challenges/challenge2.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/challenges/challenge3.py` & `spacerescue-0.2.9/spacerescue/gameplay/challenges/challenge3.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/databases/database.py` & `spacerescue-0.2.9/spacerescue/gameplay/databases/database.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/game_board.py` & `spacerescue-0.2.9/spacerescue/gameplay/game_board.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/game_scene.py` & `spacerescue-0.2.9/spacerescue/gameplay/game_scene.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/game_state.py` & `spacerescue-0.2.9/spacerescue/gameplay/game_state.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/game_states/game_states.py` & `spacerescue-0.2.9/spacerescue/gameplay/game_states/game_states.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/game_states/main_state.py` & `spacerescue-0.2.9/spacerescue/gameplay/game_states/main_state.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/computer_console.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/computer_console.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/computer_room.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/computer_room.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/game_over.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/game_over.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/logo_scene.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/logo_scene.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/menu_scene.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/menu_scene.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/quizz_console.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/quizz_console.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/simulator_console.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/simulator_console.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/title.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/title.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_in_space.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_in_space.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_to_home.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_to_home.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_to_hyperspace.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_to_hyperspace.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/gameplay/scenes/travel_to_portal.py` & `spacerescue-0.2.9/spacerescue/gameplay/scenes/travel_to_portal.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/entity.py` & `spacerescue-0.2.9/spacerescue/physic/entity.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/asteroid.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/asteroid.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/dust.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/dust.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/galaxy.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/galaxy.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/galaxy_generator.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/galaxy_generator.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/hyperspace_portal.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/hyperspace_portal.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/physic/physical_laws.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/physic/physical_laws.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/physic/physical_mapper.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/physic/physical_mapper.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/planet.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/planet.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/spaceship.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/spaceship.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/galaxy/star.py` & `spacerescue-0.2.9/spacerescue/physic/galaxy/star.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/laws.py` & `spacerescue-0.2.9/spacerescue/physic/laws.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/mapper.py` & `spacerescue-0.2.9/spacerescue/physic/mapper.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/simulation/drone.py` & `spacerescue-0.2.9/spacerescue/physic/simulation/drone.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/simulation/physic/physical_mapper.py` & `spacerescue-0.2.9/spacerescue/physic/simulation/physic/physical_mapper.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/simulation/world.py` & `spacerescue-0.2.9/spacerescue/physic/simulation/world.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/physic/universe.py` & `spacerescue-0.2.9/spacerescue/physic/universe.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/aabb.py` & `spacerescue-0.2.9/spacerescue/render/aabb.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/animators/open_horizontal.py` & `spacerescue-0.2.9/spacerescue/render/animators/open_horizontal.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/animators/open_vertical.py` & `spacerescue-0.2.9/spacerescue/render/animators/open_vertical.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/camera.py` & `spacerescue-0.2.9/spacerescue/render/camera.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/cameras/camera_entity.py` & `spacerescue-0.2.9/spacerescue/render/cameras/camera_entity.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/cameras/camera_follower.py` & `spacerescue-0.2.9/spacerescue/render/cameras/camera_follower.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/effects/fade_inout.py` & `spacerescue-0.2.9/spacerescue/render/effects/fade_inout.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/effects/fade_scr.py` & `spacerescue-0.2.9/spacerescue/render/effects/fade_scr.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/effects/star_field.py` & `spacerescue-0.2.9/spacerescue/render/effects/star_field.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/frustrum.py` & `spacerescue-0.2.9/spacerescue/render/frustrum.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/light.py` & `spacerescue-0.2.9/spacerescue/render/light.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/quadtree.py` & `spacerescue-0.2.9/spacerescue/render/quadtree.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/blueprint_box.py` & `spacerescue-0.2.9/spacerescue/render/widgets/blueprint_box.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/button.py` & `spacerescue-0.2.9/spacerescue/render/widgets/button.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/checkbox.py` & `spacerescue-0.2.9/spacerescue/render/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/markdown_box.py` & `spacerescue-0.2.9/spacerescue/render/widgets/markdown_box.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/message_box.py` & `spacerescue-0.2.9/spacerescue/render/widgets/message_box.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/progress_box.py` & `spacerescue-0.2.9/spacerescue/render/widgets/progress_box.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/quizz_box.py` & `spacerescue-0.2.9/spacerescue/render/widgets/quizz_box.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/render/widgets/screen.py` & `spacerescue-0.2.9/spacerescue/render/widgets/screen.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/resources/__init__.py` & `spacerescue-0.2.9/spacerescue/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/resources/data/missions.yml` & `spacerescue-0.2.9/spacerescue/resources/data/missions.yml`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/resources/data/planet_names.txt` & `spacerescue-0.2.9/spacerescue/resources/data/planet_names.txt`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/resources/data/questions.yml` & `spacerescue-0.2.9/spacerescue/resources/data/questions.yml`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/resources/resource_manager.py` & `spacerescue-0.2.9/spacerescue/resources/resource_manager.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/resources/resource_manager.yml` & `spacerescue-0.2.9/spacerescue/resources/resource_manager.yml`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/sketch.py` & `spacerescue-0.2.9/spacerescue/sketch.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/tools/dynamic_code.py` & `spacerescue-0.2.9/spacerescue/tools/dynamic_code.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/tools/markdown_parser.py` & `spacerescue-0.2.9/spacerescue/tools/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/tools/name_generator.py` & `spacerescue-0.2.9/spacerescue/tools/name_generator.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/spacerescue/tools/util.py` & `spacerescue-0.2.9/spacerescue/tools/util.py`

 * *Files identical despite different names*

### Comparing `spacerescue-0.2.8/PKG-INFO` & `spacerescue-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacerescue
-Version: 0.2.8
+Version: 0.2.9
 Summary: Space Rescue - A Escape Coding Adventure
 Author: Romuald Rousseau
 Author-email: romuald.rousseau@servier.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

