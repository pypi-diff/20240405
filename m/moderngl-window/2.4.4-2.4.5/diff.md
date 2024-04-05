# Comparing `tmp/moderngl-window-2.4.4.tar.gz` & `tmp/moderngl-window-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderngl-window-2.4.4.tar", last modified: Thu May 18 11:08:07 2023, max compression
+gzip compressed data, was "moderngl-window-2.4.5.tar", last modified: Sat Oct 14 19:12:20 2023, max compression
```

## Comparing `moderngl-window-2.4.4.tar` & `moderngl-window-2.4.5.tar`

### file list

```diff
@@ -1,157 +1,180 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.893470 moderngl-window-2.4.4/
--rw-rw-rw-   0        0        0     1111 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/LICENSE
--rw-rw-rw-   0        0        0      153 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7785 2023-05-18 11:08:07.893470 moderngl-window-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     6456 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.765136 moderngl-window-2.4.4/moderngl_window/
--rw-rw-rw-   0        0        0    10564 2023-05-18 11:00:51.000000 moderngl-window-2.4.4/moderngl_window/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.773368 moderngl-window-2.4.4/moderngl_window/atlas/
--rw-rw-rw-   0        0        0     1890 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/atlas/base.py
--rw-rw-rw-   0        0        0     5195 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/atlas/simple_atlas.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.775879 moderngl-window-2.4.4/moderngl_window/capture/
--rw-rw-rw-   0        0        0       87 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/capture/__init__.py
--rw-rw-rw-   0        0        0     4715 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/capture/base.py
--rw-rw-rw-   0        0        0     3333 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/capture/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.777886 moderngl-window-2.4.4/moderngl_window/conf/
--rw-rw-rw-   0        0        0    10728 2020-08-22 11:45:34.000000 moderngl-window-2.4.4/moderngl_window/conf/__init__.py
--rw-rw-rw-   0        0        0     1502 2020-08-22 11:45:09.000000 moderngl-window-2.4.4/moderngl_window/conf/default.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.749621 moderngl-window-2.4.4/moderngl_window/context/
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.780884 moderngl-window-2.4.4/moderngl_window/context/base/
--rw-rw-rw-   0        0        0      160 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/base/__init__.py
--rw-rw-rw-   0        0        0     2128 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/context/base/keys.py
--rw-rw-rw-   0        0        0    49412 2023-05-18 09:43:10.000000 moderngl-window-2.4.4/moderngl_window/context/base/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.782885 moderngl-window-2.4.4/moderngl_window/context/glfw/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/glfw/__init__.py
--rw-rw-rw-   0        0        0     2387 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/moderngl_window/context/glfw/keys.py
--rw-rw-rw-   0        0        0    13168 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/glfw/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.785393 moderngl-window-2.4.4/moderngl_window/context/headless/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/headless/__init__.py
--rw-rw-rw-   0        0        0       88 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/headless/keys.py
--rw-rw-rw-   0        0        0     2925 2023-05-18 09:50:27.000000 moderngl-window-2.4.4/moderngl_window/context/headless/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.788401 moderngl-window-2.4.4/moderngl_window/context/pygame2/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pygame2/__init__.py
--rw-rw-rw-   0        0        0     2391 2020-08-23 14:24:53.000000 moderngl-window-2.4.4/moderngl_window/context/pygame2/keys.py
--rw-rw-rw-   0        0        0    10311 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pygame2/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.791400 moderngl-window-2.4.4/moderngl_window/context/pyglet/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyglet/__init__.py
--rw-rw-rw-   0        0        0     2203 2020-08-23 14:15:48.000000 moderngl-window-2.4.4/moderngl_window/context/pyglet/keys.py
--rw-rw-rw-   0        0        0    12218 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pyglet/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.793399 moderngl-window-2.4.4/moderngl_window/context/pyqt5/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyqt5/__init__.py
--rw-rw-rw-   0        0        0     2263 2020-08-23 14:28:19.000000 moderngl-window-2.4.4/moderngl_window/context/pyqt5/keys.py
--rw-rw-rw-   0        0        0    11967 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pyqt5/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.796607 moderngl-window-2.4.4/moderngl_window/context/pyside2/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyside2/__init__.py
--rw-rw-rw-   0        0        0     2217 2020-08-23 14:28:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyside2/keys.py
--rw-rw-rw-   0        0        0    11943 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pyside2/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.798605 moderngl-window-2.4.4/moderngl_window/context/sdl2/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/sdl2/__init__.py
--rw-rw-rw-   0        0        0     2473 2020-08-23 14:33:13.000000 moderngl-window-2.4.4/moderngl_window/context/sdl2/keys.py
--rw-rw-rw-   0        0        0    10499 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/sdl2/window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.801606 moderngl-window-2.4.4/moderngl_window/context/tk/
--rw-rw-rw-   0        0        0      120 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/tk/__init__.py
--rw-rw-rw-   0        0        0     2153 2020-08-23 14:35:15.000000 moderngl-window-2.4.4/moderngl_window/context/tk/keys.py
--rw-rw-rw-   0        0        0     9364 2022-09-17 17:02:40.000000 moderngl-window-2.4.4/moderngl_window/context/tk/window.py
--rw-rw-rw-   0        0        0      137 2020-08-23 13:56:44.000000 moderngl-window-2.4.4/moderngl_window/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.805113 moderngl-window-2.4.4/moderngl_window/finders/
--rw-rw-rw-   0        0        0     3309 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/base.py
--rw-rw-rw-   0        0        0      328 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/data.py
--rw-rw-rw-   0        0        0      340 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/program.py
--rw-rw-rw-   0        0        0      333 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/scene.py
--rw-rw-rw-   0        0        0      341 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/texture.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.811121 moderngl-window-2.4.4/moderngl_window/geometry/
--rw-rw-rw-   0        0        0      312 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/geometry/__init__.py
--rw-rw-rw-   0        0        0     2305 2020-08-23 13:52:57.000000 moderngl-window-2.4.4/moderngl_window/geometry/attributes.py
--rw-rw-rw-   0        0        0     2058 2020-08-23 13:52:38.000000 moderngl-window-2.4.4/moderngl_window/geometry/bbox.py
--rw-rw-rw-   0        0        0     5375 2020-08-23 13:52:07.000000 moderngl-window-2.4.4/moderngl_window/geometry/cube.py
--rw-rw-rw-   0        0        0     2552 2023-03-03 11:50:20.000000 moderngl-window-2.4.4/moderngl_window/geometry/quad.py
--rw-rw-rw-   0        0        0     2656 2020-08-23 13:48:13.000000 moderngl-window-2.4.4/moderngl_window/geometry/sphere.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.813120 moderngl-window-2.4.4/moderngl_window/integrations/
--rw-rw-rw-   0        0        0     9890 2023-03-03 11:50:20.000000 moderngl-window-2.4.4/moderngl_window/integrations/imgui.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.814119 moderngl-window-2.4.4/moderngl_window/loaders/
--rw-rw-rw-   0        0        0     3739 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/loaders/base.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.816301 moderngl-window-2.4.4/moderngl_window/loaders/data/
--rw-rw-rw-   0        0        0      759 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/data/binary.py
--rw-rw-rw-   0        0        0      811 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/data/json.py
--rw-rw-rw-   0        0        0      803 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/data/text.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.818304 moderngl-window-2.4.4/moderngl_window/loaders/program/
--rw-rw-rw-   0        0        0     3339 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/program/separate.py
--rw-rw-rw-   0        0        0     2390 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/program/single.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.821303 moderngl-window-2.4.4/moderngl_window/loaders/scene/
--rw-rw-rw-   0        0        0    28338 2020-10-24 12:28:27.000000 moderngl-window-2.4.4/moderngl_window/loaders/scene/gltf2.py
--rw-rw-rw-   0        0        0     1648 2021-11-04 20:22:25.000000 moderngl-window-2.4.4/moderngl_window/loaders/scene/stl.py
--rw-rw-rw-   0        0        0     5710 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/scene/wavefront.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.825301 moderngl-window-2.4.4/moderngl_window/loaders/texture/
--rw-rw-rw-   0        0        0     1443 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/array.py
--rw-rw-rw-   0        0        0     2908 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/cube.py
--rw-rw-rw-   0        0        0      709 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/icon.py
--rw-rw-rw-   0        0        0     3826 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/pillow.py
--rw-rw-rw-   0        0        0     1037 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/t2d.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.859784 moderngl-window-2.4.4/moderngl_window/meta/
--rw-rw-rw-   0        0        0      186 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/meta/__init__.py
--rw-rw-rw-   0        0        0     2915 2020-08-22 11:48:01.000000 moderngl-window-2.4.4/moderngl_window/meta/base.py
--rw-rw-rw-   0        0        0     1345 2020-10-24 12:28:35.000000 moderngl-window-2.4.4/moderngl_window/meta/data.py
--rw-rw-rw-   0        0        0     4415 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/moderngl_window/meta/program.py
--rw-rw-rw-   0        0        0     1960 2020-10-24 12:29:08.000000 moderngl-window-2.4.4/moderngl_window/meta/scene.py
--rw-rw-rw-   0        0        0     5301 2020-08-23 12:37:41.000000 moderngl-window-2.4.4/moderngl_window/meta/texture.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.862780 moderngl-window-2.4.4/moderngl_window/opengl/
--rw-rw-rw-   0        0        0    15473 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/moderngl_window/opengl/program.py
--rw-rw-rw-   0        0        0     2780 2020-08-22 11:50:55.000000 moderngl-window-2.4.4/moderngl_window/opengl/projection.py
--rw-rw-rw-   0        0        0     4878 2020-10-24 12:28:52.000000 moderngl-window-2.4.4/moderngl_window/opengl/types.py
--rw-rw-rw-   0        0        0    13379 2020-08-22 11:50:56.000000 moderngl-window-2.4.4/moderngl_window/opengl/vao.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.869302 moderngl-window-2.4.4/moderngl_window/resources/
--rw-rw-rw-   0        0        0     3211 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/resources/__init__.py
--rw-rw-rw-   0        0        0     4035 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/base.py
--rw-rw-rw-   0        0        0      644 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/data.py
--rw-rw-rw-   0        0        0      482 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/resources/decorators.py
--rw-rw-rw-   0        0        0     1087 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/programs.py
--rw-rw-rw-   0        0        0      671 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/scenes.py
--rw-rw-rw-   0        0        0      860 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/resources/textures.py
--rw-rw-rw-   0        0        0      650 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/resources/tracks.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.875300 moderngl-window-2.4.4/moderngl_window/scene/
--rw-rw-rw-   0        0        0      317 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/scene/__init__.py
--rw-rw-rw-   0        0        0    18808 2023-05-18 08:47:55.000000 moderngl-window-2.4.4/moderngl_window/scene/camera.py
--rw-rw-rw-   0        0        0     2547 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/material.py
--rw-rw-rw-   0        0        0     4868 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/mesh.py
--rw-rw-rw-   0        0        0     5946 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/node.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.755125 moderngl-window-2.4.4/moderngl_window/scene/programs/
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.882340 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/
--rw-rw-rw-   0        0        0      476 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/bbox.glsl
--rw-rw-rw-   0        0        0     1139 2020-06-06 23:23:21.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/color_light.glsl
--rw-rw-rw-   0        0        0      365 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/fallback.glsl
--rw-rw-rw-   0        0        0      458 2020-06-07 01:31:46.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/texture.glsl
--rw-rw-rw-   0        0        0      796 2020-06-06 22:55:31.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/texture_light.glsl
--rw-rw-rw-   0        0        0      426 2020-06-07 01:12:04.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/vertex_color.glsl
--rw-rw-rw-   0        0        0      559 2020-06-07 01:51:45.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl
--rw-rw-rw-   0        0        0      500 2020-06-06 23:25:16.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/wireframe.glsl
--rw-rw-rw-   0        0        0     8516 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/programs.py
--rw-rw-rw-   0        0        0     9744 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/scene.py
--rw-rw-rw-   0        0        0     2590 2020-08-23 13:56:52.000000 moderngl-window-2.4.4/moderngl_window/screenshot.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.756131 moderngl-window-2.4.4/moderngl_window/text/
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.885339 moderngl-window-2.4.4/moderngl_window/text/bitmapped/
--rw-rw-rw-   0        0        0       43 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/__init__.py
--rw-rw-rw-   0        0        0     1954 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/base.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.757131 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.885339 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/programs/
--rw-rw-rw-   0        0        0     1696 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.886471 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/text/
--rw-rw-rw-   0        0        0      262 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/text/meta.json
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.887470 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/textures/
--rw-rw-rw-   0        0        0   318186 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png
--rw-rw-rw-   0        0        0     2804 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/text_2d.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.890470 moderngl-window-2.4.4/moderngl_window/timers/
--rw-rw-rw-   0        0        0     1792 2020-08-22 11:46:40.000000 moderngl-window-2.4.4/moderngl_window/timers/base.py
--rw-rw-rw-   0        0        0     2805 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/timers/clock.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.893470 moderngl-window-2.4.4/moderngl_window/utils/
--rw-rw-rw-   0        0        0       42 2020-10-19 05:57:32.000000 moderngl-window-2.4.4/moderngl_window/utils/__init__.py
--rw-rw-rw-   0        0        0      755 2023-05-18 08:47:36.000000 moderngl-window-2.4.4/moderngl_window/utils/keymaps.py
--rw-rw-rw-   0        0        0      837 2020-08-22 11:46:20.000000 moderngl-window-2.4.4/moderngl_window/utils/module_loading.py
--rw-rw-rw-   0        0        0     5381 2020-10-24 12:29:20.000000 moderngl-window-2.4.4/moderngl_window/utils/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.772367 moderngl-window-2.4.4/moderngl_window.egg-info/
--rw-rw-rw-   0        0        0     7785 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4458 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-18 11:08:07.898991 moderngl-window-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1953 2023-05-18 08:50:47.000000 moderngl-window-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.651112 moderngl-window-2.4.5/
+-rw-rw-rw-   0        0        0     1111 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0      153 2021-07-23 20:25:43.000000 moderngl-window-2.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8742 2023-10-14 19:12:20.650111 moderngl-window-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6292 2023-10-13 22:58:40.000000 moderngl-window-2.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.517191 moderngl-window-2.4.5/moderngl_window/
+-rw-rw-rw-   0        0        0    10622 2023-10-13 23:56:48.000000 moderngl-window-2.4.5/moderngl_window/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.535604 moderngl-window-2.4.5/moderngl_window/atlas/
+-rw-rw-rw-   0        0        0     1890 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/atlas/base.py
+-rw-rw-rw-   0        0        0     5195 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/atlas/simple_atlas.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.537606 moderngl-window-2.4.5/moderngl_window/capture/
+-rw-rw-rw-   0        0        0       87 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/capture/__init__.py
+-rw-rw-rw-   0        0        0     4715 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/capture/base.py
+-rw-rw-rw-   0        0        0     3333 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/capture/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.539606 moderngl-window-2.4.5/moderngl_window/conf/
+-rw-rw-rw-   0        0        0    10728 2020-08-22 11:45:34.000000 moderngl-window-2.4.5/moderngl_window/conf/__init__.py
+-rw-rw-rw-   0        0        0     1502 2020-08-22 11:45:09.000000 moderngl-window-2.4.5/moderngl_window/conf/default.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.503160 moderngl-window-2.4.5/moderngl_window/context/
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.541604 moderngl-window-2.4.5/moderngl_window/context/base/
+-rw-rw-rw-   0        0        0      160 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/base/__init__.py
+-rw-rw-rw-   0        0        0     3171 2023-10-14 17:20:49.000000 moderngl-window-2.4.5/moderngl_window/context/base/keys.py
+-rw-rw-rw-   0        0        0    49468 2023-10-14 17:27:19.000000 moderngl-window-2.4.5/moderngl_window/context/base/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.545114 moderngl-window-2.4.5/moderngl_window/context/glfw/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/glfw/__init__.py
+-rw-rw-rw-   0        0        0     2387 2021-07-23 20:25:43.000000 moderngl-window-2.4.5/moderngl_window/context/glfw/keys.py
+-rw-rw-rw-   0        0        0    13168 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/glfw/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.547115 moderngl-window-2.4.5/moderngl_window/context/headless/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/headless/__init__.py
+-rw-rw-rw-   0        0        0       88 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/headless/keys.py
+-rw-rw-rw-   0        0        0     2925 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/headless/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.550115 moderngl-window-2.4.5/moderngl_window/context/pygame2/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/pygame2/__init__.py
+-rw-rw-rw-   0        0        0     2391 2020-08-23 14:24:53.000000 moderngl-window-2.4.5/moderngl_window/context/pygame2/keys.py
+-rw-rw-rw-   0        0        0    10311 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/pygame2/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.552116 moderngl-window-2.4.5/moderngl_window/context/pyglet/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/pyglet/__init__.py
+-rw-rw-rw-   0        0        0     2203 2020-08-23 14:15:48.000000 moderngl-window-2.4.5/moderngl_window/context/pyglet/keys.py
+-rw-rw-rw-   0        0        0    12218 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/pyglet/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.554262 moderngl-window-2.4.5/moderngl_window/context/pyqt5/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/pyqt5/__init__.py
+-rw-rw-rw-   0        0        0     2263 2020-08-23 14:28:19.000000 moderngl-window-2.4.5/moderngl_window/context/pyqt5/keys.py
+-rw-rw-rw-   0        0        0    11967 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/pyqt5/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.557266 moderngl-window-2.4.5/moderngl_window/context/pyside2/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/pyside2/__init__.py
+-rw-rw-rw-   0        0        0     2217 2020-08-23 14:28:38.000000 moderngl-window-2.4.5/moderngl_window/context/pyside2/keys.py
+-rw-rw-rw-   0        0        0    11943 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/pyside2/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.560262 moderngl-window-2.4.5/moderngl_window/context/sdl2/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/sdl2/__init__.py
+-rw-rw-rw-   0        0        0     2473 2020-08-23 14:33:13.000000 moderngl-window-2.4.5/moderngl_window/context/sdl2/keys.py
+-rw-rw-rw-   0        0        0    10499 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/sdl2/window.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.562262 moderngl-window-2.4.5/moderngl_window/context/tk/
+-rw-rw-rw-   0        0        0      120 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/context/tk/__init__.py
+-rw-rw-rw-   0        0        0     2153 2023-10-13 23:40:25.000000 moderngl-window-2.4.5/moderngl_window/context/tk/keys.py
+-rw-rw-rw-   0        0        0     9364 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/context/tk/window.py
+-rw-rw-rw-   0        0        0      137 2020-08-23 13:56:44.000000 moderngl-window-2.4.5/moderngl_window/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.566440 moderngl-window-2.4.5/moderngl_window/finders/
+-rw-rw-rw-   0        0        0     3309 2020-08-22 11:47:29.000000 moderngl-window-2.4.5/moderngl_window/finders/base.py
+-rw-rw-rw-   0        0        0      328 2020-08-22 11:47:29.000000 moderngl-window-2.4.5/moderngl_window/finders/data.py
+-rw-rw-rw-   0        0        0      340 2020-08-22 11:47:29.000000 moderngl-window-2.4.5/moderngl_window/finders/program.py
+-rw-rw-rw-   0        0        0      333 2020-08-22 11:47:29.000000 moderngl-window-2.4.5/moderngl_window/finders/scene.py
+-rw-rw-rw-   0        0        0      341 2020-08-22 11:47:29.000000 moderngl-window-2.4.5/moderngl_window/finders/texture.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.570440 moderngl-window-2.4.5/moderngl_window/geometry/
+-rw-rw-rw-   0        0        0      312 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/geometry/__init__.py
+-rw-rw-rw-   0        0        0     2305 2020-08-23 13:52:57.000000 moderngl-window-2.4.5/moderngl_window/geometry/attributes.py
+-rw-rw-rw-   0        0        0     2058 2020-08-23 13:52:38.000000 moderngl-window-2.4.5/moderngl_window/geometry/bbox.py
+-rw-rw-rw-   0        0        0     5375 2020-08-23 13:52:07.000000 moderngl-window-2.4.5/moderngl_window/geometry/cube.py
+-rw-rw-rw-   0        0        0     2552 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/geometry/quad.py
+-rw-rw-rw-   0        0        0     2656 2020-08-23 13:48:13.000000 moderngl-window-2.4.5/moderngl_window/geometry/sphere.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.571440 moderngl-window-2.4.5/moderngl_window/integrations/
+-rw-rw-rw-   0        0        0     9890 2023-10-13 23:52:42.000000 moderngl-window-2.4.5/moderngl_window/integrations/imgui.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.572440 moderngl-window-2.4.5/moderngl_window/loaders/
+-rw-rw-rw-   0        0        0     3742 2023-10-14 17:04:33.000000 moderngl-window-2.4.5/moderngl_window/loaders/base.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.574519 moderngl-window-2.4.5/moderngl_window/loaders/data/
+-rw-rw-rw-   0        0        0      759 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/data/binary.py
+-rw-rw-rw-   0        0        0      811 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/data/json.py
+-rw-rw-rw-   0        0        0      803 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/data/text.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.575518 moderngl-window-2.4.5/moderngl_window/loaders/program/
+-rw-rw-rw-   0        0        0     3339 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/program/separate.py
+-rw-rw-rw-   0        0        0     2390 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/program/single.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.578518 moderngl-window-2.4.5/moderngl_window/loaders/scene/
+-rw-rw-rw-   0        0        0    28268 2023-10-14 17:06:54.000000 moderngl-window-2.4.5/moderngl_window/loaders/scene/gltf2.py
+-rw-rw-rw-   0        0        0     1648 2021-11-04 20:22:25.000000 moderngl-window-2.4.5/moderngl_window/loaders/scene/stl.py
+-rw-rw-rw-   0        0        0     5710 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/scene/wavefront.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.582519 moderngl-window-2.4.5/moderngl_window/loaders/texture/
+-rw-rw-rw-   0        0        0     1443 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/texture/array.py
+-rw-rw-rw-   0        0        0     2900 2023-10-14 17:32:04.000000 moderngl-window-2.4.5/moderngl_window/loaders/texture/cube.py
+-rw-rw-rw-   0        0        0      709 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/texture/icon.py
+-rw-rw-rw-   0        0        0     3826 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/texture/pillow.py
+-rw-rw-rw-   0        0        0     1037 2020-08-23 13:54:00.000000 moderngl-window-2.4.5/moderngl_window/loaders/texture/t2d.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.587558 moderngl-window-2.4.5/moderngl_window/meta/
+-rw-rw-rw-   0        0        0      186 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/meta/__init__.py
+-rw-rw-rw-   0        0        0     2911 2023-10-14 17:24:26.000000 moderngl-window-2.4.5/moderngl_window/meta/base.py
+-rw-rw-rw-   0        0        0     1345 2020-10-24 12:28:35.000000 moderngl-window-2.4.5/moderngl_window/meta/data.py
+-rw-rw-rw-   0        0        0     4525 2023-10-13 23:31:56.000000 moderngl-window-2.4.5/moderngl_window/meta/program.py
+-rw-rw-rw-   0        0        0     1960 2020-10-24 12:29:08.000000 moderngl-window-2.4.5/moderngl_window/meta/scene.py
+-rw-rw-rw-   0        0        0     5301 2020-08-23 12:37:41.000000 moderngl-window-2.4.5/moderngl_window/meta/texture.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.590557 moderngl-window-2.4.5/moderngl_window/opengl/
+-rw-rw-rw-   0        0        0    15550 2023-10-13 23:48:31.000000 moderngl-window-2.4.5/moderngl_window/opengl/program.py
+-rw-rw-rw-   0        0        0     2780 2020-08-22 11:50:55.000000 moderngl-window-2.4.5/moderngl_window/opengl/projection.py
+-rw-rw-rw-   0        0        0     4878 2020-10-24 12:28:52.000000 moderngl-window-2.4.5/moderngl_window/opengl/types.py
+-rw-rw-rw-   0        0        0    13379 2020-08-22 11:50:56.000000 moderngl-window-2.4.5/moderngl_window/opengl/vao.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.597074 moderngl-window-2.4.5/moderngl_window/resources/
+-rw-rw-rw-   0        0        0     3206 2023-10-13 23:59:00.000000 moderngl-window-2.4.5/moderngl_window/resources/__init__.py
+-rw-rw-rw-   0        0        0     4035 2020-08-23 13:56:01.000000 moderngl-window-2.4.5/moderngl_window/resources/base.py
+-rw-rw-rw-   0        0        0      644 2020-08-23 13:56:01.000000 moderngl-window-2.4.5/moderngl_window/resources/data.py
+-rw-rw-rw-   0        0        0      482 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/resources/decorators.py
+-rw-rw-rw-   0        0        0     1087 2020-08-23 13:56:01.000000 moderngl-window-2.4.5/moderngl_window/resources/programs.py
+-rw-rw-rw-   0        0        0      671 2020-08-23 13:56:01.000000 moderngl-window-2.4.5/moderngl_window/resources/scenes.py
+-rw-rw-rw-   0        0        0      860 2021-05-13 09:43:41.000000 moderngl-window-2.4.5/moderngl_window/resources/textures.py
+-rw-rw-rw-   0        0        0      650 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/resources/tracks.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.603069 moderngl-window-2.4.5/moderngl_window/scene/
+-rw-rw-rw-   0        0        0      317 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/scene/__init__.py
+-rw-rw-rw-   0        0        0    18808 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/scene/camera.py
+-rw-rw-rw-   0        0        0     2547 2020-08-22 11:49:55.000000 moderngl-window-2.4.5/moderngl_window/scene/material.py
+-rw-rw-rw-   0        0        0     4868 2020-08-22 11:49:55.000000 moderngl-window-2.4.5/moderngl_window/scene/mesh.py
+-rw-rw-rw-   0        0        0     5946 2020-08-22 11:49:55.000000 moderngl-window-2.4.5/moderngl_window/scene/node.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.507673 moderngl-window-2.4.5/moderngl_window/scene/programs/
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.610399 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/
+-rw-rw-rw-   0        0        0      476 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/bbox.glsl
+-rw-rw-rw-   0        0        0     1139 2020-06-06 23:23:21.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/color_light.glsl
+-rw-rw-rw-   0        0        0      365 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/fallback.glsl
+-rw-rw-rw-   0        0        0      458 2020-06-07 01:31:46.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/texture.glsl
+-rw-rw-rw-   0        0        0      796 2020-06-06 22:55:31.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/texture_light.glsl
+-rw-rw-rw-   0        0        0      426 2020-06-07 01:12:04.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/vertex_color.glsl
+-rw-rw-rw-   0        0        0      559 2020-06-07 01:51:45.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl
+-rw-rw-rw-   0        0        0      500 2020-06-06 23:25:16.000000 moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/wireframe.glsl
+-rw-rw-rw-   0        0        0     8516 2020-08-22 11:49:55.000000 moderngl-window-2.4.5/moderngl_window/scene/programs.py
+-rw-rw-rw-   0        0        0     9744 2020-08-22 11:49:55.000000 moderngl-window-2.4.5/moderngl_window/scene/scene.py
+-rw-rw-rw-   0        0        0     2590 2020-08-23 13:56:52.000000 moderngl-window-2.4.5/moderngl_window/screenshot.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.507673 moderngl-window-2.4.5/moderngl_window/text/
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.613400 moderngl-window-2.4.5/moderngl_window/text/bitmapped/
+-rw-rw-rw-   0        0        0       43 2021-06-22 07:43:02.000000 moderngl-window-2.4.5/moderngl_window/text/bitmapped/__init__.py
+-rw-rw-rw-   0        0        0     1954 2021-06-22 07:43:02.000000 moderngl-window-2.4.5/moderngl_window/text/bitmapped/base.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.509675 moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.618553 moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/programs/
+-rw-rw-rw-   0        0        0     1696 2021-06-22 07:43:02.000000 moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.623060 moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/text/
+-rw-rw-rw-   0        0        0      262 2021-06-22 07:43:02.000000 moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/text/meta.json
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.624071 moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/textures/
+-rw-rw-rw-   0        0        0   318186 2021-06-22 07:43:02.000000 moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png
+-rw-rw-rw-   0        0        0     2804 2022-06-18 19:36:00.000000 moderngl-window-2.4.5/moderngl_window/text/bitmapped/text_2d.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.626069 moderngl-window-2.4.5/moderngl_window/timers/
+-rw-rw-rw-   0        0        0     1792 2020-08-22 11:46:40.000000 moderngl-window-2.4.5/moderngl_window/timers/base.py
+-rw-rw-rw-   0        0        0     2805 2021-05-13 09:43:41.000000 moderngl-window-2.4.5/moderngl_window/timers/clock.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.629069 moderngl-window-2.4.5/moderngl_window/utils/
+-rw-rw-rw-   0        0        0       42 2020-10-19 05:57:32.000000 moderngl-window-2.4.5/moderngl_window/utils/__init__.py
+-rw-rw-rw-   0        0        0      755 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/moderngl_window/utils/keymaps.py
+-rw-rw-rw-   0        0        0      837 2020-08-22 11:46:20.000000 moderngl-window-2.4.5/moderngl_window/utils/module_loading.py
+-rw-rw-rw-   0        0        0     5381 2020-10-24 12:29:20.000000 moderngl-window-2.4.5/moderngl_window/utils/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.533436 moderngl-window-2.4.5/moderngl_window.egg-info/
+-rw-rw-rw-   0        0        0     8742 2023-10-14 19:12:20.000000 moderngl-window-2.4.5/moderngl_window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5014 2023-10-14 19:12:20.000000 moderngl-window-2.4.5/moderngl_window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-14 19:12:20.000000 moderngl-window-2.4.5/moderngl_window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      421 2023-10-14 19:12:20.000000 moderngl-window-2.4.5/moderngl_window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-10-14 19:12:20.000000 moderngl-window-2.4.5/moderngl_window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3121 2023-10-14 17:25:08.000000 moderngl-window-2.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       98 2023-10-14 19:12:20.652112 moderngl-window-2.4.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-10-14 19:12:20.648113 moderngl-window-2.4.5/tests/
+-rw-rw-rw-   0        0        0      499 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_attribute_names.py
+-rw-rw-rw-   0        0        0     1523 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_camera.py
+-rw-rw-rw-   0        0        0     2976 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_conf.py
+-rw-rw-rw-   0        0        0     9514 2023-10-13 18:25:54.000000 moderngl-window-2.4.5/tests/test_docs.py
+-rw-rw-rw-   0        0        0     3442 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_finders.py
+-rw-rw-rw-   0        0        0     3583 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_geometry.py
+-rw-rw-rw-   0        0        0     3080 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_headless.py
+-rw-rw-rw-   0        0        0     2523 2021-05-13 09:43:41.000000 moderngl-window-2.4.5/tests/test_loaders_data.py
+-rw-rw-rw-   0        0        0     5732 2021-07-23 20:25:43.000000 moderngl-window-2.4.5/tests/test_loaders_program.py
+-rw-rw-rw-   0        0        0     2051 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_loaders_scene.py
+-rw-rw-rw-   0        0        0     3674 2021-05-13 09:43:41.000000 moderngl-window-2.4.5/tests/test_loaders_texture.py
+-rw-rw-rw-   0        0        0     1019 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_moderngl_window.py
+-rw-rw-rw-   0        0        0     1180 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_projection.py
+-rw-rw-rw-   0        0        0     3252 2020-08-23 12:39:13.000000 moderngl-window-2.4.5/tests/test_resource_descriptions.py
+-rw-rw-rw-   0        0        0     2796 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_resources.py
+-rw-rw-rw-   0        0        0     1275 2021-07-23 20:25:43.000000 moderngl-window-2.4.5/tests/test_scheduler.py
+-rw-rw-rw-   0        0        0     1073 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_screenshot.py
+-rw-rw-rw-   0        0        0     6810 2020-07-30 15:13:16.000000 moderngl-window-2.4.5/tests/test_shader_source.py
+-rw-rw-rw-   0        0        0      718 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_timers.py
+-rw-rw-rw-   0        0        0      862 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_utils.py
+-rw-rw-rw-   0        0        0     3833 2020-01-10 17:44:38.000000 moderngl-window-2.4.5/tests/test_vao.py
+-rw-rw-rw-   0        0        0     6569 2021-09-15 19:27:40.000000 moderngl-window-2.4.5/tests/test_windowconfig.py
```

### Comparing `moderngl-window-2.4.4/LICENSE` & `moderngl-window-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/PKG-INFO` & `moderngl-window-2.4.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,67 @@
 Metadata-Version: 2.1
 Name: moderngl-window
-Version: 2.4.4
+Version: 2.4.5
 Summary: A cross platform helper library for ModernGL making window creation and resource loading simple
-Home-page: https://github.com/moderngl/moderngl_window
-Author: Einar Forselv
-Author-email: eforselv@gmail.com
-License: MIT
+Author-email: Einar Forselv <eforselv@gmail.com>
+Project-URL: Source, https://github.com/moderngl/moderngl_window
 Project-URL: Documentation, https://moderngl-window.readthedocs.io
 Project-URL: ModernGL, https://github.com/moderngl/moderngl
-Keywords: moderngl,window,context
-Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: PySide2
-Provides-Extra: pyqt5
-Provides-Extra: glfw
-Provides-Extra: PySDL2
-Provides-Extra: pywavefront
-Provides-Extra: trimesh
-Provides-Extra: tk
-Provides-Extra: pygame
 License-File: LICENSE
+Requires-Dist: moderngl<6
+Requires-Dist: pyglet~=2.0.0
+Requires-Dist: numpy<2,>=1.16
+Requires-Dist: pyrr<1,>=0.10.3
+Requires-Dist: Pillow~=10.0.1
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pywavefront; extra == "dev"
+Requires-Dist: trimesh; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: Sphinx~=7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme~=1.3.0; extra == "docs"
+Requires-Dist: doc8; extra == "docs"
+Provides-Extra: pygame
+Requires-Dist: pygame>=2.0.1; extra == "pygame"
+Provides-Extra: pygame-ce
+Requires-Dist: pygame-ce>=2.0.1; extra == "pygame-ce"
+Provides-Extra: tk
+Requires-Dist: pyopengltk>=0.0.3; extra == "tk"
+Provides-Extra: trimesh
+Requires-Dist: trimesh<4,>=3.2.6; extra == "trimesh"
+Provides-Extra: pywavefront
+Requires-Dist: pywavefront<2,>=1.2.0; extra == "pywavefront"
+Provides-Extra: pysdl2
+Requires-Dist: PySDL2; extra == "pysdl2"
+Provides-Extra: glfw
+Requires-Dist: glfw; extra == "glfw"
+Provides-Extra: pyqt5
+Requires-Dist: PyQt5; extra == "pyqt5"
+Provides-Extra: pyside2
+Requires-Dist: PySide2<6; extra == "pyside2"
+Provides-Extra: pdf
+Requires-Dist: ReportLab>=1.2; extra == "pdf"
 
 [![pypi](https://badge.fury.io/py/moderngl-window.svg)](https://pypi.python.org/pypi/moderngl-window) [![rtd](https://readthedocs.org/projects/moderngl-window/badge/?version=latest)](https://moderngl-window.readthedocs.io)
 
 # moderngl-window
 
 A cross platform utility library for [ModernGL](https://github.com/moderngl/moderngl) making window
 creation and resource loading simple. It can also be used with PyOpenGL for
@@ -69,15 +95,15 @@
 library. If you have an exiting project and just need texture loading
 you will be able to do this without unnecessary hurdles as long as
 you provide us your `moderngl.Context`.
 
 ## Install
 
 ```bash
-pip install moderngl-window
+$ pip install moderngl-window
 ```
 
 ## Supported Platforms
 
 * [x] Windows
 * [x] Linux
 * [x] Mac OS X
@@ -98,58 +124,52 @@
 
 Test.run()
 ```
 
 Run the example with different window backends:
 
 ```bash
-python test.py --window pyglet
-python test.py --window pygame2
-python test.py --window glfw
-python test.py --window sdl2
-python test.py --window pyside2
-python test.py --window pyqt5
-python test.py --window tk
+$ python test.py --window pyglet
+$ python test.py --window pygame2
+$ python test.py --window glfw
+$ python test.py --window sdl2
+$ python test.py --window pyside2
+$ python test.py --window pyqt5
+$ python test.py --window tk
 ```
 
 `WindowConfig` classes are the simplest way to get started without knowing
 a lot about this library. For more advanced usage see documentation
 or examples.
 
 ## Setup from source
 
 We assume the user knows how to handle virtualenvs.
 
 ```bash
 # Install the package in editable mode
 $ pip install -e .
 
-# Set up and dev requirements
-pip install -r requirements.txt
-pip install -r tests/requirements.txt
+# Install development requirements
+$ pip install -e .[dev]
 ```
 
 ## Running Tests
 
-Tests are set up with `tox` running pytest with coverage and flake8.
+With dev requirements installed:
 
-```bash
-pip install -r tests/requirements.txt
-tox -e py36
-tox -e py37
-tox -e py38
-tox -e py39
-tox -e pep8
+```
+pytest
 ```
 
 ## Building Docs
 
 ```bash
-pip install -r docs/requirements.txt
-python setup.py build_sphinx
+$ pip install -e .[dev]
+$ sphinx-build -b html docs docs/_build
 ```
 
 ## Contributing
 
 Contributions are welcome regardless of experience level.
 Don't hesitate submitting issues, opening partial or completed
 pull requests.
```

### Comparing `moderngl-window-2.4.4/README.md` & `moderngl-window-2.4.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 library. If you have an exiting project and just need texture loading
 you will be able to do this without unnecessary hurdles as long as
 you provide us your `moderngl.Context`.
 
 ## Install
 
 ```bash
-pip install moderngl-window
+$ pip install moderngl-window
 ```
 
 ## Supported Platforms
 
 * [x] Windows
 * [x] Linux
 * [x] Mac OS X
@@ -63,58 +63,52 @@
 
 Test.run()
 ```
 
 Run the example with different window backends:
 
 ```bash
-python test.py --window pyglet
-python test.py --window pygame2
-python test.py --window glfw
-python test.py --window sdl2
-python test.py --window pyside2
-python test.py --window pyqt5
-python test.py --window tk
+$ python test.py --window pyglet
+$ python test.py --window pygame2
+$ python test.py --window glfw
+$ python test.py --window sdl2
+$ python test.py --window pyside2
+$ python test.py --window pyqt5
+$ python test.py --window tk
 ```
 
 `WindowConfig` classes are the simplest way to get started without knowing
 a lot about this library. For more advanced usage see documentation
 or examples.
 
 ## Setup from source
 
 We assume the user knows how to handle virtualenvs.
 
 ```bash
 # Install the package in editable mode
 $ pip install -e .
 
-# Set up and dev requirements
-pip install -r requirements.txt
-pip install -r tests/requirements.txt
+# Install development requirements
+$ pip install -e .[dev]
 ```
 
 ## Running Tests
 
-Tests are set up with `tox` running pytest with coverage and flake8.
+With dev requirements installed:
 
-```bash
-pip install -r tests/requirements.txt
-tox -e py36
-tox -e py37
-tox -e py38
-tox -e py39
-tox -e pep8
+```
+pytest
 ```
 
 ## Building Docs
 
 ```bash
-pip install -r docs/requirements.txt
-python setup.py build_sphinx
+$ pip install -e .[dev]
+$ sphinx-build -b html docs docs/_build
 ```
 
 ## Contributing
 
 Contributions are welcome regardless of experience level.
 Don't hesitate submitting issues, opening partial or completed
 pull requests.
```

### Comparing `moderngl-window-2.4.4/moderngl_window/__init__.py` & `moderngl-window-2.4.5/moderngl_window/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import argparse
 import logging
 import os
 import sys
 import weakref
 
 from pathlib import Path
-from typing import List, Type
+from typing import List, Type, Optional
 
 import moderngl
 from moderngl_window.context.base import WindowConfig, BaseWindow
 from moderngl_window.timers.clock import Timer
 from moderngl_window.conf import settings
 from moderngl_window.utils.module_loading import import_string
 from moderngl_window.utils.keymaps import KeyMapFactory, KeyMap, QWERTY, AZERTY  # noqa
 
-__version__ = "2.4.4"
+__version__ = "2.4.5"
 
 IGNORE_DIRS = [
     "__pycache__",
     "base",
 ]
 
 # Add new windows classes here to be recognized by the command line option --window
@@ -56,17 +56,16 @@
             logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         )
         logger.addHandler(ch)
 
 
 class ContextRefs:
     """Namespace for window/context references"""
-
-    WINDOW = None
-    CONTEXT = None
+    WINDOW: Optional[BaseWindow] = None
+    CONTEXT: Optional[moderngl.Context] = None
 
 
 def activate_context(window: BaseWindow = None, ctx: moderngl.Context = None):
     """
     Register the active window and context.
     If only a window is supplied the context is taken from the window.
     Only a context can also be passed in.
```

### Comparing `moderngl-window-2.4.4/moderngl_window/atlas/base.py` & `moderngl-window-2.4.5/moderngl_window/atlas/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/atlas/simple_atlas.py` & `moderngl-window-2.4.5/moderngl_window/atlas/simple_atlas.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/capture/base.py` & `moderngl-window-2.4.5/moderngl_window/capture/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/capture/ffmpeg.py` & `moderngl-window-2.4.5/moderngl_window/capture/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/conf/__init__.py` & `moderngl-window-2.4.5/moderngl_window/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/conf/default.py` & `moderngl-window-2.4.5/moderngl_window/conf/default.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/base/window.py` & `moderngl-window-2.4.5/moderngl_window/context/base/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser
 from functools import wraps
 from pathlib import Path
 import logging
 import sys
 import weakref
-from typing import Any, Tuple, Type, List, Optional
+from typing import Any, Tuple, Type, List, Optional, Dict
 
 import moderngl
 from moderngl_window.context.base import KeyModifiers, BaseKeys
 from moderngl_window.timers.base import BaseTimer
 from moderngl_window import resources
 from moderngl_window.geometry.attributes import AttributeNames
 from moderngl_window.meta import (
@@ -66,15 +66,15 @@
 
 class BaseWindow:
     """
     Helper base class for a generic window implementation
     """
 
     #: Name of the window. For example ``pyglet``, ``glfw``
-    name = None
+    name = "base"
     #: Window specific key constants
     keys = BaseKeys
     #: Mouse button enum
     mouse = MouseButtons
 
     def __init__(
         self,
@@ -1214,15 +1214,15 @@
     def load_texture_2d(
         self,
         path: str,
         flip=True,
         flip_x=False,
         flip_y=True,
         mipmap=False,
-        mipmap_levels: Tuple[int, int] = None,
+        mipmap_levels: Optional[Tuple[int, int]] = None,
         anisotropy=1.0,
         **kwargs
     ) -> moderngl.Texture:
         """Loads a 2D texture.
 
         If the path is relative the resource system is used expecting one or more
         resource directories to be registered first. Absolute paths will attempt
@@ -1258,15 +1258,15 @@
 
     def load_texture_array(
         self,
         path: str,
         layers: int = 0,
         flip=True,
         mipmap=False,
-        mipmap_levels: Tuple[int, int] = None,
+        mipmap_levels: Optional[Tuple[int, int]] = None,
         anisotropy=1.0,
         **kwargs
     ) -> moderngl.TextureArray:
         """Loads a texture array.
 
         If the path is relative the resource system is used expecting one or more
         resource directories to be registered first. Absolute paths will attempt
@@ -1303,25 +1303,25 @@
                 anisotropy=anisotropy,
                 **kwargs,
             )
         )
 
     def load_texture_cube(
         self,
-        pos_x: str = None,
-        pos_y: str = None,
-        pos_z: str = None,
-        neg_x: str = None,
-        neg_y: str = None,
-        neg_z: str = None,
+        pos_x: str = "",
+        pos_y: str = "",
+        pos_z: str = "",
+        neg_x: str = "",
+        neg_y: str = "",
+        neg_z: str = "",
         flip=False,
         flip_x=False,
         flip_y=False,
         mipmap=False,
-        mipmap_levels: Tuple[int, int] = None,
+        mipmap_levels: Optional[Tuple[int, int]] = None,
         anisotropy=1.0,
         **kwargs
     ) -> moderngl.TextureCube:
         """Loads a texture cube.
 
         If the path is relative the resource system is used expecting one or more
         resource directories to be registered first. Absolute paths will attempt
@@ -1369,16 +1369,16 @@
         self,
         path=None,
         vertex_shader=None,
         geometry_shader=None,
         fragment_shader=None,
         tess_control_shader=None,
         tess_evaluation_shader=None,
-        defines: dict = None,
-        varyings: List[str] = None,
+        defines: Optional[dict] = None,
+        varyings: Optional[List[str]] = None,
     ) -> moderngl.Program:
         """Loads a shader program.
 
         Note that `path` should only be used if all shaders are defined
         in the same glsl file separated by defines.
 
         If the path is relative the resource system is used expecting one or more
@@ -1408,15 +1408,15 @@
                 tess_evaluation_shader=tess_evaluation_shader,
                 defines=defines,
                 varyings=varyings,
             )
         )
 
     def load_compute_shader(
-        self, path, defines: dict = None, **kwargs
+        self, path, defines: Optional[Dict] = None, **kwargs
     ) -> moderngl.ComputeShader:
         """Loads a compute shader.
 
         Args:
             path (str): Path to a single glsl file
             defines (dict): ``#define`` values to replace in the shader source.
                             Example: ``{'VALUE1': 10, 'VALUE2': '3.1415'}``.
```

### Comparing `moderngl-window-2.4.4/moderngl_window/context/glfw/keys.py` & `moderngl-window-2.4.5/moderngl_window/context/glfw/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/glfw/window.py` & `moderngl-window-2.4.5/moderngl_window/context/glfw/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/headless/window.py` & `moderngl-window-2.4.5/moderngl_window/context/headless/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pygame2/keys.py` & `moderngl-window-2.4.5/moderngl_window/context/pygame2/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pygame2/window.py` & `moderngl-window-2.4.5/moderngl_window/context/pygame2/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pyglet/keys.py` & `moderngl-window-2.4.5/moderngl_window/context/pyglet/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pyglet/window.py` & `moderngl-window-2.4.5/moderngl_window/context/pyglet/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pyqt5/keys.py` & `moderngl-window-2.4.5/moderngl_window/context/pyqt5/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pyqt5/window.py` & `moderngl-window-2.4.5/moderngl_window/context/pyqt5/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pyside2/keys.py` & `moderngl-window-2.4.5/moderngl_window/context/pyside2/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/pyside2/window.py` & `moderngl-window-2.4.5/moderngl_window/context/pyside2/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/sdl2/keys.py` & `moderngl-window-2.4.5/moderngl_window/context/sdl2/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/sdl2/window.py` & `moderngl-window-2.4.5/moderngl_window/context/sdl2/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/tk/keys.py` & `moderngl-window-2.4.5/moderngl_window/context/tk/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/context/tk/window.py` & `moderngl-window-2.4.5/moderngl_window/context/tk/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/finders/base.py` & `moderngl-window-2.4.5/moderngl_window/finders/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/geometry/attributes.py` & `moderngl-window-2.4.5/moderngl_window/geometry/attributes.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/geometry/bbox.py` & `moderngl-window-2.4.5/moderngl_window/geometry/bbox.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/geometry/cube.py` & `moderngl-window-2.4.5/moderngl_window/geometry/cube.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/geometry/quad.py` & `moderngl-window-2.4.5/moderngl_window/geometry/quad.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/geometry/sphere.py` & `moderngl-window-2.4.5/moderngl_window/geometry/sphere.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/integrations/imgui.py` & `moderngl-window-2.4.5/moderngl_window/integrations/imgui.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/base.py` & `moderngl-window-2.4.5/moderngl_window/loaders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from moderngl_window.finders import data, program, scene, texture
 
 logger = logging.getLogger(__name__)
 
 
 class BaseLoader:
     """Base loader class for all resources"""
-
-    kind = None
+    kind = "unknown"
     """
     The kind of resource this loaded supports.
     This can be used when file extensions is not enough
     to decide what loader should be selected.
     """
     file_extensions = []
     """
```

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/data/binary.py` & `moderngl-window-2.4.5/moderngl_window/loaders/data/binary.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/data/json.py` & `moderngl-window-2.4.5/moderngl_window/loaders/data/json.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/data/text.py` & `moderngl-window-2.4.5/moderngl_window/loaders/data/text.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/program/separate.py` & `moderngl-window-2.4.5/moderngl_window/loaders/program/separate.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/program/single.py` & `moderngl-window-2.4.5/moderngl_window/loaders/program/single.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/scene/gltf2.py` & `moderngl-window-2.4.5/moderngl_window/loaders/scene/gltf2.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                         self.path, magic, GLTF_MAGIC_HEADER
                     )
                 )
 
             version = struct.unpack("<I", fd.read(4))[0]
             if version != 2:
                 raise ValueError(
-                    "{} has unsupported version {}".format(self.path, version)
+                    f"{self.path} has unsupported version {version}"
                 )
 
             # Total file size including headers
             _ = struct.unpack("<I", fd.read(4))[0]  # noqa
 
             # Chunk 0 - json
             chunk_0_length = struct.unpack("<I", fd.read(4))[0]
@@ -383,33 +383,31 @@
 
     @property
     def version(self):
         return self.asset.version
 
     def check_version(self, required="2.0"):
         if not self.version == required:
-            msg = "GLTF Format version is not 2.0. Version states '{}' in file {}".format(
-                self.version, self.path,
-            )
+            msg = f"GLTF Format version is not 2.0. Version states '{self.version}' in file {self.path}"
             raise ValueError(msg)
 
     def check_extensions(self, supported):
         """
         "extensionsRequired": ["KHR_draco_mesh_compression"],
         "extensionsUsed": ["KHR_draco_mesh_compression"]
         """
         if self.data.get("extensionsRequired"):
             for ext in self.data.get("extensionsRequired"):
                 if ext not in supported:
-                    raise ValueError("Extension {} not supported".format(ext))
+                    raise ValueError(f"Extension {ext} not supported")
 
         if self.data.get("extensionsUsed"):
             for ext in self.data.get("extensionsUsed"):
                 if ext not in supported:
-                    raise ValueError("Extension {} not supported".format(ext))
+                    raise ValueError("Extension {ext} not supported")
 
     def buffers_exist(self):
         """Checks if the bin files referenced exist"""
         for buff in self.buffers:
             if not buff.is_separate_file:
                 continue
```

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/scene/stl.py` & `moderngl-window-2.4.5/moderngl_window/loaders/scene/stl.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/scene/wavefront.py` & `moderngl-window-2.4.5/moderngl_window/loaders/scene/wavefront.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/texture/array.py` & `moderngl-window-2.4.5/moderngl_window/loaders/texture/array.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/texture/cube.py` & `moderngl-window-2.4.5/moderngl_window/loaders/texture/cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import namedtuple
 
 from moderngl_window.loaders.texture.pillow import PillowLoader, image_data
 from moderngl_window.exceptions import ImproperlyConfigured
 
-FaceInfo = namedtuple("FaceData", ["width", "height", "data", "components"])
+FaceInfo = namedtuple("FaceInfo", ["width", "height", "data", "components"])
 
 
 class Loader(PillowLoader):
     kind = "cube"
 
     def __init__(self, meta):
         super().__init__(meta)
@@ -51,15 +51,15 @@
     def _load_face(self, path: str, face_name: str = None):
         """Obtain raw byte data for a face
 
         Returns:
             Tuple[int, bytes]: number of components, byte data
         """
         if not path:
-            raise ImproperlyConfigured("{} texture face not supplied".format(face_name))
+            raise ImproperlyConfigured(f"{face_name} texture face not supplied")
 
         image = self._load_texture(path)
         components, data = image_data(image)
         return FaceInfo(
             width=image.size[0], height=image.size[1], data=data, components=components
         )
```

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/texture/icon.py` & `moderngl-window-2.4.5/moderngl_window/loaders/texture/icon.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/texture/pillow.py` & `moderngl-window-2.4.5/moderngl_window/loaders/texture/pillow.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/loaders/texture/t2d.py` & `moderngl-window-2.4.5/moderngl_window/loaders/texture/t2d.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/meta/base.py` & `moderngl-window-2.4.5/moderngl_window/meta/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 class ResourceDescription:
     """ Description of any resource.
     Resource descriptions are required to load a resource.
     This class can be extended to add more specific properties.
     """
 
-    default_kind = None  # The default kind of loader
+    default_kind = ""  # The default kind of loader
     """str: The default kind for this resource type"""
-    resource_type = None  # What resource type is described
+    resource_type = ""  # What resource type is described
     """str: A unique identifier for the resource type"""
 
     def __init__(self, **kwargs):
         """Initialize a resource description
 
         Args:
             **kwargs: Attributes describing the resource to load
```

### Comparing `moderngl-window-2.4.4/moderngl_window/meta/data.py` & `moderngl-window-2.4.5/moderngl_window/meta/data.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/meta/program.py` & `moderngl-window-2.4.5/moderngl_window/meta/program.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 from moderngl_window.meta.base import ResourceDescription
 
 
 class ProgramDescription(ResourceDescription):
     """Describes a program to load
 
     By default a program can be loaded in the following ways:
@@ -25,25 +25,25 @@
     """
 
     default_kind = None
     resource_type = "programs"
 
     def __init__(
         self,
-        path: str = None,
-        kind: str = None,
+        path: Optional[str] = None,
+        kind: Optional[str] = None,
         reloadable=False,
-        vertex_shader: str = None,
-        geometry_shader: str = None,
-        fragment_shader: str = None,
-        tess_control_shader: str = None,
-        tess_evaluation_shader: str = None,
-        compute_shader: str = None,
-        defines: dict = None,
-        varyings: List = None,
+        vertex_shader: Optional[str] = None,
+        geometry_shader: Optional[str] = None,
+        fragment_shader: Optional[str] = None,
+        tess_control_shader: Optional[str] = None,
+        tess_evaluation_shader: Optional[str] = None,
+        compute_shader: Optional[str] = None,
+        defines: Optional[dict] = None,
+        varyings: Optional[List] = None,
         **kwargs
     ):
         """Create a program description
 
         Keyword Args:
             path (str): path to the resource relative to search directories
             kind (str): The kind of loader to use
```

### Comparing `moderngl-window-2.4.4/moderngl_window/meta/scene.py` & `moderngl-window-2.4.5/moderngl_window/meta/scene.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/meta/texture.py` & `moderngl-window-2.4.5/moderngl_window/meta/texture.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/opengl/program.py` & `moderngl-window-2.4.5/moderngl_window/opengl/program.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Helper classes for loading shader
 """
-from typing import List, Tuple, Union
+from typing import List, Tuple, Union, Optional
 import re
 
 import moderngl
 import moderngl_window
 from moderngl_window.meta import ProgramDescription
 
 VERTEX_SHADER = "VERTEX_SHADER"
@@ -17,20 +17,20 @@
 
 
 class ProgramShaders:
     """Helper class preparing shader source strings for a program"""
 
     def __init__(self, meta: ProgramDescription):
         self.meta = meta
-        self.vertex_source = None
-        self.geometry_source = None
-        self.fragment_source = None
-        self.tess_control_source = None
-        self.tess_evaluation_source = None
-        self.compute_shader_source = None
+        self.vertex_source: Optional[ShaderSource] = None
+        self.geometry_source: Optional[ShaderSource] = None
+        self.fragment_source: Optional[ShaderSource] = None
+        self.tess_control_source: Optional[ShaderSource] = None
+        self.tess_evaluation_source: Optional[ShaderSource] = None
+        self.compute_shader_source: Optional[ShaderSource] = None
 
     @property
     def ctx(self) -> moderngl.Context:
         """The moderngl context"""
         return moderngl_window.ctx()
 
     @classmethod
@@ -205,16 +205,16 @@
             self.compute_shader_source.handle_includes(load_source_func)
 
 
 class ShaderSource:
     """
     Helper class representing a single shader type.
 
-    It ensures the source has the right format, injects ``#define`` preprocessors,
-    resolves ``#include`` preprocessors etc.
+    It ensures the source has the right format, injects ``#define`` pre-processors,
+    resolves ``#include`` pre-processors etc.
 
     A ``ShaderSource`` can be the base/root shader or a source referenced in an ``#include``.
     """
 
     def __init__(
         self,
         shader_type: str,
@@ -246,24 +246,22 @@
             source = source.strip()
         self._lines = source.split("\n")
 
         # Make sure version is present (only if root shader)
         if self._root and not self._lines[0].startswith("#version"):
             self.print()
             raise ShaderError(
-                "Missing #version in {}. A version must be defined in the first line".format(
-                    self._name
-                ),
+                f"Missing #version in {self._name}. A version must be defined in the first line"
             )
 
         self.apply_defines(defines)
 
         # Inject source with shade type
         if self._root:
-            self._lines.insert(1, "#define {} 1".format(self._type))
+            self._lines.insert(1, f"#define {self._type} 1")
             self._lines.insert(2, "#line 2")
 
     @property
     def id(self) -> int:
         """int: The shader number/id"""
         return self._id
 
@@ -295,20 +293,21 @@
     @property
     def defines(self) -> dict:
         """dict: Defines configured for this shader"""
         return self._defines
 
     def handle_includes(self, load_source_func, depth=0, source_id=0):
         """Inject includes into the shader source.
-        This happens recursively up to a max level in case the users has circular includes.
-        We also build up a list of all the included sources in the root shader.
+        This happens recursively up to a max level in case the users has
+        circular includes. We also build up a list of all the included
+        sources in the root shader.
 
         Args:
             load_source_func (func): A function for finding and loading a source
-            depth (int): The current include depth (incease by 1 for every call)
+            depth (int): The current include depth (increase by 1 for every call)
         """
         if depth > 100:
             raise ShaderError(
                 "Reaching an include depth of 100. You probably have circular includes"
             )
 
         current_id = source_id
@@ -347,15 +346,15 @@
             if line.startswith("#define"):
                 try:
                     name = line.split()[1]
                     value = defines.get(name)
                     if not value:
                         continue
 
-                    self.lines[nr] = "#define {} {}".format(name, str(value))
+                    self.lines[nr] = f"#define {name} {value}"
                 except IndexError:
                     pass
 
     def find_out_attribs(self) -> List[str]:
         """
         Get all out attributes in the shader source.
 
@@ -370,27 +369,27 @@
             if res:
                 names.append(res.groups()[-1])
 
         return names
 
     def print(self):
         """Print the shader lines (for debugging)"""
-        print("---[ START {} ]---".format(self.name))
+        print(f"---[ START {self.name} ]---")
 
         for i, line in enumerate(self.lines):
-            print("{}: {}".format(str(i).zfill(3), line))
+            print(f"{str(i).zfill(3)}: {line}")
 
-        print("---[ END {} ]---".format(self.name))
+        print("---[ END {self.name} ]---")
 
     def __repr__(self):
-        return "<ShaderSource: {} id={}>".format(self.name, self.id)
+        return f"<ShaderSource: {self.name} id={self.id}>"
 
 
 class ShaderError(Exception):
-    pass
+    """Generic shader related error"""
 
 
 class ReloadableProgram:
     """
     Programs we want to be reloadable must be created with this wrapper.
     """
 
@@ -477,8 +476,8 @@
         """
         int: The maximum number of vertices that
         the geometry shader will output.
         """
         return self.program.geometry_vertices
 
     def __repr__(self):
-        return "<ReloadableProgram: {} id={}>".format(self.name, self.glo)
+        return f"<ReloadableProgram: {self.name} id={self.glo}>"
```

### Comparing `moderngl-window-2.4.4/moderngl_window/opengl/projection.py` & `moderngl-window-2.4.5/moderngl_window/opengl/projection.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/opengl/types.py` & `moderngl-window-2.4.5/moderngl_window/opengl/types.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/opengl/vao.py` & `moderngl-window-2.4.5/moderngl_window/opengl/vao.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/resources/__init__.py` & `moderngl-window-2.4.5/moderngl_window/resources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if Path(resource_path).samefile(path):
             break
     else:
         dest.append(Path(path).absolute())
 
 
 @contextmanager
-def temporary_dirs(dirs: Union[Path, str] = []):
+def temporary_dirs(dirs: Union[Path, str]):
     """Temporarily changes all resource directories
 
     Example::
 
         with temporary_dirs([path1, path2, path3]):
             # Load some resource here
```

### Comparing `moderngl-window-2.4.4/moderngl_window/resources/base.py` & `moderngl-window-2.4.5/moderngl_window/resources/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/resources/data.py` & `moderngl-window-2.4.5/moderngl_window/resources/data.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/resources/programs.py` & `moderngl-window-2.4.5/moderngl_window/resources/programs.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/resources/scenes.py` & `moderngl-window-2.4.5/moderngl_window/resources/scenes.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/resources/textures.py` & `moderngl-window-2.4.5/moderngl_window/resources/textures.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/resources/tracks.py` & `moderngl-window-2.4.5/moderngl_window/resources/tracks.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/camera.py` & `moderngl-window-2.4.5/moderngl_window/scene/camera.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/material.py` & `moderngl-window-2.4.5/moderngl_window/scene/material.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/mesh.py` & `moderngl-window-2.4.5/moderngl_window/scene/mesh.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/node.py` & `moderngl-window-2.4.5/moderngl_window/scene/node.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/color_light.glsl` & `moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/color_light.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/texture_light.glsl` & `moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/texture_light.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl` & `moderngl-window-2.4.5/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/programs.py` & `moderngl-window-2.4.5/moderngl_window/scene/programs.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/scene/scene.py` & `moderngl-window-2.4.5/moderngl_window/scene/scene.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/screenshot.py` & `moderngl-window-2.4.5/moderngl_window/screenshot.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/text/bitmapped/base.py` & `moderngl-window-2.4.5/moderngl_window/text/bitmapped/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl` & `moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png` & `moderngl-window-2.4.5/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/text/bitmapped/text_2d.py` & `moderngl-window-2.4.5/moderngl_window/text/bitmapped/text_2d.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/timers/base.py` & `moderngl-window-2.4.5/moderngl_window/timers/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/timers/clock.py` & `moderngl-window-2.4.5/moderngl_window/timers/clock.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/utils/keymaps.py` & `moderngl-window-2.4.5/moderngl_window/utils/keymaps.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/utils/module_loading.py` & `moderngl-window-2.4.5/moderngl_window/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window/utils/scheduler.py` & `moderngl-window-2.4.5/moderngl_window/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.4/moderngl_window.egg-info/PKG-INFO` & `moderngl-window-2.4.5/moderngl_window.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,67 @@
 Metadata-Version: 2.1
 Name: moderngl-window
-Version: 2.4.4
+Version: 2.4.5
 Summary: A cross platform helper library for ModernGL making window creation and resource loading simple
-Home-page: https://github.com/moderngl/moderngl_window
-Author: Einar Forselv
-Author-email: eforselv@gmail.com
-License: MIT
+Author-email: Einar Forselv <eforselv@gmail.com>
+Project-URL: Source, https://github.com/moderngl/moderngl_window
 Project-URL: Documentation, https://moderngl-window.readthedocs.io
 Project-URL: ModernGL, https://github.com/moderngl/moderngl
-Keywords: moderngl,window,context
-Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: PySide2
-Provides-Extra: pyqt5
-Provides-Extra: glfw
-Provides-Extra: PySDL2
-Provides-Extra: pywavefront
-Provides-Extra: trimesh
-Provides-Extra: tk
-Provides-Extra: pygame
 License-File: LICENSE
+Requires-Dist: moderngl<6
+Requires-Dist: pyglet~=2.0.0
+Requires-Dist: numpy<2,>=1.16
+Requires-Dist: pyrr<1,>=0.10.3
+Requires-Dist: Pillow~=10.0.1
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pywavefront; extra == "dev"
+Requires-Dist: trimesh; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: Sphinx~=7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme~=1.3.0; extra == "docs"
+Requires-Dist: doc8; extra == "docs"
+Provides-Extra: pygame
+Requires-Dist: pygame>=2.0.1; extra == "pygame"
+Provides-Extra: pygame-ce
+Requires-Dist: pygame-ce>=2.0.1; extra == "pygame-ce"
+Provides-Extra: tk
+Requires-Dist: pyopengltk>=0.0.3; extra == "tk"
+Provides-Extra: trimesh
+Requires-Dist: trimesh<4,>=3.2.6; extra == "trimesh"
+Provides-Extra: pywavefront
+Requires-Dist: pywavefront<2,>=1.2.0; extra == "pywavefront"
+Provides-Extra: pysdl2
+Requires-Dist: PySDL2; extra == "pysdl2"
+Provides-Extra: glfw
+Requires-Dist: glfw; extra == "glfw"
+Provides-Extra: pyqt5
+Requires-Dist: PyQt5; extra == "pyqt5"
+Provides-Extra: pyside2
+Requires-Dist: PySide2<6; extra == "pyside2"
+Provides-Extra: pdf
+Requires-Dist: ReportLab>=1.2; extra == "pdf"
 
 [![pypi](https://badge.fury.io/py/moderngl-window.svg)](https://pypi.python.org/pypi/moderngl-window) [![rtd](https://readthedocs.org/projects/moderngl-window/badge/?version=latest)](https://moderngl-window.readthedocs.io)
 
 # moderngl-window
 
 A cross platform utility library for [ModernGL](https://github.com/moderngl/moderngl) making window
 creation and resource loading simple. It can also be used with PyOpenGL for
@@ -69,15 +95,15 @@
 library. If you have an exiting project and just need texture loading
 you will be able to do this without unnecessary hurdles as long as
 you provide us your `moderngl.Context`.
 
 ## Install
 
 ```bash
-pip install moderngl-window
+$ pip install moderngl-window
 ```
 
 ## Supported Platforms
 
 * [x] Windows
 * [x] Linux
 * [x] Mac OS X
@@ -98,58 +124,52 @@
 
 Test.run()
 ```
 
 Run the example with different window backends:
 
 ```bash
-python test.py --window pyglet
-python test.py --window pygame2
-python test.py --window glfw
-python test.py --window sdl2
-python test.py --window pyside2
-python test.py --window pyqt5
-python test.py --window tk
+$ python test.py --window pyglet
+$ python test.py --window pygame2
+$ python test.py --window glfw
+$ python test.py --window sdl2
+$ python test.py --window pyside2
+$ python test.py --window pyqt5
+$ python test.py --window tk
 ```
 
 `WindowConfig` classes are the simplest way to get started without knowing
 a lot about this library. For more advanced usage see documentation
 or examples.
 
 ## Setup from source
 
 We assume the user knows how to handle virtualenvs.
 
 ```bash
 # Install the package in editable mode
 $ pip install -e .
 
-# Set up and dev requirements
-pip install -r requirements.txt
-pip install -r tests/requirements.txt
+# Install development requirements
+$ pip install -e .[dev]
 ```
 
 ## Running Tests
 
-Tests are set up with `tox` running pytest with coverage and flake8.
+With dev requirements installed:
 
-```bash
-pip install -r tests/requirements.txt
-tox -e py36
-tox -e py37
-tox -e py38
-tox -e py39
-tox -e pep8
+```
+pytest
 ```
 
 ## Building Docs
 
 ```bash
-pip install -r docs/requirements.txt
-python setup.py build_sphinx
+$ pip install -e .[dev]
+$ sphinx-build -b html docs docs/_build
 ```
 
 ## Contributing
 
 Contributions are welcome regardless of experience level.
 Don't hesitate submitting issues, opening partial or completed
 pull requests.
```

### Comparing `moderngl-window-2.4.4/moderngl_window.egg-info/SOURCES.txt` & `moderngl-window-2.4.5/moderngl_window.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
-setup.py
 moderngl_window/__init__.py
 moderngl_window/exceptions.py
 moderngl_window/screenshot.py
 moderngl_window.egg-info/PKG-INFO
 moderngl_window.egg-info/SOURCES.txt
 moderngl_window.egg-info/dependency_links.txt
 moderngl_window.egg-info/requires.txt
@@ -111,8 +111,30 @@
 moderngl_window/text/bitmapped/bitmapped/text/meta.json
 moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png
 moderngl_window/timers/base.py
 moderngl_window/timers/clock.py
 moderngl_window/utils/__init__.py
 moderngl_window/utils/keymaps.py
 moderngl_window/utils/module_loading.py
-moderngl_window/utils/scheduler.py
+moderngl_window/utils/scheduler.py
+tests/test_attribute_names.py
+tests/test_camera.py
+tests/test_conf.py
+tests/test_docs.py
+tests/test_finders.py
+tests/test_geometry.py
+tests/test_headless.py
+tests/test_loaders_data.py
+tests/test_loaders_program.py
+tests/test_loaders_scene.py
+tests/test_loaders_texture.py
+tests/test_moderngl_window.py
+tests/test_projection.py
+tests/test_resource_descriptions.py
+tests/test_resources.py
+tests/test_scheduler.py
+tests/test_screenshot.py
+tests/test_shader_source.py
+tests/test_timers.py
+tests/test_utils.py
+tests/test_vao.py
+tests/test_windowconfig.py
```

