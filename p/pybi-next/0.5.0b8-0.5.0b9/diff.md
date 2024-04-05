# Comparing `tmp/pybi-next-0.5.0b8.tar.gz` & `tmp/pybi-next-0.5.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybi-next-0.5.0b8.tar", last modified: Mon Jan 29 09:57:31 2024, max compression
+gzip compressed data, was "pybi-next-0.5.0b9.tar", last modified: Sun Mar 17 11:04:42 2024, max compression
```

## Comparing `pybi-next-0.5.0b8.tar` & `pybi-next-0.5.0b9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.285632 pybi-next-0.5.0b8/
--rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.5.0b8/LICENSE
--rw-rw-rw-   0        0        0      479 2024-01-29 09:57:31.270422 pybi-next-0.5.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     2400 2024-01-20 14:43:41.000000 pybi-next-0.5.0b8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.002236 pybi-next-0.5.0b8/pybi/
--rw-rw-rw-   0        0        0     2773 2024-01-20 14:43:41.000000 pybi-next-0.5.0b8/pybi/__index.py
--rw-rw-rw-   0        0        0       51 2024-01-29 09:57:14.000000 pybi-next-0.5.0b8/pybi/__init__.py
--rw-rw-rw-   0        0        0    30655 2024-01-20 14:43:41.000000 pybi-next-0.5.0b8/pybi/app.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.019167 pybi-next-0.5.0b8/pybi/core/
--rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.5.0b8/pybi/core/__init__.py
--rw-rw-rw-   0        0        0      176 2023-11-15 18:09:14.000000 pybi-next-0.5.0b8/pybi/core/actions.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.036180 pybi-next-0.5.0b8/pybi/core/components/
--rw-rw-rw-   0        0        0      735 2023-11-16 05:59:00.000000 pybi-next-0.5.0b8/pybi/core/components/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-11-15 18:09:14.000000 pybi-next-0.5.0b8/pybi/core/components/component.py
--rw-rw-rw-   0        0        0      805 2023-11-16 05:59:00.000000 pybi-next-0.5.0b8/pybi/core/components/componentTag.py
--rw-rw-rw-   0        0        0    15329 2023-11-17 08:26:13.000000 pybi-next-0.5.0b8/pybi/core/components/containerComponent.py
--rw-rw-rw-   0        0        0     1964 2023-07-12 09:24:47.000000 pybi-next-0.5.0b8/pybi/core/components/mermaid.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.052984 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/
--rw-rw-rw-   0        0        0      246 2023-06-07 17:40:57.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-11-15 18:09:14.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/base.py
--rw-rw-rw-   0        0        0     2759 2023-06-07 17:40:57.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/checkbox.py
--rw-rw-rw-   0        0        0     5251 2023-08-26 13:10:50.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/echarts.py
--rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/input.py
--rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/markdown.py
--rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/numberSlider.py
--rw-rw-rw-   0        0        0      688 2023-11-09 16:13:09.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/qsInput.py
--rw-rw-rw-   0        0        0     1625 2023-11-09 16:13:09.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/qsSlicer.py
--rw-rw-rw-   0        0        0     5689 2023-11-16 06:07:36.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/qsTable.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 06:06:20.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/slicer.py
--rw-rw-rw-   0        0        0     2889 2023-11-06 15:47:17.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/table.py
--rw-rw-rw-   0        0        0      460 2023-06-05 17:53:25.000000 pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/textValue.py
--rw-rw-rw-   0        0        0     2541 2024-01-20 14:43:41.000000 pybi-next-0.5.0b8/pybi/core/components/staticComponent.py
--rw-rw-rw-   0        0        0     6135 2023-04-21 15:56:29.000000 pybi-next-0.5.0b8/pybi/core/dataSource.py
--rw-rw-rw-   0        0        0      863 2023-11-16 05:59:00.000000 pybi-next-0.5.0b8/pybi/core/imgManager.py
--rw-rw-rw-   0        0        0     5155 2023-11-06 12:43:20.000000 pybi-next-0.5.0b8/pybi/core/sql.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.069414 pybi-next-0.5.0b8/pybi/core/styles/
--rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.5.0b8/pybi/core/styles/__init__.py
--rw-rw-rw-   0        0        0      535 2023-04-17 04:53:14.000000 pybi-next-0.5.0b8/pybi/core/styles/styleTag.py
--rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.5.0b8/pybi/core/styles/styles.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.069414 pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/
--rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/boxShadow.py
--rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/textAlign.py
--rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/textColor.py
--rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/textSize.py
--rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.5.0b8/pybi/core/styles/utils.py
--rw-rw-rw-   0        0        0     5548 2023-11-16 05:59:00.000000 pybi-next-0.5.0b8/pybi/core/uiResource.py
--rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.5.0b8/pybi/core/webResources.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.102563 pybi-next-0.5.0b8/pybi/easyEcharts/
--rw-rw-rw-   0        0        0     3901 2023-11-01 17:02:37.000000 pybi-next-0.5.0b8/pybi/easyEcharts/__init__.py
--rw-rw-rw-   0        0        0     3300 2023-05-22 12:03:15.000000 pybi-next-0.5.0b8/pybi/easyEcharts/bar.py
--rw-rw-rw-   0        0        0     4041 2023-11-01 17:02:37.000000 pybi-next-0.5.0b8/pybi/easyEcharts/base.py
--rw-rw-rw-   0        0        0     2636 2023-05-22 12:03:15.000000 pybi-next-0.5.0b8/pybi/easyEcharts/candlestick.py
--rw-rw-rw-   0        0        0      502 2023-11-01 17:02:37.000000 pybi-next-0.5.0b8/pybi/easyEcharts/dictChart.py
--rw-rw-rw-   0        0        0     3415 2023-05-22 12:03:15.000000 pybi-next-0.5.0b8/pybi/easyEcharts/line.py
--rw-rw-rw-   0        0        0     1678 2023-05-22 12:03:15.000000 pybi-next-0.5.0b8/pybi/easyEcharts/map.py
--rw-rw-rw-   0        0        0     2423 2023-05-22 12:03:15.000000 pybi-next-0.5.0b8/pybi/easyEcharts/pie.py
--rw-rw-rw-   0        0        0     2716 2023-05-22 12:03:15.000000 pybi-next-0.5.0b8/pybi/easyEcharts/radar.py
--rw-rw-rw-   0        0        0     1920 2023-05-22 12:03:15.000000 pybi-next-0.5.0b8/pybi/easyEcharts/scatter.py
--rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.5.0b8/pybi/easyEcharts/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.102563 pybi-next-0.5.0b8/pybi/icons/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.5.0b8/pybi/icons/__init__.py
--rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.5.0b8/pybi/icons/iconManager.py
--rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.5.0b8/pybi/icons/material_icons.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.219614 pybi-next-0.5.0b8/pybi/static/
--rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.5.0b8/pybi/static/echarts.min.js
--rw-rw-rw-   0        0        0      597 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/echartsCps-style.css
--rw-rw-rw-   0        0        0    35733 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/echartsCps.iife.js
--rw-rw-rw-   0        0        0   127313 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/elementCps-style.css
--rw-rw-rw-   0        0        0   377610 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/elementCps.iife.js
--rw-rw-rw-   0        0        0     1672 2023-05-31 14:01:04.000000 pybi-next-0.5.0b8/pybi/static/experimentalCps-style.css
--rw-rw-rw-   0        0        0    17540 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/experimentalCps.iife.js
--rw-rw-rw-   0        0        0   171735 2023-11-04 15:18:39.000000 pybi-next-0.5.0b8/pybi/static/material_icons.css
--rw-rw-rw-   0        0        0      584 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/mermaidCps-style.css
--rw-rw-rw-   0        0        0  2889888 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/mermaidCps.iife.js
--rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.5.0b8/pybi/static/province_map_full.json
--rw-rw-rw-   0        0        0     2480 2023-11-04 19:17:57.000000 pybi-next-0.5.0b8/pybi/static/quasar.lang.zh-CN.umd.prod.js
--rw-rw-rw-   0        0        0   204438 2023-11-04 13:15:12.000000 pybi-next-0.5.0b8/pybi/static/quasar.prod.css
--rw-rw-rw-   0        0        0   511132 2023-11-04 13:15:17.000000 pybi-next-0.5.0b8/pybi/static/quasar.umd.prod.js
--rw-rw-rw-   0        0        0     4653 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/quasarCps-style.css
--rw-rw-rw-   0        0        0   233143 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/quasarCps.iife.js
--rw-rw-rw-   0        0        0     7251 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/sysApp-style.css
--rw-rw-rw-   0        0        0  1021589 2024-01-29 09:54:49.000000 pybi-next-0.5.0b8/pybi/static/sysApp.iife.js
--rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.5.0b8/pybi/static/vue.global.prod.min.js
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.219614 pybi-next-0.5.0b8/pybi/template/
--rw-rw-rw-   0        0        0     2488 2023-11-09 16:13:09.000000 pybi-next-0.5.0b8/pybi/template/index.html
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.236117 pybi-next-0.5.0b8/pybi/utils/
--rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.5.0b8/pybi/utils/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.5.0b8/pybi/utils/dataSourceUtils.py
--rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.5.0b8/pybi/utils/data_gen.py
--rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.5.0b8/pybi/utils/dictUtils.py
--rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.5.0b8/pybi/utils/echarts_opts_utils.py
--rw-rw-rw-   0        0        0     1105 2023-10-16 07:13:05.000000 pybi-next-0.5.0b8/pybi/utils/helper.py
--rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.5.0b8/pybi/utils/markdown2.py
--rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.5.0b8/pybi/utils/pyecharts_utils.py
--rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.5.0b8/pybi/utils/sql.py
-drwxrwxrwx   0        0        0        0 2024-01-29 09:57:31.252790 pybi-next-0.5.0b8/pybi_next.egg-info/
--rw-rw-rw-   0        0        0      479 2024-01-29 09:57:30.000000 pybi-next-0.5.0b8/pybi_next.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2866 2024-01-29 09:57:30.000000 pybi-next-0.5.0b8/pybi_next.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 09:57:30.000000 pybi-next-0.5.0b8/pybi_next.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.5.0b8/pybi_next.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2024-01-29 09:57:30.000000 pybi-next-0.5.0b8/pybi_next.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-01-29 09:57:30.000000 pybi-next-0.5.0b8/pybi_next.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-29 09:57:31.286628 pybi-next-0.5.0b8/setup.cfg
--rw-rw-rw-   0        0        0     1611 2023-11-09 16:13:09.000000 pybi-next-0.5.0b8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:42.025696 pybi-next-0.5.0b9/
+-rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.5.0b9/LICENSE
+-rw-rw-rw-   0        0        0      479 2024-03-17 11:04:42.023805 pybi-next-0.5.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     2400 2024-01-20 14:43:41.000000 pybi-next-0.5.0b9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.302371 pybi-next-0.5.0b9/pybi/
+-rw-rw-rw-   0        0        0     2773 2024-01-20 14:43:41.000000 pybi-next-0.5.0b9/pybi/__index.py
+-rw-rw-rw-   0        0        0       51 2024-03-17 11:04:06.000000 pybi-next-0.5.0b9/pybi/__init__.py
+-rw-rw-rw-   0        0        0    30655 2024-01-20 14:43:41.000000 pybi-next-0.5.0b9/pybi/app.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.332105 pybi-next-0.5.0b9/pybi/core/
+-rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.5.0b9/pybi/core/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-11-15 18:09:14.000000 pybi-next-0.5.0b9/pybi/core/actions.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.345071 pybi-next-0.5.0b9/pybi/core/components/
+-rw-rw-rw-   0        0        0      735 2023-11-16 05:59:00.000000 pybi-next-0.5.0b9/pybi/core/components/__init__.py
+-rw-rw-rw-   0        0        0     2699 2023-11-15 18:09:14.000000 pybi-next-0.5.0b9/pybi/core/components/component.py
+-rw-rw-rw-   0        0        0      805 2023-11-16 05:59:00.000000 pybi-next-0.5.0b9/pybi/core/components/componentTag.py
+-rw-rw-rw-   0        0        0    15329 2023-11-17 08:26:13.000000 pybi-next-0.5.0b9/pybi/core/components/containerComponent.py
+-rw-rw-rw-   0        0        0     1964 2023-07-12 09:24:47.000000 pybi-next-0.5.0b9/pybi/core/components/mermaid.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.389733 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/
+-rw-rw-rw-   0        0        0      246 2023-06-07 17:40:57.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-11-15 18:09:14.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/base.py
+-rw-rw-rw-   0        0        0     2759 2023-06-07 17:40:57.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/checkbox.py
+-rw-rw-rw-   0        0        0     5251 2023-08-26 13:10:50.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/echarts.py
+-rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/input.py
+-rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/markdown.py
+-rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/numberSlider.py
+-rw-rw-rw-   0        0        0      688 2023-11-09 16:13:09.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/qsInput.py
+-rw-rw-rw-   0        0        0     1625 2023-11-09 16:13:09.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/qsSlicer.py
+-rw-rw-rw-   0        0        0     5689 2023-11-16 06:07:36.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/qsTable.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 06:06:20.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/slicer.py
+-rw-rw-rw-   0        0        0     2889 2023-11-06 15:47:17.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/table.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 17:53:25.000000 pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/textValue.py
+-rw-rw-rw-   0        0        0     2541 2024-01-20 14:43:41.000000 pybi-next-0.5.0b9/pybi/core/components/staticComponent.py
+-rw-rw-rw-   0        0        0     6135 2023-04-21 15:56:29.000000 pybi-next-0.5.0b9/pybi/core/dataSource.py
+-rw-rw-rw-   0        0        0      863 2023-11-16 05:59:00.000000 pybi-next-0.5.0b9/pybi/core/imgManager.py
+-rw-rw-rw-   0        0        0     5155 2023-11-06 12:43:20.000000 pybi-next-0.5.0b9/pybi/core/sql.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.397712 pybi-next-0.5.0b9/pybi/core/styles/
+-rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.5.0b9/pybi/core/styles/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-04-17 04:53:14.000000 pybi-next-0.5.0b9/pybi/core/styles/styleTag.py
+-rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.5.0b9/pybi/core/styles/styles.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.423681 pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/
+-rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/boxShadow.py
+-rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/textAlign.py
+-rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/textColor.py
+-rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/textSize.py
+-rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.5.0b9/pybi/core/styles/utils.py
+-rw-rw-rw-   0        0        0     5548 2023-11-16 05:59:00.000000 pybi-next-0.5.0b9/pybi/core/uiResource.py
+-rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.5.0b9/pybi/core/webResources.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.456350 pybi-next-0.5.0b9/pybi/easyEcharts/
+-rw-rw-rw-   0        0        0     3901 2023-11-01 17:02:37.000000 pybi-next-0.5.0b9/pybi/easyEcharts/__init__.py
+-rw-rw-rw-   0        0        0     3300 2023-05-22 12:03:15.000000 pybi-next-0.5.0b9/pybi/easyEcharts/bar.py
+-rw-rw-rw-   0        0        0     4041 2023-11-01 17:02:37.000000 pybi-next-0.5.0b9/pybi/easyEcharts/base.py
+-rw-rw-rw-   0        0        0     2636 2023-05-22 12:03:15.000000 pybi-next-0.5.0b9/pybi/easyEcharts/candlestick.py
+-rw-rw-rw-   0        0        0      502 2023-11-01 17:02:37.000000 pybi-next-0.5.0b9/pybi/easyEcharts/dictChart.py
+-rw-rw-rw-   0        0        0     3415 2023-05-22 12:03:15.000000 pybi-next-0.5.0b9/pybi/easyEcharts/line.py
+-rw-rw-rw-   0        0        0     1678 2023-05-22 12:03:15.000000 pybi-next-0.5.0b9/pybi/easyEcharts/map.py
+-rw-rw-rw-   0        0        0     2423 2023-05-22 12:03:15.000000 pybi-next-0.5.0b9/pybi/easyEcharts/pie.py
+-rw-rw-rw-   0        0        0     2716 2023-05-22 12:03:15.000000 pybi-next-0.5.0b9/pybi/easyEcharts/radar.py
+-rw-rw-rw-   0        0        0     1920 2023-05-22 12:03:15.000000 pybi-next-0.5.0b9/pybi/easyEcharts/scatter.py
+-rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.5.0b9/pybi/easyEcharts/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.485752 pybi-next-0.5.0b9/pybi/icons/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.5.0b9/pybi/icons/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.5.0b9/pybi/icons/iconManager.py
+-rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.5.0b9/pybi/icons/material_icons.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.898405 pybi-next-0.5.0b9/pybi/static/
+-rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.5.0b9/pybi/static/echarts.min.js
+-rw-rw-rw-   0        0        0      597 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/echartsCps-style.css
+-rw-rw-rw-   0        0        0    35733 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/echartsCps.iife.js
+-rw-rw-rw-   0        0        0   127313 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/elementCps-style.css
+-rw-rw-rw-   0        0        0   377610 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/elementCps.iife.js
+-rw-rw-rw-   0        0        0     1672 2023-05-31 14:01:04.000000 pybi-next-0.5.0b9/pybi/static/experimentalCps-style.css
+-rw-rw-rw-   0        0        0    17540 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/experimentalCps.iife.js
+-rw-rw-rw-   0        0        0   171735 2023-11-04 15:18:39.000000 pybi-next-0.5.0b9/pybi/static/material_icons.css
+-rw-rw-rw-   0        0        0      584 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/mermaidCps-style.css
+-rw-rw-rw-   0        0        0  2889888 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/mermaidCps.iife.js
+-rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.5.0b9/pybi/static/province_map_full.json
+-rw-rw-rw-   0        0        0     2480 2023-11-04 19:17:57.000000 pybi-next-0.5.0b9/pybi/static/quasar.lang.zh-CN.umd.prod.js
+-rw-rw-rw-   0        0        0   204438 2023-11-04 13:15:12.000000 pybi-next-0.5.0b9/pybi/static/quasar.prod.css
+-rw-rw-rw-   0        0        0   511132 2023-11-04 13:15:17.000000 pybi-next-0.5.0b9/pybi/static/quasar.umd.prod.js
+-rw-rw-rw-   0        0        0     4653 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/quasarCps-style.css
+-rw-rw-rw-   0        0        0   233221 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/quasarCps.iife.js
+-rw-rw-rw-   0        0        0     7251 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/sysApp-style.css
+-rw-rw-rw-   0        0        0  1021589 2024-01-29 14:02:53.000000 pybi-next-0.5.0b9/pybi/static/sysApp.iife.js
+-rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.5.0b9/pybi/static/vue.global.prod.min.js
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.918293 pybi-next-0.5.0b9/pybi/template/
+-rw-rw-rw-   0        0        0     2488 2023-11-09 16:13:09.000000 pybi-next-0.5.0b9/pybi/template/index.html
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:41.978927 pybi-next-0.5.0b9/pybi/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.5.0b9/pybi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.5.0b9/pybi/utils/dataSourceUtils.py
+-rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.5.0b9/pybi/utils/data_gen.py
+-rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.5.0b9/pybi/utils/dictUtils.py
+-rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.5.0b9/pybi/utils/echarts_opts_utils.py
+-rw-rw-rw-   0        0        0     1105 2023-10-16 07:13:05.000000 pybi-next-0.5.0b9/pybi/utils/helper.py
+-rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.5.0b9/pybi/utils/markdown2.py
+-rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.5.0b9/pybi/utils/pyecharts_utils.py
+-rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.5.0b9/pybi/utils/sql.py
+drwxrwxrwx   0        0        0        0 2024-03-17 11:04:42.019815 pybi-next-0.5.0b9/pybi_next.egg-info/
+-rw-rw-rw-   0        0        0      479 2024-03-17 11:04:40.000000 pybi-next-0.5.0b9/pybi_next.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2866 2024-03-17 11:04:40.000000 pybi-next-0.5.0b9/pybi_next.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-17 11:04:40.000000 pybi-next-0.5.0b9/pybi_next.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.5.0b9/pybi_next.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2024-03-17 11:04:40.000000 pybi-next-0.5.0b9/pybi_next.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-03-17 11:04:40.000000 pybi-next-0.5.0b9/pybi_next.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-17 11:04:42.025696 pybi-next-0.5.0b9/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2023-11-09 16:13:09.000000 pybi-next-0.5.0b9/setup.py
```

### Comparing `pybi-next-0.5.0b8/LICENSE` & `pybi-next-0.5.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/README.md` & `pybi-next-0.5.0b9/README.md`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/__index.py` & `pybi-next-0.5.0b9/pybi/__index.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/app.py` & `pybi-next-0.5.0b9/pybi/app.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/__init__.py` & `pybi-next-0.5.0b9/pybi/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/component.py` & `pybi-next-0.5.0b9/pybi/core/components/component.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/componentTag.py` & `pybi-next-0.5.0b9/pybi/core/components/componentTag.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/containerComponent.py` & `pybi-next-0.5.0b9/pybi/core/components/containerComponent.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/mermaid.py` & `pybi-next-0.5.0b9/pybi/core/components/mermaid.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/base.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/base.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/checkbox.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/checkbox.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/echarts.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/echarts.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/input.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/input.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/markdown.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/markdown.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/numberSlider.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/numberSlider.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/qsInput.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/qsInput.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/qsSlicer.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/qsSlicer.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/qsTable.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/qsTable.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/slicer.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/slicer.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/reactiveComponent/table.py` & `pybi-next-0.5.0b9/pybi/core/components/reactiveComponent/table.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/components/staticComponent.py` & `pybi-next-0.5.0b9/pybi/core/components/staticComponent.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/dataSource.py` & `pybi-next-0.5.0b9/pybi/core/dataSource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/imgManager.py` & `pybi-next-0.5.0b9/pybi/core/imgManager.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/sql.py` & `pybi-next-0.5.0b9/pybi/core/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/styles/__init__.py` & `pybi-next-0.5.0b9/pybi/core/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/styles/styleTag.py` & `pybi-next-0.5.0b9/pybi/core/styles/styleTag.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/styles/styles.py` & `pybi-next-0.5.0b9/pybi/core/styles/styles.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/boxShadow.py` & `pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/boxShadow.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/textAlign.py` & `pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/textAlign.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/textColor.py` & `pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/textColor.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/styles/tailwindStyles/textSize.py` & `pybi-next-0.5.0b9/pybi/core/styles/tailwindStyles/textSize.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/uiResource.py` & `pybi-next-0.5.0b9/pybi/core/uiResource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/core/webResources.py` & `pybi-next-0.5.0b9/pybi/core/webResources.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/__init__.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/bar.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/bar.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/base.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/base.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/candlestick.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/candlestick.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/line.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/line.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/map.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/map.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/pie.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/pie.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/radar.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/radar.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/scatter.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/scatter.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/easyEcharts/utils.py` & `pybi-next-0.5.0b9/pybi/easyEcharts/utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/icons/iconManager.py` & `pybi-next-0.5.0b9/pybi/icons/iconManager.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/icons/material_icons.py` & `pybi-next-0.5.0b9/pybi/icons/material_icons.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/echarts.min.js` & `pybi-next-0.5.0b9/pybi/static/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/echartsCps-style.css` & `pybi-next-0.5.0b9/pybi/static/echartsCps-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/echartsCps.iife.js` & `pybi-next-0.5.0b9/pybi/static/echartsCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/elementCps-style.css` & `pybi-next-0.5.0b9/pybi/static/elementCps-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/elementCps.iife.js` & `pybi-next-0.5.0b9/pybi/static/elementCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/experimentalCps-style.css` & `pybi-next-0.5.0b9/pybi/static/experimentalCps-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/experimentalCps.iife.js` & `pybi-next-0.5.0b9/pybi/static/experimentalCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/material_icons.css` & `pybi-next-0.5.0b9/pybi/static/material_icons.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/mermaidCps-style.css` & `pybi-next-0.5.0b9/pybi/static/mermaidCps-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/mermaidCps.iife.js` & `pybi-next-0.5.0b9/pybi/static/mermaidCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/province_map_full.json` & `pybi-next-0.5.0b9/pybi/static/province_map_full.json`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/quasar.lang.zh-CN.umd.prod.js` & `pybi-next-0.5.0b9/pybi/static/quasar.lang.zh-CN.umd.prod.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/quasar.prod.css` & `pybi-next-0.5.0b9/pybi/static/quasar.prod.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/quasar.umd.prod.js` & `pybi-next-0.5.0b9/pybi/static/quasar.umd.prod.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/quasarCps-style.css` & `pybi-next-0.5.0b9/pybi/static/quasarCps-style.css`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-.slicer-box[data-v-3bcb5e70]{margin-right:.8rem;min-width:10rem;max-width:20rem}.slicer-box .cp-select[data-v-3bcb5e70]{width:100%}.pybi-box[data-v-a6587c10]{position:relative;width:100%;display:flex;flex-direction:column;align-items:var(--75d7665f);justify-content:var(--17c2b856);overflow:auto;gap:.8em}.pybi-box .item-box[data-v-a6587c10]{width:100%;overflow:visible;display:flex}.pybi-flow-box[data-v-de89203e]{display:flex;flex-direction:row;flex-wrap:wrap;align-items:center;justify-content:var(--57ed0846);width:100%}.pybi-flow-box[data-v-de89203e]>.pybi-space[data-auto-grow]{flex-grow:9999}.pybi-flow-box[data-v-de89203e]>*[data-pybi-auto-width]{width:unset}.grid-box[data-v-c795c342]{display:grid;grid-template-areas:var(--5f386d28);grid-template-columns:var(--9f82b32e);grid-template-rows:var(--7e13decd);gap:.8rem;justify-items:var(--21ef3978);align-items:var(--64b0babb);width:100%}.grid-box>.item[data-v-c795c342]{display:flex}.grid-box>.item[data-v-c795c342]>p{overflow:hidden;overflow-wrap:break-word}.grid-box[data-v-c795c342]>*{overflow-x:auto;width:100%}.textValue-box[data-v-63313f93]{display:inline-block;white-space:pre-wrap;margin:0;box-sizing:initial}.md-box[data-v-1bf08f37]{width:100%;height:var(--4fd07687)}.md-box[data-v-1bf08f37][data-v-1bf08f37] h1{display:block;font-size:2em;margin-block-start:.67em;margin-block-end:.67em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h2{display:block;font-size:1.5em;margin-block-start:.83em;margin-block-end:.83em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h3{display:block;font-size:1.17em;margin-block-start:1em;margin-block-end:1em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h4{display:block;margin-block-start:1.33em;margin-block-end:1.33em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h5{display:block;font-size:.83em;margin-block-start:1.67em;margin-block-end:1.67em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.pybi-foreach[data-v-d293d89e]{position:relative}.pybi-checkbox[data-v-2f3725fd]{display:flex;flex-direction:column;flex-wrap:nowrap;width:100%;position:relative}.pybi-checkbox svg[data-v-2f3725fd]{width:1em;height:1em}.pybi-checkbox>header[data-v-2f3725fd]{background-color:#adcff3;border-radius:5px;height:25px;width:100%;flex-shrink:0;display:flex;justify-content:space-between;align-items:center}.pybi-checkbox>header .title[data-v-2f3725fd]{font-size:1.1em;padding:.1em .3em}.pybi-checkbox>header .funs-buttons[data-v-2f3725fd]{display:flex;flex-direction:row}.pybi-checkbox>header .funs-buttons .funs-icon[data-v-2f3725fd]{border-radius:50%;display:flex;justify-content:center;align-items:center;padding:.3em;-webkit-user-select:none;user-select:none;transition:.3s;cursor:pointer}.pybi-checkbox>header .funs-buttons .funs-icon[data-v-2f3725fd]:hover{box-shadow:0 4px 6px #0000001a}.pybi-checkbox .list-mode[data-v-2f3725fd]{overflow:auto}.pybi-checkbox .list-mode .labels-box[data-v-2f3725fd]{display:flex;flex-wrap:nowrap;flex-direction:column;gap:.5em}.pybi-checkbox .list-mode .labels-box .pybi-checkbox_content[data-v-2f3725fd]{display:flex;gap:.3em;justify-content:flex-start;align-items:center;-webkit-user-select:none;user-select:none;height:1.5em}.pybi-checkbox .tile-mode[data-v-2f3725fd]{--label-main-color: rgba(203, 222, 242, .9);overflow:auto}.pybi-checkbox .tile-mode .labels-box[data-v-2f3725fd]{display:flex;flex-wrap:wrap;flex-direction:var(--6c5c2c06);gap:.2em;padding:.3em .1em .3em 0}.pybi-checkbox .tile-mode .labels-box .pybi-checkbox_content[data-v-2f3725fd]{border:1px solid var(--label-main-color);border-radius:15px;height:3em;padding:1em;display:flex;gap:.3em;justify-content:center;align-items:center;-webkit-user-select:none;user-select:none;cursor:pointer;height:1.5em;transition:.3s}.pybi-checkbox .tile-mode .labels-box .pybi-checkbox_content[data-v-2f3725fd]:hover{text-decoration:underline}.pybi-checkbox .tile-mode .labels-box .pybi-checkbox_content-checked[data-v-2f3725fd]{background-color:var(--label-main-color)}.err[data-v-938c3bc4]{width:100%;color:red;border:2px dashed #ba4949;padding:.8rem}.err>p[data-v-938c3bc4]:first-child{font-size:1.2rem;margin:.2rem 0}.pybi-tabs[data-v-f31e0371]{width:100%;display:flex}.pybi-input[data-v-56484143]{min-width:18em}
+.slicer-box[data-v-3bcb5e70]{margin-right:.8rem;min-width:10rem;max-width:20rem}.slicer-box .cp-select[data-v-3bcb5e70]{width:100%}.pybi-box[data-v-a6587c10]{position:relative;width:100%;display:flex;flex-direction:column;align-items:var(--75d7665f);justify-content:var(--17c2b856);overflow:auto;gap:.8em}.pybi-box .item-box[data-v-a6587c10]{width:100%;overflow:visible;display:flex}.pybi-flow-box[data-v-de89203e]{display:flex;flex-direction:row;flex-wrap:wrap;align-items:center;justify-content:var(--57ed0846);width:100%}.pybi-flow-box[data-v-de89203e]>.pybi-space[data-auto-grow]{flex-grow:9999}.pybi-flow-box[data-v-de89203e]>*[data-pybi-auto-width]{width:unset}.grid-box[data-v-c795c342]{display:grid;grid-template-areas:var(--5f386d28);grid-template-columns:var(--9f82b32e);grid-template-rows:var(--7e13decd);gap:.8rem;justify-items:var(--21ef3978);align-items:var(--64b0babb);width:100%}.grid-box>.item[data-v-c795c342]{display:flex}.grid-box>.item[data-v-c795c342]>p{overflow:hidden;overflow-wrap:break-word}.grid-box[data-v-c795c342]>*{overflow-x:auto;width:100%}.textValue-box[data-v-63313f93]{display:inline-block;white-space:pre-wrap;margin:0;box-sizing:initial}.md-box[data-v-1bf08f37]{width:100%;height:var(--4fd07687)}.md-box[data-v-1bf08f37][data-v-1bf08f37] h1{display:block;font-size:2em;margin-block-start:.67em;margin-block-end:.67em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h2{display:block;font-size:1.5em;margin-block-start:.83em;margin-block-end:.83em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h3{display:block;font-size:1.17em;margin-block-start:1em;margin-block-end:1em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h4{display:block;margin-block-start:1.33em;margin-block-end:1.33em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.md-box[data-v-1bf08f37][data-v-1bf08f37] h5{display:block;font-size:.83em;margin-block-start:1.67em;margin-block-end:1.67em;margin-inline-start:0px;margin-inline-end:0px;font-weight:700;line-height:normal;letter-spacing:normal}.pybi-foreach[data-v-d293d89e]{position:relative}.pybi-checkbox[data-v-68848832]{display:flex;flex-direction:column;flex-wrap:nowrap;width:100%;position:relative}.pybi-checkbox svg[data-v-68848832]{width:1em;height:1em}.pybi-checkbox>header[data-v-68848832]{background-color:#adcff3;border-radius:5px;height:25px;width:100%;flex-shrink:0;display:flex;justify-content:space-between;align-items:center}.pybi-checkbox>header .title[data-v-68848832]{font-size:1.1em;padding:.1em .3em}.pybi-checkbox>header .funs-buttons[data-v-68848832]{display:flex;flex-direction:row}.pybi-checkbox>header .funs-buttons .funs-icon[data-v-68848832]{border-radius:50%;display:flex;justify-content:center;align-items:center;padding:.3em;-webkit-user-select:none;user-select:none;transition:.3s;cursor:pointer}.pybi-checkbox>header .funs-buttons .funs-icon[data-v-68848832]:hover{box-shadow:0 4px 6px #0000001a}.pybi-checkbox .list-mode[data-v-68848832]{overflow:auto}.pybi-checkbox .list-mode .labels-box[data-v-68848832]{display:flex;flex-wrap:nowrap;flex-direction:column;gap:.5em}.pybi-checkbox .list-mode .labels-box .pybi-checkbox_content[data-v-68848832]{display:flex;gap:.3em;justify-content:flex-start;align-items:center;-webkit-user-select:none;user-select:none;height:1.5em}.pybi-checkbox .tile-mode[data-v-68848832]{--label-main-color: rgba(203, 222, 242, .9);overflow:auto}.pybi-checkbox .tile-mode .labels-box[data-v-68848832]{display:flex;flex-wrap:wrap;flex-direction:var(--cf2e820e);gap:.2em;padding:.3em .1em .3em 0}.pybi-checkbox .tile-mode .labels-box .pybi-checkbox_content[data-v-68848832]{border:1px solid var(--label-main-color);border-radius:15px;height:3em;padding:1em;display:flex;gap:.3em;justify-content:center;align-items:center;-webkit-user-select:none;user-select:none;cursor:pointer;height:1.5em;transition:.3s}.pybi-checkbox .tile-mode .labels-box .pybi-checkbox_content[data-v-68848832]:hover{text-decoration:underline}.pybi-checkbox .tile-mode .labels-box .pybi-checkbox_content-checked[data-v-68848832]{background-color:var(--label-main-color)}.err[data-v-938c3bc4]{width:100%;color:red;border:2px dashed #ba4949;padding:.8rem}.err>p[data-v-938c3bc4]:first-child{font-size:1.2rem;margin:.2rem 0}.pybi-tabs[data-v-f31e0371]{width:100%;display:flex}.pybi-input[data-v-0964b155]{min-width:18em}
```

### Comparing `pybi-next-0.5.0b8/pybi/static/quasarCps.iife.js` & `pybi-next-0.5.0b9/pybi/static/quasarCps.iife.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
             platform: n[0] || ""
         }
     }
 
     function Qa(e) {
         return /(ipad)/.exec(e) || /(ipod)/.exec(e) || /(windows phone)/.exec(e) || /(iphone)/.exec(e) || /(kindle)/.exec(e) || /(silk)/.exec(e) || /(android)/.exec(e) || /(win)/.exec(e) || /(mac)/.exec(e) || /(linux)/.exec(e) || /(cros)/.exec(e) || /(playbook)/.exec(e) || /(bb)/.exec(e) || /(blackberry)/.exec(e) || []
     }
-    const el = "ontouchstart" in window || window.navigator.maxTouchPoints > 0;
+    const tl = "ontouchstart" in window || window.navigator.maxTouchPoints > 0;
 
     function Ga(e) {
         zn = {
             is: {
                 ...e
             }
         }, delete e.mac, delete e.desktop;
@@ -49,31 +49,31 @@
     function Xa(e) {
         const n = e.toLowerCase(),
             o = Qa(n),
             l = Ka(n, o),
             r = {};
         l.browser && (r[l.browser] = !0, r.version = l.version, r.versionNumber = parseInt(l.versionNumber, 10)), l.platform && (r[l.platform] = !0);
         const a = r.android || r.ios || r.bb || r.blackberry || r.ipad || r.iphone || r.ipod || r.kindle || r.playbook || r.silk || r["windows phone"];
-        return a === !0 || n.indexOf("mobile") > -1 ? (r.mobile = !0, r.edga || r.edgios ? (r.edge = !0, l.browser = "edge") : r.crios ? (r.chrome = !0, l.browser = "chrome") : r.fxios && (r.firefox = !0, l.browser = "firefox")) : r.desktop = !0, (r.ipod || r.ipad || r.iphone) && (r.ios = !0), r["windows phone"] && (r.winphone = !0, delete r["windows phone"]), (r.chrome || r.opr || r.safari || r.vivaldi || r.mobile === !0 && r.ios !== !0 && a !== !0) && (r.webkit = !0), r.edg && (l.browser = "edgechromium", r.edgeChromium = !0), (r.safari && r.blackberry || r.bb) && (l.browser = "blackberry", r.blackberry = !0), r.safari && r.playbook && (l.browser = "playbook", r.playbook = !0), r.opr && (l.browser = "opera", r.opera = !0), r.safari && r.android && (l.browser = "android", r.android = !0), r.safari && r.kindle && (l.browser = "kindle", r.kindle = !0), r.safari && r.silk && (l.browser = "silk", r.silk = !0), r.vivaldi && (l.browser = "vivaldi", r.vivaldi = !0), r.name = l.browser, r.platform = l.platform, n.indexOf("electron") > -1 ? r.electron = !0 : document.location.href.indexOf("-extension://") > -1 ? r.bex = !0 : (window.Capacitor !== void 0 ? (r.capacitor = !0, r.nativeMobile = !0, r.nativeMobileWrapper = "capacitor") : (window._cordovaNative !== void 0 || window.cordova !== void 0) && (r.cordova = !0, r.nativeMobile = !0, r.nativeMobileWrapper = "cordova"), el === !0 && r.mac === !0 && (r.desktop === !0 && r.safari === !0 || r.nativeMobile === !0 && r.android !== !0 && r.ios !== !0 && r.ipad !== !0) && Ga(r)), r
+        return a === !0 || n.indexOf("mobile") > -1 ? (r.mobile = !0, r.edga || r.edgios ? (r.edge = !0, l.browser = "edge") : r.crios ? (r.chrome = !0, l.browser = "chrome") : r.fxios && (r.firefox = !0, l.browser = "firefox")) : r.desktop = !0, (r.ipod || r.ipad || r.iphone) && (r.ios = !0), r["windows phone"] && (r.winphone = !0, delete r["windows phone"]), (r.chrome || r.opr || r.safari || r.vivaldi || r.mobile === !0 && r.ios !== !0 && a !== !0) && (r.webkit = !0), r.edg && (l.browser = "edgechromium", r.edgeChromium = !0), (r.safari && r.blackberry || r.bb) && (l.browser = "blackberry", r.blackberry = !0), r.safari && r.playbook && (l.browser = "playbook", r.playbook = !0), r.opr && (l.browser = "opera", r.opera = !0), r.safari && r.android && (l.browser = "android", r.android = !0), r.safari && r.kindle && (l.browser = "kindle", r.kindle = !0), r.safari && r.silk && (l.browser = "silk", r.silk = !0), r.vivaldi && (l.browser = "vivaldi", r.vivaldi = !0), r.name = l.browser, r.platform = l.platform, n.indexOf("electron") > -1 ? r.electron = !0 : document.location.href.indexOf("-extension://") > -1 ? r.bex = !0 : (window.Capacitor !== void 0 ? (r.capacitor = !0, r.nativeMobile = !0, r.nativeMobileWrapper = "capacitor") : (window._cordovaNative !== void 0 || window.cordova !== void 0) && (r.cordova = !0, r.nativeMobile = !0, r.nativeMobileWrapper = "cordova"), tl === !0 && r.mac === !0 && (r.desktop === !0 && r.safari === !0 || r.nativeMobile === !0 && r.android !== !0 && r.ios !== !0 && r.ipad !== !0) && Ga(r)), r
     }
-    const tl = navigator.userAgent || navigator.vendor || window.opera,
+    const nl = navigator.userAgent || navigator.vendor || window.opera,
         Ya = {
             has: {
                 touch: !1,
                 webStorage: !1
             },
             within: {
                 iframe: !1
             }
         },
         he = {
-            userAgent: tl,
-            is: Xa(tl),
+            userAgent: nl,
+            is: Xa(nl),
             has: {
-                touch: el
+                touch: tl
             },
             within: {
                 iframe: window.self !== window.top
             }
         },
         Ln = {
             install(e) {
@@ -114,15 +114,15 @@
     const se = e => t.markRaw(t.defineComponent(e)),
         Dn = e => t.markRaw(e);
 
     function we(e, n) {
         return e !== void 0 && e() || n
     }
 
-    function nl(e, n) {
+    function ol(e, n) {
         if (e !== void 0) {
             const o = e();
             if (o != null) return o.slice()
         }
         return n
     }
 
@@ -135,42 +135,42 @@
     }
 
     function cn(e, n, o, l, r, a) {
         n.key = l + r;
         const i = t.h(e, n, o);
         return r === !0 ? t.withDirectives(i, a()) : i
     }
-    const ol = "0 0 24 24",
-        ll = e => e,
+    const ll = "0 0 24 24",
+        rl = e => e,
         jn = e => `ionicons ${e}`,
-        rl = {
+        al = {
             "mdi-": e => `mdi ${e}`,
-            "icon-": ll,
+            "icon-": rl,
             "bt-": e => `bt ${e}`,
             "eva-": e => `eva ${e}`,
             "ion-md": jn,
             "ion-ios": jn,
             "ion-logo": jn,
-            "iconfont ": ll,
+            "iconfont ": rl,
             "ti-": e => `themify-icon ${e}`,
             "bi-": e => `bootstrap-icons ${e}`
         },
-        al = {
+        il = {
             o_: "-outlined",
             r_: "-round",
             s_: "-sharp"
         },
-        il = {
+        ul = {
             sym_o_: "-outlined",
             sym_r_: "-rounded",
             sym_s_: "-sharp"
         },
-        Ja = new RegExp("^(" + Object.keys(rl).join("|") + ")"),
-        ei = new RegExp("^(" + Object.keys(al).join("|") + ")"),
-        ul = new RegExp("^(" + Object.keys(il).join("|") + ")"),
+        Ja = new RegExp("^(" + Object.keys(al).join("|") + ")"),
+        ei = new RegExp("^(" + Object.keys(il).join("|") + ")"),
+        sl = new RegExp("^(" + Object.keys(ul).join("|") + ")"),
         ti = /^[Mm]\s?[-+]?\.?\d/,
         ni = /^img:/,
         oi = /^svguse:/,
         li = /^ion-/,
         ri = /^(fa-(sharp|solid|regular|light|brands|duotone|thin)|[lf]a[srlbdk]?) /,
         Be = se({
             name: "QIcon",
@@ -206,53 +206,53 @@
                                 }
                             } else return {
                                 cls: s.cls,
                                 content: s.content !== void 0 ? s.content : " "
                             }
                     }
                     if (ti.test(u) === !0) {
-                        const [s, h = ol] = u.split("|");
+                        const [s, m = ll] = u.split("|");
                         return {
                             svg: !0,
-                            viewBox: h,
+                            viewBox: m,
                             nodes: s.split("&&").map(f => {
-                                const [m, v, x] = f.split("@@");
+                                const [h, v, _] = f.split("@@");
                                 return t.h("path", {
                                     style: v,
-                                    d: m,
-                                    transform: x
+                                    d: h,
+                                    transform: _
                                 })
                             })
                         }
                     }
                     if (ni.test(u) === !0) return {
                         img: !0,
                         src: u.substring(4)
                     };
                     if (oi.test(u) === !0) {
-                        const [s, h = ol] = u.split("|");
+                        const [s, m = ll] = u.split("|");
                         return {
                             svguse: !0,
                             src: s.substring(7),
-                            viewBox: h
+                            viewBox: m
                         }
                     }
                     let c = " ";
                     const d = u.match(Ja);
-                    if (d !== null) i = rl[d[1]](u);
+                    if (d !== null) i = al[d[1]](u);
                     else if (ri.test(u) === !0) i = u;
                     else if (li.test(u) === !0) i = `ionicons ion-${o.platform.is.ios===!0?"ios":"md"}${u.substring(3)}`;
-                    else if (ul.test(u) === !0) {
+                    else if (sl.test(u) === !0) {
                         i = "notranslate material-symbols";
-                        const s = u.match(ul);
-                        s !== null && (u = u.substring(6), i += il[s[1]]), c = u
+                        const s = u.match(sl);
+                        s !== null && (u = u.substring(6), i += ul[s[1]]), c = u
                     } else {
                         i = "notranslate material-icons";
                         const s = u.match(ei);
-                        s !== null && (u = u.substring(2), i += al[s[1]]), c = u
+                        s !== null && (u = u.substring(2), i += il[s[1]]), c = u
                     }
                     return {
                         cls: i,
                         content: c
                     }
                 });
                 return () => {
@@ -325,17 +325,17 @@
                 default: null
             }
         };
 
     function Fe(e, n) {
         return t.computed(() => e.dark === null ? n.dark.isActive : e.dark)
     }
-    const sl = "_q_l_",
+    const cl = "_q_l_",
         ui = "_q_fo_",
-        cl = "_q_tabs_",
+        dl = "_q_tabs_",
         et = () => {};
 
     function si({
         validate: e,
         resetValidation: n,
         requiresQForm: o
     }) {
@@ -353,34 +353,34 @@
             }), t.onMounted(() => {
                 r.disable !== !0 && l.bindComponent(a)
             }), t.onBeforeUnmount(() => {
                 r.disable !== !0 && l.unbindComponent(a)
             })
         } else o === !0 && console.error("Parent QForm not found on useFormChild()!")
     }
-    const dl = /^#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?$/,
-        fl = /^#[0-9a-fA-F]{4}([0-9a-fA-F]{4})?$/,
-        ml = /^#([0-9a-fA-F]{3}|[0-9a-fA-F]{4}|[0-9a-fA-F]{6}|[0-9a-fA-F]{8})$/,
+    const fl = /^#[0-9a-fA-F]{3}([0-9a-fA-F]{3})?$/,
+        ml = /^#[0-9a-fA-F]{4}([0-9a-fA-F]{4})?$/,
+        hl = /^#([0-9a-fA-F]{3}|[0-9a-fA-F]{4}|[0-9a-fA-F]{6}|[0-9a-fA-F]{8})$/,
         dn = /^rgb\(((0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5]),){2}(0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5])\)$/,
         fn = /^rgba\(((0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5]),){2}(0|[1-9][\d]?|1[\d]{0,2}|2[\d]?|2[0-4][\d]|25[0-5]),(0|0\.[0-9]+[1-9]|0\.[1-9]+|1)\)$/,
         Hn = {
             date: e => /^-?[\d]+\/[0-1]\d\/[0-3]\d$/.test(e),
             time: e => /^([0-1]?\d|2[0-3]):[0-5]\d$/.test(e),
             fulltime: e => /^([0-1]?\d|2[0-3]):[0-5]\d:[0-5]\d$/.test(e),
             timeOrFulltime: e => /^([0-1]?\d|2[0-3]):[0-5]\d(:[0-5]\d)?$/.test(e),
             email: e => /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/.test(e),
-            hexColor: e => dl.test(e),
-            hexaColor: e => fl.test(e),
-            hexOrHexaColor: e => ml.test(e),
+            hexColor: e => fl.test(e),
+            hexaColor: e => ml.test(e),
+            hexOrHexaColor: e => hl.test(e),
             rgbColor: e => dn.test(e),
             rgbaColor: e => fn.test(e),
             rgbOrRgbaColor: e => dn.test(e) || fn.test(e),
-            hexOrRgbColor: e => dl.test(e) || dn.test(e),
-            hexaOrRgbaColor: e => fl.test(e) || fn.test(e),
-            anyColor: e => ml.test(e) || dn.test(e) || fn.test(e)
+            hexOrRgbColor: e => fl.test(e) || dn.test(e),
+            hexaOrRgbaColor: e => ml.test(e) || fn.test(e),
+            anyColor: e => hl.test(e) || dn.test(e) || fn.test(e)
         };
 
     function Un(e, n = 250, o) {
         let l = null;
 
         function r() {
             const a = arguments,
@@ -413,92 +413,92 @@
     function fi(e, n) {
         const {
             props: o,
             proxy: l
         } = t.getCurrentInstance(), r = t.ref(!1), a = t.ref(null), i = t.ref(null);
         si({
             validate: v,
-            resetValidation: m
+            resetValidation: h
         });
         let u = 0,
             c;
         const d = t.computed(() => o.rules !== void 0 && o.rules !== null && o.rules.length !== 0),
             s = t.computed(() => o.disable !== !0 && d.value === !0),
-            h = t.computed(() => o.error === !0 || r.value === !0),
+            m = t.computed(() => o.error === !0 || r.value === !0),
             f = t.computed(() => typeof o.errorMessage == "string" && o.errorMessage.length !== 0 ? o.errorMessage : a.value);
         t.watch(() => o.modelValue, () => {
-            x()
-        }), t.watch(() => o.reactiveRules, S => {
-            S === !0 ? c === void 0 && (c = t.watch(() => o.rules, () => {
-                x(!0)
+            _()
+        }), t.watch(() => o.reactiveRules, k => {
+            k === !0 ? c === void 0 && (c = t.watch(() => o.rules, () => {
+                _(!0)
             })) : c !== void 0 && (c(), c = void 0)
         }, {
             immediate: !0
-        }), t.watch(e, S => {
-            S === !0 ? i.value === null && (i.value = !1) : i.value === !1 && (i.value = !0, s.value === !0 && o.lazyRules !== "ondemand" && n.value === !1 && p())
+        }), t.watch(e, k => {
+            k === !0 ? i.value === null && (i.value = !1) : i.value === !1 && (i.value = !0, s.value === !0 && o.lazyRules !== "ondemand" && n.value === !1 && p())
         });
 
-        function m() {
+        function h() {
             u++, n.value = !1, i.value = null, r.value = !1, a.value = null, p.cancel()
         }
 
-        function v(S = o.modelValue) {
+        function v(k = o.modelValue) {
             if (s.value !== !0) return !0;
-            const C = ++u,
-                y = n.value !== !0 ? () => {
+            const q = ++u,
+                w = n.value !== !0 ? () => {
                     i.value = !0
                 } : () => {},
-                P = (M, V) => {
-                    M === !0 && y(), r.value = M, a.value = V || null, n.value = !1
+                C = (M, V) => {
+                    M === !0 && w(), r.value = M, a.value = V || null, n.value = !1
                 },
                 A = [];
             for (let M = 0; M < o.rules.length; M++) {
                 const V = o.rules[M];
                 let R;
-                if (typeof V == "function" ? R = V(S, Hn) : typeof V == "string" && Hn[V] !== void 0 && (R = Hn[V](S)), R === !1 || typeof R == "string") return P(!0, R), !1;
+                if (typeof V == "function" ? R = V(k, Hn) : typeof V == "string" && Hn[V] !== void 0 && (R = Hn[V](k)), R === !1 || typeof R == "string") return C(!0, R), !1;
                 R !== !0 && R !== void 0 && A.push(R)
             }
-            return A.length === 0 ? (P(!1), !0) : (n.value = !0, Promise.all(A).then(M => {
-                if (M === void 0 || Array.isArray(M) === !1 || M.length === 0) return C === u && P(!1), !0;
+            return A.length === 0 ? (C(!1), !0) : (n.value = !0, Promise.all(A).then(M => {
+                if (M === void 0 || Array.isArray(M) === !1 || M.length === 0) return q === u && C(!1), !0;
                 const V = M.find(R => R === !1 || typeof R == "string");
-                return C === u && P(V !== void 0, V), V === void 0
-            }, M => (C === u && (console.error(M), P(!0)), !1)))
+                return q === u && C(V !== void 0, V), V === void 0
+            }, M => (q === u && (console.error(M), C(!0)), !1)))
         }
 
-        function x(S) {
-            s.value === !0 && o.lazyRules !== "ondemand" && (i.value === !0 || o.lazyRules !== !0 && S !== !0) && p()
+        function _(k) {
+            s.value === !0 && o.lazyRules !== "ondemand" && (i.value === !0 || o.lazyRules !== !0 && k !== !0) && p()
         }
         const p = Un(v, 0);
         return t.onBeforeUnmount(() => {
             c !== void 0 && c(), p.cancel()
         }), Object.assign(l, {
-            resetValidation: m,
+            resetValidation: h,
             validate: v
-        }), Ze(l, "hasError", () => h.value), {
+        }), Ze(l, "hasError", () => m.value), {
             isDirtyModel: i,
             hasRules: d,
-            hasError: h,
+            hasError: m,
             errorMessage: f,
             validate: v,
-            resetValidation: m
+            resetValidation: h
         }
     }
-    const hl = /^on[A-Z]/;
+    const vl = /^on[A-Z]/;
 
     function mi(e, n) {
         const o = {
             listeners: t.ref({}),
             attributes: t.ref({})
         };
 
         function l() {
             const r = {},
                 a = {};
-            for (const i in e) i !== "class" && i !== "style" && hl.test(i) === !1 && (r[i] = e[i]);
-            for (const i in n.props) hl.test(i) === !0 && (a[i] = n.props[i]);
+            for (const i in e) i !== "class" && i !== "style" && vl.test(i) === !1 && (r[i] = e[i]);
+            for (const i in n.props) vl.test(i) === !0 && (a[i] = n.props[i]);
             o.attributes.value = r, o.listeners.value = a
         }
         return t.onBeforeUpdate(l), l(), o
     }
     let Wn, mn = 0;
     const Pe = new Array(256);
     for (let e = 0; e < 256; e++) Pe[e] = (e + 256).toString(16).substring(1);
@@ -513,18 +513,18 @@
             }
             return n => {
                 const o = [];
                 for (let l = n; l > 0; l--) o.push(Math.floor(Math.random() * 256));
                 return o
             }
         })(),
-        vl = 4096;
+        gl = 4096;
 
-    function gl() {
-        (Wn === void 0 || mn + 16 > vl) && (mn = 0, Wn = hi(vl));
+    function pl() {
+        (Wn === void 0 || mn + 16 > gl) && (mn = 0, Wn = hi(gl));
         const e = Array.prototype.slice.call(Wn, mn, mn += 16);
         return e[6] = e[6] & 15 | 64, e[8] = e[8] & 63 | 128, Pe[e[0]] + Pe[e[1]] + Pe[e[2]] + Pe[e[3]] + "-" + Pe[e[4]] + Pe[e[5]] + "-" + Pe[e[6]] + Pe[e[7]] + "-" + Pe[e[8]] + Pe[e[9]] + "-" + Pe[e[10]] + Pe[e[11]] + Pe[e[12]] + Pe[e[13]] + Pe[e[14]] + Pe[e[15]]
     }
     const Se = {
         hasPassive: !1,
         passiveCapture: !0,
         notPassiveCapture: !0
@@ -552,15 +552,15 @@
             }
         });
         window.addEventListener("qtest", null, e), window.removeEventListener("qtest", null, e)
     } catch {}
 
     function Ut() {}
 
-    function pl(e) {
+    function bl(e) {
         return e.button === 0
     }
 
     function dt(e) {
         return e.touches && e.touches[0] ? e = e.touches[0] : e.changedTouches && e.changedTouches[0] ? e = e.changedTouches[0] : e.targetTouches && e.targetTouches[0] && (e = e.targetTouches[0]), {
             top: e.clientY,
             left: e.clientX
@@ -612,36 +612,36 @@
         e[o] !== void 0 && (e[o].forEach(l => {
             l[0].removeEventListener(l[1], e[l[2]], Se[l[3]])
         }), e[o] = void 0)
     }
     let ft = [],
         Wt = [];
 
-    function bl(e) {
+    function yl(e) {
         Wt = Wt.filter(n => n !== e)
     }
 
     function gi(e) {
-        bl(e), Wt.push(e)
+        yl(e), Wt.push(e)
     }
 
-    function yl(e) {
-        bl(e), Wt.length === 0 && ft.length !== 0 && (ft[ft.length - 1](), ft = [])
+    function wl(e) {
+        yl(e), Wt.length === 0 && ft.length !== 0 && (ft[ft.length - 1](), ft = [])
     }
 
     function hn(e) {
         Wt.length === 0 ? e() : ft.push(e)
     }
 
     function pi(e) {
         ft = ft.filter(n => n !== e)
     }
 
     function Kn(e) {
-        return e === void 0 ? `f_${gl()}` : e
+        return e === void 0 ? `f_${pl()}` : e
     }
 
     function Kt(e) {
         return e != null && ("" + e).length !== 0
     }
     const vn = {
             ...Le,
@@ -706,158 +706,158 @@
             slots: l,
             attrs: r,
             proxy: a
         } = t.getCurrentInstance(), {
             $q: i
         } = a;
         let u = null;
-        e.hasValue === void 0 && (e.hasValue = t.computed(() => Kt(n.modelValue))), e.emitValue === void 0 && (e.emitValue = w => {
-            o("update:modelValue", w)
+        e.hasValue === void 0 && (e.hasValue = t.computed(() => Kt(n.modelValue))), e.emitValue === void 0 && (e.emitValue = y => {
+            o("update:modelValue", y)
         }), e.controlEvents === void 0 && (e.controlEvents = {
-            onFocusin: T,
-            onFocusout: B
+            onFocusin: B,
+            onFocusout: P
         }), Object.assign(e, {
             clearValue: I,
-            onControlFocusin: T,
-            onControlFocusout: B,
+            onControlFocusin: B,
+            onControlFocusout: P,
             focus: V
         }), e.computedCounter === void 0 && (e.computedCounter = t.computed(() => {
             if (n.counter !== !1) {
-                const w = typeof n.modelValue == "string" || typeof n.modelValue == "number" ? ("" + n.modelValue).length : Array.isArray(n.modelValue) === !0 ? n.modelValue.length : 0,
+                const y = typeof n.modelValue == "string" || typeof n.modelValue == "number" ? ("" + n.modelValue).length : Array.isArray(n.modelValue) === !0 ? n.modelValue.length : 0,
                     z = n.maxlength !== void 0 ? n.maxlength : n.maxValues;
-                return w + (z !== void 0 ? " / " + z : "")
+                return y + (z !== void 0 ? " / " + z : "")
             }
         }));
         const {
             isDirtyModel: c,
             hasRules: d,
             hasError: s,
-            errorMessage: h,
+            errorMessage: m,
             resetValidation: f
-        } = fi(e.focused, e.innerLoading), m = e.floatingLabel !== void 0 ? t.computed(() => n.stackLabel === !0 || e.focused.value === !0 || e.floatingLabel.value === !0) : t.computed(() => n.stackLabel === !0 || e.focused.value === !0 || e.hasValue.value === !0), v = t.computed(() => n.bottomSlots === !0 || n.hint !== void 0 || d.value === !0 || n.counter === !0 || n.error !== null), x = t.computed(() => n.filled === !0 ? "filled" : n.outlined === !0 ? "outlined" : n.borderless === !0 ? "borderless" : n.standout ? "standout" : "standard"), p = t.computed(() => `q-field row no-wrap items-start q-field--${x.value}` + (e.fieldClass !== void 0 ? ` ${e.fieldClass.value}` : "") + (n.rounded === !0 ? " q-field--rounded" : "") + (n.square === !0 ? " q-field--square" : "") + (m.value === !0 ? " q-field--float" : "") + (C.value === !0 ? " q-field--labeled" : "") + (n.dense === !0 ? " q-field--dense" : "") + (n.itemAligned === !0 ? " q-field--item-aligned q-item-type" : "") + (e.isDark.value === !0 ? " q-field--dark" : "") + (e.getControl === void 0 ? " q-field--auto-height" : "") + (e.focused.value === !0 ? " q-field--focused" : "") + (s.value === !0 ? " q-field--error" : "") + (s.value === !0 || e.focused.value === !0 ? " q-field--highlighted" : "") + (n.hideBottomSpace !== !0 && v.value === !0 ? " q-field--with-bottom" : "") + (n.disable === !0 ? " q-field--disabled" : n.readonly === !0 ? " q-field--readonly" : "")), S = t.computed(() => "q-field__control relative-position row no-wrap" + (n.bgColor !== void 0 ? ` bg-${n.bgColor}` : "") + (s.value === !0 ? " text-negative" : typeof n.standout == "string" && n.standout.length !== 0 && e.focused.value === !0 ? ` ${n.standout}` : n.color !== void 0 ? ` text-${n.color}` : "")), C = t.computed(() => n.labelSlot === !0 || n.label !== void 0), y = t.computed(() => "q-field__label no-pointer-events absolute ellipsis" + (n.labelColor !== void 0 && s.value !== !0 ? ` text-${n.labelColor}` : "")), P = t.computed(() => ({
+        } = fi(e.focused, e.innerLoading), h = e.floatingLabel !== void 0 ? t.computed(() => n.stackLabel === !0 || e.focused.value === !0 || e.floatingLabel.value === !0) : t.computed(() => n.stackLabel === !0 || e.focused.value === !0 || e.hasValue.value === !0), v = t.computed(() => n.bottomSlots === !0 || n.hint !== void 0 || d.value === !0 || n.counter === !0 || n.error !== null), _ = t.computed(() => n.filled === !0 ? "filled" : n.outlined === !0 ? "outlined" : n.borderless === !0 ? "borderless" : n.standout ? "standout" : "standard"), p = t.computed(() => `q-field row no-wrap items-start q-field--${_.value}` + (e.fieldClass !== void 0 ? ` ${e.fieldClass.value}` : "") + (n.rounded === !0 ? " q-field--rounded" : "") + (n.square === !0 ? " q-field--square" : "") + (h.value === !0 ? " q-field--float" : "") + (q.value === !0 ? " q-field--labeled" : "") + (n.dense === !0 ? " q-field--dense" : "") + (n.itemAligned === !0 ? " q-field--item-aligned q-item-type" : "") + (e.isDark.value === !0 ? " q-field--dark" : "") + (e.getControl === void 0 ? " q-field--auto-height" : "") + (e.focused.value === !0 ? " q-field--focused" : "") + (s.value === !0 ? " q-field--error" : "") + (s.value === !0 || e.focused.value === !0 ? " q-field--highlighted" : "") + (n.hideBottomSpace !== !0 && v.value === !0 ? " q-field--with-bottom" : "") + (n.disable === !0 ? " q-field--disabled" : n.readonly === !0 ? " q-field--readonly" : "")), k = t.computed(() => "q-field__control relative-position row no-wrap" + (n.bgColor !== void 0 ? ` bg-${n.bgColor}` : "") + (s.value === !0 ? " text-negative" : typeof n.standout == "string" && n.standout.length !== 0 && e.focused.value === !0 ? ` ${n.standout}` : n.color !== void 0 ? ` text-${n.color}` : "")), q = t.computed(() => n.labelSlot === !0 || n.label !== void 0), w = t.computed(() => "q-field__label no-pointer-events absolute ellipsis" + (n.labelColor !== void 0 && s.value !== !0 ? ` text-${n.labelColor}` : "")), C = t.computed(() => ({
             id: e.targetUid.value,
             editable: e.editable.value,
             focused: e.focused.value,
-            floatingLabel: m.value,
+            floatingLabel: h.value,
             modelValue: n.modelValue,
             emitValue: e.emitValue
         })), A = t.computed(() => {
-            const w = {
+            const y = {
                 for: e.targetUid.value
             };
-            return n.disable === !0 ? w["aria-disabled"] = "true" : n.readonly === !0 && (w["aria-readonly"] = "true"), w
+            return n.disable === !0 ? y["aria-disabled"] = "true" : n.readonly === !0 && (y["aria-readonly"] = "true"), y
         });
-        t.watch(() => n.for, w => {
-            e.targetUid.value = Kn(w)
+        t.watch(() => n.for, y => {
+            e.targetUid.value = Kn(y)
         });
 
         function M() {
-            const w = document.activeElement;
+            const y = document.activeElement;
             let z = e.targetRef !== void 0 && e.targetRef.value;
-            z && (w === null || w.id !== e.targetUid.value) && (z.hasAttribute("tabindex") === !0 || (z = z.querySelector("[tabindex]")), z && z !== w && z.focus({
+            z && (y === null || y.id !== e.targetUid.value) && (z.hasAttribute("tabindex") === !0 || (z = z.querySelector("[tabindex]")), z && z !== y && z.focus({
                 preventScroll: !0
             }))
         }
 
         function V() {
             hn(M)
         }
 
         function R() {
             pi(M);
-            const w = document.activeElement;
-            w !== null && e.rootRef.value.contains(w) && w.blur()
+            const y = document.activeElement;
+            y !== null && e.rootRef.value.contains(y) && y.blur()
         }
 
-        function T(w) {
-            u !== null && (clearTimeout(u), u = null), e.editable.value === !0 && e.focused.value === !1 && (e.focused.value = !0, o("focus", w))
+        function B(y) {
+            u !== null && (clearTimeout(u), u = null), e.editable.value === !0 && e.focused.value === !1 && (e.focused.value = !0, o("focus", y))
         }
 
-        function B(w, z) {
+        function P(y, z) {
             u !== null && clearTimeout(u), u = setTimeout(() => {
-                u = null, !(document.hasFocus() === !0 && (e.hasPopupOpen === !0 || e.controlRef === void 0 || e.controlRef.value === null || e.controlRef.value.contains(document.activeElement) !== !1)) && (e.focused.value === !0 && (e.focused.value = !1, o("blur", w)), z !== void 0 && z())
+                u = null, !(document.hasFocus() === !0 && (e.hasPopupOpen === !0 || e.controlRef === void 0 || e.controlRef.value === null || e.controlRef.value.contains(document.activeElement) !== !1)) && (e.focused.value === !0 && (e.focused.value = !1, o("blur", y)), z !== void 0 && z())
             })
         }
 
-        function I(w) {
-            ve(w), i.platform.is.mobile !== !0 ? (e.targetRef !== void 0 && e.targetRef.value || e.rootRef.value).focus() : e.rootRef.value.contains(document.activeElement) === !0 && document.activeElement.blur(), n.type === "file" && (e.inputRef.value.value = null), o("update:modelValue", null), o("clear", n.modelValue), t.nextTick(() => {
+        function I(y) {
+            ve(y), i.platform.is.mobile !== !0 ? (e.targetRef !== void 0 && e.targetRef.value || e.rootRef.value).focus() : e.rootRef.value.contains(document.activeElement) === !0 && document.activeElement.blur(), n.type === "file" && (e.inputRef.value.value = null), o("update:modelValue", null), o("clear", n.modelValue), t.nextTick(() => {
                 f(), i.platform.is.mobile !== !0 && (c.value = !1)
             })
         }
 
-        function k() {
-            const w = [];
-            return l.prepend !== void 0 && w.push(t.h("div", {
+        function x() {
+            const y = [];
+            return l.prepend !== void 0 && y.push(t.h("div", {
                 class: "q-field__prepend q-field__marginal row no-wrap items-center",
                 key: "prepend",
                 onClick: $e
-            }, l.prepend())), w.push(t.h("div", {
+            }, l.prepend())), y.push(t.h("div", {
                 class: "q-field__control-container col relative-position row no-wrap q-anchor--skip"
-            }, O())), s.value === !0 && n.noErrorIcon === !1 && w.push(j("error", [t.h(Be, {
+            }, O())), s.value === !0 && n.noErrorIcon === !1 && y.push(j("error", [t.h(Be, {
                 name: i.iconSet.field.error,
                 color: "negative"
-            })])), n.loading === !0 || e.innerLoading.value === !0 ? w.push(j("inner-loading-append", l.loading !== void 0 ? l.loading() : [t.h(Nn, {
+            })])), n.loading === !0 || e.innerLoading.value === !0 ? y.push(j("inner-loading-append", l.loading !== void 0 ? l.loading() : [t.h(Nn, {
                 color: n.color
-            })])) : n.clearable === !0 && e.hasValue.value === !0 && e.editable.value === !0 && w.push(j("inner-clearable-append", [t.h(Be, {
+            })])) : n.clearable === !0 && e.hasValue.value === !0 && e.editable.value === !0 && y.push(j("inner-clearable-append", [t.h(Be, {
                 class: "q-field__focusable-action",
                 tag: "button",
                 name: n.clearIcon || i.iconSet.field.clear,
                 tabindex: 0,
                 type: "button",
                 "aria-hidden": null,
                 role: null,
                 onClick: I
-            })])), l.append !== void 0 && w.push(t.h("div", {
+            })])), l.append !== void 0 && y.push(t.h("div", {
                 class: "q-field__append q-field__marginal row no-wrap items-center",
                 key: "append",
                 onClick: $e
-            }, l.append())), e.getInnerAppend !== void 0 && w.push(j("inner-append", e.getInnerAppend())), e.getControlChild !== void 0 && w.push(e.getControlChild()), w
+            }, l.append())), e.getInnerAppend !== void 0 && y.push(j("inner-append", e.getInnerAppend())), e.getControlChild !== void 0 && y.push(e.getControlChild()), y
         }
 
         function O() {
-            const w = [];
-            return n.prefix !== void 0 && n.prefix !== null && w.push(t.h("div", {
+            const y = [];
+            return n.prefix !== void 0 && n.prefix !== null && y.push(t.h("div", {
                 class: "q-field__prefix no-pointer-events row items-center"
-            }, n.prefix)), e.getShadowControl !== void 0 && e.hasShadow.value === !0 && w.push(e.getShadowControl()), e.getControl !== void 0 ? w.push(e.getControl()) : l.rawControl !== void 0 ? w.push(l.rawControl()) : l.control !== void 0 && w.push(t.h("div", {
+            }, n.prefix)), e.getShadowControl !== void 0 && e.hasShadow.value === !0 && y.push(e.getShadowControl()), e.getControl !== void 0 ? y.push(e.getControl()) : l.rawControl !== void 0 ? y.push(l.rawControl()) : l.control !== void 0 && y.push(t.h("div", {
                 ref: e.targetRef,
                 class: "q-field__native row",
                 tabindex: -1,
                 ...e.splitAttrs.attributes.value,
                 "data-autofocus": n.autofocus === !0 || void 0
-            }, l.control(P.value))), C.value === !0 && w.push(t.h("div", {
-                class: y.value
-            }, we(l.label, n.label))), n.suffix !== void 0 && n.suffix !== null && w.push(t.h("div", {
+            }, l.control(C.value))), q.value === !0 && y.push(t.h("div", {
+                class: w.value
+            }, we(l.label, n.label))), n.suffix !== void 0 && n.suffix !== null && y.push(t.h("div", {
                 class: "q-field__suffix no-pointer-events row items-center"
-            }, n.suffix)), w.concat(we(l.default))
+            }, n.suffix)), y.concat(we(l.default))
         }
 
-        function q() {
-            let w, z;
-            s.value === !0 ? h.value !== null ? (w = [t.h("div", {
+        function T() {
+            let y, z;
+            s.value === !0 ? m.value !== null ? (y = [t.h("div", {
                 role: "alert"
-            }, h.value)], z = `q--slot-error-${h.value}`) : (w = we(l.error), z = "q--slot-error") : (n.hideHint !== !0 || e.focused.value === !0) && (n.hint !== void 0 ? (w = [t.h("div", n.hint)], z = `q--slot-hint-${n.hint}`) : (w = we(l.hint), z = "q--slot-hint"));
+            }, m.value)], z = `q--slot-error-${m.value}`) : (y = we(l.error), z = "q--slot-error") : (n.hideHint !== !0 || e.focused.value === !0) && (n.hint !== void 0 ? (y = [t.h("div", n.hint)], z = `q--slot-hint-${n.hint}`) : (y = we(l.hint), z = "q--slot-hint"));
             const G = n.counter === !0 || l.counter !== void 0;
-            if (n.hideBottomSpace === !0 && G === !1 && w === void 0) return;
+            if (n.hideBottomSpace === !0 && G === !1 && y === void 0) return;
             const J = t.h("div", {
                 key: z,
                 class: "q-field__messages col"
-            }, w);
+            }, y);
             return t.h("div", {
                 class: "q-field__bottom row items-start q-field__bottom--" + (n.hideBottomSpace !== !0 ? "animated" : "stale"),
                 onClick: $e
             }, [n.hideBottomSpace === !0 ? J : t.h(t.Transition, {
                 name: "q-transition--field-message"
             }, () => J), G === !0 ? t.h("div", {
                 class: "q-field__counter"
             }, l.counter !== void 0 ? l.counter() : e.computedCounter.value) : null])
         }
 
-        function j(w, z) {
+        function j(y, z) {
             return z === null ? null : t.h("div", {
-                key: w,
+                key: y,
                 class: "q-field__append q-field__marginal row no-wrap items-center q-anchor--skip"
             }, z)
         }
         let N = !1;
         return t.onDeactivated(() => {
                 N = !0
             }), t.onActivated(() => {
@@ -884,18 +884,18 @@
                 }, [l.before !== void 0 ? t.h("div", {
                     class: "q-field__before q-field__marginal row no-wrap items-center",
                     onClick: $e
                 }, l.before()) : null, t.h("div", {
                     class: "q-field__inner relative-position col self-stretch"
                 }, [t.h("div", {
                     ref: e.controlRef,
-                    class: S.value,
+                    class: k.value,
                     tabindex: -1,
                     ...e.controlEvents
-                }, k()), v.value === !0 ? q() : null]), l.after !== void 0 ? t.h("div", {
+                }, x()), v.value === !0 ? T() : null]), l.after !== void 0 ? t.h("div", {
                     class: "q-field__after q-field__marginal row no-wrap items-center",
                     onClick: $e
                 }, l.after()) : null])
             }
     }
     const bi = se({
         name: "QField",
@@ -919,15 +919,15 @@
         } catch {
             return
         }
         const n = t.unref(e);
         if (n) return n.$el || n
     }
 
-    function wl(e, n) {
+    function Sl(e, n) {
         if (e == null || e.contains(n) === !0) return !0;
         for (let o = e.nextElementSibling; o !== null; o = o.nextElementSibling)
             if (o.contains(n)) return !0;
         return !1
     }
 
     function gn(e) {
@@ -944,54 +944,54 @@
         return function() {
             return o === !1 && (o = !0, setTimeout(() => {
                 o = !1
             }, n), l = e.apply(this, arguments)), l
         }
     }
 
-    function Sl(e, n, o, l) {
+    function _l(e, n, o, l) {
         o.modifiers.stop === !0 && De(e);
         const r = o.modifiers.color;
         let a = o.modifiers.center;
         a = a === !0 || l === !0;
         const i = document.createElement("span"),
             u = document.createElement("span"),
             c = dt(e),
             {
                 left: d,
                 top: s,
-                width: h,
+                width: m,
                 height: f
             } = n.getBoundingClientRect(),
-            m = Math.sqrt(h * h + f * f),
-            v = m / 2,
-            x = `${(h-m)/2}px`,
-            p = a ? x : `${c.left-d-v}px`,
-            S = `${(f-m)/2}px`,
-            C = a ? S : `${c.top-s-v}px`;
+            h = Math.sqrt(m * m + f * f),
+            v = h / 2,
+            _ = `${(m-h)/2}px`,
+            p = a ? _ : `${c.left-d-v}px`,
+            k = `${(f-h)/2}px`,
+            q = a ? k : `${c.top-s-v}px`;
         u.className = "q-ripple__inner", Yn(u, {
-            height: `${m}px`,
-            width: `${m}px`,
-            transform: `translate3d(${p},${C},0) scale3d(.2,.2,1)`,
+            height: `${h}px`,
+            width: `${h}px`,
+            transform: `translate3d(${p},${q},0) scale3d(.2,.2,1)`,
             opacity: 0
         }), i.className = `q-ripple${r?" text-"+r:""}`, i.setAttribute("dir", "ltr"), i.appendChild(u), n.appendChild(i);
-        const y = () => {
-            i.remove(), clearTimeout(P)
+        const w = () => {
+            i.remove(), clearTimeout(C)
         };
-        o.abort.push(y);
-        let P = setTimeout(() => {
-            u.classList.add("q-ripple__inner--enter"), u.style.transform = `translate3d(${x},${S},0) scale3d(1,1,1)`, u.style.opacity = .2, P = setTimeout(() => {
-                u.classList.remove("q-ripple__inner--enter"), u.classList.add("q-ripple__inner--leave"), u.style.opacity = 0, P = setTimeout(() => {
-                    i.remove(), o.abort.splice(o.abort.indexOf(y), 1)
+        o.abort.push(w);
+        let C = setTimeout(() => {
+            u.classList.add("q-ripple__inner--enter"), u.style.transform = `translate3d(${_},${k},0) scale3d(1,1,1)`, u.style.opacity = .2, C = setTimeout(() => {
+                u.classList.remove("q-ripple__inner--enter"), u.classList.add("q-ripple__inner--leave"), u.style.opacity = 0, C = setTimeout(() => {
+                    i.remove(), o.abort.splice(o.abort.indexOf(w), 1)
                 }, 275)
             }, 250)
         }, 50)
     }
 
-    function _l(e, {
+    function xl(e, {
         modifiers: n,
         value: o,
         arg: l
     }) {
         const r = Object.assign({}, e.cfg.ripple, n, o);
         e.modifiers = {
             early: r.early === !0,
@@ -1008,31 +1008,31 @@
                 if (o.ripple === !1) return;
                 const l = {
                     cfg: o,
                     enabled: n.value !== !1,
                     modifiers: {},
                     abort: [],
                     start(r) {
-                        l.enabled === !0 && r.qSkipRipple !== !0 && r.type === (l.modifiers.early === !0 ? "pointerdown" : "click") && Sl(r, e, l, r.qKeyEvent === !0)
+                        l.enabled === !0 && r.qSkipRipple !== !0 && r.type === (l.modifiers.early === !0 ? "pointerdown" : "click") && _l(r, e, l, r.qKeyEvent === !0)
                     },
                     keystart: wi(r => {
-                        l.enabled === !0 && r.qSkipRipple !== !0 && ut(r, l.modifiers.keyCodes) === !0 && r.type === `key${l.modifiers.early===!0?"down":"up"}` && Sl(r, e, l, !0)
+                        l.enabled === !0 && r.qSkipRipple !== !0 && ut(r, l.modifiers.keyCodes) === !0 && r.type === `key${l.modifiers.early===!0?"down":"up"}` && _l(r, e, l, !0)
                     }, 300)
                 };
-                _l(l, n), e.__qripple = l, Qe(l, "main", [
+                xl(l, n), e.__qripple = l, Qe(l, "main", [
                     [e, "pointerdown", "start", "passive"],
                     [e, "click", "start", "passive"],
                     [e, "keydown", "keystart", "passive"],
                     [e, "keyup", "keystart", "passive"]
                 ])
             },
             updated(e, n) {
                 if (n.oldValue !== n.value) {
                     const o = e.__qripple;
-                    o !== void 0 && (o.enabled = n.value !== !1, o.enabled === !0 && Object(n.value) === n.value && _l(o, n))
+                    o !== void 0 && (o.enabled = n.value !== !1, o.enabled === !0 && Object(n.value) === n.value && xl(o, n))
                 }
             },
             beforeUnmount(e) {
                 const n = e.__qripple;
                 n !== void 0 && (n.abort.forEach(o => {
                     o()
                 }), it(n, "main"), delete e._qripple)
@@ -1086,79 +1086,79 @@
                 const {
                     proxy: {
                         $q: l
                     }
                 } = t.getCurrentInstance(), r = Fe(e, l), a = Ht(e, Si), i = t.computed(() => e.selected === !0 || e.icon !== void 0), u = t.computed(() => e.selected === !0 ? e.iconSelected || l.iconSet.chip.selected : e.icon), c = t.computed(() => e.iconRemove || l.iconSet.chip.remove), d = t.computed(() => e.disable === !1 && (e.clickable === !0 || e.selected !== null)), s = t.computed(() => {
                     const p = e.outline === !0 && e.color || e.textColor;
                     return "q-chip row inline no-wrap items-center" + (e.outline === !1 && e.color !== void 0 ? ` bg-${e.color}` : "") + (p ? ` text-${p} q-chip--colored` : "") + (e.disable === !0 ? " disabled" : "") + (e.dense === !0 ? " q-chip--dense" : "") + (e.outline === !0 ? " q-chip--outline" : "") + (e.selected === !0 ? " q-chip--selected" : "") + (d.value === !0 ? " q-chip--clickable cursor-pointer non-selectable q-hoverable" : "") + (e.square === !0 ? " q-chip--square" : "") + (r.value === !0 ? " q-chip--dark q-dark" : "")
-                }), h = t.computed(() => {
+                }), m = t.computed(() => {
                     const p = e.disable === !0 ? {
                             tabindex: -1,
                             "aria-disabled": "true"
                         } : {
                             tabindex: e.tabindex || 0
                         },
-                        S = {
+                        k = {
                             ...p,
                             role: "button",
                             "aria-hidden": "false",
                             "aria-label": e.removeAriaLabel || l.lang.label.remove
                         };
                     return {
                         chip: p,
-                        remove: S
+                        remove: k
                     }
                 });
 
                 function f(p) {
-                    p.keyCode === 13 && m(p)
+                    p.keyCode === 13 && h(p)
                 }
 
-                function m(p) {
+                function h(p) {
                     e.disable || (o("update:selected", !e.selected), o("click", p))
                 }
 
                 function v(p) {
                     (p.keyCode === void 0 || p.keyCode === 13) && (ve(p), e.disable === !1 && (o("update:modelValue", !1), o("remove")))
                 }
 
-                function x() {
+                function _() {
                     const p = [];
                     d.value === !0 && p.push(t.h("div", {
                         class: "q-focus-helper"
                     })), i.value === !0 && p.push(t.h(Be, {
                         class: "q-chip__icon q-chip__icon--left",
                         name: u.value
                     }));
-                    const S = e.label !== void 0 ? [t.h("div", {
+                    const k = e.label !== void 0 ? [t.h("div", {
                         class: "ellipsis"
                     }, [e.label])] : void 0;
                     return p.push(t.h("div", {
                         class: "q-chip__content col row no-wrap items-center q-anchor--skip"
-                    }, Za(n.default, S))), e.iconRight && p.push(t.h(Be, {
+                    }, Za(n.default, k))), e.iconRight && p.push(t.h(Be, {
                         class: "q-chip__icon q-chip__icon--right",
                         name: e.iconRight
                     })), e.removable === !0 && p.push(t.h(Be, {
                         class: "q-chip__icon q-chip__icon--remove cursor-pointer",
                         name: c.value,
-                        ...h.value.remove,
+                        ...m.value.remove,
                         onClick: v,
                         onKeyup: v
                     })), p
                 }
                 return () => {
                     if (e.modelValue === !1) return;
                     const p = {
                         class: s.value,
                         style: a.value
                     };
-                    return d.value === !0 && Object.assign(p, h.value.chip, {
-                        onClick: m,
+                    return d.value === !0 && Object.assign(p, m.value.chip, {
+                        onClick: h,
                         onKeyup: f
-                    }), cn("div", p, x(), "ripple", e.ripple !== !1 && e.disable !== !0, () => [
+                    }), cn("div", p, _(), "ripple", e.ripple !== !1 && e.disable !== !0, () => [
                         [Zn, e.ripple]
                     ])
                 }
             }
         });
 
     function Jn(e) {
@@ -1168,69 +1168,69 @@
         } = e.$;
         for (; Object(n) === n;) {
             if (Object(n.proxy) === n.proxy) return n.proxy;
             n = n.parent
         }
     }
 
-    function xl(e, n) {
+    function kl(e, n) {
         typeof n.type == "symbol" ? Array.isArray(n.children) === !0 && n.children.forEach(o => {
-            xl(e, o)
+            kl(e, o)
         }) : e.add(n)
     }
 
     function xi(e) {
         const n = new Set;
         return e.forEach(o => {
-            xl(n, o)
+            kl(n, o)
         }), Array.from(n)
     }
 
     function eo(e) {
         return e.appContext.config.globalProperties.$router !== void 0
     }
 
-    function kl(e) {
+    function Cl(e) {
         return e.isUnmounted === !0 || e.isDeactivated === !0
     }
 
-    function Cl(e) {
+    function ql(e) {
         return e ? e.aliasOf ? e.aliasOf.path : e.path : ""
     }
 
-    function ql(e, n) {
+    function Tl(e, n) {
         return (e.aliasOf || e) === (n.aliasOf || n)
     }
 
     function ki(e, n) {
         for (const o in n) {
             const l = n[o],
                 r = e[o];
             if (typeof l == "string") {
                 if (l !== r) return !1
             } else if (Array.isArray(r) === !1 || r.length !== l.length || l.some((a, i) => a !== r[i])) return !1
         }
         return !0
     }
 
-    function Tl(e, n) {
+    function Bl(e, n) {
         return Array.isArray(n) === !0 ? e.length === n.length && e.every((o, l) => o === n[l]) : e.length === 1 && e[0] === n
     }
 
     function Ci(e, n) {
-        return Array.isArray(e) === !0 ? Tl(e, n) : Array.isArray(n) === !0 ? Tl(n, e) : e === n
+        return Array.isArray(e) === !0 ? Bl(e, n) : Array.isArray(n) === !0 ? Bl(n, e) : e === n
     }
 
     function qi(e, n) {
         if (Object.keys(e).length !== Object.keys(n).length) return !1;
         for (const o in e)
             if (Ci(e[o], n[o]) === !1) return !1;
         return !0
     }
-    const Bl = {
+    const Pl = {
         to: [String, Object],
         replace: Boolean,
         exact: Boolean,
         activeClass: {
             type: String,
             default: "q-router-link--active"
         },
@@ -1239,32 +1239,32 @@
             default: "q-router-link--exact-active"
         },
         href: String,
         target: String,
         disable: Boolean
     };
 
-    function Pl({
+    function El({
         fallbackTag: e,
         useDisableForRouterLinkProps: n = !0
     } = {}) {
         const o = t.getCurrentInstance(),
             {
                 props: l,
                 proxy: r,
                 emit: a
             } = o,
             i = eo(o),
             u = t.computed(() => l.disable !== !0 && l.href !== void 0),
             c = n === !0 ? t.computed(() => i === !0 && l.disable !== !0 && u.value !== !0 && l.to !== void 0 && l.to !== null && l.to !== "") : t.computed(() => i === !0 && u.value !== !0 && l.to !== void 0 && l.to !== null && l.to !== ""),
-            d = t.computed(() => c.value === !0 ? C(l.to) : null),
+            d = t.computed(() => c.value === !0 ? q(l.to) : null),
             s = t.computed(() => d.value !== null),
-            h = t.computed(() => u.value === !0 || s.value === !0),
-            f = t.computed(() => l.type === "a" || h.value === !0 ? "a" : l.tag || e || "div"),
-            m = t.computed(() => u.value === !0 ? {
+            m = t.computed(() => u.value === !0 || s.value === !0),
+            f = t.computed(() => l.type === "a" || m.value === !0 ? "a" : l.tag || e || "div"),
+            h = t.computed(() => u.value === !0 ? {
                 href: l.href,
                 target: l.target
             } : s.value === !0 ? {
                 href: d.value.href,
                 target: l.target
             } : {}),
             v = t.computed(() => {
@@ -1273,68 +1273,68 @@
                     matched: A
                 } = d.value, {
                     length: M
                 } = A, V = A[M - 1];
                 if (V === void 0) return -1;
                 const R = r.$route.matched;
                 if (R.length === 0) return -1;
-                const T = R.findIndex(ql.bind(null, V));
-                if (T > -1) return T;
-                const B = Cl(A[M - 2]);
-                return M > 1 && Cl(V) === B && R[R.length - 1].path !== B ? R.findIndex(ql.bind(null, A[M - 2])) : T
+                const B = R.findIndex(Tl.bind(null, V));
+                if (B > -1) return B;
+                const P = ql(A[M - 2]);
+                return M > 1 && ql(V) === P && R[R.length - 1].path !== P ? R.findIndex(Tl.bind(null, A[M - 2])) : B
             }),
-            x = t.computed(() => s.value === !0 && v.value !== -1 && ki(r.$route.params, d.value.params)),
-            p = t.computed(() => x.value === !0 && v.value === r.$route.matched.length - 1 && qi(r.$route.params, d.value.params)),
-            S = t.computed(() => s.value === !0 ? p.value === !0 ? ` ${l.exactActiveClass} ${l.activeClass}` : l.exact === !0 ? "" : x.value === !0 ? ` ${l.activeClass}` : "" : "");
+            _ = t.computed(() => s.value === !0 && v.value !== -1 && ki(r.$route.params, d.value.params)),
+            p = t.computed(() => _.value === !0 && v.value === r.$route.matched.length - 1 && qi(r.$route.params, d.value.params)),
+            k = t.computed(() => s.value === !0 ? p.value === !0 ? ` ${l.exactActiveClass} ${l.activeClass}` : l.exact === !0 ? "" : _.value === !0 ? ` ${l.activeClass}` : "" : "");
 
-        function C(A) {
+        function q(A) {
             try {
                 return r.$router.resolve(A)
             } catch {}
             return null
         }
 
-        function y(A, {
+        function w(A, {
             returnRouterError: M,
             to: V = l.to,
             replace: R = l.replace
         } = {}) {
             if (l.disable === !0) return A.preventDefault(), Promise.resolve(!1);
             if (A.metaKey || A.altKey || A.ctrlKey || A.shiftKey || A.button !== void 0 && A.button !== 0 || l.target === "_blank") return Promise.resolve(!1);
             A.preventDefault();
-            const T = r.$router[R === !0 ? "replace" : "push"](V);
-            return M === !0 ? T : T.then(() => {}).catch(() => {})
+            const B = r.$router[R === !0 ? "replace" : "push"](V);
+            return M === !0 ? B : B.then(() => {}).catch(() => {})
         }
 
-        function P(A) {
+        function C(A) {
             if (s.value === !0) {
-                const M = V => y(A, V);
+                const M = V => w(A, V);
                 a("click", A, M), A.defaultPrevented !== !0 && M()
             } else a("click", A)
         }
         return {
             hasRouterLink: s,
             hasHrefLink: u,
-            hasLink: h,
+            hasLink: m,
             linkTag: f,
             resolvedLink: d,
-            linkIsActive: x,
+            linkIsActive: _,
             linkIsExactActive: p,
-            linkClass: S,
-            linkAttrs: m,
-            getLink: C,
-            navigateToRouterLink: y,
-            navigateOnClick: P
+            linkClass: k,
+            linkAttrs: h,
+            getLink: q,
+            navigateToRouterLink: w,
+            navigateOnClick: C
         }
     }
-    const El = se({
+    const $l = se({
             name: "QItem",
             props: {
                 ...Le,
-                ...Bl,
+                ...Pl,
                 tag: {
                     type: String,
                     default: "div"
                 },
                 active: {
                     type: Boolean,
                     default: null
@@ -1357,49 +1357,49 @@
                     }
                 } = t.getCurrentInstance(), r = Fe(e, l), {
                     hasLink: a,
                     linkAttrs: i,
                     linkClass: u,
                     linkTag: c,
                     navigateOnClick: d
-                } = Pl(), s = t.ref(null), h = t.ref(null), f = t.computed(() => e.clickable === !0 || a.value === !0 || e.tag === "label"), m = t.computed(() => e.disable !== !0 && f.value === !0), v = t.computed(() => "q-item q-item-type row no-wrap" + (e.dense === !0 ? " q-item--dense" : "") + (r.value === !0 ? " q-item--dark" : "") + (a.value === !0 && e.active === null ? u.value : e.active === !0 ? ` q-item--active${e.activeClass!==void 0?` ${e.activeClass}`:""}` : "") + (e.disable === !0 ? " disabled" : "") + (m.value === !0 ? " q-item--clickable q-link cursor-pointer " + (e.manualFocus === !0 ? "q-manual-focusable" : "q-focusable q-hoverable") + (e.focused === !0 ? " q-manual-focusable--focused" : "") : "")), x = t.computed(() => e.insetLevel === void 0 ? null : {
+                } = El(), s = t.ref(null), m = t.ref(null), f = t.computed(() => e.clickable === !0 || a.value === !0 || e.tag === "label"), h = t.computed(() => e.disable !== !0 && f.value === !0), v = t.computed(() => "q-item q-item-type row no-wrap" + (e.dense === !0 ? " q-item--dense" : "") + (r.value === !0 ? " q-item--dark" : "") + (a.value === !0 && e.active === null ? u.value : e.active === !0 ? ` q-item--active${e.activeClass!==void 0?` ${e.activeClass}`:""}` : "") + (e.disable === !0 ? " disabled" : "") + (h.value === !0 ? " q-item--clickable q-link cursor-pointer " + (e.manualFocus === !0 ? "q-manual-focusable" : "q-focusable q-hoverable") + (e.focused === !0 ? " q-manual-focusable--focused" : "") : "")), _ = t.computed(() => e.insetLevel === void 0 ? null : {
                     ["padding" + (l.lang.rtl === !0 ? "Right" : "Left")]: 16 + e.insetLevel * 56 + "px"
                 });
 
-                function p(y) {
-                    m.value === !0 && (h.value !== null && (y.qKeyEvent !== !0 && document.activeElement === s.value ? h.value.focus() : document.activeElement === h.value && s.value.focus()), d(y))
+                function p(w) {
+                    h.value === !0 && (m.value !== null && (w.qKeyEvent !== !0 && document.activeElement === s.value ? m.value.focus() : document.activeElement === m.value && s.value.focus()), d(w))
                 }
 
-                function S(y) {
-                    if (m.value === !0 && ut(y, 13) === !0) {
-                        ve(y), y.qKeyEvent = !0;
-                        const P = new MouseEvent("click", y);
-                        P.qKeyEvent = !0, s.value.dispatchEvent(P)
+                function k(w) {
+                    if (h.value === !0 && ut(w, 13) === !0) {
+                        ve(w), w.qKeyEvent = !0;
+                        const C = new MouseEvent("click", w);
+                        C.qKeyEvent = !0, s.value.dispatchEvent(C)
                     }
-                    o("keyup", y)
+                    o("keyup", w)
                 }
 
-                function C() {
-                    const y = nl(n.default, []);
-                    return m.value === !0 && y.unshift(t.h("div", {
+                function q() {
+                    const w = ol(n.default, []);
+                    return h.value === !0 && w.unshift(t.h("div", {
                         class: "q-focus-helper",
                         tabindex: -1,
-                        ref: h
-                    })), y
+                        ref: m
+                    })), w
                 }
                 return () => {
-                    const y = {
+                    const w = {
                         ref: s,
                         class: v.value,
-                        style: x.value,
+                        style: _.value,
                         role: "listitem",
                         onClick: p,
-                        onKeyup: S
+                        onKeyup: k
                     };
-                    return m.value === !0 ? (y.tabindex = e.tabindex || "0", Object.assign(y, i.value)) : f.value === !0 && (y["aria-disabled"] = "true"), t.h(c.value, y, C())
+                    return h.value === !0 ? (w.tabindex = e.tabindex || "0", Object.assign(w, i.value)) : f.value === !0 && (w["aria-disabled"] = "true"), t.h(c.value, w, q())
                 }
             }
         }),
         to = se({
             name: "QItemSection",
             props: {
                 avatar: Boolean,
@@ -1413,15 +1413,15 @@
             }) {
                 const o = t.computed(() => `q-item__section column q-item__section--${e.avatar===!0||e.side===!0||e.thumbnail===!0?"side":"main"}` + (e.top === !0 ? " q-item__section--top justify-start" : " justify-center") + (e.avatar === !0 ? " q-item__section--avatar" : "") + (e.thumbnail === !0 ? " q-item__section--thumbnail" : "") + (e.noWrap === !0 ? " q-item__section--nowrap" : ""));
                 return () => t.h("div", {
                     class: o.value
                 }, we(n.default))
             }
         }),
-        $l = se({
+        Al = se({
             name: "QItemLabel",
             props: {
                 overline: Boolean,
                 caption: Boolean,
                 header: Boolean,
                 lines: [Number, String]
             },
@@ -1465,92 +1465,92 @@
         const {
             props: l,
             proxy: r,
             emit: a
         } = t.getCurrentInstance(), i = t.ref(null);
         let u = null;
 
-        function c(m) {
-            return i.value === null ? !1 : m === void 0 || m.touches === void 0 || m.touches.length <= 1
+        function c(h) {
+            return i.value === null ? !1 : h === void 0 || h.touches === void 0 || h.touches.length <= 1
         }
         const d = {};
         o === void 0 && (Object.assign(d, {
-            hide(m) {
-                r.hide(m)
+            hide(h) {
+                r.hide(h)
             },
-            toggle(m) {
-                r.toggle(m), m.qAnchorHandled = !0
+            toggle(h) {
+                r.toggle(h), h.qAnchorHandled = !0
             },
-            toggleKey(m) {
-                ut(m, 13) === !0 && d.toggle(m)
+            toggleKey(h) {
+                ut(h, 13) === !0 && d.toggle(h)
             },
-            contextClick(m) {
-                r.hide(m), $e(m), t.nextTick(() => {
-                    r.show(m), m.qAnchorHandled = !0
+            contextClick(h) {
+                r.hide(h), $e(h), t.nextTick(() => {
+                    r.show(h), h.qAnchorHandled = !0
                 })
             },
             prevent: $e,
-            mobileTouch(m) {
-                if (d.mobileCleanup(m), c(m) !== !0) return;
-                r.hide(m), i.value.classList.add("non-selectable");
-                const v = m.target;
+            mobileTouch(h) {
+                if (d.mobileCleanup(h), c(h) !== !0) return;
+                r.hide(h), i.value.classList.add("non-selectable");
+                const v = h.target;
                 Qe(d, "anchor", [
                     [v, "touchmove", "mobileCleanup", "passive"],
                     [v, "touchend", "mobileCleanup", "passive"],
                     [v, "touchcancel", "mobileCleanup", "passive"],
                     [i.value, "contextmenu", "prevent", "notPassive"]
                 ]), u = setTimeout(() => {
-                    u = null, r.show(m), m.qAnchorHandled = !0
+                    u = null, r.show(h), h.qAnchorHandled = !0
                 }, 300)
             },
-            mobileCleanup(m) {
-                i.value.classList.remove("non-selectable"), u !== null && (clearTimeout(u), u = null), e.value === !0 && m !== void 0 && no()
+            mobileCleanup(h) {
+                i.value.classList.remove("non-selectable"), u !== null && (clearTimeout(u), u = null), e.value === !0 && h !== void 0 && no()
             }
-        }), o = function(m = l.contextMenu) {
+        }), o = function(h = l.contextMenu) {
             if (l.noParentEvent === !0 || i.value === null) return;
             let v;
-            m === !0 ? r.$q.platform.is.mobile === !0 ? v = [
+            h === !0 ? r.$q.platform.is.mobile === !0 ? v = [
                 [i.value, "touchstart", "mobileTouch", "passive"]
             ] : v = [
                 [i.value, "mousedown", "hide", "passive"],
                 [i.value, "contextmenu", "contextClick", "notPassive"]
             ] : v = [
                 [i.value, "click", "toggle", "passive"],
                 [i.value, "keyup", "toggleKey", "passive"]
             ], Qe(d, "anchor", v)
         });
 
         function s() {
             it(d, "anchor")
         }
 
-        function h(m) {
-            for (i.value = m; i.value.classList.contains("q-anchor--skip");) i.value = i.value.parentNode;
+        function m(h) {
+            for (i.value = h; i.value.classList.contains("q-anchor--skip");) i.value = i.value.parentNode;
             o()
         }
 
         function f() {
             if (l.target === !1 || l.target === "" || r.$el.parentNode === null) i.value = null;
-            else if (l.target === !0) h(r.$el.parentNode);
+            else if (l.target === !0) m(r.$el.parentNode);
             else {
-                let m = l.target;
+                let h = l.target;
                 if (typeof l.target == "string") try {
-                    m = document.querySelector(l.target)
+                    h = document.querySelector(l.target)
                 } catch {
-                    m = void 0
+                    h = void 0
                 }
-                m != null ? (i.value = m.$el || m, o()) : (i.value = null, console.error(`Anchor: target "${l.target}" not found`))
+                h != null ? (i.value = h.$el || h, o()) : (i.value = null, console.error(`Anchor: target "${l.target}" not found`))
             }
         }
-        return t.watch(() => l.contextMenu, m => {
-            i.value !== null && (s(), o(m))
+        return t.watch(() => l.contextMenu, h => {
+            i.value !== null && (s(), o(h))
         }), t.watch(() => l.target, () => {
             i.value !== null && s(), f()
-        }), t.watch(() => l.noParentEvent, m => {
-            i.value !== null && (m === !0 ? s() : o())
+        }), t.watch(() => l.noParentEvent, h => {
+            i.value !== null && (h === !0 ? s() : o())
         }), t.onMounted(() => {
             f(), n !== !0 && l.modelValue === !0 && i.value === null && a("update:modelValue", !1)
         }), t.onBeforeUnmount(() => {
             u !== null && clearTimeout(u), s()
         }), {
             anchorEl: i,
             canShow: c,
@@ -1601,65 +1601,65 @@
             {
                 props: u,
                 emit: c,
                 proxy: d
             } = i;
         let s;
 
-        function h(C) {
-            e.value === !0 ? v(C) : f(C)
+        function m(q) {
+            e.value === !0 ? v(q) : f(q)
         }
 
-        function f(C) {
-            if (u.disable === !0 || C !== void 0 && C.qAnchorHandled === !0 || n !== void 0 && n(C) !== !0) return;
-            const y = u["onUpdate:modelValue"] !== void 0;
-            y === !0 && (c("update:modelValue", !0), s = C, t.nextTick(() => {
-                s === C && (s = void 0)
-            })), (u.modelValue === null || y === !1) && m(C)
+        function f(q) {
+            if (u.disable === !0 || q !== void 0 && q.qAnchorHandled === !0 || n !== void 0 && n(q) !== !0) return;
+            const w = u["onUpdate:modelValue"] !== void 0;
+            w === !0 && (c("update:modelValue", !0), s = q, t.nextTick(() => {
+                s === q && (s = void 0)
+            })), (u.modelValue === null || w === !1) && h(q)
         }
 
-        function m(C) {
-            e.value !== !0 && (e.value = !0, c("beforeShow", C), l !== void 0 ? l(C) : c("show", C))
+        function h(q) {
+            e.value !== !0 && (e.value = !0, c("beforeShow", q), l !== void 0 ? l(q) : c("show", q))
         }
 
-        function v(C) {
+        function v(q) {
             if (u.disable === !0) return;
-            const y = u["onUpdate:modelValue"] !== void 0;
-            y === !0 && (c("update:modelValue", !1), s = C, t.nextTick(() => {
-                s === C && (s = void 0)
-            })), (u.modelValue === null || y === !1) && x(C)
+            const w = u["onUpdate:modelValue"] !== void 0;
+            w === !0 && (c("update:modelValue", !1), s = q, t.nextTick(() => {
+                s === q && (s = void 0)
+            })), (u.modelValue === null || w === !1) && _(q)
         }
 
-        function x(C) {
-            e.value !== !1 && (e.value = !1, c("beforeHide", C), r !== void 0 ? r(C) : c("hide", C))
+        function _(q) {
+            e.value !== !1 && (e.value = !1, c("beforeHide", q), r !== void 0 ? r(q) : c("hide", q))
         }
 
-        function p(C) {
-            u.disable === !0 && C === !0 ? u["onUpdate:modelValue"] !== void 0 && c("update:modelValue", !1) : C === !0 !== e.value && (C === !0 ? m : x)(s)
+        function p(q) {
+            u.disable === !0 && q === !0 ? u["onUpdate:modelValue"] !== void 0 && c("update:modelValue", !1) : q === !0 !== e.value && (q === !0 ? h : _)(s)
         }
         t.watch(() => u.modelValue, p), o !== void 0 && eo(i) === !0 && t.watch(() => d.$route.fullPath, () => {
             o.value === !0 && e.value === !0 && v()
         }), a === !0 && t.onMounted(() => {
             p(u.modelValue)
         });
-        const S = {
+        const k = {
             show: f,
             hide: v,
-            toggle: h
+            toggle: m
         };
-        return Object.assign(d, S), S
+        return Object.assign(d, k), k
     }
-    const Al = {};
+    const Ol = {};
     let Ei = 1,
         $i = document.body;
 
     function Ai(e, n) {
         const o = document.createElement("div");
-        if (o.id = n !== void 0 ? `q-portal--${n}--${Ei++}` : e, Al.globalNodes !== void 0) {
-            const l = Al.globalNodes.class;
+        if (o.id = n !== void 0 ? `q-portal--${n}--${Ei++}` : e, Ol.globalNodes !== void 0) {
+            const l = Ol.globalNodes.class;
             l !== void 0 && (o.className = l)
         }
         return $i.appendChild(o), o
     }
 
     function Oi(e) {
         e.remove()
@@ -1683,32 +1683,32 @@
             if (e.type.name === "QGlobalDialog") return !0;
             if (e.type.name === "QDialog" || e.type.name === "QMenu") return !1;
             e = e.parent
         }
         return !1
     }
 
-    function Ol(e, n, o, l) {
+    function Ml(e, n, o, l) {
         const r = t.ref(!1),
             a = t.ref(!1);
         let i = null;
         const u = {},
             c = l === "dialog" && Ri(e);
 
-        function d(h) {
-            if (h === !0) {
-                yl(u), a.value = !0;
+        function d(m) {
+            if (m === !0) {
+                wl(u), a.value = !0;
                 return
             }
             a.value = !1, r.value === !1 && (c === !1 && i === null && (i = Ai(!1, l)), r.value = !0, Qt.push(e.proxy), gi(u))
         }
 
-        function s(h) {
-            if (a.value = !1, h !== !0) return;
-            yl(u), r.value = !1;
+        function s(m) {
+            if (a.value = !1, m !== !0) return;
+            wl(u), r.value = !1;
             const f = Qt.indexOf(e.proxy);
             f !== -1 && Qt.splice(f, 1), i !== null && (Oi(i), i = null)
         }
         return t.onUnmounted(() => {
             s(!0)
         }), e.proxy.__qPortal = !0, Ze(e.proxy, "contentEl", () => n.value), {
             showPortal: d,
@@ -1716,30 +1716,30 @@
             portalIsActive: r,
             portalIsAccessible: a,
             renderPortal: () => c === !0 ? o() : r.value === !0 ? [t.h(t.Teleport, {
                 to: i
             }, o())] : void 0
         }
     }
-    const Ml = {
+    const Rl = {
         transitionShow: {
             type: String,
             default: "fade"
         },
         transitionHide: {
             type: String,
             default: "fade"
         },
         transitionDuration: {
             type: [String, Number],
             default: 300
         }
     };
 
-    function Rl(e, n = () => {}, o = () => {}) {
+    function Vl(e, n = () => {}, o = () => {}) {
         return {
             transitionProps: t.computed(() => {
                 const l = `q-transition--${e.transitionShow||n()}`,
                     r = `q-transition--${e.transitionHide||o()}`;
                 return {
                     appear: !0,
                     enterFromClass: `${l}-enter-from`,
@@ -1761,15 +1761,15 @@
         function o() {
             e = void 0
         }
         return t.onDeactivated(o), t.onBeforeUnmount(o), {
             removeTick: o,
             registerTick(l) {
                 e = l, t.nextTick(() => {
-                    e === l && (kl(n) === !1 && e(), e = void 0)
+                    e === l && (Cl(n) === !1 && e(), e = void 0)
                 })
             }
         }
     }
 
     function Xt() {
         let e = null;
@@ -1777,15 +1777,15 @@
 
         function o() {
             e !== null && (clearTimeout(e), e = null)
         }
         return t.onDeactivated(o), t.onBeforeUnmount(o), {
             removeTimeout: o,
             registerTimeout(l, r) {
-                o(), kl(n) === !1 && (e = setTimeout(l, r))
+                o(), Cl(n) === !1 && (e = setTimeout(l, r))
             }
         }
     }
     const Vi = [null, document, document.body, document.scrollingElement, document.documentElement];
 
     function ao(e, n) {
         let o = yi(n);
@@ -1800,39 +1800,39 @@
         return e === window ? window.pageYOffset || window.scrollY || document.body.scrollTop || 0 : e.scrollTop
     }
 
     function uo(e) {
         return e === window ? window.pageXOffset || window.scrollX || document.body.scrollLeft || 0 : e.scrollLeft
     }
 
-    function Vl(e, n, o = 0) {
+    function Il(e, n, o = 0) {
         const l = arguments[3] === void 0 ? performance.now() : arguments[3],
             r = io(e);
         if (o <= 0) {
             r !== n && so(e, n);
             return
         }
         requestAnimationFrame(a => {
             const i = a - l,
                 u = r + (n - r) / Math.max(i, o) * i;
-            so(e, u), u !== n && Vl(e, n, o - i, a)
+            so(e, u), u !== n && Il(e, n, o - i, a)
         })
     }
 
-    function Il(e, n, o = 0) {
+    function zl(e, n, o = 0) {
         const l = arguments[3] === void 0 ? performance.now() : arguments[3],
             r = uo(e);
         if (o <= 0) {
             r !== n && co(e, n);
             return
         }
         requestAnimationFrame(a => {
             const i = a - l,
                 u = r + (n - r) / Math.max(i, o) * i;
-            co(e, u), u !== n && Il(e, n, o - i, a)
+            co(e, u), u !== n && zl(e, n, o - i, a)
         })
     }
 
     function so(e, n) {
         if (e === window) {
             window.scrollTo(window.pageXOffset || window.scrollX || document.body.scrollLeft || 0, n);
             return
@@ -1844,25 +1844,25 @@
         if (e === window) {
             window.scrollTo(n, window.pageYOffset || window.scrollY || document.body.scrollTop || 0);
             return
         }
         e.scrollLeft = n
     }
 
-    function zl(e, n, o) {
+    function Ll(e, n, o) {
         if (o) {
-            Vl(e, n, o);
+            Il(e, n, o);
             return
         }
         so(e, n)
     }
 
     function fo(e, n, o) {
         if (o) {
-            Il(e, n, o);
+            zl(e, n, o);
             return
         }
         co(e, n)
     }
     let pn;
 
     function Ii() {
@@ -1901,39 +1901,39 @@
         Tt === !0 && (Tt = !1)
     }
 
     function Di(e) {
         Tt === !0 && (Tt = !1, ut(e, 27) === !0 && mt[mt.length - 1](e))
     }
 
-    function Ll(e) {
+    function Fl(e) {
         window[e]("keydown", Li), window[e]("blur", Fi), window[e]("keyup", Di), Tt = !1
     }
 
-    function Fl(e) {
-        he.is.desktop === !0 && (mt.push(e), mt.length === 1 && Ll("addEventListener"))
+    function Dl(e) {
+        he.is.desktop === !0 && (mt.push(e), mt.length === 1 && Fl("addEventListener"))
     }
 
     function bn(e) {
         const n = mt.indexOf(e);
-        n > -1 && (mt.splice(n, 1), mt.length === 0 && Ll("removeEventListener"))
+        n > -1 && (mt.splice(n, 1), mt.length === 0 && Fl("removeEventListener"))
     }
     const ht = [];
 
-    function Dl(e) {
+    function jl(e) {
         ht[ht.length - 1](e)
     }
 
-    function jl(e) {
-        he.is.desktop === !0 && (ht.push(e), ht.length === 1 && document.body.addEventListener("focusin", Dl))
+    function Nl(e) {
+        he.is.desktop === !0 && (ht.push(e), ht.length === 1 && document.body.addEventListener("focusin", jl))
     }
 
     function mo(e) {
         const n = ht.indexOf(e);
-        n > -1 && (ht.splice(n, 1), ht.length === 0 && document.body.removeEventListener("focusin", Dl))
+        n > -1 && (ht.splice(n, 1), ht.length === 0 && document.body.removeEventListener("focusin", jl))
     }
     const {
         notPassiveCapture: yn
     } = Se, vt = [];
 
     function wn(e) {
         const n = e.target;
@@ -1956,21 +1956,21 @@
         }
     }
 
     function ji(e) {
         vt.push(e), vt.length === 1 && (document.addEventListener("mousedown", wn, yn), document.addEventListener("touchstart", wn, yn))
     }
 
-    function Nl(e) {
+    function Hl(e) {
         const n = vt.findIndex(o => o === e);
         n > -1 && (vt.splice(n, 1), vt.length === 0 && (document.removeEventListener("mousedown", wn, yn), document.removeEventListener("touchstart", wn, yn)))
     }
-    let Hl, Ul;
+    let Ul, Wl;
 
-    function Wl(e) {
+    function Kl(e) {
         const n = e.split(" ");
         return n.length !== 2 ? !1 : ["top", "center", "bottom"].includes(n[0]) !== !0 ? (console.error("Anchor/Self position must start with one of top/center/bottom"), !1) : ["left", "middle", "right", "start", "end"].includes(n[1]) !== !0 ? (console.error("Anchor/Self position must end with one of left/middle/right/start/end"), !1) : !0
     }
 
     function Ni(e) {
         return e ? !(e.length !== 2 || typeof e[0] != "number" || typeof e[1] != "number") : !0
     }
@@ -1980,15 +1980,15 @@
         "end#ltr": "right",
         "end#rtl": "left"
     };
     ["left", "middle", "right"].forEach(e => {
         ho[`${e}#ltr`] = e, ho[`${e}#rtl`] = e
     });
 
-    function Kl(e, n) {
+    function Ql(e, n) {
         const o = e.split(" ");
         return {
             vertical: o[0],
             horizontal: ho[`${o[1]}#${n===!0?"rtl":"ltr"}`]
         }
     }
 
@@ -2037,106 +2037,106 @@
             bottom: n,
             left: 0,
             middle: e / 2,
             right: e
         }
     }
 
-    function Ql(e, n, o, l) {
+    function Gl(e, n, o, l) {
         return {
             top: e[o.vertical] - n[l.vertical],
             left: e[o.horizontal] - n[l.horizontal]
         }
     }
 
-    function Gl(e, n = 0) {
+    function Xl(e, n = 0) {
         if (e.targetEl === null || e.anchorEl === null || n > 5) return;
         if (e.targetEl.offsetHeight === 0 || e.targetEl.offsetWidth === 0) {
             setTimeout(() => {
-                Gl(e, n + 1)
+                Xl(e, n + 1)
             }, 10);
             return
         }
         const {
             targetEl: o,
             offset: l,
             anchorEl: r,
             anchorOrigin: a,
             selfOrigin: i,
             absoluteOffset: u,
             fit: c,
             cover: d,
             maxHeight: s,
-            maxWidth: h
+            maxWidth: m
         } = e;
         if (he.is.ios === !0 && window.visualViewport !== void 0) {
             const M = document.body.style,
                 {
                     offsetLeft: V,
                     offsetTop: R
                 } = window.visualViewport;
-            V !== Hl && (M.setProperty("--q-pe-left", V + "px"), Hl = V), R !== Ul && (M.setProperty("--q-pe-top", R + "px"), Ul = R)
+            V !== Ul && (M.setProperty("--q-pe-left", V + "px"), Ul = V), R !== Wl && (M.setProperty("--q-pe-top", R + "px"), Wl = R)
         }
         const {
             scrollLeft: f,
-            scrollTop: m
+            scrollTop: h
         } = o, v = u === void 0 ? Hi(r, d === !0 ? [0, 0] : l) : Ui(r, u, l);
         Object.assign(o.style, {
             top: 0,
             left: 0,
             minWidth: null,
             minHeight: null,
-            maxWidth: h || "100vw",
+            maxWidth: m || "100vw",
             maxHeight: s || "100vh",
             visibility: "visible"
         });
         const {
-            offsetWidth: x,
+            offsetWidth: _,
             offsetHeight: p
         } = o, {
-            elWidth: S,
-            elHeight: C
+            elWidth: k,
+            elHeight: q
         } = c === !0 || d === !0 ? {
-            elWidth: Math.max(v.width, x),
+            elWidth: Math.max(v.width, _),
             elHeight: d === !0 ? Math.max(v.height, p) : p
         } : {
-            elWidth: x,
+            elWidth: _,
             elHeight: p
         };
-        let y = {
-            maxWidth: h,
+        let w = {
+            maxWidth: m,
             maxHeight: s
         };
-        (c === !0 || d === !0) && (y.minWidth = v.width + "px", d === !0 && (y.minHeight = v.height + "px")), Object.assign(o.style, y);
-        const P = Wi(S, C);
-        let A = Ql(v, P, a, i);
-        if (u === void 0 || l === void 0) vo(A, v, P, a, i);
+        (c === !0 || d === !0) && (w.minWidth = v.width + "px", d === !0 && (w.minHeight = v.height + "px")), Object.assign(o.style, w);
+        const C = Wi(k, q);
+        let A = Gl(v, C, a, i);
+        if (u === void 0 || l === void 0) vo(A, v, C, a, i);
         else {
             const {
                 top: M,
                 left: V
             } = A;
-            vo(A, v, P, a, i);
+            vo(A, v, C, a, i);
             let R = !1;
             if (A.top !== M) {
                 R = !0;
-                const T = 2 * l[1];
-                v.center = v.top -= T, v.bottom -= T + 2
+                const B = 2 * l[1];
+                v.center = v.top -= B, v.bottom -= B + 2
             }
             if (A.left !== V) {
                 R = !0;
-                const T = 2 * l[0];
-                v.middle = v.left -= T, v.right -= T + 2
+                const B = 2 * l[0];
+                v.middle = v.left -= B, v.right -= B + 2
             }
-            R === !0 && (A = Ql(v, P, a, i), vo(A, v, P, a, i))
+            R === !0 && (A = Gl(v, C, a, i), vo(A, v, C, a, i))
         }
-        y = {
+        w = {
             top: A.top + "px",
             left: A.left + "px"
-        }, A.maxHeight !== void 0 && (y.maxHeight = A.maxHeight + "px", v.height > A.maxHeight && (y.minHeight = y.maxHeight)), A.maxWidth !== void 0 && (y.maxWidth = A.maxWidth + "px", v.width > A.maxWidth && (y.minWidth = y.maxWidth)), Object.assign(o.style, y), o.scrollTop !== m && (o.scrollTop = m), o.scrollLeft !== f && (o.scrollLeft = f)
+        }, A.maxHeight !== void 0 && (w.maxHeight = A.maxHeight + "px", v.height > A.maxHeight && (w.minHeight = w.maxHeight)), A.maxWidth !== void 0 && (w.maxWidth = A.maxWidth + "px", v.width > A.maxWidth && (w.minWidth = w.maxWidth)), Object.assign(o.style, w), o.scrollTop !== h && (o.scrollTop = h), o.scrollLeft !== f && (o.scrollLeft = f)
     }
 
     function vo(e, n, o, l, r) {
         const a = o.bottom,
             i = o.right,
             u = Ii(),
             c = window.innerHeight - u,
@@ -2157,31 +2157,31 @@
     const Ki = se({
         name: "QMenu",
         inheritAttrs: !1,
         props: {
             ...Ti,
             ...oo,
             ...Le,
-            ...Ml,
+            ...Rl,
             persistent: Boolean,
             autoClose: Boolean,
             separateClosePopup: Boolean,
             noRouteDismiss: Boolean,
             noRefocus: Boolean,
             noFocus: Boolean,
             fit: Boolean,
             cover: Boolean,
             square: Boolean,
             anchor: {
                 type: String,
-                validator: Wl
+                validator: Kl
             },
             self: {
                 type: String,
-                validator: Wl
+                validator: Kl
             },
             offset: {
                 type: Array,
                 validator: Ni
             },
             scrollTarget: {
                 default: void 0
@@ -2207,174 +2207,174 @@
             const c = t.getCurrentInstance(),
                 {
                     proxy: d
                 } = c,
                 {
                     $q: s
                 } = d,
-                h = t.ref(null),
+                m = t.ref(null),
                 f = t.ref(!1),
-                m = t.computed(() => e.persistent !== !0 && e.noRouteDismiss !== !0),
+                h = t.computed(() => e.persistent !== !0 && e.noRouteDismiss !== !0),
                 v = Fe(e, s),
                 {
-                    registerTick: x,
+                    registerTick: _,
                     removeTick: p
                 } = Gt(),
                 {
-                    registerTimeout: S
+                    registerTimeout: k
                 } = Xt(),
                 {
-                    transitionProps: C,
-                    transitionStyle: y
-                } = Rl(e),
+                    transitionProps: q,
+                    transitionStyle: w
+                } = Vl(e),
                 {
-                    localScrollTarget: P,
+                    localScrollTarget: C,
                     changeScrollEvent: A,
                     unconfigureScrollTarget: M
                 } = Pi(e, H),
                 {
                     anchorEl: V,
                     canShow: R
                 } = Bi({
                     showing: f
                 }),
                 {
-                    hide: T
+                    hide: B
                 } = ro({
                     showing: f,
                     canShow: R,
                     handleShow: J,
-                    handleHide: _,
-                    hideOnRouteChange: m,
+                    handleHide: S,
+                    hideOnRouteChange: h,
                     processOnMount: !0
                 }),
                 {
-                    showPortal: B,
+                    showPortal: P,
                     hidePortal: I,
-                    renderPortal: k
-                } = Ol(c, h, ue, "menu"),
+                    renderPortal: x
+                } = Ml(c, m, ue, "menu"),
                 O = {
                     anchorEl: V,
-                    innerRef: h,
+                    innerRef: m,
                     onClickOutside(D) {
-                        if (e.persistent !== !0 && f.value === !0) return T(D), (D.type === "touchstart" || D.target.classList.contains("q-dialog__backdrop")) && ve(D), !0
+                        if (e.persistent !== !0 && f.value === !0) return B(D), (D.type === "touchstart" || D.target.classList.contains("q-dialog__backdrop")) && ve(D), !0
                     }
                 },
-                q = t.computed(() => Kl(e.anchor || (e.cover === !0 ? "center middle" : "bottom start"), s.lang.rtl)),
-                j = t.computed(() => e.cover === !0 ? q.value : Kl(e.self || "top start", s.lang.rtl)),
+                T = t.computed(() => Ql(e.anchor || (e.cover === !0 ? "center middle" : "bottom start"), s.lang.rtl)),
+                j = t.computed(() => e.cover === !0 ? T.value : Ql(e.self || "top start", s.lang.rtl)),
                 N = t.computed(() => (e.square === !0 ? " q-menu--square" : "") + (v.value === !0 ? " q-menu--dark q-dark" : "")),
-                w = t.computed(() => e.autoClose === !0 ? {
+                y = t.computed(() => e.autoClose === !0 ? {
                     onClick: te
                 } : {}),
                 z = t.computed(() => f.value === !0 && e.persistent !== !0);
             t.watch(z, D => {
-                D === !0 ? (Fl(F), ji(O)) : (bn(F), Nl(O))
+                D === !0 ? (Dl(F), ji(O)) : (bn(F), Hl(O))
             });
 
             function G() {
                 hn(() => {
-                    let D = h.value;
+                    let D = m.value;
                     D && D.contains(document.activeElement) !== !0 && (D = D.querySelector("[autofocus][tabindex], [data-autofocus][tabindex]") || D.querySelector("[autofocus] [tabindex], [data-autofocus] [tabindex]") || D.querySelector("[autofocus], [data-autofocus]") || D, D.focus({
                         preventScroll: !0
                     }))
                 })
             }
 
             function J(D) {
-                if (r = e.noRefocus === !1 ? document.activeElement : null, jl(U), B(), H(), a = void 0, D !== void 0 && (e.touchPosition || e.contextMenu)) {
+                if (r = e.noRefocus === !1 ? document.activeElement : null, Nl(U), P(), H(), a = void 0, D !== void 0 && (e.touchPosition || e.contextMenu)) {
                     const fe = dt(D);
                     if (fe.left !== void 0) {
                         const {
                             top: ke,
                             left: Ie
                         } = V.value.getBoundingClientRect();
                         a = {
                             left: fe.left - Ie,
                             top: fe.top - ke
                         }
                     }
                 }
-                i === void 0 && (i = t.watch(() => s.screen.width + "|" + s.screen.height + "|" + e.self + "|" + e.anchor + "|" + s.lang.rtl, Z)), e.noFocus !== !0 && document.activeElement.blur(), x(() => {
+                i === void 0 && (i = t.watch(() => s.screen.width + "|" + s.screen.height + "|" + e.self + "|" + e.anchor + "|" + s.lang.rtl, Z)), e.noFocus !== !0 && document.activeElement.blur(), _(() => {
                     Z(), e.noFocus !== !0 && G()
-                }), S(() => {
-                    s.platform.is.ios === !0 && (u = e.autoClose, h.value.click()), Z(), B(!0), o("show", D)
+                }), k(() => {
+                    s.platform.is.ios === !0 && (u = e.autoClose, m.value.click()), Z(), P(!0), o("show", D)
                 }, e.transitionDuration)
             }
 
-            function _(D) {
-                p(), I(), b(!0), r !== null && (D === void 0 || D.qClickOutside !== !0) && (((D && D.type.indexOf("key") === 0 ? r.closest('[tabindex]:not([tabindex^="-"])') : void 0) || r).focus(), r = null), S(() => {
+            function S(D) {
+                p(), I(), b(!0), r !== null && (D === void 0 || D.qClickOutside !== !0) && (((D && D.type.indexOf("key") === 0 ? r.closest('[tabindex]:not([tabindex^="-"])') : void 0) || r).focus(), r = null), k(() => {
                     I(!0), o("hide", D)
                 }, e.transitionDuration)
             }
 
             function b(D) {
-                a = void 0, i !== void 0 && (i(), i = void 0), (D === !0 || f.value === !0) && (mo(U), M(), Nl(O), bn(F)), D !== !0 && (r = null)
+                a = void 0, i !== void 0 && (i(), i = void 0), (D === !0 || f.value === !0) && (mo(U), M(), Hl(O), bn(F)), D !== !0 && (r = null)
             }
 
             function H() {
-                (V.value !== null || e.scrollTarget !== void 0) && (P.value = ao(V.value, e.scrollTarget), A(P.value, Z))
+                (V.value !== null || e.scrollTarget !== void 0) && (C.value = ao(V.value, e.scrollTarget), A(C.value, Z))
             }
 
             function te(D) {
                 u !== !0 ? (Mi(d, D), o("click", D)) : u = !1
             }
 
             function U(D) {
-                z.value === !0 && e.noFocus !== !0 && wl(h.value, D.target) !== !0 && G()
+                z.value === !0 && e.noFocus !== !0 && Sl(m.value, D.target) !== !0 && G()
             }
 
             function F(D) {
-                o("escapeKey"), T(D)
+                o("escapeKey"), B(D)
             }
 
             function Z() {
-                Gl({
-                    targetEl: h.value,
+                Xl({
+                    targetEl: m.value,
                     offset: e.offset,
                     anchorEl: V.value,
-                    anchorOrigin: q.value,
+                    anchorOrigin: T.value,
                     selfOrigin: j.value,
                     absoluteOffset: a,
                     fit: e.fit,
                     cover: e.cover,
                     maxHeight: e.maxHeight,
                     maxWidth: e.maxWidth
                 })
             }
 
             function ue() {
-                return t.h(t.Transition, C.value, () => f.value === !0 ? t.h("div", {
+                return t.h(t.Transition, q.value, () => f.value === !0 ? t.h("div", {
                     role: "menu",
                     ...l,
-                    ref: h,
+                    ref: m,
                     tabindex: -1,
                     class: ["q-menu q-position-engine scroll" + N.value, l.class],
-                    style: [l.style, y.value],
-                    ...w.value
+                    style: [l.style, w.value],
+                    ...y.value
                 }, we(n.default)) : null)
             }
             return t.onBeforeUnmount(b), Object.assign(d, {
                 focus: G,
                 updatePosition: Z
-            }), k
+            }), x
         }
     });
 
-    function Xl(e, n, o) {
+    function Yl(e, n, o) {
         function l() {}
         return t.onBeforeUnmount(() => {
             e.value === !0 && void 0
         }), {
             removeFromHistory: l,
             addToHistory() {}
         }
     }
     let Yt = 0,
         go, po, Zt, bo = !1,
-        Yl, Zl, Jl, gt = null;
+        Zl, Jl, er, gt = null;
 
     function Qi(e) {
         Gi(e) && ve(e)
     }
 
     function Gi(e) {
         if (e.target === document.body || e.target.classList.contains("q-layout__backdrop")) return !0;
@@ -2385,15 +2385,15 @@
         for (let a = 0; a < n.length; a++) {
             const i = n[a];
             if (zi(i, l)) return l ? r < 0 && i.scrollTop === 0 ? !0 : r > 0 && i.scrollTop + i.clientHeight === i.scrollHeight : r < 0 && i.scrollLeft === 0 ? !0 : r > 0 && i.scrollLeft + i.clientWidth === i.scrollWidth
         }
         return !0
     }
 
-    function er(e) {
+    function tr(e) {
         e.target === document && (document.scrollingElement.scrollTop = document.scrollingElement.scrollTop)
     }
 
     function Sn(e) {
         bo !== !0 && (bo = !0, requestAnimationFrame(() => {
             bo = !1;
             const {
@@ -2402,48 +2402,48 @@
                 clientHeight: o,
                 scrollTop: l
             } = document.scrollingElement;
             (Zt === void 0 || n !== window.innerHeight) && (Zt = o - n, document.scrollingElement.scrollTop = l), l > Zt && (document.scrollingElement.scrollTop -= Math.ceil((l - Zt) / 8))
         }))
     }
 
-    function tr(e) {
+    function nr(e) {
         const n = document.body,
             o = window.visualViewport !== void 0;
         if (e === "add") {
             const {
                 overflowY: l,
                 overflowX: r
             } = window.getComputedStyle(n);
-            go = uo(window), po = io(window), Yl = n.style.left, Zl = n.style.top, Jl = window.location.href, n.style.left = `-${go}px`, n.style.top = `-${po}px`, r !== "hidden" && (r === "scroll" || n.scrollWidth > window.innerWidth) && n.classList.add("q-body--force-scrollbar-x"), l !== "hidden" && (l === "scroll" || n.scrollHeight > window.innerHeight) && n.classList.add("q-body--force-scrollbar-y"), n.classList.add("q-body--prevent-scroll"), document.qScrollPrevented = !0, he.is.ios === !0 && (o === !0 ? (window.scrollTo(0, 0), window.visualViewport.addEventListener("resize", Sn, Se.passiveCapture), window.visualViewport.addEventListener("scroll", Sn, Se.passiveCapture), window.scrollTo(0, 0)) : window.addEventListener("scroll", er, Se.passiveCapture))
+            go = uo(window), po = io(window), Zl = n.style.left, Jl = n.style.top, er = window.location.href, n.style.left = `-${go}px`, n.style.top = `-${po}px`, r !== "hidden" && (r === "scroll" || n.scrollWidth > window.innerWidth) && n.classList.add("q-body--force-scrollbar-x"), l !== "hidden" && (l === "scroll" || n.scrollHeight > window.innerHeight) && n.classList.add("q-body--force-scrollbar-y"), n.classList.add("q-body--prevent-scroll"), document.qScrollPrevented = !0, he.is.ios === !0 && (o === !0 ? (window.scrollTo(0, 0), window.visualViewport.addEventListener("resize", Sn, Se.passiveCapture), window.visualViewport.addEventListener("scroll", Sn, Se.passiveCapture), window.scrollTo(0, 0)) : window.addEventListener("scroll", tr, Se.passiveCapture))
         }
-        he.is.desktop === !0 && he.is.mac === !0 && window[`${e}EventListener`]("wheel", Qi, Se.notPassive), e === "remove" && (he.is.ios === !0 && (o === !0 ? (window.visualViewport.removeEventListener("resize", Sn, Se.passiveCapture), window.visualViewport.removeEventListener("scroll", Sn, Se.passiveCapture)) : window.removeEventListener("scroll", er, Se.passiveCapture)), n.classList.remove("q-body--prevent-scroll"), n.classList.remove("q-body--force-scrollbar-x"), n.classList.remove("q-body--force-scrollbar-y"), document.qScrollPrevented = !1, n.style.left = Yl, n.style.top = Zl, window.location.href === Jl && window.scrollTo(go, po), Zt = void 0)
+        he.is.desktop === !0 && he.is.mac === !0 && window[`${e}EventListener`]("wheel", Qi, Se.notPassive), e === "remove" && (he.is.ios === !0 && (o === !0 ? (window.visualViewport.removeEventListener("resize", Sn, Se.passiveCapture), window.visualViewport.removeEventListener("scroll", Sn, Se.passiveCapture)) : window.removeEventListener("scroll", tr, Se.passiveCapture)), n.classList.remove("q-body--prevent-scroll"), n.classList.remove("q-body--force-scrollbar-x"), n.classList.remove("q-body--force-scrollbar-y"), document.qScrollPrevented = !1, n.style.left = Zl, n.style.top = Jl, window.location.href === er && window.scrollTo(go, po), Zt = void 0)
     }
 
     function Xi(e) {
         let n = "add";
         if (e === !0) {
             if (Yt++, gt !== null) {
                 clearTimeout(gt), gt = null;
                 return
             }
             if (Yt > 1) return
         } else {
             if (Yt === 0 || (Yt--, Yt > 0)) return;
             if (n = "remove", he.is.ios === !0 && he.is.nativeMobile === !0) {
                 gt !== null && clearTimeout(gt), gt = setTimeout(() => {
-                    tr(n), gt = null
+                    nr(n), gt = null
                 }, 100);
                 return
             }
         }
-        tr(n)
+        nr(n)
     }
 
-    function nr() {
+    function or() {
         let e;
         return {
             preventBodyScroll(n) {
                 n !== e && (e !== void 0 || n === !0) && (e = n, Xi(n))
             }
         }
     }
@@ -2451,27 +2451,27 @@
     const Yi = {
             standard: "fixed-full flex-center",
             top: "fixed-top justify-center",
             bottom: "fixed-bottom justify-center",
             right: "fixed-right items-center",
             left: "fixed-left items-center"
         },
-        or = {
+        lr = {
             standard: ["scale", "scale"],
             top: ["slide-down", "slide-up"],
             bottom: ["slide-up", "slide-down"],
             right: ["slide-left", "slide-right"],
             left: ["slide-right", "slide-left"]
         },
         Zi = se({
             name: "QDialog",
             inheritAttrs: !1,
             props: {
                 ...oo,
-                ...Ml,
+                ...Rl,
                 transitionShow: String,
                 transitionHide: String,
                 persistent: Boolean,
                 autoClose: Boolean,
                 allowFocusOutside: Boolean,
                 noEscDismiss: Boolean,
                 noBackdropDismiss: Boolean,
@@ -2498,130 +2498,130 @@
             }) {
                 const r = t.getCurrentInstance(),
                     a = t.ref(null),
                     i = t.ref(!1),
                     u = t.ref(!1);
                 let c = null,
                     d = null,
-                    s, h;
+                    s, m;
                 const f = t.computed(() => e.persistent !== !0 && e.noRouteDismiss !== !0 && e.seamless !== !0),
                     {
-                        preventBodyScroll: m
-                    } = nr(),
+                        preventBodyScroll: h
+                    } = or(),
                     {
                         registerTimeout: v
                     } = Xt(),
                     {
-                        registerTick: x,
+                        registerTick: _,
                         removeTick: p
                     } = Gt(),
                     {
-                        transitionProps: S,
-                        transitionStyle: C
-                    } = Rl(e, () => or[e.position][0], () => or[e.position][1]),
+                        transitionProps: k,
+                        transitionStyle: q
+                    } = Vl(e, () => lr[e.position][0], () => lr[e.position][1]),
                     {
-                        showPortal: y,
-                        hidePortal: P,
+                        showPortal: w,
+                        hidePortal: C,
                         portalIsAccessible: A,
                         renderPortal: M
-                    } = Ol(r, a, te, "dialog"),
+                    } = Ml(r, a, te, "dialog"),
                     {
                         hide: V
                     } = ro({
                         showing: i,
                         hideOnRouteChange: f,
-                        handleShow: q,
+                        handleShow: T,
                         handleHide: j,
                         processOnMount: !0
                     }),
                     {
                         addToHistory: R,
-                        removeFromHistory: T
-                    } = Xl(i),
-                    B = t.computed(() => `q-dialog__inner flex no-pointer-events q-dialog__inner--${e.maximized===!0?"maximized":"minimized"} q-dialog__inner--${e.position} ${Yi[e.position]}` + (u.value === !0 ? " q-dialog__inner--animating" : "") + (e.fullWidth === !0 ? " q-dialog__inner--fullwidth" : "") + (e.fullHeight === !0 ? " q-dialog__inner--fullheight" : "") + (e.square === !0 ? " q-dialog__inner--square" : "")),
+                        removeFromHistory: B
+                    } = Yl(i),
+                    P = t.computed(() => `q-dialog__inner flex no-pointer-events q-dialog__inner--${e.maximized===!0?"maximized":"minimized"} q-dialog__inner--${e.position} ${Yi[e.position]}` + (u.value === !0 ? " q-dialog__inner--animating" : "") + (e.fullWidth === !0 ? " q-dialog__inner--fullwidth" : "") + (e.fullHeight === !0 ? " q-dialog__inner--fullheight" : "") + (e.square === !0 ? " q-dialog__inner--square" : "")),
                     I = t.computed(() => i.value === !0 && e.seamless !== !0),
-                    k = t.computed(() => e.autoClose === !0 ? {
-                        onClick: _
+                    x = t.computed(() => e.autoClose === !0 ? {
+                        onClick: S
                     } : {}),
                     O = t.computed(() => [`q-dialog fullscreen no-pointer-events q-dialog--${I.value===!0?"modal":"seamless"}`, l.class]);
                 t.watch(() => e.maximized, U => {
                     i.value === !0 && J(U)
                 }), t.watch(I, U => {
-                    m(U), U === !0 ? (jl(H), Fl(z)) : (mo(H), bn(z))
+                    h(U), U === !0 ? (Nl(H), Dl(z)) : (mo(H), bn(z))
                 });
 
-                function q(U) {
-                    R(), d = e.noRefocus === !1 && document.activeElement !== null ? document.activeElement : null, J(e.maximized), y(), u.value = !0, e.noFocus !== !0 ? (document.activeElement !== null && document.activeElement.blur(), x(N)) : p(), v(() => {
+                function T(U) {
+                    R(), d = e.noRefocus === !1 && document.activeElement !== null ? document.activeElement : null, J(e.maximized), w(), u.value = !0, e.noFocus !== !0 ? (document.activeElement !== null && document.activeElement.blur(), _(N)) : p(), v(() => {
                         if (r.proxy.$q.platform.is.ios === !0) {
                             if (e.seamless !== !0 && document.activeElement) {
                                 const {
                                     top: F,
                                     bottom: Z
                                 } = document.activeElement.getBoundingClientRect(), {
                                     innerHeight: ue
                                 } = window, D = window.visualViewport !== void 0 ? window.visualViewport.height : ue;
                                 F > 0 && Z > D / 2 && (document.scrollingElement.scrollTop = Math.min(document.scrollingElement.scrollHeight - D, Z >= ue ? 1 / 0 : Math.ceil(document.scrollingElement.scrollTop + Z - D / 2))), document.activeElement.scrollIntoView()
                             }
-                            h = !0, a.value.click(), h = !1
+                            m = !0, a.value.click(), m = !1
                         }
-                        y(!0), u.value = !1, o("show", U)
+                        w(!0), u.value = !1, o("show", U)
                     }, e.transitionDuration)
                 }
 
                 function j(U) {
-                    p(), T(), G(!0), u.value = !0, P(), d !== null && (((U && U.type.indexOf("key") === 0 ? d.closest('[tabindex]:not([tabindex^="-"])') : void 0) || d).focus(), d = null), v(() => {
-                        P(!0), u.value = !1, o("hide", U)
+                    p(), B(), G(!0), u.value = !0, C(), d !== null && (((U && U.type.indexOf("key") === 0 ? d.closest('[tabindex]:not([tabindex^="-"])') : void 0) || d).focus(), d = null), v(() => {
+                        C(!0), u.value = !1, o("hide", U)
                     }, e.transitionDuration)
                 }
 
                 function N(U) {
                     hn(() => {
                         let F = a.value;
                         F === null || F.contains(document.activeElement) === !0 || (F = (U !== "" ? F.querySelector(U) : null) || F.querySelector("[autofocus][tabindex], [data-autofocus][tabindex]") || F.querySelector("[autofocus] [tabindex], [data-autofocus] [tabindex]") || F.querySelector("[autofocus], [data-autofocus]") || F, F.focus({
                             preventScroll: !0
                         }))
                     })
                 }
 
-                function w(U) {
+                function y(U) {
                     U && typeof U.focus == "function" ? U.focus({
                         preventScroll: !0
                     }) : N(), o("shake");
                     const F = a.value;
                     F !== null && (F.classList.remove("q-animate--scale"), F.classList.add("q-animate--scale"), c !== null && clearTimeout(c), c = setTimeout(() => {
                         c = null, a.value !== null && (F.classList.remove("q-animate--scale"), N())
                     }, 170))
                 }
 
                 function z() {
-                    e.seamless !== !0 && (e.persistent === !0 || e.noEscDismiss === !0 ? e.maximized !== !0 && e.noShake !== !0 && w() : (o("escapeKey"), V()))
+                    e.seamless !== !0 && (e.persistent === !0 || e.noEscDismiss === !0 ? e.maximized !== !0 && e.noShake !== !0 && y() : (o("escapeKey"), V()))
                 }
 
                 function G(U) {
-                    c !== null && (clearTimeout(c), c = null), (U === !0 || i.value === !0) && (J(!1), e.seamless !== !0 && (m(!1), mo(H), bn(z))), U !== !0 && (d = null)
+                    c !== null && (clearTimeout(c), c = null), (U === !0 || i.value === !0) && (J(!1), e.seamless !== !0 && (h(!1), mo(H), bn(z))), U !== !0 && (d = null)
                 }
 
                 function J(U) {
                     U === !0 ? s !== !0 && (_n < 1 && document.body.classList.add("q-body--dialog"), _n++, s = !0) : s === !0 && (_n < 2 && document.body.classList.remove("q-body--dialog"), _n--, s = !1)
                 }
 
-                function _(U) {
-                    h !== !0 && (V(U), o("click", U))
+                function S(U) {
+                    m !== !0 && (V(U), o("click", U))
                 }
 
                 function b(U) {
-                    e.persistent !== !0 && e.noBackdropDismiss !== !0 ? V(U) : e.noShake !== !0 && w()
+                    e.persistent !== !0 && e.noBackdropDismiss !== !0 ? V(U) : e.noShake !== !0 && y()
                 }
 
                 function H(U) {
-                    e.allowFocusOutside !== !0 && A.value === !0 && wl(a.value, U.target) !== !0 && N('[tabindex]:not([tabindex="-1"])')
+                    e.allowFocusOutside !== !0 && A.value === !0 && Sl(a.value, U.target) !== !0 && N('[tabindex]:not([tabindex="-1"])')
                 }
                 Object.assign(r.proxy, {
                     focus: N,
-                    shake: w,
+                    shake: y,
                     __updateRefocusTarget(U) {
                         d = U || null
                     }
                 }), t.onBeforeUnmount(G);
 
                 function te() {
                     return t.h("div", {
@@ -2630,24 +2630,24 @@
                         ...l,
                         class: O.value
                     }, [t.h(t.Transition, {
                         name: "q-transition--fade",
                         appear: !0
                     }, () => I.value === !0 ? t.h("div", {
                         class: "q-dialog__backdrop fixed-full",
-                        style: C.value,
+                        style: q.value,
                         "aria-hidden": "true",
                         tabindex: -1,
                         onClick: b
-                    }) : null), t.h(t.Transition, S.value, () => i.value === !0 ? t.h("div", {
+                    }) : null), t.h(t.Transition, k.value, () => i.value === !0 ? t.h("div", {
                         ref: a,
-                        class: B.value,
-                        style: C.value,
+                        class: P.value,
+                        style: q.value,
                         tabindex: -1,
-                        ...k.value
+                        ...x.value
                     }, we(n.default)) : null)])
                 }
                 return M
             }
         });
     let Jt = !1;
     {
@@ -2661,21 +2661,21 @@
         Object.assign(n.style, {
             width: "1000px",
             height: "1px"
         }), document.body.appendChild(e), e.appendChild(n), e.scrollLeft = -1e3, Jt = e.scrollLeft >= 0, e.remove()
     }
     const Ge = 1e3,
         Ji = ["start", "center", "end", "start-force", "center-force", "end-force"],
-        lr = Array.prototype.filter,
+        rr = Array.prototype.filter,
         eu = window.getComputedStyle(document.body).overflowAnchor === void 0 ? Ut : function(e, n) {
             e !== null && (e._qOverflowAnimationFrame !== void 0 && cancelAnimationFrame(e._qOverflowAnimationFrame), e._qOverflowAnimationFrame = requestAnimationFrame(() => {
                 if (e === null) return;
                 e._qOverflowAnimationFrame = void 0;
                 const o = e.children || [];
-                lr.call(o, r => r.dataset && r.dataset.qVsAnchor !== void 0).forEach(r => {
+                rr.call(o, r => r.dataset && r.dataset.qVsAnchor !== void 0).forEach(r => {
                     delete r.dataset.qVsAnchor
                 });
                 const l = o[n];
                 l && l.dataset && (l.dataset.qVsAnchor = "")
             }))
         };
 
@@ -2690,38 +2690,38 @@
                 scrollStart: 0,
                 scrollViewSize: -i - u,
                 scrollMaxSize: 0,
                 offsetStart: -i,
                 offsetEnd: -u
             };
         if (r === !0 ? (e === window ? (s.scrollStart = window.pageXOffset || window.scrollX || document.body.scrollLeft || 0, s.scrollViewSize += document.documentElement.clientWidth) : (s.scrollStart = c.scrollLeft, s.scrollViewSize += c.clientWidth), s.scrollMaxSize = c.scrollWidth, a === !0 && (s.scrollStart = (Jt === !0 ? s.scrollMaxSize - s.scrollViewSize : 0) - s.scrollStart)) : (e === window ? (s.scrollStart = window.pageYOffset || window.scrollY || document.body.scrollTop || 0, s.scrollViewSize += document.documentElement.clientHeight) : (s.scrollStart = c.scrollTop, s.scrollViewSize += c.clientHeight), s.scrollMaxSize = c.scrollHeight), o !== null)
-            for (let h = o.previousElementSibling; h !== null; h = h.previousElementSibling) h.classList.contains("q-virtual-scroll--skip") === !1 && (s.offsetStart += h[d]);
+            for (let m = o.previousElementSibling; m !== null; m = m.previousElementSibling) m.classList.contains("q-virtual-scroll--skip") === !1 && (s.offsetStart += m[d]);
         if (l !== null)
-            for (let h = l.nextElementSibling; h !== null; h = h.nextElementSibling) h.classList.contains("q-virtual-scroll--skip") === !1 && (s.offsetEnd += h[d]);
+            for (let m = l.nextElementSibling; m !== null; m = m.nextElementSibling) m.classList.contains("q-virtual-scroll--skip") === !1 && (s.offsetEnd += m[d]);
         if (n !== e) {
-            const h = c.getBoundingClientRect(),
+            const m = c.getBoundingClientRect(),
                 f = n.getBoundingClientRect();
-            r === !0 ? (s.offsetStart += f.left - h.left, s.offsetEnd -= f.width) : (s.offsetStart += f.top - h.top, s.offsetEnd -= f.height), e !== window && (s.offsetStart += s.scrollStart), s.offsetEnd += s.scrollMaxSize - s.offsetStart
+            r === !0 ? (s.offsetStart += f.left - m.left, s.offsetEnd -= f.width) : (s.offsetStart += f.top - m.top, s.offsetEnd -= f.height), e !== window && (s.offsetStart += s.scrollStart), s.offsetEnd += s.scrollMaxSize - s.offsetStart
         }
         return s
     }
 
-    function rr(e, n, o, l) {
+    function ar(e, n, o, l) {
         n === "end" && (n = (e === window ? document.body : e)[o === !0 ? "scrollWidth" : "scrollHeight"]), e === window ? o === !0 ? (l === !0 && (n = (Jt === !0 ? document.body.scrollWidth - document.documentElement.clientWidth : 0) - n), window.scrollTo(n, window.pageYOffset || window.scrollY || document.body.scrollTop || 0)) : window.scrollTo(window.pageXOffset || window.scrollX || document.body.scrollLeft || 0, n) : o === !0 ? (l === !0 && (n = (Jt === !0 ? e.scrollWidth - e.offsetWidth : 0) - n), e.scrollLeft = n) : e.scrollTop = n
     }
 
     function en(e, n, o, l) {
         if (o >= l) return 0;
         const r = n.length,
             a = Math.floor(o / Ge),
             i = Math.floor((l - 1) / Ge) + 1;
         let u = e.slice(a, i).reduce(Bt, 0);
         return o % Ge !== 0 && (u -= n.slice(a * Ge, o).reduce(Bt, 0)), l % Ge !== 0 && l !== r && (u -= n.slice(l, i * Ge).reduce(Bt, 0)), u
     }
-    const ar = {
+    const ir = {
             virtualScrollSliceSize: {
                 type: [Number, String],
                 default: null
             },
             virtualScrollSliceRatioBefore: {
                 type: [Number, String],
                 default: 1
@@ -2740,45 +2740,45 @@
             },
             virtualScrollStickySizeEnd: {
                 type: [Number, String],
                 default: 0
             },
             tableColspan: [Number, String]
         },
-        ir = Object.keys(ar),
-        ur = {
+        ur = Object.keys(ir),
+        sr = {
             virtualScrollHorizontal: Boolean,
             onVirtualScroll: Function,
-            ...ar
+            ...ir
         };
 
-    function sr({
+    function cr({
         virtualScrollLength: e,
         getVirtualScrollTarget: n,
         getVirtualScrollEl: o,
         virtualScrollItemSizeComputed: l
     }) {
         const r = t.getCurrentInstance(),
             {
                 props: a,
                 emit: i,
                 proxy: u
             } = r,
             {
                 $q: c
             } = u;
-        let d, s, h, f = [],
-            m;
+        let d, s, m, f = [],
+            h;
         const v = t.ref(0),
-            x = t.ref(0),
+            _ = t.ref(0),
             p = t.ref({}),
-            S = t.ref(null),
-            C = t.ref(null),
-            y = t.ref(null),
-            P = t.ref({
+            k = t.ref(null),
+            q = t.ref(null),
+            w = t.ref(null),
+            C = t.ref({
                 from: 0,
                 to: 0
             }),
             A = t.computed(() => a.tableColspan !== void 0 ? a.tableColspan : 100);
         l === void 0 && (l = t.computed(() => a.virtualScrollItemSize));
         const M = t.computed(() => l.value + ";" + a.virtualScrollHorizontal),
             V = t.computed(() => M.value + ";" + a.virtualScrollSliceRatioBefore + ";" + a.virtualScrollSliceRatioAfter);
@@ -2786,243 +2786,243 @@
             N()
         }), t.watch(M, R);
 
         function R() {
             j(s, !0)
         }
 
-        function T(_) {
-            j(_ === void 0 ? s : _)
+        function B(S) {
+            j(S === void 0 ? s : S)
         }
 
-        function B(_, b) {
+        function P(S, b) {
             const H = n();
             if (H == null || H.nodeType === 8) return;
-            const te = yo(H, o(), S.value, C.value, a.virtualScrollHorizontal, c.lang.rtl, a.virtualScrollStickySizeStart, a.virtualScrollStickySizeEnd);
-            h !== te.scrollViewSize && N(te.scrollViewSize), k(H, te, Math.min(e.value - 1, Math.max(0, parseInt(_, 10) || 0)), 0, Ji.indexOf(b) > -1 ? b : s > -1 && _ > s ? "end" : "start")
+            const te = yo(H, o(), k.value, q.value, a.virtualScrollHorizontal, c.lang.rtl, a.virtualScrollStickySizeStart, a.virtualScrollStickySizeEnd);
+            m !== te.scrollViewSize && N(te.scrollViewSize), x(H, te, Math.min(e.value - 1, Math.max(0, parseInt(S, 10) || 0)), 0, Ji.indexOf(b) > -1 ? b : s > -1 && S > s ? "end" : "start")
         }
 
         function I() {
-            const _ = n();
-            if (_ == null || _.nodeType === 8) return;
-            const b = yo(_, o(), S.value, C.value, a.virtualScrollHorizontal, c.lang.rtl, a.virtualScrollStickySizeStart, a.virtualScrollStickySizeEnd),
+            const S = n();
+            if (S == null || S.nodeType === 8) return;
+            const b = yo(S, o(), k.value, q.value, a.virtualScrollHorizontal, c.lang.rtl, a.virtualScrollStickySizeStart, a.virtualScrollStickySizeEnd),
                 H = e.value - 1,
-                te = b.scrollMaxSize - b.offsetStart - b.offsetEnd - x.value;
+                te = b.scrollMaxSize - b.offsetStart - b.offsetEnd - _.value;
             if (d === b.scrollStart) return;
             if (b.scrollMaxSize <= 0) {
-                k(_, b, 0, 0);
+                x(S, b, 0, 0);
                 return
             }
-            h !== b.scrollViewSize && N(b.scrollViewSize), O(P.value.from);
-            const U = Math.floor(b.scrollMaxSize - Math.max(b.scrollViewSize, b.offsetEnd) - Math.min(m[H], b.scrollViewSize / 2));
+            m !== b.scrollViewSize && N(b.scrollViewSize), O(C.value.from);
+            const U = Math.floor(b.scrollMaxSize - Math.max(b.scrollViewSize, b.offsetEnd) - Math.min(h[H], b.scrollViewSize / 2));
             if (U > 0 && Math.ceil(b.scrollStart) >= U) {
-                k(_, b, H, b.scrollMaxSize - b.offsetEnd - f.reduce(Bt, 0));
+                x(S, b, H, b.scrollMaxSize - b.offsetEnd - f.reduce(Bt, 0));
                 return
             }
             let F = 0,
                 Z = b.scrollStart - b.offsetStart,
                 ue = Z;
-            if (Z <= te && Z + b.scrollViewSize >= v.value) Z -= v.value, F = P.value.from, ue = Z;
+            if (Z <= te && Z + b.scrollViewSize >= v.value) Z -= v.value, F = C.value.from, ue = Z;
             else
                 for (let D = 0; Z >= f[D] && F < H; D++) Z -= f[D], F += Ge;
-            for (; Z > 0 && F < H;) Z -= m[F], Z > -b.scrollViewSize ? (F++, ue = Z) : ue = m[F] + Z;
-            k(_, b, F, ue)
+            for (; Z > 0 && F < H;) Z -= h[F], Z > -b.scrollViewSize ? (F++, ue = Z) : ue = h[F] + Z;
+            x(S, b, F, ue)
         }
 
-        function k(_, b, H, te, U) {
+        function x(S, b, H, te, U) {
             const F = typeof U == "string" && U.indexOf("-force") > -1,
                 Z = F === !0 ? U.replace("-force", "") : U,
                 ue = Z !== void 0 ? Z : "start";
             let D = Math.max(0, H - p.value[ue]),
                 fe = D + p.value.total;
             fe > e.value && (fe = e.value, D = Math.max(0, fe - p.value.total)), d = b.scrollStart;
-            const ke = D !== P.value.from || fe !== P.value.to;
+            const ke = D !== C.value.from || fe !== C.value.to;
             if (ke === !1 && Z === void 0) {
                 z(H);
                 return
             }
             const {
                 activeElement: Ie
-            } = document, ce = y.value;
-            ke === !0 && ce !== null && ce !== Ie && ce.contains(Ie) === !0 && (ce.addEventListener("focusout", q), setTimeout(() => {
-                ce !== null && ce.removeEventListener("focusout", q)
+            } = document, ce = w.value;
+            ke === !0 && ce !== null && ce !== Ie && ce.contains(Ie) === !0 && (ce.addEventListener("focusout", T), setTimeout(() => {
+                ce !== null && ce.removeEventListener("focusout", T)
             })), eu(ce, H - D);
-            const ye = Z !== void 0 ? m.slice(D, H).reduce(Bt, 0) : 0;
+            const ye = Z !== void 0 ? h.slice(D, H).reduce(Bt, 0) : 0;
             if (ke === !0) {
-                const Te = fe >= P.value.from && D <= P.value.to ? P.value.to : fe;
-                P.value = {
+                const Te = fe >= C.value.from && D <= C.value.to ? C.value.to : fe;
+                C.value = {
                     from: D,
                     to: Te
-                }, v.value = en(f, m, 0, D), x.value = en(f, m, fe, e.value), requestAnimationFrame(() => {
-                    P.value.to !== fe && d === b.scrollStart && (P.value = {
-                        from: P.value.from,
+                }, v.value = en(f, h, 0, D), _.value = en(f, h, fe, e.value), requestAnimationFrame(() => {
+                    C.value.to !== fe && d === b.scrollStart && (C.value = {
+                        from: C.value.from,
                         to: fe
-                    }, x.value = en(f, m, fe, e.value))
+                    }, _.value = en(f, h, fe, e.value))
                 })
             }
             requestAnimationFrame(() => {
                 if (d !== b.scrollStart) return;
                 ke === !0 && O(D);
-                const Te = m.slice(D, H).reduce(Bt, 0),
+                const Te = h.slice(D, H).reduce(Bt, 0),
                     Ae = Te + b.offsetStart + v.value,
-                    Ue = Ae + m[H];
+                    Ue = Ae + h[H];
                 let je = Ae + te;
                 if (Z !== void 0) {
                     const We = Te - ye,
                         Ce = b.scrollStart + We;
-                    je = F !== !0 && Ce < Ae && Ue < Ce + b.scrollViewSize ? Ce : Z === "end" ? Ue - b.scrollViewSize : Ae - (Z === "start" ? 0 : Math.round((b.scrollViewSize - m[H]) / 2))
+                    je = F !== !0 && Ce < Ae && Ue < Ce + b.scrollViewSize ? Ce : Z === "end" ? Ue - b.scrollViewSize : Ae - (Z === "start" ? 0 : Math.round((b.scrollViewSize - h[H]) / 2))
                 }
-                d = je, rr(_, je, a.virtualScrollHorizontal, c.lang.rtl), z(H)
+                d = je, ar(S, je, a.virtualScrollHorizontal, c.lang.rtl), z(H)
             })
         }
 
-        function O(_) {
-            const b = y.value;
+        function O(S) {
+            const b = w.value;
             if (b) {
-                const H = lr.call(b.children, D => D.classList && D.classList.contains("q-virtual-scroll--skip") === !1),
+                const H = rr.call(b.children, D => D.classList && D.classList.contains("q-virtual-scroll--skip") === !1),
                     te = H.length,
                     U = a.virtualScrollHorizontal === !0 ? D => D.getBoundingClientRect().width : D => D.offsetHeight;
-                let F = _,
+                let F = S,
                     Z, ue;
                 for (let D = 0; D < te;) {
                     for (Z = U(H[D]), D++; D < te && H[D].classList.contains("q-virtual-scroll--with-prev") === !0;) Z += U(H[D]), D++;
-                    ue = Z - m[F], ue !== 0 && (m[F] += ue, f[Math.floor(F / Ge)] += ue), F++
+                    ue = Z - h[F], ue !== 0 && (h[F] += ue, f[Math.floor(F / Ge)] += ue), F++
                 }
             }
         }
 
-        function q() {
-            y.value !== null && y.value !== void 0 && y.value.focus()
+        function T() {
+            w.value !== null && w.value !== void 0 && w.value.focus()
         }
 
-        function j(_, b) {
+        function j(S, b) {
             const H = 1 * l.value;
-            (b === !0 || Array.isArray(m) === !1) && (m = []);
-            const te = m.length;
-            m.length = e.value;
-            for (let F = e.value - 1; F >= te; F--) m[F] = H;
+            (b === !0 || Array.isArray(h) === !1) && (h = []);
+            const te = h.length;
+            h.length = e.value;
+            for (let F = e.value - 1; F >= te; F--) h[F] = H;
             const U = Math.floor((e.value - 1) / Ge);
             f = [];
             for (let F = 0; F <= U; F++) {
                 let Z = 0;
                 const ue = Math.min((F + 1) * Ge, e.value);
-                for (let D = F * Ge; D < ue; D++) Z += m[D];
+                for (let D = F * Ge; D < ue; D++) Z += h[D];
                 f.push(Z)
             }
-            s = -1, d = void 0, v.value = en(f, m, 0, P.value.from), x.value = en(f, m, P.value.to, e.value), _ >= 0 ? (O(P.value.from), t.nextTick(() => {
-                B(_)
+            s = -1, d = void 0, v.value = en(f, h, 0, C.value.from), _.value = en(f, h, C.value.to, e.value), S >= 0 ? (O(C.value.from), t.nextTick(() => {
+                P(S)
             })) : G()
         }
 
-        function N(_) {
-            if (_ === void 0 && typeof window < "u") {
+        function N(S) {
+            if (S === void 0 && typeof window < "u") {
                 const Z = n();
-                Z != null && Z.nodeType !== 8 && (_ = yo(Z, o(), S.value, C.value, a.virtualScrollHorizontal, c.lang.rtl, a.virtualScrollStickySizeStart, a.virtualScrollStickySizeEnd).scrollViewSize)
+                Z != null && Z.nodeType !== 8 && (S = yo(Z, o(), k.value, q.value, a.virtualScrollHorizontal, c.lang.rtl, a.virtualScrollStickySizeStart, a.virtualScrollStickySizeEnd).scrollViewSize)
             }
-            h = _;
+            m = S;
             const b = parseFloat(a.virtualScrollSliceRatioBefore) || 0,
                 H = parseFloat(a.virtualScrollSliceRatioAfter) || 0,
                 te = 1 + b + H,
-                U = _ === void 0 || _ <= 0 ? 1 : Math.ceil(_ / l.value),
+                U = S === void 0 || S <= 0 ? 1 : Math.ceil(S / l.value),
                 F = Math.max(1, U, Math.ceil((a.virtualScrollSliceSize > 0 ? a.virtualScrollSliceSize : 10) / te));
             p.value = {
                 total: Math.ceil(F * te),
                 start: Math.ceil(F * b),
                 center: Math.ceil(F * (.5 + b)),
                 end: Math.ceil(F * (1 + b)),
                 view: U
             }
         }
 
-        function w(_, b) {
+        function y(S, b) {
             const H = a.virtualScrollHorizontal === !0 ? "width" : "height",
                 te = {
                     ["--q-virtual-scroll-item-" + H]: l.value + "px"
                 };
-            return [_ === "tbody" ? t.h(_, {
+            return [S === "tbody" ? t.h(S, {
                 class: "q-virtual-scroll__padding",
                 key: "before",
-                ref: S
+                ref: k
             }, [t.h("tr", [t.h("td", {
                 style: {
                     [H]: `${v.value}px`,
                     ...te
                 },
                 colspan: A.value
-            })])]) : t.h(_, {
+            })])]) : t.h(S, {
                 class: "q-virtual-scroll__padding",
                 key: "before",
-                ref: S,
+                ref: k,
                 style: {
                     [H]: `${v.value}px`,
                     ...te
                 }
-            }), t.h(_, {
+            }), t.h(S, {
                 class: "q-virtual-scroll__content",
                 key: "content",
-                ref: y,
+                ref: w,
                 tabindex: -1
-            }, b.flat()), _ === "tbody" ? t.h(_, {
+            }, b.flat()), S === "tbody" ? t.h(S, {
                 class: "q-virtual-scroll__padding",
                 key: "after",
-                ref: C
+                ref: q
             }, [t.h("tr", [t.h("td", {
                 style: {
-                    [H]: `${x.value}px`,
+                    [H]: `${_.value}px`,
                     ...te
                 },
                 colspan: A.value
-            })])]) : t.h(_, {
+            })])]) : t.h(S, {
                 class: "q-virtual-scroll__padding",
                 key: "after",
-                ref: C,
+                ref: q,
                 style: {
-                    [H]: `${x.value}px`,
+                    [H]: `${_.value}px`,
                     ...te
                 }
             })]
         }
 
-        function z(_) {
-            s !== _ && (a.onVirtualScroll !== void 0 && i("virtualScroll", {
-                index: _,
-                from: P.value.from,
-                to: P.value.to - 1,
-                direction: _ < s ? "decrease" : "increase",
+        function z(S) {
+            s !== S && (a.onVirtualScroll !== void 0 && i("virtualScroll", {
+                index: S,
+                from: C.value.from,
+                to: C.value.to - 1,
+                direction: S < s ? "decrease" : "increase",
                 ref: u
-            }), s = _)
+            }), s = S)
         }
         N();
         const G = Un(I, c.platform.is.ios === !0 ? 120 : 35);
         t.onBeforeMount(() => {
             N()
         });
         let J = !1;
         return t.onDeactivated(() => {
             J = !0
         }), t.onActivated(() => {
             if (J !== !0) return;
-            const _ = n();
-            d !== void 0 && _ !== void 0 && _ !== null && _.nodeType !== 8 ? rr(_, d, a.virtualScrollHorizontal, c.lang.rtl) : B(s)
+            const S = n();
+            d !== void 0 && S !== void 0 && S !== null && S.nodeType !== 8 ? ar(S, d, a.virtualScrollHorizontal, c.lang.rtl) : P(s)
         }), t.onBeforeUnmount(() => {
             G.cancel()
         }), Object.assign(u, {
-            scrollTo: B,
+            scrollTo: P,
             reset: R,
-            refresh: T
+            refresh: B
         }), {
-            virtualScrollSliceRange: P,
+            virtualScrollSliceRange: C,
             virtualScrollSliceSizeComputed: p,
             setVirtualScrollSize: N,
             onVirtualScrollEvt: G,
             localResetVirtualScroll: j,
-            padVirtualScroll: w,
-            scrollTo: B,
+            padVirtualScroll: y,
+            scrollTo: P,
             reset: R,
-            refresh: T
+            refresh: B
         }
     }
     const wo = {
         name: String
     };
 
     function tu(e = {}) {
@@ -3030,23 +3030,23 @@
             n[o](t.h("input", {
                 class: "hidden" + (l || ""),
                 ...e.value
             }))
         }
     }
 
-    function cr(e) {
+    function dr(e) {
         return t.computed(() => e.name || e.for)
     }
     const nu = /[\u3000-\u303f\u3040-\u309f\u30a0-\u30ff\uff00-\uff9f\u4e00-\u9faf\u3400-\u4dbf]/,
         ou = /[\u4e00-\u9fff\u3400-\u4dbf\u{20000}-\u{2a6df}\u{2a700}-\u{2b73f}\u{2b740}-\u{2b81f}\u{2b820}-\u{2ceaf}\uf900-\ufaff\u3300-\u33ff\ufe30-\ufe4f\uf900-\ufaff\u{2f800}-\u{2fa1f}]/u,
         lu = /[\u3131-\u314e\u314f-\u3163\uac00-\ud7a3]/,
         ru = /[a-z0-9_ -]$/i;
 
-    function dr(e) {
+    function fr(e) {
         return function(o) {
             if (o.type === "compositionend" || o.type === "change") {
                 if (o.target.qComposing !== !0) return;
                 o.target.qComposing = !1, e(o)
             } else o.type === "compositionupdate" && o.target.qComposing !== !0 && typeof o.data == "string" && (he.is.firefox === !0 ? ru.test(o.data) === !1 : nu.test(o.data) === !0 || ou.test(o.data) === !0 || lu.test(o.data) === !0) === !0 && (o.target.qComposing = !0)
         }
     }
@@ -3104,40 +3104,40 @@
         return e !== e && n !== n
     }
 
     function au(e) {
         return e !== null && typeof e == "object" && Array.isArray(e) !== !0
     }
 
-    function fr(e) {
+    function mr(e) {
         return Object.prototype.toString.call(e) === "[object Date]"
     }
 
     function So(e) {
         return typeof e == "number" && isFinite(e)
     }
 
     function st(e, n, o) {
         return o <= n ? n : Math.min(o, Math.max(n, e))
     }
 
-    function mr(e, n, o) {
+    function hr(e, n, o) {
         if (o <= n) return n;
         const l = o - n + 1;
         let r = n + (e - n) % l;
         return r < n && (r = l + r), r === 0 ? 0 : r
     }
-    const hr = e => ["add", "add-unique", "toggle"].includes(e),
+    const vr = e => ["add", "add-unique", "toggle"].includes(e),
         iu = ".*+?^${}()|[]\\",
         uu = Object.keys(vn),
         _o = se({
             name: "QSelect",
             inheritAttrs: !1,
             props: {
-                ...ur,
+                ...sr,
                 ...wo,
                 ...vn,
                 modelValue: {
                     required: !0
                 },
                 multiple: Boolean,
                 displayValue: [String, Number],
@@ -3168,15 +3168,15 @@
                 menuOffset: Array,
                 popupContentClass: String,
                 popupContentStyle: [String, Array, Object],
                 useInput: Boolean,
                 useChips: Boolean,
                 newValueMode: {
                     type: String,
-                    validator: hr
+                    validator: vr
                 },
                 mapOptions: Boolean,
                 emitValue: Boolean,
                 inputDebounce: {
                     type: [Number, String],
                     default: 500
                 },
@@ -3208,119 +3208,119 @@
                 emit: o
             }) {
                 const {
                     proxy: l
                 } = t.getCurrentInstance(), {
                     $q: r
                 } = l, a = t.ref(!1), i = t.ref(!1), u = t.ref(-1), c = t.ref(""), d = t.ref(!1), s = t.ref(!1);
-                let h = null,
+                let m = null,
                     f = null,
-                    m, v, x, p = null,
-                    S, C, y, P;
+                    h, v, _, p = null,
+                    k, q, w, C;
                 const A = t.ref(null),
                     M = t.ref(null),
                     V = t.ref(null),
                     R = t.ref(null),
-                    T = t.ref(null),
-                    B = cr(e),
-                    I = dr(X),
-                    k = t.computed(() => Array.isArray(e.options) ? e.options.length : 0),
+                    B = t.ref(null),
+                    P = dr(e),
+                    I = fr(X),
+                    x = t.computed(() => Array.isArray(e.options) ? e.options.length : 0),
                     O = t.computed(() => e.virtualScrollItemSize === void 0 ? e.optionsDense === !0 ? 24 : 48 : e.virtualScrollItemSize),
                     {
-                        virtualScrollSliceRange: q,
+                        virtualScrollSliceRange: T,
                         virtualScrollSliceSizeComputed: j,
                         localResetVirtualScroll: N,
-                        padVirtualScroll: w,
+                        padVirtualScroll: y,
                         onVirtualScrollEvt: z,
                         scrollTo: G,
                         setVirtualScrollSize: J
-                    } = sr({
-                        virtualScrollLength: k,
-                        getVirtualScrollTarget: Go,
+                    } = cr({
+                        virtualScrollLength: x,
+                        getVirtualScrollTarget: Xo,
                         getVirtualScrollEl: Vn,
                         virtualScrollItemSizeComputed: O
                     }),
-                    _ = Gn(),
+                    S = Gn(),
                     b = t.computed(() => {
                         const g = e.mapOptions === !0 && e.multiple !== !0,
                             Q = e.modelValue !== void 0 && (e.modelValue !== null || g === !0) ? e.multiple === !0 && Array.isArray(e.modelValue) ? e.modelValue : [e.modelValue] : [];
                         if (e.mapOptions === !0 && Array.isArray(e.options) === !0) {
-                            const K = e.mapOptions === !0 && m !== void 0 ? m : [],
+                            const K = e.mapOptions === !0 && h !== void 0 ? h : [],
                                 oe = Q.map(me => xt(me, K));
                             return e.modelValue === null && g === !0 ? oe.filter(me => me !== null) : oe
                         }
                         return Q
                     }),
                     H = t.computed(() => {
                         const g = {};
                         return uu.forEach(Q => {
                             const K = e[Q];
                             K !== void 0 && (g[Q] = K)
                         }), g
                     }),
-                    te = t.computed(() => e.optionsDark === null ? _.isDark.value : e.optionsDark),
+                    te = t.computed(() => e.optionsDark === null ? S.isDark.value : e.optionsDark),
                     U = t.computed(() => Kt(b.value)),
                     F = t.computed(() => {
                         let g = "q-field__input q-placeholder col";
                         return e.hideSelected === !0 || b.value.length === 0 ? [g, e.inputClass] : (g += " q-field__input--padding", e.inputClass === void 0 ? g : [g, e.inputClass])
                     }),
                     Z = t.computed(() => (e.virtualScrollHorizontal === !0 ? "q-virtual-scroll--horizontal" : "") + (e.popupContentClass ? " " + e.popupContentClass : "")),
-                    ue = t.computed(() => k.value === 0),
+                    ue = t.computed(() => x.value === 0),
                     D = t.computed(() => b.value.map(g => W.value(g)).join(", ")),
                     fe = t.computed(() => e.displayValue !== void 0 ? e.displayValue : D.value),
                     ke = t.computed(() => e.optionsHtml === !0 ? () => !0 : g => g != null && g.html === !0),
                     Ie = t.computed(() => e.displayValueHtml === !0 || e.displayValue === void 0 && (e.optionsHtml === !0 || b.value.some(ke.value))),
-                    ce = t.computed(() => _.focused.value === !0 ? e.tabindex : -1),
+                    ce = t.computed(() => S.focused.value === !0 ? e.tabindex : -1),
                     ye = t.computed(() => {
                         const g = {
                             tabindex: e.tabindex,
                             role: "combobox",
                             "aria-label": e.label,
                             "aria-readonly": e.readonly === !0 ? "true" : "false",
                             "aria-autocomplete": e.useInput === !0 ? "list" : "none",
                             "aria-expanded": a.value === !0 ? "true" : "false",
-                            "aria-controls": `${_.targetUid.value}_lb`
+                            "aria-controls": `${S.targetUid.value}_lb`
                         };
-                        return u.value >= 0 && (g["aria-activedescendant"] = `${_.targetUid.value}_${u.value}`), g
+                        return u.value >= 0 && (g["aria-activedescendant"] = `${S.targetUid.value}_${u.value}`), g
                     }),
                     Te = t.computed(() => ({
-                        id: `${_.targetUid.value}_lb`,
+                        id: `${S.targetUid.value}_lb`,
                         role: "listbox",
                         "aria-multiselectable": e.multiple === !0 ? "true" : "false"
                     })),
                     Ae = t.computed(() => b.value.map((g, Q) => ({
                         index: Q,
                         opt: g,
                         html: ke.value(g),
                         selected: !0,
                         removeAtIndex: qe,
                         toggleOption: Oe,
                         tabindex: ce.value
                     }))),
                     Ue = t.computed(() => {
-                        if (k.value === 0) return [];
+                        if (x.value === 0) return [];
                         const {
                             from: g,
                             to: Q
-                        } = q.value;
+                        } = T.value;
                         return e.options.slice(g, Q).map((K, oe) => {
                             const me = E.value(K) === !0,
                                 de = g + oe,
                                 _e = {
                                     clickable: !0,
                                     active: !1,
                                     activeClass: Ce.value,
                                     manualFocus: !0,
                                     focused: !1,
                                     disable: me,
                                     tabindex: -1,
                                     dense: e.optionsDense,
                                     dark: te.value,
                                     role: "option",
-                                    id: `${_.targetUid.value}_${de}`,
+                                    id: `${S.targetUid.value}_${de}`,
                                     onClick: () => {
                                         Oe(K)
                                     }
                                 };
                             return me !== !0 && (Rt(K) === !0 && (_e.active = !0), u.value === de && (_e.focused = !0), _e["aria-selected"] = _e.active === !0 ? "true" : "false", r.platform.is.desktop === !0 && (_e.onMousemove = () => {
                                 a.value === !0 && Me(de)
                             })), {
@@ -3354,18 +3354,18 @@
                             onClick(Q) {
                                 v === !0 && De(Q)
                             }
                         };
                         return g.onCompositionstart = g.onCompositionupdate = g.onCompositionend = I, g
                     });
                 t.watch(b, g => {
-                    m = g, e.useInput === !0 && e.fillInput === !0 && e.multiple !== !0 && _.innerLoading.value !== !0 && (i.value !== !0 && a.value !== !0 || U.value !== !0) && (x !== !0 && Dt(), (i.value === !0 || a.value === !0) && le(""))
+                    h = g, e.useInput === !0 && e.fillInput === !0 && e.multiple !== !0 && S.innerLoading.value !== !0 && (i.value !== !0 && a.value !== !0 || U.value !== !0) && (_ !== !0 && Dt(), (i.value === !0 || a.value === !0) && le(""))
                 }, {
                     immediate: !0
-                }), t.watch(() => e.fillInput, Dt), t.watch(a, Zo), t.watch(k, _v);
+                }), t.watch(() => e.fillInput, Dt), t.watch(a, Jo), t.watch(x, _v);
 
                 function ie(g) {
                     return e.emitValue === !0 ? L.value(g) : g
                 }
 
                 function ae(g) {
                     if (g > -1 && g < b.value.length)
@@ -3375,15 +3375,15 @@
                                 index: g,
                                 value: Q.splice(g, 1)[0]
                             }), o("update:modelValue", Q)
                         } else o("update:modelValue", null)
                 }
 
                 function qe(g) {
-                    ae(g), _.focus()
+                    ae(g), S.focus()
                 }
 
                 function ze(g, Q) {
                     const K = ie(g);
                     if (e.multiple !== !0) {
                         e.fillInput === !0 && ne(W.value(g), !0, !0), o("update:modelValue", K);
                         return
@@ -3400,21 +3400,21 @@
                     o("add", {
                         index: oe.length,
                         value: K
                     }), oe.push(K), o("update:modelValue", oe)
                 }
 
                 function Oe(g, Q) {
-                    if (_.editable.value !== !0 || g === void 0 || E.value(g) === !0) return;
+                    if (S.editable.value !== !0 || g === void 0 || E.value(g) === !0) return;
                     const K = L.value(g);
                     if (e.multiple !== !0) {
                         Q !== !0 && (ne(e.fillInput === !0 ? W.value(g) : "", !0, !0), Ct()), M.value !== null && M.value.focus(), (b.value.length === 0 || tt(L.value(b.value[0]), K) !== !0) && o("update:modelValue", e.emitValue === !0 ? K : g);
                         return
                     }
-                    if ((v !== !0 || d.value === !0) && _.focus(), Mn(), b.value.length === 0) {
+                    if ((v !== !0 || d.value === !0) && S.focus(), Mn(), b.value.length === 0) {
                         const de = e.emitValue === !0 ? K : g;
                         o("add", {
                             index: 0,
                             value: de
                         }), o("update:modelValue", e.multiple === !0 ? [de] : de);
                         return
                     }
@@ -3433,23 +3433,23 @@
                         }), oe.push(de)
                     }
                     o("update:modelValue", oe)
                 }
 
                 function Me(g) {
                     if (r.platform.is.desktop !== !0) return;
-                    const Q = g > -1 && g < k.value ? g : -1;
+                    const Q = g > -1 && g < x.value ? g : -1;
                     u.value !== Q && (u.value = Q)
                 }
 
                 function Ne(g = 1, Q) {
                     if (a.value === !0) {
                         let K = u.value;
-                        do K = mr(K + g, -1, k.value - 1); while (K !== -1 && K !== u.value && E.value(e.options[K]) === !0);
-                        u.value !== K && (Me(K), G(K), Q !== !0 && e.useInput === !0 && e.fillInput === !0 && ee(K >= 0 ? W.value(e.options[K]) : S, !0))
+                        do K = hr(K + g, -1, x.value - 1); while (K !== -1 && K !== u.value && E.value(e.options[K]) === !0);
+                        u.value !== K && (Me(K), G(K), Q !== !0 && e.useInput === !0 && e.fillInput === !0 && ee(K >= 0 ? W.value(e.options[K]) : k, !0))
                     }
                 }
 
                 function xt(g, Q) {
                     const K = oe => tt(L.value(oe), g);
                     return e.options.find(K) || Q.find(K) || g
                 }
@@ -3476,25 +3476,25 @@
                     const {
                         value: Q
                     } = g.target;
                     if (g.keyCode !== void 0) {
                         Vt(g);
                         return
                     }
-                    if (g.target.value = "", h !== null && (clearTimeout(h), h = null), f !== null && (clearTimeout(f), f = null), Dt(), typeof Q == "string" && Q.length !== 0) {
+                    if (g.target.value = "", m !== null && (clearTimeout(m), m = null), f !== null && (clearTimeout(f), f = null), Dt(), typeof Q == "string" && Q.length !== 0) {
                         const K = Q.toLocaleLowerCase(),
                             oe = de => {
                                 const _e = e.options.find(Ve => de.value(Ve).toLocaleLowerCase() === K);
                                 return _e === void 0 ? !1 : (b.value.indexOf(_e) === -1 ? Oe(_e) : Ct(), !0)
                             },
                             me = de => {
                                 oe(L) !== !0 && (oe(W) === !0 || de === !0 || le(Q, !0, () => me(!0)))
                             };
                         me()
-                    } else _.clearValue(g)
+                    } else S.clearValue(g)
                 }
 
                 function kt(g) {
                     o("keypress", g)
                 }
 
                 function Rn(g) {
@@ -3505,69 +3505,69 @@
                         $e(g);
                         return
                     }
                     if (g.keyCode === 9 && K === !1) {
                         Lt();
                         return
                     }
-                    if (g.target === void 0 || g.target.id !== _.targetUid.value || _.editable.value !== !0) return;
-                    if (g.keyCode === 40 && _.innerLoading.value !== !0 && a.value === !1) {
+                    if (g.target === void 0 || g.target.id !== S.targetUid.value || S.editable.value !== !0) return;
+                    if (g.keyCode === 40 && S.innerLoading.value !== !0 && a.value === !1) {
                         ve(g), Ft();
                         return
                     }
                     if (g.keyCode === 8 && (e.useChips === !0 || e.clearable === !0) && e.hideSelected !== !0 && c.value.length === 0) {
                         e.multiple === !0 && Array.isArray(e.modelValue) === !0 ? ae(e.modelValue.length - 1) : e.multiple !== !0 && e.modelValue !== null && o("update:modelValue", null);
                         return
-                    }(g.keyCode === 35 || g.keyCode === 36) && (typeof c.value != "string" || c.value.length === 0) && (ve(g), u.value = -1, Ne(g.keyCode === 36 ? 1 : -1, e.multiple)), (g.keyCode === 33 || g.keyCode === 34) && j.value !== void 0 && (ve(g), u.value = Math.max(-1, Math.min(k.value, u.value + (g.keyCode === 33 ? -1 : 1) * j.value.view)), Ne(g.keyCode === 33 ? 1 : -1, e.multiple)), (g.keyCode === 38 || g.keyCode === 40) && (ve(g), Ne(g.keyCode === 38 ? -1 : 1, e.multiple));
-                    const oe = k.value;
-                    if ((y === void 0 || P < Date.now()) && (y = ""), oe > 0 && e.useInput !== !0 && g.key !== void 0 && g.key.length === 1 && g.altKey === !1 && g.ctrlKey === !1 && g.metaKey === !1 && (g.keyCode !== 32 || y.length !== 0)) {
+                    }(g.keyCode === 35 || g.keyCode === 36) && (typeof c.value != "string" || c.value.length === 0) && (ve(g), u.value = -1, Ne(g.keyCode === 36 ? 1 : -1, e.multiple)), (g.keyCode === 33 || g.keyCode === 34) && j.value !== void 0 && (ve(g), u.value = Math.max(-1, Math.min(x.value, u.value + (g.keyCode === 33 ? -1 : 1) * j.value.view)), Ne(g.keyCode === 33 ? 1 : -1, e.multiple)), (g.keyCode === 38 || g.keyCode === 40) && (ve(g), Ne(g.keyCode === 38 ? -1 : 1, e.multiple));
+                    const oe = x.value;
+                    if ((w === void 0 || C < Date.now()) && (w = ""), oe > 0 && e.useInput !== !0 && g.key !== void 0 && g.key.length === 1 && g.altKey === !1 && g.ctrlKey === !1 && g.metaKey === !1 && (g.keyCode !== 32 || w.length !== 0)) {
                         a.value !== !0 && Ft(g);
                         const me = g.key.toLocaleLowerCase(),
-                            de = y.length === 1 && y[0] === me;
-                        P = Date.now() + 1500, de === !1 && (ve(g), y += me);
-                        const _e = new RegExp("^" + y.split("").map(Jo => iu.indexOf(Jo) > -1 ? "\\" + Jo : Jo).join(".*"), "i");
+                            de = w.length === 1 && w[0] === me;
+                        C = Date.now() + 1500, de === !1 && (ve(g), w += me);
+                        const _e = new RegExp("^" + w.split("").map(el => iu.indexOf(el) > -1 ? "\\" + el : el).join(".*"), "i");
                         let Ve = u.value;
                         if (de === !0 || Ve < 0 || _e.test(W.value(e.options[Ve])) !== !0)
-                            do Ve = mr(Ve + 1, -1, oe - 1); while (Ve !== u.value && (E.value(e.options[Ve]) === !0 || _e.test(W.value(e.options[Ve])) !== !0));
+                            do Ve = hr(Ve + 1, -1, oe - 1); while (Ve !== u.value && (E.value(e.options[Ve]) === !0 || _e.test(W.value(e.options[Ve])) !== !0));
                         u.value !== Ve && t.nextTick(() => {
                             Me(Ve), G(Ve), Ve >= 0 && e.useInput === !0 && e.fillInput === !0 && ee(W.value(e.options[Ve]), !0)
                         });
                         return
                     }
-                    if (!(g.keyCode !== 13 && (g.keyCode !== 32 || e.useInput === !0 || y !== "") && (g.keyCode !== 9 || K === !1))) {
+                    if (!(g.keyCode !== 13 && (g.keyCode !== 32 || e.useInput === !0 || w !== "") && (g.keyCode !== 9 || K === !1))) {
                         if (g.keyCode !== 9 && ve(g), u.value > -1 && u.value < oe) {
                             Oe(e.options[u.value]);
                             return
                         }
                         if (Q === !0) {
                             const me = (de, _e) => {
                                 if (_e) {
-                                    if (hr(_e) !== !0) return
+                                    if (vr(_e) !== !0) return
                                 } else _e = e.newValueMode;
                                 if (ne("", e.multiple !== !0, !0), de == null) return;
                                 (_e === "toggle" ? Oe : ze)(de, _e === "add-unique"), e.multiple !== !0 && (M.value !== null && M.value.focus(), Ct())
                             };
                             if (e.onNewValue !== void 0 ? o("newValue", c.value, me) : me(c.value), e.multiple !== !0) return
                         }
-                        a.value === !0 ? Lt() : _.innerLoading.value !== !0 && Ft()
+                        a.value === !0 ? Lt() : S.innerLoading.value !== !0 && Ft()
                     }
                 }
 
                 function Vn() {
-                    return v === !0 ? T.value : V.value !== null && V.value.contentEl !== null ? V.value.contentEl : void 0
+                    return v === !0 ? B.value : V.value !== null && V.value.contentEl !== null ? V.value.contentEl : void 0
                 }
 
-                function Go() {
+                function Xo() {
                     return Vn()
                 }
 
-                function Xo() {
+                function Yo() {
                     return e.hideSelected === !0 ? [] : n["selected-item"] !== void 0 ? Ae.value.map(g => n["selected-item"](g)).slice() : n.selected !== void 0 ? [].concat(n.selected()) : e.useChips === !0 ? Ae.value.map((g, Q) => t.h(_i, {
                         key: "option-" + Q,
-                        removable: _.editable.value === !0 && E.value(g.opt) !== !0,
+                        removable: S.editable.value === !0 && E.value(g.opt) !== !0,
                         dense: !0,
                         textColor: e.color,
                         tabindex: ce.value,
                         onRemove() {
                             g.removeAtIndex(Q)
                         }
                     }, () => t.h("span", {
@@ -3578,80 +3578,80 @@
                     })]
                 }
 
                 function In() {
                     if (ue.value === !0) return n["no-option"] !== void 0 ? n["no-option"]({
                         inputValue: c.value
                     }) : void 0;
-                    const g = n.option !== void 0 ? n.option : K => t.h(El, {
+                    const g = n.option !== void 0 ? n.option : K => t.h($l, {
                         key: K.index,
                         ...K.itemProps
-                    }, () => t.h(to, () => t.h($l, () => t.h("span", {
+                    }, () => t.h(to, () => t.h(Al, () => t.h("span", {
                         [K.html === !0 ? "innerHTML" : "textContent"]: K.label
                     }))));
-                    let Q = w("div", Ue.value.map(g));
+                    let Q = y("div", Ue.value.map(g));
                     return n["before-options"] !== void 0 && (Q = n["before-options"]().concat(Q)), Ke(n["after-options"], Q)
                 }
 
                 function $(g, Q) {
                     const K = Q === !0 ? {
                             ...ye.value,
-                            ..._.splitAttrs.attributes.value
+                            ...S.splitAttrs.attributes.value
                         } : void 0,
                         oe = {
                             ref: Q === !0 ? M : void 0,
                             key: "i_t",
                             class: F.value,
                             style: e.inputStyle,
                             value: c.value !== void 0 ? c.value : "",
                             type: "search",
                             ...K,
-                            id: Q === !0 ? _.targetUid.value : void 0,
+                            id: Q === !0 ? S.targetUid.value : void 0,
                             maxlength: e.maxlength,
                             autocomplete: e.autocomplete,
                             "data-autofocus": g === !0 || e.autofocus === !0 || void 0,
                             disabled: e.disable === !0,
                             readonly: e.readonly === !0,
                             ...re.value
                         };
                     return g !== !0 && v === !0 && (Array.isArray(oe.class) === !0 ? oe.class = [...oe.class, "no-pointer-events"] : oe.class += " no-pointer-events"), t.h("input", oe)
                 }
 
                 function X(g) {
-                    h !== null && (clearTimeout(h), h = null), f !== null && (clearTimeout(f), f = null), !(g && g.target && g.target.qComposing === !0) && (ee(g.target.value || ""), x = !0, S = c.value, _.focused.value !== !0 && (v !== !0 || d.value === !0) && _.focus(), e.onFilter !== void 0 && (h = setTimeout(() => {
-                        h = null, le(c.value)
+                    m !== null && (clearTimeout(m), m = null), f !== null && (clearTimeout(f), f = null), !(g && g.target && g.target.qComposing === !0) && (ee(g.target.value || ""), _ = !0, k = c.value, S.focused.value !== !0 && (v !== !0 || d.value === !0) && S.focus(), e.onFilter !== void 0 && (m = setTimeout(() => {
+                        m = null, le(c.value)
                     }, e.inputDebounce)))
                 }
 
                 function ee(g, Q) {
                     c.value !== g && (c.value = g, Q === !0 || e.inputDebounce === 0 || e.inputDebounce === "0" ? o("inputValue", g) : f = setTimeout(() => {
                         f = null, o("inputValue", g)
                     }, e.inputDebounce))
                 }
 
                 function ne(g, Q, K) {
-                    x = K !== !0, e.useInput === !0 && (ee(g, !0), (Q === !0 || K !== !0) && (S = g), Q !== !0 && le(g))
+                    _ = K !== !0, e.useInput === !0 && (ee(g, !0), (Q === !0 || K !== !0) && (k = g), Q !== !0 && le(g))
                 }
 
                 function le(g, Q, K) {
-                    if (e.onFilter === void 0 || Q !== !0 && _.focused.value !== !0) return;
-                    _.innerLoading.value === !0 ? o("filterAbort") : (_.innerLoading.value = !0, s.value = !0), g !== "" && e.multiple !== !0 && b.value.length !== 0 && x !== !0 && g === W.value(b.value[0]) && (g = "");
+                    if (e.onFilter === void 0 || Q !== !0 && S.focused.value !== !0) return;
+                    S.innerLoading.value === !0 ? o("filterAbort") : (S.innerLoading.value = !0, s.value = !0), g !== "" && e.multiple !== !0 && b.value.length !== 0 && _ !== !0 && g === W.value(b.value[0]) && (g = "");
                     const oe = setTimeout(() => {
                         a.value === !0 && (a.value = !1)
                     }, 10);
                     p !== null && clearTimeout(p), p = oe, o("filter", g, (me, de) => {
-                        (Q === !0 || _.focused.value === !0) && p === oe && (clearTimeout(p), typeof me == "function" && me(), s.value = !1, t.nextTick(() => {
-                            _.innerLoading.value = !1, _.editable.value === !0 && (Q === !0 ? a.value === !0 && Ct() : a.value === !0 ? Zo(!0) : a.value = !0), typeof de == "function" && t.nextTick(() => {
+                        (Q === !0 || S.focused.value === !0) && p === oe && (clearTimeout(p), typeof me == "function" && me(), s.value = !1, t.nextTick(() => {
+                            S.innerLoading.value = !1, S.editable.value === !0 && (Q === !0 ? a.value === !0 && Ct() : a.value === !0 ? Jo(!0) : a.value = !0), typeof de == "function" && t.nextTick(() => {
                                 de(l)
                             }), typeof K == "function" && t.nextTick(() => {
                                 K(l)
                             })
                         }))
                     }, () => {
-                        _.focused.value === !0 && p === oe && (clearTimeout(p), _.innerLoading.value = !1, s.value = !1), a.value === !0 && (a.value = !1)
+                        S.focused.value === !0 && p === oe && (clearTimeout(p), S.innerLoading.value = !1, s.value = !1), a.value === !0 && (a.value = !1)
                     })
                 }
 
                 function be() {
                     return t.h(Ki, {
                         ref: V,
                         class: Z.value,
@@ -3695,121 +3695,121 @@
                     De(g), t.nextTick(() => {
                         d.value = !1
                     })
                 }
 
                 function zt() {
                     const g = [t.h(bi, {
-                        class: `col-auto ${_.fieldClass.value}`,
+                        class: `col-auto ${S.fieldClass.value}`,
                         ...H.value,
-                        for: _.targetUid.value,
+                        for: S.targetUid.value,
                         dark: te.value,
                         square: !0,
                         loading: s.value,
                         itemAligned: !1,
                         filled: !0,
                         stackLabel: c.value.length !== 0,
-                        ..._.splitAttrs.listeners.value,
+                        ...S.splitAttrs.listeners.value,
                         onFocus: Ee,
                         onBlur: It
                     }, {
                         ...n,
-                        rawControl: () => _.getControl(!0),
+                        rawControl: () => S.getControl(!0),
                         before: void 0,
                         after: void 0
                     })];
                     return a.value === !0 && g.push(t.h("div", {
-                        ref: T,
+                        ref: B,
                         class: Z.value + " scroll",
                         style: e.popupContentStyle,
                         ...Te.value,
                         onClick: $e,
                         onScrollPassive: z
                     }, In())), t.h(Zi, {
                         ref: R,
                         modelValue: i.value,
                         position: e.useInput === !0 ? "top" : void 0,
-                        transitionShow: C,
+                        transitionShow: q,
                         transitionHide: e.transitionHide,
                         transitionDuration: e.transitionDuration,
                         onBeforeShow: Na,
-                        onBeforeHide: Yo,
+                        onBeforeHide: Zo,
                         onHide: wv,
                         onShow: Sv
                     }, () => t.h("div", {
                         class: "q-select__dialog" + (te.value === !0 ? " q-select__dialog--dark q-dark" : "") + (d.value === !0 ? " q-select__dialog--focused" : "")
                     }, g))
                 }
 
-                function Yo(g) {
-                    Ha(g), R.value !== null && R.value.__updateRefocusTarget(_.rootRef.value.querySelector(".q-field__native > [tabindex]:last-child")), _.focused.value = !1
+                function Zo(g) {
+                    Ha(g), R.value !== null && R.value.__updateRefocusTarget(S.rootRef.value.querySelector(".q-field__native > [tabindex]:last-child")), S.focused.value = !1
                 }
 
                 function wv(g) {
-                    Ct(), _.focused.value === !1 && o("blur", g), Dt()
+                    Ct(), S.focused.value === !1 && o("blur", g), Dt()
                 }
 
                 function Sv() {
                     const g = document.activeElement;
-                    (g === null || g.id !== _.targetUid.value) && M.value !== null && M.value !== g && M.value.focus(), J()
+                    (g === null || g.id !== S.targetUid.value) && M.value !== null && M.value !== g && M.value.focus(), J()
                 }
 
                 function Lt() {
-                    i.value !== !0 && (u.value = -1, a.value === !0 && (a.value = !1), _.focused.value === !1 && (p !== null && (clearTimeout(p), p = null), _.innerLoading.value === !0 && (o("filterAbort"), _.innerLoading.value = !1, s.value = !1)))
+                    i.value !== !0 && (u.value = -1, a.value === !0 && (a.value = !1), S.focused.value === !1 && (p !== null && (clearTimeout(p), p = null), S.innerLoading.value === !0 && (o("filterAbort"), S.innerLoading.value = !1, s.value = !1)))
                 }
 
                 function Ft(g) {
-                    _.editable.value === !0 && (v === !0 ? (_.onControlFocusin(g), i.value = !0, t.nextTick(() => {
-                        _.focus()
-                    })) : _.focus(), e.onFilter !== void 0 ? le(c.value) : (ue.value !== !0 || n["no-option"] !== void 0) && (a.value = !0))
+                    S.editable.value === !0 && (v === !0 ? (S.onControlFocusin(g), i.value = !0, t.nextTick(() => {
+                        S.focus()
+                    })) : S.focus(), e.onFilter !== void 0 ? le(c.value) : (ue.value !== !0 || n["no-option"] !== void 0) && (a.value = !0))
                 }
 
                 function Ct() {
                     i.value = !1, Lt()
                 }
 
                 function Dt() {
                     e.useInput === !0 && ne(e.multiple !== !0 && e.fillInput === !0 && b.value.length !== 0 && W.value(b.value[0]) || "", !0, !0)
                 }
 
-                function Zo(g) {
+                function Jo(g) {
                     let Q = -1;
                     if (g === !0) {
                         if (b.value.length !== 0) {
                             const K = L.value(b.value[0]);
                             Q = e.options.findIndex(oe => tt(L.value(oe), K))
                         }
                         N(Q)
                     }
                     Me(Q)
                 }
 
                 function _v(g, Q) {
-                    a.value === !0 && _.innerLoading.value === !1 && (N(-1, !0), t.nextTick(() => {
-                        a.value === !0 && _.innerLoading.value === !1 && (g > Q ? N() : Zo(!0))
+                    a.value === !0 && S.innerLoading.value === !1 && (N(-1, !0), t.nextTick(() => {
+                        a.value === !0 && S.innerLoading.value === !1 && (g > Q ? N() : Jo(!0))
                     }))
                 }
 
                 function ja() {
                     i.value === !1 && V.value !== null && V.value.updatePosition()
                 }
 
                 function Na(g) {
-                    g !== void 0 && De(g), o("popupShow", g), _.hasPopupOpen = !0, _.onControlFocusin(g)
+                    g !== void 0 && De(g), o("popupShow", g), S.hasPopupOpen = !0, S.onControlFocusin(g)
                 }
 
                 function Ha(g) {
-                    g !== void 0 && De(g), o("popupHide", g), _.hasPopupOpen = !1, _.onControlFocusout(g)
+                    g !== void 0 && De(g), o("popupHide", g), S.hasPopupOpen = !1, S.onControlFocusout(g)
                 }
 
                 function Ua() {
-                    v = r.platform.is.mobile !== !0 && e.behavior !== "dialog" ? !1 : e.behavior !== "menu" && (e.useInput === !0 ? n["no-option"] !== void 0 || e.onFilter !== void 0 || ue.value === !1 : !0), C = r.platform.is.ios === !0 && v === !0 && e.useInput === !0 ? "fade" : e.transitionShow
+                    v = r.platform.is.mobile !== !0 && e.behavior !== "dialog" ? !1 : e.behavior !== "menu" && (e.useInput === !0 ? n["no-option"] !== void 0 || e.onFilter !== void 0 || ue.value === !1 : !0), q = r.platform.is.ios === !0 && v === !0 && e.useInput === !0 ? "fade" : e.transitionShow
                 }
                 return t.onBeforeUpdate(Ua), t.onUpdated(ja), Ua(), t.onBeforeUnmount(() => {
-                    h !== null && clearTimeout(h), f !== null && clearTimeout(f)
+                    m !== null && clearTimeout(m), f !== null && clearTimeout(f)
                 }), Object.assign(l, {
                     showPopup: Ft,
                     hidePopup: Ct,
                     removeAtIndex: ae,
                     add: ze,
                     toggleOption: Oe,
                     getOptionIndex: () => u.value,
@@ -3819,154 +3819,154 @@
                     updateMenuPosition: ja,
                     updateInputValue: ne,
                     isOptionSelected: Rt,
                     getEmittingOptionValue: ie,
                     isOptionDisabled: (...g) => E.value.apply(null, g) === !0,
                     getOptionValue: (...g) => L.value.apply(null, g),
                     getOptionLabel: (...g) => W.value.apply(null, g)
-                }), Object.assign(_, {
+                }), Object.assign(S, {
                     innerValue: b,
                     fieldClass: t.computed(() => `q-select q-field--auto-height q-select--with${e.useInput!==!0?"out":""}-input q-select--with${e.useChips!==!0?"out":""}-chips q-select--${e.multiple===!0?"multiple":"single"}`),
                     inputRef: A,
                     targetRef: M,
                     hasValue: U,
                     showPopup: Ft,
                     floatingLabel: t.computed(() => e.hideSelected !== !0 && U.value === !0 || typeof c.value == "number" || c.value.length !== 0 || Kt(e.displayValue)),
                     getControlChild: () => {
-                        if (_.editable.value !== !1 && (i.value === !0 || ue.value !== !0 || n["no-option"] !== void 0)) return v === !0 ? zt() : be();
-                        _.hasPopupOpen === !0 && (_.hasPopupOpen = !1)
+                        if (S.editable.value !== !1 && (i.value === !0 || ue.value !== !0 || n["no-option"] !== void 0)) return v === !0 ? zt() : be();
+                        S.hasPopupOpen === !0 && (S.hasPopupOpen = !1)
                     },
                     controlEvents: {
                         onFocusin(g) {
-                            _.onControlFocusin(g)
+                            S.onControlFocusin(g)
                         },
                         onFocusout(g) {
-                            _.onControlFocusout(g, () => {
+                            S.onControlFocusout(g, () => {
                                 Dt(), Lt()
                             })
                         },
                         onClick(g) {
                             if ($e(g), v !== !0 && a.value === !0) {
                                 Lt(), M.value !== null && M.value.focus();
                                 return
                             }
                             Ft(g)
                         }
                     },
                     getControl: g => {
-                        const Q = Xo(),
+                        const Q = Yo(),
                             K = g === !0 || i.value !== !0 || v !== !0;
                         if (e.useInput === !0) Q.push($(g, K));
-                        else if (_.editable.value === !0) {
+                        else if (S.editable.value === !0) {
                             const me = K === !0 ? ye.value : void 0;
                             Q.push(t.h("input", {
                                 ref: K === !0 ? M : void 0,
                                 key: "d_t",
                                 class: "q-select__focus-target",
-                                id: K === !0 ? _.targetUid.value : void 0,
+                                id: K === !0 ? S.targetUid.value : void 0,
                                 value: fe.value,
                                 readonly: !0,
                                 "data-autofocus": g === !0 || e.autofocus === !0 || void 0,
                                 ...me,
                                 onKeydown: Rn,
                                 onKeyup: Vt,
                                 onKeypress: kt
                             })), K === !0 && typeof e.autocomplete == "string" && e.autocomplete.length !== 0 && Q.push(t.h("input", {
                                 class: "q-select__autocomplete-input",
                                 autocomplete: e.autocomplete,
                                 tabindex: -1,
                                 onKeyup: sn
                             }))
                         }
-                        if (B.value !== void 0 && e.disable !== !0 && Y.value.length !== 0) {
+                        if (P.value !== void 0 && e.disable !== !0 && Y.value.length !== 0) {
                             const me = Y.value.map(de => t.h("option", {
                                 value: de,
                                 selected: !0
                             }));
                             Q.push(t.h("select", {
                                 class: "hidden",
-                                name: B.value,
+                                name: P.value,
                                 multiple: e.multiple
                             }, me))
                         }
-                        const oe = e.useInput === !0 || K !== !0 ? void 0 : _.splitAttrs.attributes.value;
+                        const oe = e.useInput === !0 || K !== !0 ? void 0 : S.splitAttrs.attributes.value;
                         return t.h("div", {
                             class: "q-field__native row items-center",
                             ...oe,
-                            ..._.splitAttrs.listeners.value
+                            ...S.splitAttrs.listeners.value
                         }, Q)
                     },
                     getInnerAppend: () => e.loading !== !0 && s.value !== !0 && e.hideDropdownIcon !== !0 ? [t.h(Be, {
                         class: "q-select__dropdown-icon" + (a.value === !0 ? " rotate-180" : ""),
                         name: je.value
                     })] : null
-                }), Xn(_)
+                }), Xn(S)
             }
         }),
-        vr = "dbKey",
+        gr = "dbKey",
         xn = "utilsKey",
         kn = "reactdataServicesKey",
         su = "dynamicComponentKey",
         cu = "metaInfoKey",
-        gr = "actionsServiceKey",
-        pr = "appEventServiceKey",
+        pr = "actionsServiceKey",
+        xo = "appEventServiceKey",
         br = "componentInfosServiceKey",
         du = "imgServiceKey",
         fu = {
             class: "slicer-box"
         },
         mu = t.defineComponent({
             __name: "Slicer",
             props: {
                 model: {}
             },
             setup(e) {
                 const n = e,
                     o = n.model,
-                    l = t.inject(vr),
+                    l = t.inject(gr),
                     r = t.inject(kn);
-                t.inject(pr).onResetFilters(() => {
-                    o.multiple ? h.value = [] : h.value = null
+                t.inject(xo).onResetFilters(() => {
+                    o.multiple ? m.value = [] : m.value = null
                 });
                 const i = r.getFilterUtils(o),
                     u = i.getData();
                 let c = null;
                 const d = t.computed(() => {
                         if (u.value.rows.length > 0) {
                             const f = u.value.rows;
-                            return c || (c = u.value.fields[0]), f.map(m => ({
-                                label: m[c] === void 0 || m[c] === null ? "(空白)" : m[c].toString(),
-                                value: m[c] ?? null
+                            return c || (c = u.value.fields[0]), f.map(h => ({
+                                label: h[c] === void 0 || h[c] === null ? "(空白)" : h[c].toString(),
+                                value: h[c] ?? null
                             }))
                         }
                         return []
                     }),
                     s = d.value.length,
-                    h = t.ref();
+                    m = t.ref();
                 if (o.defaultSelected && s > 0) {
                     let f = d.value[0].value;
-                    o.multiple && (f = [f]), h.value = f
+                    o.multiple && (f = [f]), m.value = f
                 }
-                return t.watch(h, f => {
-                    if (f || (f = []), Array.isArray(f) || (f = [f]), f = f.map(m => m.value), f.length === 0) i.removeFilter();
+                return t.watch(m, f => {
+                    if (f || (f = []), Array.isArray(f) || (f = [f]), f = f.map(h => h.value), f.length === 0) i.removeFilter();
                     else {
                         const {
-                            hasNull: m,
+                            hasNull: h,
                             values: v
-                        } = l.extractNullInValues(f), x = l.valuesArray2sqlArray(v).join(",");
+                        } = l.extractNullInValues(f), _ = l.valuesArray2sqlArray(v).join(",");
                         i.addFilterWithExprFn(p => {
-                            const S = `${p} in (${x})`;
-                            return m ? `${S} or ${p} is null` : S
+                            const k = `${p} in (${_})`;
+                            return h ? `${k} or ${p} is null` : k
                         })
                     }
                 }, {
                     immediate: !0
-                }), t.computed(() => h.value && h.value.length > 3), (f, m) => (t.openBlock(), t.createElementBlock("div", fu, [t.createVNode(_o, t.mergeProps({
-                    modelValue: h.value,
-                    "onUpdate:modelValue": m[0] || (m[0] = v => h.value = v),
+                }), t.computed(() => m.value && m.value.length > 3), (f, h) => (t.openBlock(), t.createElementBlock("div", fu, [t.createVNode(_o, t.mergeProps({
+                    modelValue: m.value,
+                    "onUpdate:modelValue": h[0] || (h[0] = v => m.value = v),
                     options: d.value,
                     label: n.model.title,
                     class: "cp-select",
                     clearable: "",
                     dense: "",
                     outlined: "",
                     "use-chips": ""
@@ -4010,15 +4010,15 @@
                     let i, u;
                     const c = l.vnode.key;
                     if (c) {
                         if (i = e.props.colsMap[c], i === void 0) return
                     } else i = e.props.col;
                     if (i.sortable === !0) {
                         const s = i.align === "right" ? "unshift" : "push";
-                        u = nl(n.default, []), u[s](t.h(Be, {
+                        u = ol(n.default, []), u[s](t.h(Be, {
                             class: i.__iconClass,
                             name: r.iconSet.table.arrowUp
                         }))
                     } else u = we(n.default);
                     const d = {
                         class: i.__thClass + (e.autoWidth === !0 ? " q-table--col-auto-width" : ""),
                         style: i.headerStyle,
@@ -4031,15 +4031,15 @@
             }
         }),
         gu = {
             true: "inset",
             item: "item-inset",
             "item-thumbnail": "item-thumbnail-inset"
         },
-        xo = {
+        ko = {
             xs: 2,
             sm: 4,
             md: 8,
             lg: 16,
             xl: 24
         },
         pu = se({
@@ -4058,15 +4058,15 @@
                     l = t.computed(() => e.vertical === !0 ? "vertical" : "horizontal"),
                     r = t.computed(() => ` q-separator--${l.value}`),
                     a = t.computed(() => e.inset !== !1 ? `${r.value}-${gu[e.inset]}` : ""),
                     i = t.computed(() => `q-separator${r.value}${a.value}` + (e.color !== void 0 ? ` bg-${e.color}` : "") + (o.value === !0 ? " q-separator--dark" : "")),
                     u = t.computed(() => {
                         const c = {};
                         if (e.size !== void 0 && (c[e.vertical === !0 ? "width" : "height"] = e.size), e.spaced !== !1) {
-                            const d = e.spaced === !0 ? `${xo.md}px` : e.spaced in xo ? `${xo[e.spaced]}px` : e.spaced,
+                            const d = e.spaced === !0 ? `${ko.md}px` : e.spaced in ko ? `${ko[e.spaced]}px` : e.spaced,
                                 s = e.vertical === !0 ? ["Left", "Right"] : ["Top", "Bottom"];
                             c[`margin${s[0]}`] = c[`margin${s[1]}`] = d
                         }
                         return c
                     });
                 return () => t.h("hr", {
                     class: i.value,
@@ -4138,15 +4138,15 @@
             list: bu,
             table: wu
         },
         _u = ["list", "table", "__qtable"],
         xu = se({
             name: "QVirtualScroll",
             props: {
-                ...ur,
+                ...sr,
                 type: {
                     type: String,
                     default: "list",
                     validator: e => _u.includes(e)
                 },
                 items: {
                     type: Array,
@@ -4166,81 +4166,81 @@
                 const r = t.ref(null),
                     a = t.computed(() => e.itemsSize >= 0 && e.itemsFn !== void 0 ? parseInt(e.itemsSize, 10) : Array.isArray(e.items) ? e.items.length : 0),
                     {
                         virtualScrollSliceRange: i,
                         localResetVirtualScroll: u,
                         padVirtualScroll: c,
                         onVirtualScrollEvt: d
-                    } = sr({
+                    } = cr({
                         virtualScrollLength: a,
                         getVirtualScrollTarget: v,
-                        getVirtualScrollEl: m
+                        getVirtualScrollEl: h
                     }),
                     s = t.computed(() => {
                         if (a.value === 0) return [];
-                        const C = (y, P) => ({
-                            index: i.value.from + P,
-                            item: y
+                        const q = (w, C) => ({
+                            index: i.value.from + C,
+                            item: w
                         });
-                        return e.itemsFn === void 0 ? e.items.slice(i.value.from, i.value.to).map(C) : e.itemsFn(i.value.from, i.value.to - i.value.from).map(C)
+                        return e.itemsFn === void 0 ? e.items.slice(i.value.from, i.value.to).map(q) : e.itemsFn(i.value.from, i.value.to - i.value.from).map(q)
                     }),
-                    h = t.computed(() => "q-virtual-scroll q-virtual-scroll" + (e.virtualScrollHorizontal === !0 ? "--horizontal" : "--vertical") + (e.scrollTarget !== void 0 ? "" : " scroll")),
+                    m = t.computed(() => "q-virtual-scroll q-virtual-scroll" + (e.virtualScrollHorizontal === !0 ? "--horizontal" : "--vertical") + (e.scrollTarget !== void 0 ? "" : " scroll")),
                     f = t.computed(() => e.scrollTarget !== void 0 ? {} : {
                         tabindex: 0
                     });
                 t.watch(a, () => {
                     u()
                 }), t.watch(() => e.scrollTarget, () => {
-                    p(), x()
+                    p(), _()
                 });
 
-                function m() {
+                function h() {
                     return r.value.$el || r.value
                 }
 
                 function v() {
                     return l
                 }
 
-                function x() {
-                    l = ao(m(), e.scrollTarget), l.addEventListener("scroll", d, Se.passive)
+                function _() {
+                    l = ao(h(), e.scrollTarget), l.addEventListener("scroll", d, Se.passive)
                 }
 
                 function p() {
                     l !== void 0 && (l.removeEventListener("scroll", d, Se.passive), l = void 0)
                 }
 
-                function S() {
-                    let C = c(e.type === "list" ? "div" : "tbody", s.value.map(n.default));
-                    return n.before !== void 0 && (C = n.before().concat(C)), Ke(n.after, C)
+                function k() {
+                    let q = c(e.type === "list" ? "div" : "tbody", s.value.map(n.default));
+                    return n.before !== void 0 && (q = n.before().concat(q)), Ke(n.after, q)
                 }
                 return t.onBeforeMount(() => {
                     u()
                 }), t.onMounted(() => {
-                    x()
+                    _()
                 }), t.onActivated(() => {
-                    x()
+                    _()
                 }), t.onDeactivated(() => {
                     p()
                 }), t.onBeforeUnmount(() => {
                     p()
                 }), () => {
                     if (n.default === void 0) {
                         console.error("QVirtualScroll: default scoped slot is required for rendering");
                         return
                     }
                     return e.type === "__qtable" ? yr({
                         ref: r,
-                        class: "q-table__middle " + h.value
-                    }, S()) : t.h(Su[e.type], {
+                        class: "q-table__middle " + m.value
+                    }, k()) : t.h(Su[e.type], {
                         ...o,
                         ref: r,
-                        class: [o.class, h.value],
+                        class: [o.class, m.value],
                         ...f.value
-                    }, S)
+                    }, k)
                 }
             }
         }),
         ku = {
             xs: 2,
             sm: 4,
             md: 6,
@@ -4280,27 +4280,27 @@
             slots: n
         }) {
             const {
                 proxy: o
             } = t.getCurrentInstance(), l = Fe(e, o.$q), r = Ht(e, ku), a = t.computed(() => e.indeterminate === !0 || e.query === !0), i = t.computed(() => e.reverse !== e.query), u = t.computed(() => ({
                 ...r.value !== null ? r.value : {},
                 "--q-linear-progress-speed": `${e.animationSpeed}ms`
-            })), c = t.computed(() => "q-linear-progress" + (e.color !== void 0 ? ` text-${e.color}` : "") + (e.reverse === !0 || e.query === !0 ? " q-linear-progress--reverse" : "") + (e.rounded === !0 ? " rounded-borders" : "")), d = t.computed(() => wr(e.buffer !== void 0 ? e.buffer : 1, i.value, o.$q)), s = t.computed(() => `with${e.instantFeedback===!0?"out":""}-transition`), h = t.computed(() => `q-linear-progress__track absolute-full q-linear-progress__track--${s.value} q-linear-progress__track--${l.value===!0?"dark":"light"}` + (e.trackColor !== void 0 ? ` bg-${e.trackColor}` : "")), f = t.computed(() => wr(a.value === !0 ? 1 : e.value, i.value, o.$q)), m = t.computed(() => `q-linear-progress__model absolute-full q-linear-progress__model--${s.value} q-linear-progress__model--${a.value===!0?"in":""}determinate`), v = t.computed(() => ({
+            })), c = t.computed(() => "q-linear-progress" + (e.color !== void 0 ? ` text-${e.color}` : "") + (e.reverse === !0 || e.query === !0 ? " q-linear-progress--reverse" : "") + (e.rounded === !0 ? " rounded-borders" : "")), d = t.computed(() => wr(e.buffer !== void 0 ? e.buffer : 1, i.value, o.$q)), s = t.computed(() => `with${e.instantFeedback===!0?"out":""}-transition`), m = t.computed(() => `q-linear-progress__track absolute-full q-linear-progress__track--${s.value} q-linear-progress__track--${l.value===!0?"dark":"light"}` + (e.trackColor !== void 0 ? ` bg-${e.trackColor}` : "")), f = t.computed(() => wr(a.value === !0 ? 1 : e.value, i.value, o.$q)), h = t.computed(() => `q-linear-progress__model absolute-full q-linear-progress__model--${s.value} q-linear-progress__model--${a.value===!0?"in":""}determinate`), v = t.computed(() => ({
                 width: `${e.value*100}%`
-            })), x = t.computed(() => `q-linear-progress__stripe absolute-${e.reverse===!0?"right":"left"} q-linear-progress__stripe--${s.value}`);
+            })), _ = t.computed(() => `q-linear-progress__stripe absolute-${e.reverse===!0?"right":"left"} q-linear-progress__stripe--${s.value}`);
             return () => {
                 const p = [t.h("div", {
-                    class: h.value,
+                    class: m.value,
                     style: d.value
                 }), t.h("div", {
-                    class: m.value,
+                    class: h.value,
                     style: f.value
                 })];
                 return e.stripe === !0 && a.value === !1 && p.push(t.h("div", {
-                    class: x.value,
+                    class: _.value,
                     style: v.value
                 })), t.h("div", {
                     class: c.value,
                     style: u.value,
                     role: "progressbar",
                     "aria-valuemin": 0,
                     "aria-valuemax": 1,
@@ -4377,90 +4377,90 @@
             emit: r,
             proxy: a
         } = t.getCurrentInstance(), {
             $q: i
         } = a, u = Fe(o, i), c = t.ref(null), {
             refocusTargetEl: d,
             refocusTarget: s
-        } = qu(o, c), h = Ht(o, Tu), f = t.computed(() => o.val !== void 0 && Array.isArray(o.modelValue)), m = t.computed(() => {
-            const k = t.toRaw(o.val);
-            return f.value === !0 ? o.modelValue.findIndex(O => t.toRaw(O) === k) : -1
-        }), v = t.computed(() => f.value === !0 ? m.value > -1 : t.toRaw(o.modelValue) === t.toRaw(o.trueValue)), x = t.computed(() => f.value === !0 ? m.value === -1 : t.toRaw(o.modelValue) === t.toRaw(o.falseValue)), p = t.computed(() => v.value === !1 && x.value === !1), S = t.computed(() => o.disable === !0 ? -1 : o.tabindex || 0), C = t.computed(() => `q-${e} cursor-pointer no-outline row inline no-wrap items-center` + (o.disable === !0 ? " disabled" : "") + (u.value === !0 ? ` q-${e}--dark` : "") + (o.dense === !0 ? ` q-${e}--dense` : "") + (o.leftLabel === !0 ? " reverse" : "")), y = t.computed(() => {
-            const k = v.value === !0 ? "truthy" : x.value === !0 ? "falsy" : "indet",
-                O = o.color !== void 0 && (o.keepColor === !0 || (e === "toggle" ? v.value === !0 : x.value !== !0)) ? ` text-${o.color}` : "";
-            return `q-${e}__inner relative-position non-selectable q-${e}__inner--${k}${O}`
-        }), P = t.computed(() => {
-            const k = {
+        } = qu(o, c), m = Ht(o, Tu), f = t.computed(() => o.val !== void 0 && Array.isArray(o.modelValue)), h = t.computed(() => {
+            const x = t.toRaw(o.val);
+            return f.value === !0 ? o.modelValue.findIndex(O => t.toRaw(O) === x) : -1
+        }), v = t.computed(() => f.value === !0 ? h.value > -1 : t.toRaw(o.modelValue) === t.toRaw(o.trueValue)), _ = t.computed(() => f.value === !0 ? h.value === -1 : t.toRaw(o.modelValue) === t.toRaw(o.falseValue)), p = t.computed(() => v.value === !1 && _.value === !1), k = t.computed(() => o.disable === !0 ? -1 : o.tabindex || 0), q = t.computed(() => `q-${e} cursor-pointer no-outline row inline no-wrap items-center` + (o.disable === !0 ? " disabled" : "") + (u.value === !0 ? ` q-${e}--dark` : "") + (o.dense === !0 ? ` q-${e}--dense` : "") + (o.leftLabel === !0 ? " reverse" : "")), w = t.computed(() => {
+            const x = v.value === !0 ? "truthy" : _.value === !0 ? "falsy" : "indet",
+                O = o.color !== void 0 && (o.keepColor === !0 || (e === "toggle" ? v.value === !0 : _.value !== !0)) ? ` text-${o.color}` : "";
+            return `q-${e}__inner relative-position non-selectable q-${e}__inner--${x}${O}`
+        }), C = t.computed(() => {
+            const x = {
                 type: "checkbox"
             };
-            return o.name !== void 0 && Object.assign(k, {
+            return o.name !== void 0 && Object.assign(x, {
                 ".checked": v.value,
                 "^checked": v.value === !0 ? "checked" : void 0,
                 name: o.name,
                 value: f.value === !0 ? o.val : o.trueValue
-            }), k
-        }), A = tu(P), M = t.computed(() => {
-            const k = {
-                tabindex: S.value,
+            }), x
+        }), A = tu(C), M = t.computed(() => {
+            const x = {
+                tabindex: k.value,
                 role: e === "toggle" ? "switch" : "checkbox",
                 "aria-label": o.label,
                 "aria-checked": p.value === !0 ? "mixed" : v.value === !0 ? "true" : "false"
             };
-            return o.disable === !0 && (k["aria-disabled"] = "true"), k
+            return o.disable === !0 && (x["aria-disabled"] = "true"), x
         });
 
-        function V(k) {
-            k !== void 0 && (ve(k), s(k)), o.disable !== !0 && r("update:modelValue", R(), k)
+        function V(x) {
+            x !== void 0 && (ve(x), s(x)), o.disable !== !0 && r("update:modelValue", R(), x)
         }
 
         function R() {
             if (f.value === !0) {
                 if (v.value === !0) {
-                    const k = o.modelValue.slice();
-                    return k.splice(m.value, 1), k
+                    const x = o.modelValue.slice();
+                    return x.splice(h.value, 1), x
                 }
                 return o.modelValue.concat([o.val])
             }
             if (v.value === !0) {
                 if (o.toggleOrder !== "ft" || o.toggleIndeterminate === !1) return o.falseValue
-            } else if (x.value === !0) {
+            } else if (_.value === !0) {
                 if (o.toggleOrder === "ft" || o.toggleIndeterminate === !1) return o.trueValue
             } else return o.toggleOrder !== "ft" ? o.trueValue : o.falseValue;
             return o.indeterminateValue
         }
 
-        function T(k) {
-            (k.keyCode === 13 || k.keyCode === 32) && ve(k)
+        function B(x) {
+            (x.keyCode === 13 || x.keyCode === 32) && ve(x)
         }
 
-        function B(k) {
-            (k.keyCode === 13 || k.keyCode === 32) && V(k)
+        function P(x) {
+            (x.keyCode === 13 || x.keyCode === 32) && V(x)
         }
         const I = n(v, p);
         return Object.assign(a, {
             toggle: V
         }), () => {
-            const k = I();
-            o.disable !== !0 && A(k, "unshift", ` q-${e}__native absolute q-ma-none q-pa-none`);
+            const x = I();
+            o.disable !== !0 && A(x, "unshift", ` q-${e}__native absolute q-ma-none q-pa-none`);
             const O = [t.h("div", {
-                class: y.value,
-                style: h.value,
+                class: w.value,
+                style: m.value,
                 "aria-hidden": "true"
-            }, k)];
+            }, x)];
             d.value !== null && O.push(d.value);
-            const q = o.label !== void 0 ? Ke(l.default, [o.label]) : we(l.default);
-            return q !== void 0 && O.push(t.h("div", {
+            const T = o.label !== void 0 ? Ke(l.default, [o.label]) : we(l.default);
+            return T !== void 0 && O.push(t.h("div", {
                 class: `q-${e}__label q-anchor--skip`
-            }, q)), t.h("div", {
+            }, T)), t.h("div", {
                 ref: c,
-                class: C.value,
+                class: q.value,
                 ...M.value,
                 onClick: V,
-                onKeydown: T,
-                onKeyup: B
+                onKeydown: B,
+                onKeyup: P
             }, O)
         }
     }
     const Bu = t.h("div", {
             key: "svg",
             class: "q-checkbox__bg absolute"
         }, [t.h("svg", {
@@ -4470,15 +4470,15 @@
             class: "q-checkbox__truthy",
             fill: "none",
             d: "M1.73,12.91 8.1,19.28 22.79,4.59"
         }), t.h("path", {
             class: "q-checkbox__indet",
             d: "M4,14H20V10H4"
         })])]),
-        ko = se({
+        Co = se({
             name: "QCheckbox",
             props: Sr,
             emits: _r,
             setup(e) {
                 function n(o, l) {
                     const r = t.computed(() => (o.value === !0 ? e.checkedIcon : l.value === !0 ? e.indeterminateIcon : e.uncheckedIcon) || null);
                     return () => r.value !== null ? [t.h("div", {
@@ -4532,15 +4532,15 @@
         },
         Ou = ["button", "submit", "reset"],
         Mu = /[^\s]\/[^\s]/,
         Ru = ["flat", "outline", "push", "unelevated"],
         Vu = (e, n) => e.flat === !0 ? "flat" : e.outline === !0 ? "outline" : e.push === !0 ? "push" : e.unelevated === !0 ? "unelevated" : n,
         Iu = {
             ...Nt,
-            ...Bl,
+            ...Pl,
             type: {
                 type: String,
                 default: "button"
             },
             label: [Number, String],
             icon: String,
             iconRight: String,
@@ -4581,52 +4581,52 @@
             o = $u(e),
             {
                 hasRouterLink: l,
                 hasLink: r,
                 linkTag: a,
                 linkAttrs: i,
                 navigateOnClick: u
-            } = Pl({
+            } = El({
                 fallbackTag: "button"
             }),
             c = t.computed(() => {
                 const p = e.fab === !1 && e.fabMini === !1 ? n.value : {};
                 return e.padding !== void 0 ? Object.assign({}, p, {
-                    padding: e.padding.split(/\s+/).map(S => S in Cr ? Cr[S] + "px" : S).join(" "),
+                    padding: e.padding.split(/\s+/).map(k => k in Cr ? Cr[k] + "px" : k).join(" "),
                     minWidth: "0",
                     minHeight: "0"
                 }) : p
             }),
             d = t.computed(() => e.rounded === !0 || e.fab === !0 || e.fabMini === !0),
             s = t.computed(() => e.disable !== !0 && e.loading !== !0),
-            h = t.computed(() => s.value === !0 ? e.tabindex || 0 : -1),
+            m = t.computed(() => s.value === !0 ? e.tabindex || 0 : -1),
             f = t.computed(() => Vu(e, "standard")),
-            m = t.computed(() => {
+            h = t.computed(() => {
                 const p = {
-                    tabindex: h.value
+                    tabindex: m.value
                 };
                 return r.value === !0 ? Object.assign(p, i.value) : Ou.includes(e.type) === !0 && (p.type = e.type), a.value === "a" ? (e.disable === !0 ? p["aria-disabled"] = "true" : p.href === void 0 && (p.role = "button"), l.value !== !0 && Mu.test(e.type) === !0 && (p.type = e.type)) : e.disable === !0 && (p.disabled = "", p["aria-disabled"] = "true"), e.loading === !0 && e.percentage !== void 0 && Object.assign(p, {
                     role: "progressbar",
                     "aria-valuemin": 0,
                     "aria-valuemax": 100,
                     "aria-valuenow": e.percentage
                 }), p
             }),
             v = t.computed(() => {
                 let p;
                 e.color !== void 0 ? e.flat === !0 || e.outline === !0 ? p = `text-${e.textColor||e.color}` : p = `bg-${e.color} text-${e.textColor||"white"}` : e.textColor && (p = `text-${e.textColor}`);
-                const S = e.round === !0 ? "round" : `rectangle${d.value===!0?" q-btn--rounded":e.square===!0?" q-btn--square":""}`;
-                return `q-btn--${f.value} q-btn--${S}` + (p !== void 0 ? " " + p : "") + (s.value === !0 ? " q-btn--actionable q-focusable q-hoverable" : e.disable === !0 ? " disabled" : "") + (e.fab === !0 ? " q-btn--fab" : e.fabMini === !0 ? " q-btn--fab-mini" : "") + (e.noCaps === !0 ? " q-btn--no-uppercase" : "") + (e.dense === !0 ? " q-btn--dense" : "") + (e.stretch === !0 ? " no-border-radius self-stretch" : "") + (e.glossy === !0 ? " glossy" : "") + (e.square ? " q-btn--square" : "")
+                const k = e.round === !0 ? "round" : `rectangle${d.value===!0?" q-btn--rounded":e.square===!0?" q-btn--square":""}`;
+                return `q-btn--${f.value} q-btn--${k}` + (p !== void 0 ? " " + p : "") + (s.value === !0 ? " q-btn--actionable q-focusable q-hoverable" : e.disable === !0 ? " disabled" : "") + (e.fab === !0 ? " q-btn--fab" : e.fabMini === !0 ? " q-btn--fab-mini" : "") + (e.noCaps === !0 ? " q-btn--no-uppercase" : "") + (e.dense === !0 ? " q-btn--dense" : "") + (e.stretch === !0 ? " no-border-radius self-stretch" : "") + (e.glossy === !0 ? " glossy" : "") + (e.square ? " q-btn--square" : "")
             }),
-            x = t.computed(() => o.value + (e.stack === !0 ? " column" : " row") + (e.noWrap === !0 ? " no-wrap text-no-wrap" : "") + (e.loading === !0 ? " q-btn__content--hidden" : ""));
+            _ = t.computed(() => o.value + (e.stack === !0 ? " column" : " row") + (e.noWrap === !0 ? " no-wrap text-no-wrap" : "") + (e.loading === !0 ? " q-btn__content--hidden" : ""));
         return {
             classes: v,
             style: c,
-            innerClasses: x,
-            attributes: m,
+            innerClasses: _,
+            attributes: h,
             hasLink: r,
             linkTag: a,
             navigateOnClick: u,
             isActionable: s
         }
     }
     const {
@@ -4654,154 +4654,154 @@
                 classes: r,
                 style: a,
                 innerClasses: i,
                 attributes: u,
                 hasLink: c,
                 linkTag: d,
                 navigateOnClick: s,
-                isActionable: h
-            } = zu(e), f = t.ref(null), m = t.ref(null);
+                isActionable: m
+            } = zu(e), f = t.ref(null), h = t.ref(null);
             let v = null,
-                x, p = null;
-            const S = t.computed(() => e.label !== void 0 && e.label !== null && e.label !== ""),
-                C = t.computed(() => e.disable === !0 || e.ripple === !1 ? !1 : {
+                _, p = null;
+            const k = t.computed(() => e.label !== void 0 && e.label !== null && e.label !== ""),
+                q = t.computed(() => e.disable === !0 || e.ripple === !1 ? !1 : {
                     keyCodes: c.value === !0 ? [13, 32] : [13],
                     ...e.ripple === !0 ? {} : e.ripple
                 }),
-                y = t.computed(() => ({
+                w = t.computed(() => ({
                     center: e.round
                 })),
-                P = t.computed(() => {
-                    const q = Math.max(0, Math.min(100, e.percentage));
-                    return q > 0 ? {
+                C = t.computed(() => {
+                    const T = Math.max(0, Math.min(100, e.percentage));
+                    return T > 0 ? {
                         transition: "transform 0.6s",
-                        transform: `translateX(${q-100}%)`
+                        transform: `translateX(${T-100}%)`
                     } : {}
                 }),
                 A = t.computed(() => {
                     if (e.loading === !0) return {
                         onMousedown: O,
                         onTouchstart: O,
                         onClick: O,
                         onKeydown: O,
                         onKeyup: O
                     };
-                    if (h.value === !0) {
-                        const q = {
+                    if (m.value === !0) {
+                        const T = {
                             onClick: V,
                             onKeydown: R,
-                            onMousedown: B
+                            onMousedown: P
                         };
                         if (l.$q.platform.has.touch === !0) {
                             const j = e.onTouchstart !== void 0 ? "" : "Passive";
-                            q[`onTouchstart${j}`] = T
+                            T[`onTouchstart${j}`] = B
                         }
-                        return q
+                        return T
                     }
                     return {
                         onClick: ve
                     }
                 }),
                 M = t.computed(() => ({
                     ref: f,
                     class: "q-btn q-btn-item non-selectable no-outline " + r.value,
                     style: a.value,
                     ...u.value,
                     ...A.value
                 }));
 
-            function V(q) {
+            function V(T) {
                 if (f.value !== null) {
-                    if (q !== void 0) {
-                        if (q.defaultPrevented === !0) return;
+                    if (T !== void 0) {
+                        if (T.defaultPrevented === !0) return;
                         const j = document.activeElement;
                         if (e.type === "submit" && j !== document.body && f.value.contains(j) === !1 && j.contains(f.value) === !1) {
                             f.value.focus();
                             const N = () => {
                                 document.removeEventListener("keydown", ve, !0), document.removeEventListener("keyup", N, He), f.value !== null && f.value.removeEventListener("blur", N, He)
                             };
                             document.addEventListener("keydown", ve, !0), document.addEventListener("keyup", N, He), f.value.addEventListener("blur", N, He)
                         }
                     }
-                    s(q)
+                    s(T)
                 }
             }
 
-            function R(q) {
-                f.value !== null && (o("keydown", q), ut(q, [13, 32]) === !0 && Et !== f.value && (Et !== null && k(), q.defaultPrevented !== !0 && (f.value.focus(), Et = f.value, f.value.classList.add("q-btn--active"), document.addEventListener("keyup", I, !0), f.value.addEventListener("blur", I, He)), ve(q)))
+            function R(T) {
+                f.value !== null && (o("keydown", T), ut(T, [13, 32]) === !0 && Et !== f.value && (Et !== null && x(), T.defaultPrevented !== !0 && (f.value.focus(), Et = f.value, f.value.classList.add("q-btn--active"), document.addEventListener("keyup", I, !0), f.value.addEventListener("blur", I, He)), ve(T)))
             }
 
-            function T(q) {
-                f.value !== null && (o("touchstart", q), q.defaultPrevented !== !0 && (Pt !== f.value && (Pt !== null && k(), Pt = f.value, v = q.target, v.addEventListener("touchcancel", I, He), v.addEventListener("touchend", I, He)), x = !0, p !== null && clearTimeout(p), p = setTimeout(() => {
-                    p = null, x = !1
+            function B(T) {
+                f.value !== null && (o("touchstart", T), T.defaultPrevented !== !0 && (Pt !== f.value && (Pt !== null && x(), Pt = f.value, v = T.target, v.addEventListener("touchcancel", I, He), v.addEventListener("touchend", I, He)), _ = !0, p !== null && clearTimeout(p), p = setTimeout(() => {
+                    p = null, _ = !1
                 }, 200)))
             }
 
-            function B(q) {
-                f.value !== null && (q.qSkipRipple = x === !0, o("mousedown", q), q.defaultPrevented !== !0 && $t !== f.value && ($t !== null && k(), $t = f.value, f.value.classList.add("q-btn--active"), document.addEventListener("mouseup", I, He)))
+            function P(T) {
+                f.value !== null && (T.qSkipRipple = _ === !0, o("mousedown", T), T.defaultPrevented !== !0 && $t !== f.value && ($t !== null && x(), $t = f.value, f.value.classList.add("q-btn--active"), document.addEventListener("mouseup", I, He)))
             }
 
-            function I(q) {
-                if (f.value !== null && !(q !== void 0 && q.type === "blur" && document.activeElement === f.value)) {
-                    if (q !== void 0 && q.type === "keyup") {
-                        if (Et === f.value && ut(q, [13, 32]) === !0) {
-                            const j = new MouseEvent("click", q);
-                            j.qKeyEvent = !0, q.defaultPrevented === !0 && $e(j), q.cancelBubble === !0 && De(j), f.value.dispatchEvent(j), ve(q), q.qKeyEvent = !0
+            function I(T) {
+                if (f.value !== null && !(T !== void 0 && T.type === "blur" && document.activeElement === f.value)) {
+                    if (T !== void 0 && T.type === "keyup") {
+                        if (Et === f.value && ut(T, [13, 32]) === !0) {
+                            const j = new MouseEvent("click", T);
+                            j.qKeyEvent = !0, T.defaultPrevented === !0 && $e(j), T.cancelBubble === !0 && De(j), f.value.dispatchEvent(j), ve(T), T.qKeyEvent = !0
                         }
-                        o("keyup", q)
+                        o("keyup", T)
                     }
-                    k()
+                    x()
                 }
             }
 
-            function k(q) {
-                const j = m.value;
-                q !== !0 && (Pt === f.value || $t === f.value) && j !== null && j !== document.activeElement && (j.setAttribute("tabindex", -1), j.focus()), Pt === f.value && (v !== null && (v.removeEventListener("touchcancel", I, He), v.removeEventListener("touchend", I, He)), Pt = v = null), $t === f.value && (document.removeEventListener("mouseup", I, He), $t = null), Et === f.value && (document.removeEventListener("keyup", I, !0), f.value !== null && f.value.removeEventListener("blur", I, He), Et = null), f.value !== null && f.value.classList.remove("q-btn--active")
+            function x(T) {
+                const j = h.value;
+                T !== !0 && (Pt === f.value || $t === f.value) && j !== null && j !== document.activeElement && (j.setAttribute("tabindex", -1), j.focus()), Pt === f.value && (v !== null && (v.removeEventListener("touchcancel", I, He), v.removeEventListener("touchend", I, He)), Pt = v = null), $t === f.value && (document.removeEventListener("mouseup", I, He), $t = null), Et === f.value && (document.removeEventListener("keyup", I, !0), f.value !== null && f.value.removeEventListener("blur", I, He), Et = null), f.value !== null && f.value.classList.remove("q-btn--active")
             }
 
-            function O(q) {
-                ve(q), q.qSkipRipple = !0
+            function O(T) {
+                ve(T), T.qSkipRipple = !0
             }
             return t.onBeforeUnmount(() => {
-                k(!0)
+                x(!0)
             }), Object.assign(l, {
                 click: V
             }), () => {
-                let q = [];
-                e.icon !== void 0 && q.push(t.h(Be, {
+                let T = [];
+                e.icon !== void 0 && T.push(t.h(Be, {
                     name: e.icon,
-                    left: e.stack === !1 && S.value === !0,
+                    left: e.stack === !1 && k.value === !0,
                     role: "img",
                     "aria-hidden": "true"
-                })), S.value === !0 && q.push(t.h("span", {
+                })), k.value === !0 && T.push(t.h("span", {
                     class: "block"
-                }, [e.label])), q = Ke(n.default, q), e.iconRight !== void 0 && e.round === !1 && q.push(t.h(Be, {
+                }, [e.label])), T = Ke(n.default, T), e.iconRight !== void 0 && e.round === !1 && T.push(t.h(Be, {
                     name: e.iconRight,
-                    right: e.stack === !1 && S.value === !0,
+                    right: e.stack === !1 && k.value === !0,
                     role: "img",
                     "aria-hidden": "true"
                 }));
                 const j = [t.h("span", {
                     class: "q-focus-helper",
-                    ref: m
+                    ref: h
                 })];
                 return e.loading === !0 && e.percentage !== void 0 && j.push(t.h("span", {
                     class: "q-btn__progress absolute-full overflow-hidden" + (e.darkPercentage === !0 ? " q-btn__progress--dark" : "")
                 }, [t.h("span", {
                     class: "q-btn__progress-indicator fit block",
-                    style: P.value
+                    style: C.value
                 })])), j.push(t.h("span", {
                     class: "q-btn__content text-center col items-center q-anchor--skip " + i.value
-                }, q)), e.loading !== null && j.push(t.h(t.Transition, {
+                }, T)), e.loading !== null && j.push(t.h(t.Transition, {
                     name: "q-transition--fade"
                 }, () => e.loading === !0 ? [t.h("span", {
                     key: "loading",
                     class: "absolute-full flex flex-center"
                 }, n.loading !== void 0 ? n.loading() : [t.h(Nn)])] : null)), t.withDirectives(t.h(d.value, M.value, j), [
-                    [Zn, C.value, void 0, y.value]
+                    [Zn, q.value, void 0, w.value]
                 ])
             }
         }
     });
     let tn = 0;
     const Lu = {
             fullscreen: Boolean,
@@ -4870,31 +4870,31 @@
         const r = t.computed(() => {
                 const {
                     sortBy: u
                 } = n.value;
                 return u && o.value.find(c => c.name === u) || null
             }),
             a = t.computed(() => e.sortMethod !== void 0 ? e.sortMethod : (u, c, d) => {
-                const s = o.value.find(m => m.name === c);
+                const s = o.value.find(h => h.name === c);
                 if (s === void 0 || s.field === void 0) return u;
-                const h = d === !0 ? -1 : 1,
-                    f = typeof s.field == "function" ? m => s.field(m) : m => m[s.field];
-                return u.sort((m, v) => {
-                    let x = f(m),
+                const m = d === !0 ? -1 : 1,
+                    f = typeof s.field == "function" ? h => s.field(h) : h => h[s.field];
+                return u.sort((h, v) => {
+                    let _ = f(h),
                         p = f(v);
-                    return s.rawSort !== void 0 ? s.rawSort(x, p, m, v) * h : x == null ? -1 * h : p == null ? 1 * h : s.sort !== void 0 ? s.sort(x, p, m, v) * h : So(x) === !0 && So(p) === !0 ? (x - p) * h : fr(x) === !0 && fr(p) === !0 ? ju(x, p) * h : typeof x == "boolean" && typeof p == "boolean" ? (x - p) * h : ([x, p] = [x, p].map(S => (S + "").toLocaleString().toLowerCase()), x < p ? -1 * h : x === p ? 0 : h)
+                    return s.rawSort !== void 0 ? s.rawSort(_, p, h, v) * m : _ == null ? -1 * m : p == null ? 1 * m : s.sort !== void 0 ? s.sort(_, p, h, v) * m : So(_) === !0 && So(p) === !0 ? (_ - p) * m : mr(_) === !0 && mr(p) === !0 ? ju(_, p) * m : typeof _ == "boolean" && typeof p == "boolean" ? (_ - p) * m : ([_, p] = [_, p].map(k => (k + "").toLocaleString().toLowerCase()), _ < p ? -1 * m : _ === p ? 0 : m)
                 })
             });
 
         function i(u) {
             let c = e.columnSortOrder;
             if (au(u) === !0) u.sortOrder && (c = u.sortOrder), u = u.name;
             else {
-                const h = o.value.find(f => f.name === u);
-                h !== void 0 && h.sortOrder && (c = h.sortOrder)
+                const m = o.value.find(f => f.name === u);
+                m !== void 0 && m.sortOrder && (c = m.sortOrder)
             }
             let {
                 sortBy: d,
                 descending: s
             } = n.value;
             d !== u ? (d = u, s = c === "da") : e.binaryStateSort === !0 ? s = !s : s === !0 ? c === "ad" ? d = null : s = !1 : c === "ad" ? s = !0 : d = null, l({
                 sortBy: d,
@@ -4982,21 +4982,21 @@
                     pagination: s.pagination || a.value,
                     filter: s.filter || o.filter,
                     getCellValue: n
                 })
             })
         }
 
-        function d(s, h) {
+        function d(s, m) {
             const f = qr({
                 ...a.value,
                 ...s
             });
             if (Ku(a.value, f) === !0) {
-                i.value === !0 && h === !0 && u(f);
+                i.value === !0 && m === !0 && u(f);
                 return
             }
             if (i.value === !0) {
                 u(f);
                 return
             }
             o.pagination !== void 0 && o["onUpdate:pagination"] !== void 0 ? l("update:pagination", f) : r.value = f
@@ -5015,82 +5015,82 @@
             props: i,
             emit: u,
             proxy: {
                 $q: c
             }
         } = e, d = t.computed(() => l.value === !0 ? o.value.rowsNumber || 0 : a.value), s = t.computed(() => {
             const {
-                page: P,
+                page: C,
                 rowsPerPage: A
             } = o.value;
-            return (P - 1) * A
-        }), h = t.computed(() => {
+            return (C - 1) * A
+        }), m = t.computed(() => {
             const {
-                page: P,
+                page: C,
                 rowsPerPage: A
             } = o.value;
-            return P * A
-        }), f = t.computed(() => o.value.page === 1), m = t.computed(() => o.value.rowsPerPage === 0 ? 1 : Math.max(1, Math.ceil(d.value / o.value.rowsPerPage))), v = t.computed(() => h.value === 0 ? !0 : o.value.page >= m.value), x = t.computed(() => (i.rowsPerPageOptions.includes(n.value.rowsPerPage) ? i.rowsPerPageOptions : [n.value.rowsPerPage].concat(i.rowsPerPageOptions)).map(A => ({
+            return C * A
+        }), f = t.computed(() => o.value.page === 1), h = t.computed(() => o.value.rowsPerPage === 0 ? 1 : Math.max(1, Math.ceil(d.value / o.value.rowsPerPage))), v = t.computed(() => m.value === 0 ? !0 : o.value.page >= h.value), _ = t.computed(() => (i.rowsPerPageOptions.includes(n.value.rowsPerPage) ? i.rowsPerPageOptions : [n.value.rowsPerPage].concat(i.rowsPerPageOptions)).map(A => ({
             label: A === 0 ? c.lang.table.allRows : "" + A,
             value: A
         })));
-        t.watch(m, (P, A) => {
-            if (P === A) return;
+        t.watch(h, (C, A) => {
+            if (C === A) return;
             const M = o.value.page;
-            P && !M ? r({
+            C && !M ? r({
                 page: 1
-            }) : P < M && r({
-                page: P
+            }) : C < M && r({
+                page: C
             })
         });
 
         function p() {
             r({
                 page: 1
             })
         }
 
-        function S() {
+        function k() {
             const {
-                page: P
+                page: C
             } = o.value;
-            P > 1 && r({
-                page: P - 1
+            C > 1 && r({
+                page: C - 1
             })
         }
 
-        function C() {
+        function q() {
             const {
-                page: P,
+                page: C,
                 rowsPerPage: A
             } = o.value;
-            h.value > 0 && P * A < d.value && r({
-                page: P + 1
+            m.value > 0 && C * A < d.value && r({
+                page: C + 1
             })
         }
 
-        function y() {
+        function w() {
             r({
-                page: m.value
+                page: h.value
             })
         }
         return i["onUpdate:pagination"] !== void 0 && u("update:pagination", {
             ...o.value
         }), {
             firstRowIndex: s,
-            lastRowIndex: h,
+            lastRowIndex: m,
             isFirstPage: f,
             isLastPage: v,
-            pagesNumber: m,
-            computedRowsPerPageOptions: x,
+            pagesNumber: h,
+            computedRowsPerPageOptions: _,
             computedRowsNumber: d,
             firstPage: p,
-            prevPage: S,
-            nextPage: C,
-            lastPage: y
+            prevPage: k,
+            nextPage: q,
+            lastPage: w
         }
     }
     const Yu = {
             selection: {
                 type: String,
                 default: "none",
                 validator: e => ["single", "multiple", "none"].includes(e)
@@ -5101,53 +5101,53 @@
             }
         },
         Zu = ["update:selected", "selection"];
 
     function Ju(e, n, o, l) {
         const r = t.computed(() => {
                 const v = {};
-                return e.selected.map(l.value).forEach(x => {
-                    v[x] = !0
+                return e.selected.map(l.value).forEach(_ => {
+                    v[_] = !0
                 }), v
             }),
             a = t.computed(() => e.selection !== "none"),
             i = t.computed(() => e.selection === "single"),
             u = t.computed(() => e.selection === "multiple"),
             c = t.computed(() => o.value.length !== 0 && o.value.every(v => r.value[l.value(v)] === !0)),
             d = t.computed(() => c.value !== !0 && o.value.some(v => r.value[l.value(v)] === !0)),
             s = t.computed(() => e.selected.length);
 
-        function h(v) {
+        function m(v) {
             return r.value[v] === !0
         }
 
         function f() {
             n("update:selected", [])
         }
 
-        function m(v, x, p, S) {
+        function h(v, _, p, k) {
             n("selection", {
-                rows: x,
+                rows: _,
                 added: p,
                 keys: v,
-                evt: S
+                evt: k
             });
-            const C = i.value === !0 ? p === !0 ? x : [] : p === !0 ? e.selected.concat(x) : e.selected.filter(y => v.includes(l.value(y)) === !1);
-            n("update:selected", C)
+            const q = i.value === !0 ? p === !0 ? _ : [] : p === !0 ? e.selected.concat(_) : e.selected.filter(w => v.includes(l.value(w)) === !1);
+            n("update:selected", q)
         }
         return {
             hasSelectionMode: a,
             singleSelection: i,
             multipleSelection: u,
             allRowsSelected: c,
             someRowsSelected: d,
             rowsSelectedNumber: s,
-            isRowSelected: h,
+            isRowSelected: m,
             clearSelection: f,
-            updateSelection: m
+            updateSelection: h
         }
     }
 
     function Tr(e) {
         return Array.isArray(e) ? e.slice() : []
     }
     const es = {
@@ -5198,23 +5198,23 @@
             }),
             r = t.computed(() => {
                 const {
                     sortBy: u,
                     descending: c
                 } = n.value;
                 return (e.visibleColumns !== void 0 ? l.value.filter(s => s.required === !0 || e.visibleColumns.includes(s.name) === !0) : l.value).map(s => {
-                    const h = s.align || "right",
-                        f = `text-${h}`;
+                    const m = s.align || "right",
+                        f = `text-${m}`;
                     return {
                         ...s,
-                        align: h,
-                        __iconClass: `q-table__sort-icon q-table__sort-icon--${h}`,
+                        align: m,
+                        __iconClass: `q-table__sort-icon q-table__sort-icon--${m}`,
                         __thClass: f + (s.headerClasses !== void 0 ? " " + s.headerClasses : "") + (s.sortable === !0 ? " sortable" : "") + (s.name === u ? ` sorted ${c===!0?"sort-desc":""}` : ""),
                         __tdStyle: s.style !== void 0 ? typeof s.style != "function" ? () => s.style : s.style : () => null,
-                        __tdClass: s.classes !== void 0 ? typeof s.classes != "function" ? () => f + " " + s.classes : m => f + " " + s.classes(m) : () => f
+                        __tdClass: s.classes !== void 0 ? typeof s.classes != "function" ? () => f + " " + s.classes : h => f + " " + s.classes(h) : () => f
                     }
                 })
             }),
             a = t.computed(() => {
                 const u = {};
                 return r.value.forEach(c => {
                     u[c.name] = c
@@ -5226,15 +5226,15 @@
             computedCols: r,
             computedColsMap: a,
             computedColspan: i
         }
     }
     const Cn = "q-table__bottom row items-center",
         Br = {};
-    ir.forEach(e => {
+    ur.forEach(e => {
         Br[e] = {}
     });
     const rs = se({
         name: "QTable",
         props: {
             rows: {
                 type: Array,
@@ -5319,114 +5319,114 @@
                 {
                     inFullscreen: i,
                     toggleFullscreen: u
                 } = Du(),
                 c = t.computed(() => typeof e.rowKey == "function" ? e.rowKey : $ => $[e.rowKey]),
                 d = t.ref(null),
                 s = t.ref(null),
-                h = t.computed(() => e.grid !== !0 && e.virtualScroll === !0),
+                m = t.computed(() => e.grid !== !0 && e.virtualScroll === !0),
                 f = t.computed(() => " q-table__card" + (a.value === !0 ? " q-table__card--dark q-dark" : "") + (e.square === !0 ? " q-table--square" : "") + (e.flat === !0 ? " q-table--flat" : "") + (e.bordered === !0 ? " q-table--bordered" : "")),
-                m = t.computed(() => `q-table__container q-table--${e.separator}-separator column no-wrap` + (e.grid === !0 ? " q-table--grid" : f.value) + (a.value === !0 ? " q-table--dark" : "") + (e.dense === !0 ? " q-table--dense" : "") + (e.wrapCells === !1 ? " q-table--no-wrap" : "") + (i.value === !0 ? " fullscreen scroll" : "")),
-                v = t.computed(() => m.value + (e.loading === !0 ? " q-table--loading" : ""));
-            t.watch(() => e.tableStyle + e.tableClass + e.tableHeaderStyle + e.tableHeaderClass + m.value, () => {
-                h.value === !0 && s.value !== null && s.value.reset()
+                h = t.computed(() => `q-table__container q-table--${e.separator}-separator column no-wrap` + (e.grid === !0 ? " q-table--grid" : f.value) + (a.value === !0 ? " q-table--dark" : "") + (e.dense === !0 ? " q-table--dense" : "") + (e.wrapCells === !1 ? " q-table--no-wrap" : "") + (i.value === !0 ? " fullscreen scroll" : "")),
+                v = t.computed(() => h.value + (e.loading === !0 ? " q-table--loading" : ""));
+            t.watch(() => e.tableStyle + e.tableClass + e.tableHeaderStyle + e.tableHeaderClass + h.value, () => {
+                m.value === !0 && s.value !== null && s.value.reset()
             });
             const {
-                innerPagination: x,
+                innerPagination: _,
                 computedPagination: p,
-                isServerSide: S,
-                requestServerInteraction: C,
-                setPagination: y
+                isServerSide: k,
+                requestServerInteraction: q,
+                setPagination: w
             } = Gu(l, Me), {
-                computedFilterMethod: P
-            } = Wu(e, y), {
+                computedFilterMethod: C
+            } = Wu(e, w), {
                 isRowExpanded: A,
                 setExpanded: M,
                 updateExpanded: V
             } = ns(e, o), R = t.computed(() => {
                 let $ = e.rows;
-                if (S.value === !0 || $.length === 0) return $;
+                if (k.value === !0 || $.length === 0) return $;
                 const {
                     sortBy: X,
                     descending: ee
                 } = p.value;
-                return e.filter && ($ = P.value($, e.filter, _.value, Me)), te.value !== null && ($ = U.value(e.rows === $ ? $.slice() : $, X, ee)), $
-            }), T = t.computed(() => R.value.length), B = t.computed(() => {
+                return e.filter && ($ = C.value($, e.filter, S.value, Me)), te.value !== null && ($ = U.value(e.rows === $ ? $.slice() : $, X, ee)), $
+            }), B = t.computed(() => R.value.length), P = t.computed(() => {
                 let $ = R.value;
-                if (S.value === !0) return $;
+                if (k.value === !0) return $;
                 const {
                     rowsPerPage: X
                 } = p.value;
                 return X !== 0 && (Z.value === 0 && e.rows !== $ ? $.length > ue.value && ($ = $.slice(0, ue.value)) : $ = $.slice(Z.value, ue.value)), $
             }), {
                 hasSelectionMode: I,
-                singleSelection: k,
+                singleSelection: x,
                 multipleSelection: O,
-                allRowsSelected: q,
+                allRowsSelected: T,
                 someRowsSelected: j,
                 rowsSelectedNumber: N,
-                isRowSelected: w,
+                isRowSelected: y,
                 clearSelection: z,
                 updateSelection: G
-            } = Ju(e, o, B, c), {
+            } = Ju(e, o, P, c), {
                 colList: J,
-                computedCols: _,
+                computedCols: S,
                 computedColsMap: b,
                 computedColspan: H
             } = ls(e, p, I), {
                 columnToSort: te,
                 computedSortMethod: U,
                 sort: F
-            } = Hu(e, p, J, y), {
+            } = Hu(e, p, J, w), {
                 firstRowIndex: Z,
                 lastRowIndex: ue,
                 isFirstPage: D,
                 isLastPage: fe,
                 pagesNumber: ke,
                 computedRowsPerPageOptions: Ie,
                 computedRowsNumber: ce,
                 firstPage: ye,
                 prevPage: Te,
                 nextPage: Ae,
                 lastPage: Ue
-            } = Xu(l, x, p, S, y, T), je = t.computed(() => B.value.length === 0), We = t.computed(() => {
+            } = Xu(l, _, p, k, w, B), je = t.computed(() => P.value.length === 0), We = t.computed(() => {
                 const $ = {};
-                return ir.forEach(X => {
+                return ur.forEach(X => {
                     $[X] = e[X]
                 }), $.virtualScrollItemSize === void 0 && ($.virtualScrollItemSize = e.dense === !0 ? 28 : 48), $
             });
 
             function Ce() {
-                h.value === !0 && s.value.reset()
+                m.value === !0 && s.value.reset()
             }
 
             function L() {
                 if (e.grid === !0) return In();
                 const $ = e.hideHeader !== !0 ? Rt : null;
-                if (h.value === !0) {
+                if (m.value === !0) {
                     const ee = n["top-row"],
                         ne = n["bottom-row"],
                         le = {
                             default: be => re(be.item, n.body, be.index)
                         };
                     if (ee !== void 0) {
                         const be = t.h("tbody", ee({
-                            cols: _.value
+                            cols: S.value
                         }));
                         le.before = $ === null ? () => be : () => [$()].concat(be)
                     } else $ !== null && (le.before = $);
                     return ne !== void 0 && (le.after = () => t.h("tbody", ne({
-                        cols: _.value
+                        cols: S.value
                     }))), t.h(xu, {
                         ref: s,
                         class: e.tableClass,
                         style: e.tableStyle,
                         ...We.value,
                         scrollTarget: e.virtualScrollTarget,
-                        items: B.value,
+                        items: P.value,
                         type: "__qtable",
                         tableColspan: H.value,
                         onVirtualScroll: E
                     }, le)
                 }
                 const X = [ie()];
                 return $ !== null && X.unshift($()), yr({
@@ -5445,15 +5445,15 @@
                 if (ee !== null) {
                     const ne = d.value.querySelector(".q-table__middle.scroll"),
                         le = ee.offsetTop - e.virtualScrollStickySizeStart,
                         be = le < ne.scrollTop ? "decrease" : "increase";
                     ne.scrollTop = le, o("virtualScroll", {
                         index: $,
                         from: 0,
-                        to: x.value.rowsPerPage - 1,
+                        to: _.value.rowsPerPage - 1,
                         direction: be
                     })
                 }
             }
 
             function E($) {
                 o("virtualScroll", $)
@@ -5467,23 +5467,23 @@
                     indeterminate: !0,
                     trackColor: "transparent"
                 })]
             }
 
             function re($, X, ee) {
                 const ne = c.value($),
-                    le = w(ne);
+                    le = y(ne);
                 if (X !== void 0) return X(ae({
                     key: ne,
                     row: $,
                     pageIndex: ee,
                     __trClass: le ? "selected" : ""
                 }));
                 const be = n["body-cell"],
-                    pe = _.value.map(Ee => {
+                    pe = S.value.map(Ee => {
                         const It = n[`body-cell-${Ee.name}`],
                             zt = It !== void 0 ? It : be;
                         return zt !== void 0 ? zt(qe({
                             key: ne,
                             row: $,
                             pageIndex: ee,
                             col: Ee
@@ -5494,21 +5494,21 @@
                     });
                 if (I.value === !0) {
                     const Ee = n["body-selection"],
                         It = Ee !== void 0 ? Ee(ze({
                             key: ne,
                             row: $,
                             pageIndex: ee
-                        })) : [t.h(ko, {
+                        })) : [t.h(Co, {
                             modelValue: le,
                             color: e.color,
                             dark: a.value,
                             dense: e.dense,
-                            "onUpdate:modelValue": (zt, Yo) => {
-                                G([ne], [$], zt, Yo)
+                            "onUpdate:modelValue": (zt, Zo) => {
+                                G([ne], [$], zt, Zo)
                             }
                         })];
                     pe.unshift(t.h("td", {
                         class: "q-table--col-auto-width"
                     }, It))
                 }
                 const Ye = {
@@ -5526,19 +5526,19 @@
                 }), t.h("tr", Ye, pe)
             }
 
             function ie() {
                 const $ = n.body,
                     X = n["top-row"],
                     ee = n["bottom-row"];
-                let ne = B.value.map((le, be) => re(le, $, be));
+                let ne = P.value.map((le, be) => re(le, $, be));
                 return X !== void 0 && (ne = X({
-                    cols: _.value
+                    cols: S.value
                 }).concat(ne)), ee !== void 0 && (ne = ne.concat(ee({
-                    cols: _.value
+                    cols: S.value
                 }))), t.h("tbody", ne)
             }
 
             function ae($) {
                 return Oe($), $.cols = $.cols.map(X => Ze({
                     ...X
                 }, "value", () => Me(X, $.row))), $
@@ -5550,22 +5550,22 @@
 
             function ze($) {
                 return Oe($), $
             }
 
             function Oe($) {
                 Object.assign($, {
-                    cols: _.value,
+                    cols: S.value,
                     colsMap: b.value,
                     sort: F,
                     rowIndex: Z.value + $.pageIndex,
                     color: e.color,
                     dark: a.value,
                     dense: e.dense
-                }), I.value === !0 && Ze($, "selected", () => w($.key), (X, ee) => {
+                }), I.value === !0 && Ze($, "selected", () => y($.key), (X, ee) => {
                     G([$.key], [$.row], X, ee)
                 }), Ze($, "expand", () => A($.key), X => {
                     V($.key, X)
                 })
             }
 
             function Me($, X) {
@@ -5606,15 +5606,15 @@
                         class: "q-table__separator col"
                     })), pe.push(t.h("div", {
                         class: "q-table__control"
                     }, [ee(Ne.value)]))), pe.length !== 0) return t.h("div", {
                     class: be
                 }, pe)
             }
-            const Re = t.computed(() => j.value === !0 ? null : q.value);
+            const Re = t.computed(() => j.value === !0 ? null : T.value);
 
             function Rt() {
                 const $ = Mn();
                 return e.loading === !0 && n.loading === void 0 && $.push(t.h("tr", {
                     class: "q-table__progress"
                 }, [t.h("th", {
                     class: "relative-position",
@@ -5624,31 +5624,31 @@
 
             function Mn() {
                 const $ = n.header,
                     X = n["header-cell"];
                 if ($ !== void 0) return $(Vt({
                     header: !0
                 })).slice();
-                const ee = _.value.map(ne => {
+                const ee = S.value.map(ne => {
                     const le = n[`header-cell-${ne.name}`],
                         be = le !== void 0 ? le : X,
                         pe = Vt({
                             col: ne
                         });
                     return be !== void 0 ? be(pe) : t.h(vu, {
                         key: ne.name,
                         props: pe
                     }, () => ne.label)
                 });
-                if (k.value === !0 && e.grid !== !0) ee.unshift(t.h("th", {
+                if (x.value === !0 && e.grid !== !0) ee.unshift(t.h("th", {
                     class: "q-table--col-auto-width"
                 }, " "));
                 else if (O.value === !0) {
                     const ne = n["header-selection"],
-                        le = ne !== void 0 ? ne(Vt({})) : [t.h(ko, {
+                        le = ne !== void 0 ? ne(Vt({})) : [t.h(Co, {
                             color: e.color,
                             modelValue: Re.value,
                             dark: a.value,
                             dense: e.dense,
                             "onUpdate:modelValue": sn
                         })];
                     ee.unshift(t.h("th", {
@@ -5659,25 +5659,25 @@
                     class: e.tableHeaderClass,
                     style: e.tableHeaderStyle
                 }, ee)]
             }
 
             function Vt($) {
                 return Object.assign($, {
-                    cols: _.value,
+                    cols: S.value,
                     sort: F,
                     colsMap: b.value,
                     color: e.color,
                     dark: a.value,
                     dense: e.dense
                 }), O.value === !0 && Ze($, "selected", () => Re.value, sn), $
             }
 
             function sn($) {
-                j.value === !0 && ($ = !1), G(B.value.map(c.value), B.value, $)
+                j.value === !0 && ($ = !1), G(P.value.map(c.value), P.value, $)
             }
             const kt = t.computed(() => {
                 const $ = [e.iconFirstPage || r.iconSet.table.firstPage, e.iconPrevPage || r.iconSet.table.prevPage, e.iconNextPage || r.iconSet.table.nextPage, e.iconLastPage || r.iconSet.table.lastPage];
                 return r.lang.rtl === !0 ? $.reverse() : $
             });
 
             function Rn() {
@@ -5703,28 +5703,28 @@
                     class: Cn
                 }, [$(Ne.value)]);
                 const X = e.hideSelectedBanner !== !0 && I.value === !0 && N.value > 0 ? [t.h("div", {
                     class: "q-table__control"
                 }, [t.h("div", [(e.selectedRowsLabel || r.lang.table.selectedRecords)(N.value)])])] : [];
                 if (e.hidePagination !== !0) return t.h("div", {
                     class: Cn + " justify-end"
-                }, Go(X));
+                }, Xo(X));
                 if (X.length !== 0) return t.h("div", {
                     class: Cn
                 }, X)
             }
 
             function Vn($) {
-                y({
+                w({
                     page: 1,
                     rowsPerPage: $.value
                 })
             }
 
-            function Go($) {
+            function Xo($) {
                 let X;
                 const {
                     rowsPerPage: ee
                 } = p.value, ne = e.paginationLabel || r.lang.table.pagination, le = n.pagination, be = e.rowsPerPageOptions.length > 1;
                 if ($.push(t.h("div", {
                         class: "q-table__separator col"
                     })), be === !0 && $.push(t.h("div", {
@@ -5742,15 +5742,15 @@
                         dense: !0,
                         optionsDense: !0,
                         optionsCover: !0,
                         "onUpdate:modelValue": Vn
                     })])), le !== void 0) X = le(Ne.value);
                 else if (X = [t.h("span", ee !== 0 ? {
                         class: "q-table__bottom-item"
-                    } : {}, [ee ? ne(Z.value + 1, Math.min(ue.value, ce.value), ce.value) : ne(1, T.value, ce.value)])], ee !== 0 && ke.value > 1) {
+                    } : {}, [ee ? ne(Z.value + 1, Math.min(ue.value, ce.value), ce.value) : ne(1, B.value, ce.value)])], ee !== 0 && ke.value > 1) {
                     const pe = {
                         color: e.color,
                         round: !0,
                         dense: !0,
                         flat: !0
                     };
                     e.dense === !0 && (pe.size = "sm"), ke.value > 2 && X.push(t.h(pt, {
@@ -5780,15 +5780,15 @@
                     }))
                 }
                 return $.push(t.h("div", {
                     class: "q-table__control"
                 }, X)), $
             }
 
-            function Xo() {
+            function Yo() {
                 const $ = e.gridHeader === !0 ? [t.h("table", {
                     class: "q-table"
                 }, [Rt()])] : e.loading === !0 && n.loading === void 0 ? Y() : void 0;
                 return t.h("div", {
                     class: "q-table__middle"
                 }, $)
             }
@@ -5800,15 +5800,15 @@
                     }, [t.h("div", {
                         class: "q-table__grid-item-title"
                     }, [le.label]), t.h("div", {
                         class: "q-table__grid-item-value"
                     }, [le.value])]));
                     if (I.value === !0) {
                         const le = n["body-selection"],
-                            be = le !== void 0 ? le(X) : [t.h(ko, {
+                            be = le !== void 0 ? le(X) : [t.h(Co, {
                                 modelValue: X.selected,
                                 color: e.color,
                                 dark: a.value,
                                 dense: e.dense,
                                 "onUpdate:modelValue": (pe, Ye) => {
                                     G([X.key], [X.row], pe, Ye)
                                 }
@@ -5830,46 +5830,46 @@
                     })), t.h("div", {
                         class: "q-table__grid-item col-xs-12 col-sm-6 col-md-4 col-lg-3" + (X.selected === !0 ? " q-table__grid-item--selected" : "")
                     }, [t.h("div", ne, ee)])
                 };
                 return t.h("div", {
                     class: ["q-table__grid-content row", e.cardContainerClass],
                     style: e.cardContainerStyle
-                }, B.value.map((X, ee) => $(ae({
+                }, P.value.map((X, ee) => $(ae({
                     key: c.value(X),
                     row: X,
                     pageIndex: ee
                 }))))
             }
             return Object.assign(l.proxy, {
-                requestServerInteraction: C,
-                setPagination: y,
+                requestServerInteraction: q,
+                setPagination: w,
                 firstPage: ye,
                 prevPage: Te,
                 nextPage: Ae,
                 lastPage: Ue,
-                isRowSelected: w,
+                isRowSelected: y,
                 clearSelection: z,
                 isRowExpanded: A,
                 setExpanded: M,
                 sort: F,
                 resetVirtualScroll: Ce,
                 scrollTo: W,
                 getCellValue: Me
             }), Wa(l.proxy, {
                 filteredSortedRows: () => R.value,
-                computedRows: () => B.value,
+                computedRows: () => P.value,
                 computedRowsNumber: () => ce.value
             }), () => {
                 const $ = [xt()],
                     X = {
                         ref: d,
                         class: v.value
                     };
-                return e.grid === !0 ? $.push(Xo()) : Object.assign(X, {
+                return e.grid === !0 ? $.push(Yo()) : Object.assign(X, {
                     class: [X.class, e.cardClass],
                     style: e.cardStyle
                 }), $.push(L(), Rn()), e.loading === !0 && n.loading !== void 0 && $.push(n.loading()), t.h("div", X, $)
             }
         }
     });
 
@@ -6016,58 +6016,58 @@
     }
 
     function bt(e) {
         return e != null && typeof e == "object"
     }
     var Bs = "[object Symbol]";
 
-    function Co(e) {
+    function qo(e) {
         return typeof e == "symbol" || bt(e) && At(e) == Bs
     }
 
-    function qo(e, n) {
+    function To(e, n) {
         for (var o = -1, l = e == null ? 0 : e.length, r = Array(l); ++o < l;) r[o] = n(e[o], o, e);
         return r
     }
     var Ps = Array.isArray;
     const Je = Ps;
     var Es = 1 / 0,
         Ar = ct ? ct.prototype : void 0,
         Or = Ar ? Ar.toString : void 0;
 
     function Mr(e) {
         if (typeof e == "string") return e;
-        if (Je(e)) return qo(e, Mr) + "";
-        if (Co(e)) return Or ? Or.call(e) : "";
+        if (Je(e)) return To(e, Mr) + "";
+        if (qo(e)) return Or ? Or.call(e) : "";
         var n = e + "";
         return n == "0" && 1 / e == -Es ? "-0" : n
     }
 
-    function To(e) {
+    function Bo(e) {
         var n = typeof e;
         return e != null && (n == "object" || n == "function")
     }
 
-    function Bo(e) {
+    function Po(e) {
         return e
     }
     var $s = "[object AsyncFunction]",
         As = "[object Function]",
         Os = "[object GeneratorFunction]",
         Ms = "[object Proxy]";
 
     function Rr(e) {
-        if (!To(e)) return !1;
+        if (!Bo(e)) return !1;
         var n = At(e);
         return n == As || n == Os || n == $s || n == Ms
     }
     var Rs = ot["__core-js_shared__"];
-    const Po = Rs;
+    const Eo = Rs;
     var Vr = function() {
-        var e = /[^.]+$/.exec(Po && Po.keys && Po.keys.IE_PROTO || "");
+        var e = /[^.]+$/.exec(Eo && Eo.keys && Eo.keys.IE_PROTO || "");
         return e ? "Symbol(src)_1." + e : ""
     }();
 
     function Vs(e) {
         return !!Vr && Vr in e
     }
     var Is = Function.prototype,
@@ -6089,29 +6089,29 @@
         Ds = Function.prototype,
         js = Object.prototype,
         Ns = Ds.toString,
         Hs = js.hasOwnProperty,
         Us = RegExp("^" + Ns.call(Hs).replace(Ls, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
 
     function Ws(e) {
-        if (!To(e) || Vs(e)) return !1;
+        if (!Bo(e) || Vs(e)) return !1;
         var n = Rr(e) ? Us : Fs;
         return n.test(yt(e))
     }
 
     function Ks(e, n) {
         return e == null ? void 0 : e[n]
     }
 
     function wt(e, n) {
         var o = Ks(e, n);
         return Ws(o) ? o : void 0
     }
     var Qs = wt(ot, "WeakMap");
-    const Eo = Qs;
+    const $o = Qs;
 
     function Ir(e, n, o) {
         switch (o.length) {
             case 0:
                 return e.call(n);
             case 1:
                 return e.call(n, o[0]);
@@ -6156,15 +6156,15 @@
     var nc = qn ? function(e, n) {
             return qn(e, "toString", {
                 configurable: !0,
                 enumerable: !1,
                 value: ec(n),
                 writable: !0
             })
-        } : Bo,
+        } : Po,
         oc = Js(nc);
     const lc = oc;
 
     function rc(e, n, o, l) {
         for (var r = e.length, a = o + (l ? 1 : -1); l ? a-- : ++a < r;)
             if (n(e[a], a, e)) return a;
         return -1
@@ -6217,24 +6217,24 @@
                 r = -1;
                 for (var u = Array(n + 1); ++r < n;) u[r] = l[r];
                 return u[n] = o(i), Ir(e, this, u)
             }
     }
 
     function hc(e, n) {
-        return lc(mc(e, n, Bo), e + "")
+        return lc(mc(e, n, Po), e + "")
     }
     var vc = 9007199254740991;
 
-    function $o(e) {
+    function Ao(e) {
         return typeof e == "number" && e > -1 && e % 1 == 0 && e <= vc
     }
 
-    function Ao(e) {
-        return e != null && $o(e.length) && !Rr(e)
+    function Oo(e) {
+        return e != null && Ao(e.length) && !Rr(e)
     }
     var gc = Object.prototype;
 
     function pc(e) {
         var n = e && e.constructor,
             o = typeof n == "function" && n.prototype || gc;
         return e === o
@@ -6264,15 +6264,15 @@
     }
     var Ur = typeof exports == "object" && exports && !exports.nodeType && exports,
         Wr = Ur && typeof module == "object" && module && !module.nodeType && module,
         xc = Wr && Wr.exports === Ur,
         Kr = xc ? ot.Buffer : void 0,
         kc = Kr ? Kr.isBuffer : void 0,
         Cc = kc || _c;
-    const Oo = Cc;
+    const Mo = Cc;
     var qc = "[object Arguments]",
         Tc = "[object Array]",
         Bc = "[object Boolean]",
         Pc = "[object Date]",
         Ec = "[object Error]",
         $c = "[object Function]",
         Ac = "[object Map]",
@@ -6293,43 +6293,43 @@
         Kc = "[object Uint8ClampedArray]",
         Qc = "[object Uint16Array]",
         Gc = "[object Uint32Array]",
         ge = {};
     ge[Dc] = ge[jc] = ge[Nc] = ge[Hc] = ge[Uc] = ge[Wc] = ge[Kc] = ge[Qc] = ge[Gc] = !0, ge[qc] = ge[Tc] = ge[Lc] = ge[Bc] = ge[Fc] = ge[Pc] = ge[Ec] = ge[$c] = ge[Ac] = ge[Oc] = ge[Mc] = ge[Rc] = ge[Vc] = ge[Ic] = ge[zc] = !1;
 
     function Xc(e) {
-        return bt(e) && $o(e.length) && !!ge[At(e)]
+        return bt(e) && Ao(e.length) && !!ge[At(e)]
     }
 
     function Yc(e) {
         return function(n) {
             return e(n)
         }
     }
     var Qr = typeof exports == "object" && exports && !exports.nodeType && exports,
         on = Qr && typeof module == "object" && module && !module.nodeType && module,
         Zc = on && on.exports === Qr,
-        Mo = Zc && Pr.process,
+        Ro = Zc && Pr.process,
         Jc = function() {
             try {
                 var e = on && on.require && on.require("util").types;
-                return e || Mo && Mo.binding && Mo.binding("util")
+                return e || Ro && Ro.binding && Ro.binding("util")
             } catch {}
         }();
     const Gr = Jc;
     var Xr = Gr && Gr.isTypedArray,
         ed = Xr ? Yc(Xr) : Xc;
     const Yr = ed;
     var td = Object.prototype,
         nd = td.hasOwnProperty;
 
     function od(e, n) {
         var o = Je(e),
             l = !o && Hr(e),
-            r = !o && !l && Oo(e),
+            r = !o && !l && Mo(e),
             a = !o && !l && !r && Yr(e),
             i = o || l || r || a,
             u = i ? Dr(e.length, String) : [],
             c = u.length;
         for (var d in e)(n || nd.call(e, d)) && !(i && (d == "length" || r && (d == "offset" || d == "parent") || a && (d == "buffer" || d == "byteLength" || d == "byteOffset") || zr(d, c))) && u.push(d);
         return u
     }
@@ -6347,24 +6347,24 @@
     function sd(e) {
         if (!pc(e)) return ad(e);
         var n = [];
         for (var o in Object(e)) ud.call(e, o) && o != "constructor" && n.push(o);
         return n
     }
 
-    function Ro(e) {
-        return Ao(e) ? od(e) : sd(e)
+    function Vo(e) {
+        return Oo(e) ? od(e) : sd(e)
     }
     var cd = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
         dd = /^\w*$/;
 
-    function Vo(e, n) {
+    function Io(e, n) {
         if (Je(e)) return !1;
         var o = typeof e;
-        return o == "number" || o == "symbol" || o == "boolean" || e == null || Co(e) ? !0 : dd.test(e) || !cd.test(e) || n != null && e in Object(n)
+        return o == "number" || o == "symbol" || o == "boolean" || e == null || qo(e) ? !0 : dd.test(e) || !cd.test(e) || n != null && e in Object(n)
     }
     var fd = wt(Object, "create");
     const ln = fd;
 
     function md() {
         this.__data__ = ln ? ln(null) : {}, this.size = 0
     }
@@ -6501,31 +6501,31 @@
             var l = e[n];
             this.set(l[0], l[1])
         }
     }
     rt.prototype.clear = Ad, rt.prototype.delete = Md, rt.prototype.get = Rd, rt.prototype.has = Vd, rt.prototype.set = Id;
     var zd = "Expected a function";
 
-    function Io(e, n) {
+    function zo(e, n) {
         if (typeof e != "function" || n != null && typeof n != "function") throw new TypeError(zd);
         var o = function() {
             var l = arguments,
                 r = n ? n.apply(this, l) : l[0],
                 a = o.cache;
             if (a.has(r)) return a.get(r);
             var i = e.apply(this, l);
             return o.cache = a.set(r, i) || a, i
         };
-        return o.cache = new(Io.Cache || rt), o
+        return o.cache = new(zo.Cache || rt), o
     }
-    Io.Cache = rt;
+    zo.Cache = rt;
     var Ld = 500;
 
     function Fd(e) {
-        var n = Io(e, function(l) {
+        var n = zo(e, function(l) {
                 return o.size === Ld && o.clear(), l
             }),
             o = n.cache;
         return n
     }
     var Dd = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
         jd = /\\(\\)?/g,
@@ -6538,20 +6538,20 @@
     const Hd = Nd;
 
     function Ud(e) {
         return e == null ? "" : Mr(e)
     }
 
     function Zr(e, n) {
-        return Je(e) ? e : Vo(e, n) ? [e] : Hd(Ud(e))
+        return Je(e) ? e : Io(e, n) ? [e] : Hd(Ud(e))
     }
     var Wd = 1 / 0;
 
     function Pn(e) {
-        if (typeof e == "string" || Co(e)) return e;
+        if (typeof e == "string" || qo(e)) return e;
         var n = e + "";
         return n == "0" && 1 / e == -Wd ? "-0" : n
     }
 
     function Jr(e, n) {
         n = Zr(n, e);
         for (var o = 0, l = n.length; e != null && o < l;) e = e[Pn(n[o++])];
@@ -6626,35 +6626,35 @@
 
     function af(e, n, o) {
         var l = n(e);
         return Je(e) ? l : Qd(l, o(e))
     }
 
     function na(e) {
-        return af(e, Ro, rf)
+        return af(e, Vo, rf)
     }
     var uf = wt(ot, "DataView");
-    const zo = uf;
+    const Lo = uf;
     var sf = wt(ot, "Promise");
-    const Lo = sf;
+    const Fo = sf;
     var cf = wt(ot, "Set");
     const Ot = cf;
     var oa = "[object Map]",
         df = "[object Object]",
         la = "[object Promise]",
         ra = "[object Set]",
         aa = "[object WeakMap]",
         ia = "[object DataView]",
-        ff = yt(zo),
+        ff = yt(Lo),
         mf = yt(rn),
-        hf = yt(Lo),
+        hf = yt(Fo),
         vf = yt(Ot),
-        gf = yt(Eo),
+        gf = yt($o),
         _t = At;
-    (zo && _t(new zo(new ArrayBuffer(1))) != ia || rn && _t(new rn) != oa || Lo && _t(Lo.resolve()) != la || Ot && _t(new Ot) != ra || Eo && _t(new Eo) != aa) && (_t = function(e) {
+    (Lo && _t(new Lo(new ArrayBuffer(1))) != ia || rn && _t(new rn) != oa || Fo && _t(Fo.resolve()) != la || Ot && _t(new Ot) != ra || $o && _t(new $o) != aa) && (_t = function(e) {
         var n = At(e),
             o = n == df ? e.constructor : void 0,
             l = o ? yt(o) : "";
         if (l) switch (l) {
             case ff:
                 return ia;
             case mf:
@@ -6704,34 +6704,34 @@
         var i = o & _f,
             u = e.length,
             c = n.length;
         if (u != c && !(i && c > u)) return !1;
         var d = a.get(e),
             s = a.get(n);
         if (d && s) return d == n && s == e;
-        var h = -1,
+        var m = -1,
             f = !0,
-            m = o & xf ? new an : void 0;
-        for (a.set(e, n), a.set(n, e); ++h < u;) {
-            var v = e[h],
-                x = n[h];
-            if (l) var p = i ? l(x, v, h, n, e, a) : l(v, x, h, e, n, a);
+            h = o & xf ? new an : void 0;
+        for (a.set(e, n), a.set(n, e); ++m < u;) {
+            var v = e[m],
+                _ = n[m];
+            if (l) var p = i ? l(_, v, m, n, e, a) : l(v, _, m, e, n, a);
             if (p !== void 0) {
                 if (p) continue;
                 f = !1;
                 break
             }
-            if (m) {
-                if (!Sf(n, function(S, C) {
-                        if (!ca(m, C) && (v === S || r(v, S, o, l, a))) return m.push(C)
+            if (h) {
+                if (!Sf(n, function(k, q) {
+                        if (!ca(h, q) && (v === k || r(v, k, o, l, a))) return h.push(q)
                     })) {
                     f = !1;
                     break
                 }
-            } else if (!(v === x || r(v, x, o, l, a))) {
+            } else if (!(v === _ || r(v, _, o, l, a))) {
                 f = !1;
                 break
             }
         }
         return a.delete(e), a.delete(n), f
     }
 
@@ -6739,15 +6739,15 @@
         var n = -1,
             o = Array(e.size);
         return e.forEach(function(l, r) {
             o[++n] = [r, l]
         }), o
     }
 
-    function Fo(e) {
+    function Do(e) {
         var n = -1,
             o = Array(e.size);
         return e.forEach(function(l) {
             o[++n] = l
         }), o
     }
     var Cf = 1,
@@ -6760,15 +6760,15 @@
         Af = "[object RegExp]",
         Of = "[object Set]",
         Mf = "[object String]",
         Rf = "[object Symbol]",
         Vf = "[object ArrayBuffer]",
         If = "[object DataView]",
         fa = ct ? ct.prototype : void 0,
-        Do = fa ? fa.valueOf : void 0;
+        jo = fa ? fa.valueOf : void 0;
 
     function zf(e, n, o, l, r, a, i) {
         switch (o) {
             case If:
                 if (e.byteLength != n.byteLength || e.byteOffset != n.byteOffset) return !1;
                 e = e.buffer, n = n.buffer;
             case Vf:
@@ -6782,62 +6782,62 @@
             case Af:
             case Mf:
                 return e == n + "";
             case Ef:
                 var u = kf;
             case Of:
                 var c = l & Cf;
-                if (u || (u = Fo), e.size != n.size && !c) return !1;
+                if (u || (u = Do), e.size != n.size && !c) return !1;
                 var d = i.get(e);
                 if (d) return d == n;
                 l |= qf, i.set(e, n);
                 var s = da(u(e), u(n), l, r, a, i);
                 return i.delete(e), s;
             case Rf:
-                if (Do) return Do.call(e) == Do.call(n)
+                if (jo) return jo.call(e) == jo.call(n)
         }
         return !1
     }
     var Lf = 1,
         Ff = Object.prototype,
         Df = Ff.hasOwnProperty;
 
     function jf(e, n, o, l, r, a) {
         var i = o & Lf,
             u = na(e),
             c = u.length,
             d = na(n),
             s = d.length;
         if (c != s && !i) return !1;
-        for (var h = c; h--;) {
-            var f = u[h];
+        for (var m = c; m--;) {
+            var f = u[m];
             if (!(i ? f in n : Df.call(n, f))) return !1
         }
-        var m = a.get(e),
+        var h = a.get(e),
             v = a.get(n);
-        if (m && v) return m == n && v == e;
-        var x = !0;
+        if (h && v) return h == n && v == e;
+        var _ = !0;
         a.set(e, n), a.set(n, e);
-        for (var p = i; ++h < c;) {
-            f = u[h];
-            var S = e[f],
-                C = n[f];
-            if (l) var y = i ? l(C, S, f, n, e, a) : l(S, C, f, e, n, a);
-            if (!(y === void 0 ? S === C || r(S, C, o, l, a) : y)) {
-                x = !1;
+        for (var p = i; ++m < c;) {
+            f = u[m];
+            var k = e[f],
+                q = n[f];
+            if (l) var w = i ? l(q, k, f, n, e, a) : l(k, q, f, e, n, a);
+            if (!(w === void 0 ? k === q || r(k, q, o, l, a) : w)) {
+                _ = !1;
                 break
             }
             p || (p = f == "constructor")
         }
-        if (x && !p) {
-            var P = e.constructor,
+        if (_ && !p) {
+            var C = e.constructor,
                 A = n.constructor;
-            P != A && "constructor" in e && "constructor" in n && !(typeof P == "function" && P instanceof P && typeof A == "function" && A instanceof A) && (x = !1)
+            C != A && "constructor" in e && "constructor" in n && !(typeof C == "function" && C instanceof C && typeof A == "function" && A instanceof A) && (_ = !1)
         }
-        return a.delete(e), a.delete(n), x
+        return a.delete(e), a.delete(n), _
     }
     var Nf = 1,
         ma = "[object Arguments]",
         ha = "[object Array]",
         En = "[object Object]",
         Hf = Object.prototype,
         va = Hf.hasOwnProperty;
@@ -6845,35 +6845,35 @@
     function Uf(e, n, o, l, r, a) {
         var i = Je(e),
             u = Je(n),
             c = i ? ha : ua(e),
             d = u ? ha : ua(n);
         c = c == ma ? En : c, d = d == ma ? En : d;
         var s = c == En,
-            h = d == En,
+            m = d == En,
             f = c == d;
-        if (f && Oo(e)) {
-            if (!Oo(n)) return !1;
+        if (f && Mo(e)) {
+            if (!Mo(n)) return !1;
             i = !0, s = !1
         }
         if (f && !s) return a || (a = new at), i || Yr(e) ? da(e, n, o, l, r, a) : zf(e, n, c, o, l, r, a);
         if (!(o & Nf)) {
-            var m = s && va.call(e, "__wrapped__"),
-                v = h && va.call(n, "__wrapped__");
-            if (m || v) {
-                var x = m ? e.value() : e,
+            var h = s && va.call(e, "__wrapped__"),
+                v = m && va.call(n, "__wrapped__");
+            if (h || v) {
+                var _ = h ? e.value() : e,
                     p = v ? n.value() : n;
-                return a || (a = new at), r(x, p, o, l, a)
+                return a || (a = new at), r(_, p, o, l, a)
             }
         }
         return f ? (a || (a = new at), jf(e, n, o, l, r, a)) : !1
     }
 
-    function jo(e, n, o, l, r) {
-        return e === n ? !0 : e == null || n == null || !bt(e) && !bt(n) ? e !== e && n !== n : Uf(e, n, o, l, jo, r)
+    function No(e, n, o, l, r) {
+        return e === n ? !0 : e == null || n == null || !bt(e) && !bt(n) ? e !== e && n !== n : Uf(e, n, o, l, No, r)
     }
     var Wf = 1,
         Kf = 2;
 
     function Qf(e, n, o, l) {
         var r = o.length,
             a = r,
@@ -6887,28 +6887,28 @@
             u = o[r];
             var c = u[0],
                 d = e[c],
                 s = u[1];
             if (i && u[2]) {
                 if (d === void 0 && !(c in e)) return !1
             } else {
-                var h = new at;
-                if (l) var f = l(d, s, c, e, n, h);
-                if (!(f === void 0 ? jo(s, d, Wf | Kf, l, h) : f)) return !1
+                var m = new at;
+                if (l) var f = l(d, s, c, e, n, m);
+                if (!(f === void 0 ? No(s, d, Wf | Kf, l, m) : f)) return !1
             }
         }
         return !0
     }
 
     function ga(e) {
-        return e === e && !To(e)
+        return e === e && !Bo(e)
     }
 
     function Gf(e) {
-        for (var n = Ro(e), o = n.length; o--;) {
+        for (var n = Vo(e), o = n.length; o--;) {
             var l = n[o],
                 r = e[l];
             n[o] = [l, r, ga(r)]
         }
         return n
     }
 
@@ -6932,27 +6932,27 @@
     function Zf(e, n, o) {
         n = Zr(n, e);
         for (var l = -1, r = n.length, a = !1; ++l < r;) {
             var i = Pn(n[l]);
             if (!(a = e != null && o(e, i))) break;
             e = e[i]
         }
-        return a || ++l != r ? a : (r = e == null ? 0 : e.length, !!r && $o(r) && zr(i, r) && (Je(e) || Hr(e)))
+        return a || ++l != r ? a : (r = e == null ? 0 : e.length, !!r && Ao(r) && zr(i, r) && (Je(e) || Hr(e)))
     }
 
     function Jf(e, n) {
         return e != null && Zf(e, n, Yf)
     }
     var em = 1,
         tm = 2;
 
     function nm(e, n) {
-        return Vo(e) && ga(n) ? pa(Pn(e), n) : function(o) {
+        return Io(e) && ga(n) ? pa(Pn(e), n) : function(o) {
             var l = Kd(o, e);
-            return l === void 0 && l === n ? Jf(o, e) : jo(n, l, em | tm)
+            return l === void 0 && l === n ? Jf(o, e) : No(n, l, em | tm)
         }
     }
 
     function ba(e) {
         return function(n) {
             return n == null ? void 0 : n[e]
         }
@@ -6961,19 +6961,19 @@
     function om(e) {
         return function(n) {
             return Jr(n, e)
         }
     }
 
     function lm(e) {
-        return Vo(e) ? ba(Pn(e)) : om(e)
+        return Io(e) ? ba(Pn(e)) : om(e)
     }
 
     function rm(e) {
-        return typeof e == "function" ? e : e == null ? Bo : typeof e == "object" ? Je(e) ? nm(e[0], e[1]) : Xf(e) : lm(e)
+        return typeof e == "function" ? e : e == null ? Po : typeof e == "object" ? Je(e) ? nm(e[0], e[1]) : Xf(e) : lm(e)
     }
 
     function am(e, n, o, l) {
         for (var r = -1, a = e == null ? 0 : e.length; ++r < a;) {
             var i = e[r];
             n(l, i, o(i), e)
         }
@@ -6989,21 +6989,21 @@
             return n
         }
     }
     var um = im();
     const sm = um;
 
     function cm(e, n) {
-        return e && sm(e, n, Ro)
+        return e && sm(e, n, Vo)
     }
 
     function dm(e, n) {
         return function(o, l) {
             if (o == null) return o;
-            if (!Ao(o)) return e(o, l);
+            if (!Oo(o)) return e(o, l);
             for (var r = o.length, a = n ? r : -1, i = Object(o);
                 (n ? a-- : ++a < r) && l(i[a], a, i) !== !1;);
             return o
         }
     }
     var fm = dm(cm);
     const mm = fm;
@@ -7019,30 +7019,30 @@
             var r = Je(o) ? am : hm,
                 a = n ? n() : {};
             return r(o, e, rm(l), a)
         }
     }
 
     function gm(e) {
-        return bt(e) && Ao(e)
+        return bt(e) && Oo(e)
     }
 
     function pm(e, n, o) {
         for (var l = -1, r = e == null ? 0 : e.length; ++l < r;)
             if (o(n, e[l])) return !0;
         return !1
     }
     var bm = Object.prototype,
         ym = bm.hasOwnProperty,
         wm = vm(function(e, n, o) {
             ym.call(e, o) ? e[o].push(n) : fc(e, o, [n])
         });
     const Sm = wm;
     var _m = 1 / 0,
-        xm = Ot && 1 / Fo(new Ot([, -0]))[1] == _m ? function(e) {
+        xm = Ot && 1 / Do(new Ot([, -0]))[1] == _m ? function(e) {
             return new Ot(e)
         } : Gs;
     const km = xm;
     var Cm = 200;
 
     function qm(e, n, o) {
         var l = -1,
@@ -7050,25 +7050,25 @@
             a = e.length,
             i = !0,
             u = [],
             c = u;
         if (o) i = !1, r = pm;
         else if (a >= Cm) {
             var d = n ? null : km(e);
-            if (d) return Fo(d);
+            if (d) return Do(d);
             i = !1, r = ca, c = new an
         } else c = n ? [] : u;
         e: for (; ++l < a;) {
             var s = e[l],
-                h = n ? n(s) : s;
-            if (s = o || s !== 0 ? s : 0, i && h === h) {
+                m = n ? n(s) : s;
+            if (s = o || s !== 0 ? s : 0, i && m === m) {
                 for (var f = c.length; f--;)
-                    if (c[f] === h) continue e;
-                n && c.push(h), u.push(s)
-            } else r(c, h, o) || (c !== u && c.push(h), u.push(s))
+                    if (c[f] === m) continue e;
+                n && c.push(m), u.push(s)
+            } else r(c, m, o) || (c !== u && c.push(m), u.push(s))
         }
         return u
     }
 
     function Tm(e) {
         return e && e.length ? qm(e) : []
     }
@@ -7076,37 +7076,37 @@
 
     function Pm(e) {
         if (!(e && e.length)) return [];
         var n = 0;
         return e = ea(e, function(o) {
             if (gm(o)) return n = Bm(o.length, n), !0
         }), Dr(n, function(o) {
-            return qo(e, ba(o))
+            return To(e, ba(o))
         })
     }
 
     function Em(e, n) {
         if (!(e && e.length)) return [];
         var o = Pm(e);
-        return n == null ? o : qo(o, function(l) {
+        return n == null ? o : To(o, function(l) {
             return Ir(n, void 0, l)
         })
     }
     var $m = hc(function(e) {
         var n = e.length,
             o = n > 1 ? e[n - 1] : void 0;
         return o = typeof o == "function" ? (e.pop(), o) : void 0, Em(e, o)
     });
     const Am = $m,
         Om = {
             uniq: Tm,
             groupBy: Sm
         };
 
-    function No(e, n) {
+    function Ho(e, n) {
         const o = new Function("utils", "rows", "fields", e ?? "");
 
         function l(r) {
             switch (n) {
                 case "udf":
                     if (e !== null) return o(Om, r.rows, r.fields);
                     break;
@@ -7176,16 +7176,16 @@
             } = l,
             a = jm(l, ["window"]);
         let i;
         const u = Lm(() => r && "ResizeObserver" in r),
             c = () => {
                 i && (i.disconnect(), i = void 0)
             },
-            d = t.watch(() => _a(e), h => {
-                c(), u.value && r && h && (i = new ResizeObserver(n), i.observe(h, a))
+            d = t.watch(() => _a(e), m => {
+                c(), u.value && r && m && (i = new ResizeObserver(n), i.observe(m, a))
             }, {
                 immediate: !0,
                 flush: "post"
             }),
             s = () => {
                 c(), d()
             };
@@ -7277,21 +7277,21 @@
             setup(e) {
                 const n = t.inject(xn),
                     l = e.model,
                     r = t.computed(() => l.contexts.map(d => {
                         if (typeof d == "string") return d;
                         if (Qm(d)) {
                             const f = d,
-                                m = n.createSqlQuery(l.id, f.sql),
-                                v = No(f.jsMap, f.type),
-                                x = m.query();
-                            if (x.rows.length === 0) return null;
-                            const p = v.map(x);
-                            let S = JSON.stringify(p);
-                            return typeof p == "string" && (S = S.slice(1, -1)), S
+                                h = n.createSqlQuery(l.id, f.sql),
+                                v = Ho(f.jsMap, f.type),
+                                _ = h.query();
+                            if (_.rows.length === 0) return null;
+                            const p = v.map(_);
+                            let k = JSON.stringify(p);
+                            return typeof p == "string" && (k = k.slice(1, -1)), k
                         }
                         const s = d;
                         return t.inject("foreachRow")[s.field]
                     }).join("")),
                     a = t.ref(null),
                     i = t.ref("initial"),
                     {
@@ -7322,19 +7322,19 @@
                     "4fd07687": i.value
                 }));
                 const n = t.inject(xn),
                     l = e.model,
                     r = l.contexts.map(d => {
                         if (typeof d == "string") return t.computed(() => d);
                         const s = d,
-                            h = n.createSqlQuery(l.id, s.sql),
-                            f = No(s.jsMap, s.type);
+                            m = n.createSqlQuery(l.id, s.sql),
+                            f = Ho(s.jsMap, s.type);
                         return t.computed(() => {
-                            const m = h.query();
-                            return m.rows.length === 0 ? null : JSON.stringify(f.map(m))
+                            const h = m.query();
+                            return h.rows.length === 0 ? null : JSON.stringify(f.map(h))
                         })
                     }),
                     a = t.ref(null),
                     i = t.ref("initial"),
                     {
                         height: u
                     } = qa(a);
@@ -7382,15 +7382,15 @@
             setup(e) {
                 const n = t.inject(xn),
                     o = e,
                     l = o.model,
                     r = l.sql,
                     a = t.computed(() => {
                         const i = n.createSqlQuery(l.id, r.sql),
-                            u = No(r.jsMap, r.type),
+                            u = Ho(r.jsMap, r.type),
                             c = i.query();
                         return u.map(c)
                     });
                 return (i, u) => (t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(a.value, c => (t.openBlock(), t.createElementBlock(t.Fragment, {
                     key: c
                 }, [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(o.model.children, d => (t.openBlock(), t.createBlock(Mt, {
                     component: d,
@@ -7398,35 +7398,35 @@
                 }, null, 8, ["component", "foreachRow"]))), 256))], 64))), 128))
             }
         }),
         $v = "",
         rh = Xe(lh, [
             ["__scopeId", "data-v-d293d89e"]
         ]),
-        Ho = e => (t.pushScopeId("data-v-2f3725fd"), e = e(), t.popScopeId(), e),
+        Uo = e => (t.pushScopeId("data-v-68848832"), e = e(), t.popScopeId(), e),
         ah = {
             class: "pybi-checkbox"
         },
         ih = {
             class: "title"
         },
         uh = {
             class: "funs-buttons"
         },
-        sh = [Ho(() => t.createElementVNode("svg", {
+        sh = [Uo(() => t.createElementVNode("svg", {
             viewBox: "0 0 1024 1024"
         }, [t.createElementVNode("path", {
             d: "M511.1 957.94c-246.456 0-446.857-200.401-446.857-446.859S264.644 64.223 511.1 64.223c246.457 0 446.858 200.401 446.858 446.858S757.557 957.94 511.1 957.94z m0-851.396c-222.806 0-404.537 181.73-404.537 404.537S288.295 915.619 511.1 915.619c222.807 0 404.537-181.73 404.537-404.537S734.53 106.544 511.1 106.544z m167.417 262.017L447.619 601.325 343.685 496.767c-9.335-9.335-24.895-9.335-34.853 0-9.335 9.335-9.335 24.895 0 34.853l121.984 121.983c9.336 9.336 24.895 9.336 34.853 0 1.244-1.244 1.866-2.489 3.112-3.733l245.211-246.457c9.336-9.335 9.336-24.895 0-34.852-9.959-9.959-25.518-9.959-35.475 0z"
         })], -1))],
-        ch = [Ho(() => t.createElementVNode("svg", {
+        ch = [Uo(() => t.createElementVNode("svg", {
             viewBox: "0 0 1024 1024"
         }, [t.createElementVNode("path", {
             d: "M832 448a64 64 0 0 1 64 64v320a64 64 0 0 1-64 64H512a64 64 0 0 1-64-64V512a64 64 0 0 1 64-64h320z m-576.448 218.496L256 672V832h96a32 32 0 0 1 31.488 26.24L384 864a32 32 0 0 1-26.24 31.488L352 896h-128a32 32 0 0 1-31.488-26.24L192 864v-114.816l-41.344 41.472a32 32 0 0 1-40.832 3.648l-4.48-3.648a32 32 0 0 1-3.648-40.832l3.648-4.48 96-96a32 32 0 0 1 54.208 17.152zM832 512H512v320h320V512z m-9.344 73.344a32 32 0 0 1 3.648 40.832l-3.648 4.48-128 128a32 32 0 0 1-35.456 6.656l-4.928-2.688-96-64a32 32 0 0 1 30.4-56l5.12 2.752 74.112 49.408 109.44-109.44a32 32 0 0 1 45.312 0zM512 128a64 64 0 0 1 64 64v192H512V192H192v320h192v64H192a64 64 0 0 1-64-64V192a64 64 0 0 1 64-64h320z m288-0.064a32 32 0 0 1 31.488 26.24L832 160v114.816l41.344-41.472a32 32 0 0 1 40.832-3.648l4.48 3.648a32 32 0 0 1 3.648 40.832l-3.648 4.48-96 96a32 32 0 0 1-54.208-17.152L768 351.936v-160h-96a32 32 0 0 1-31.488-26.24L640 159.936a32 32 0 0 1 26.24-31.488L672 128h128z"
         })], -1))],
-        dh = [Ho(() => t.createElementVNode("svg", {
+        dh = [Uo(() => t.createElementVNode("svg", {
             viewBox: "0 0 1024 1024"
         }, [t.createElementVNode("path", {
             d: "M214.864 440.317l69.471-41.742c20.83-12.516 47.862-5.776 60.377 15.053 12.516 20.83 5.776 47.862-15.053 60.377L137.653 589.374 22.285 397.369c-12.516-20.83-5.776-47.862 15.053-60.378 20.83-12.515 47.862-5.775 60.377 15.054l34.478 57.38c36.81-123.472 126.622-227 249.697-279.243 223.634-94.927 481.893 9.459 576.842 233.144 94.948 223.685-9.365 481.973-232.998 576.9-161.485 68.546-346.059 34.258-472.152-83.359-17.77-16.575-18.738-44.418-2.162-62.188 16.575-17.77 44.418-18.738 62.187-2.163 100.9 94.117 248.546 121.546 377.742 66.705C870.24 783.287 953.688 576.663 877.727 397.71c-75.96-178.953-282.562-262.459-461.452-186.524-100.372 42.605-173.066 127.8-201.411 229.131z",
             fill: "#000000"
         })], -1))],
         fh = {
             key: 0,
@@ -7446,144 +7446,148 @@
         ph = ["onClick"],
         bh = t.defineComponent({
             __name: "Checkbox",
             props: {
                 model: {}
             },
             setup(e) {
-                t.useCssVars(S => ({
-                    "6c5c2c06": t.unref(p)
+                t.useCssVars(q => ({
+                    cf2e820e: t.unref(k)
                 }));
                 const o = e.model,
-                    l = t.inject(vr),
-                    a = t.inject(kn).getFilterUtils(o),
-                    i = a.getData();
-                let u = null;
-                const c = t.computed(() => {
-                        if (i.value.rows.length > 0) {
-                            const S = i.value.rows;
-                            return u || (u = i.value.fields[0]), S.map(C => {
-                                const y = C[u] === void 0 || C[u] === null;
+                    l = t.inject(gr),
+                    r = t.inject(kn);
+                t.inject(xo).onResetFilters(() => {
+                    s.clear()
+                });
+                const i = r.getFilterUtils(o),
+                    u = i.getData();
+                let c = null;
+                const d = t.computed(() => {
+                        if (u.value.rows.length > 0) {
+                            const q = u.value.rows;
+                            return c || (c = u.value.fields[0]), q.map(w => {
+                                const C = w[c] === void 0 || w[c] === null;
                                 return {
-                                    label: y ? "(空白)" : C[u].toString(),
-                                    value: y ? null : C[u]
+                                    label: C ? "(空白)" : w[c].toString(),
+                                    value: C ? null : w[c]
                                 }
                             })
                         }
                         return []
                     }),
-                    d = t.reactive(new Set);
-                t.watch(d, S => {
-                    let C = Array.from(S.keys());
-                    if (C = C.map(y => y === "(空白)" ? null : y), C.length === 0) a.removeFilter();
+                    s = t.reactive(new Set);
+                t.watch(s, q => {
+                    let w = Array.from(q.keys());
+                    if (w = w.map(C => C === "(空白)" ? null : C), w.length === 0) i.removeFilter();
                     else {
                         const {
-                            hasNull: y,
-                            values: P
-                        } = l.extractNullInValues(C), A = l.valuesArray2sqlArray(P).join(",");
-                        a.addFilterWithExprFn(M => {
-                            const V = `${M} in (${A})`;
-                            return y ? `${V} or ${M} is null` : V
+                            hasNull: C,
+                            values: A
+                        } = l.extractNullInValues(w), M = l.valuesArray2sqlArray(A).join(",");
+                        i.addFilterWithExprFn(V => {
+                            const R = `${V} in (${M})`;
+                            return C ? `${R} or ${V} is null` : R
                         })
                     }
                 }), o.hiddenTitle;
-                const s = t.computed(() => {
-                    const S = new Set(d.keys());
-                    return c.value.map(C => {
-                        const y = !!S.has(C.label);
+                const m = t.computed(() => {
+                    const q = new Set(s.keys());
+                    return d.value.map(w => {
+                        const C = !!q.has(w.label);
                         return t.ref({
-                            name: C.label,
-                            checked: y
+                            name: w.label,
+                            checked: C
                         })
                     })
                 });
 
-                function h(S, C) {
-                    for (let y = C; y >= 0; y--)
-                        if (S.value[y].value.checked) return y;
+                function f(q, w) {
+                    for (let C = w; C >= 0; C--)
+                        if (q.value[C].value.checked) return C;
                     return 0
                 }
 
-                function f(S, C, y) {
-                    const P = S;
-                    if (o.multiple && P.shiftKey) {
-                        const M = h(s, y);
-                        s.value.slice(M, y + 1).forEach(V => {
-                            !V.value.checked && !d.has(V.value.name) && d.add(V.value.name)
+                function h(q, w, C) {
+                    const A = q;
+                    if (o.multiple && A.shiftKey) {
+                        const V = f(m, C);
+                        m.value.slice(V, C + 1).forEach(R => {
+                            !R.value.checked && !s.has(R.value.name) && s.add(R.value.name)
                         });
                         return
                     }
-                    const A = !s.value[y].value.checked;
-                    A && !d.has(C) && (o.multiple || d.clear(), d.add(C)), !A && d.has(C) && d.delete(C)
+                    const M = !m.value[C].value.checked;
+                    M && !s.has(w) && (o.multiple || s.clear(), s.add(w)), !M && s.has(w) && s.delete(w)
                 }
 
-                function m() {
-                    d.clear()
+                function v() {
+                    s.clear()
                 }
 
-                function v() {
-                    s.value.forEach(S => {
-                        d.has(S.value.name) || d.add(S.value.name)
+                function _() {
+                    m.value.forEach(q => {
+                        s.has(q.value.name) || s.add(q.value.name)
                     })
                 }
 
-                function x() {
-                    s.value.forEach(S => {
-                        S.value.checked && d.has(S.value.name) && d.delete(S.value.name), !S.value.checked && !d.has(S.value.name) && d.add(S.value.name)
+                function p() {
+                    m.value.forEach(q => {
+                        q.value.checked && s.has(q.value.name) && s.delete(q.value.name), !q.value.checked && !s.has(q.value.name) && s.add(q.value.name)
                     })
                 }
-                const p = o.itemDirection;
-                return (S, C) => {
-                    const y = t.resolveDirective("tooltip");
+                const k = o.itemDirection;
+                return (q, w) => {
+                    const C = t.resolveDirective("tooltip");
                     return t.openBlock(), t.createElementBlock("div", ah, [t.createElementVNode("header", null, [t.createElementVNode("span", ih, t.toDisplayString(t.unref(o).title), 1), t.createElementVNode("div", uh, [t.unref(o).multiple ? t.withDirectives((t.openBlock(), t.createElementBlock("span", {
                         key: 0,
                         class: "all-selected funs-icon",
-                        onClick: v
+                        onClick: _
                     }, sh)), [
-                        [y, {
+                        [C, {
                             content: "全选",
                             position: "left"
                         }]
                     ]) : t.createCommentVNode("", !0), t.unref(o).multiple ? t.withDirectives((t.openBlock(), t.createElementBlock("span", {
                         key: 1,
                         class: "de-selected funs-icon",
-                        onClick: x
+                        onClick: p
                     }, ch)), [
-                        [y, {
+                        [C, {
                             content: "反选",
                             position: "left"
                         }]
                     ]) : t.createCommentVNode("", !0), t.withDirectives((t.openBlock(), t.createElementBlock("span", {
                         class: "reset-filter funs-icon",
-                        onClick: m
+                        onClick: v
                     }, dh)), [
-                        [y, {
+                        [C, {
                             content: "重置",
                             position: "left"
                         }]
-                    ])])]), t.unref(o).mode === "list" ? (t.openBlock(), t.createElementBlock("div", fh, [t.createElementVNode("div", mh, [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(c.value, (P, A) => (t.openBlock(), t.createElementBlock("div", {
-                        key: P.label,
+                    ])])]), t.unref(o).mode === "list" ? (t.openBlock(), t.createElementBlock("div", fh, [t.createElementVNode("div", mh, [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(d.value, (A, M) => (t.openBlock(), t.createElementBlock("div", {
+                        key: A.label,
                         class: "pybi-checkbox_content"
                     }, [t.createElementVNode("input", {
                         type: "checkbox",
-                        checked: s.value[A].value.checked,
-                        onChange: M => f(M, P.label, A)
-                    }, null, 40, hh), t.createElementVNode("span", null, t.toDisplayString(P.label), 1)]))), 128))])])) : t.createCommentVNode("", !0), t.unref(o).mode === "tile" ? (t.openBlock(), t.createElementBlock("div", vh, [t.createElementVNode("div", gh, [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(c.value, (P, A) => (t.openBlock(), t.createElementBlock("div", {
-                        key: P.label,
+                        checked: m.value[M].value.checked,
+                        onChange: V => h(V, A.label, M)
+                    }, null, 40, hh), t.createElementVNode("span", null, t.toDisplayString(A.label), 1)]))), 128))])])) : t.createCommentVNode("", !0), t.unref(o).mode === "tile" ? (t.openBlock(), t.createElementBlock("div", vh, [t.createElementVNode("div", gh, [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(d.value, (A, M) => (t.openBlock(), t.createElementBlock("div", {
+                        key: A.label,
                         class: t.normalizeClass(["pybi-checkbox_content", {
-                            "pybi-checkbox_content-checked": d.has(P.label)
+                            "pybi-checkbox_content-checked": s.has(A.label)
                         }]),
-                        onClick: M => f(M, P.label, A)
-                    }, [t.createElementVNode("span", null, t.toDisplayString(P.label), 1)], 10, ph))), 128))])])) : t.createCommentVNode("", !0)])
+                        onClick: V => h(V, A.label, M)
+                    }, [t.createElementVNode("span", null, t.toDisplayString(A.label), 1)], 10, ph))), 128))])])) : t.createCommentVNode("", !0)])
                 }
             }
         }),
         Rv = "",
         yh = Xe(bh, [
-            ["__scopeId", "data-v-2f3725fd"]
+            ["__scopeId", "data-v-68848832"]
         ]),
         wh = new Map([
             [nt.Box, ss],
             [nt.FlowBox, fs],
             [nt.GridBox, vs],
             [nt.TextValue, Ym],
             [nt.Markdown, eh],
@@ -7666,70 +7670,70 @@
                 model: {}
             },
             setup(e) {
                 const o = e.model,
                     l = t.ref(null),
                     r = new Map(Object.entries(o.columnProps ?? {}));
 
-                function a(S) {
-                    return r.has(S) ? r.get(S) : {}
+                function a(k) {
+                    return r.has(k) ? r.get(k) : {}
                 }
                 const i = t.inject(kn),
-                    u = t.inject(gr),
+                    u = t.inject(pr),
                     c = t.inject(br),
                     s = i.getFilterUtils(o).getData(),
-                    h = t.computed(() => s.value.rows),
-                    f = t.computed(() => s.value.fields.map(S => ({
-                        name: S,
-                        label: S,
-                        field: S,
-                        ...a(S)
+                    m = t.computed(() => s.value.rows),
+                    f = t.computed(() => s.value.fields.map(k => ({
+                        name: k,
+                        label: k,
+                        field: k,
+                        ...a(k)
                     }))),
-                    m = t.ref(f.value.map(S => S.name)),
+                    h = t.ref(f.value.map(k => k.name)),
                     v = t.computed({
-                        get: () => m.value,
-                        set: S => {
-                            m.value = S ?? []
+                        get: () => h.value,
+                        set: k => {
+                            h.value = k ?? []
                         }
                     });
                 c.setInfo(o.id, {
                     visibleColumns: v,
                     columns: f
                 });
                 const {
-                    copy: x
+                    copy: _
                 } = as();
 
                 function p() {
-                    x(s)
+                    _(s)
                 }
                 return u.register(o.id, "copy_to_clipboard_by_excel_format", p), t.onMounted(() => {
                     u.register(o.id, "toggleFullscreen", l.value.toggleFullscreen)
-                }), (S, C) => (t.openBlock(), t.createElementBlock("div", {
+                }), (k, q) => (t.openBlock(), t.createElementBlock("div", {
                     class: "bi-table",
                     "data-tag": t.unref(o).tag
                 }, [t.createVNode(rs, t.mergeProps({
                     ref_key: "tableRef",
                     ref: l,
-                    rows: h.value,
+                    rows: m.value,
                     columns: f.value,
                     "visible-columns": v.value,
                     dense: ""
                 }, t.unref(o).props, {
                     style: [{
                         width: "100%",
                         height: "100%"
                     }, t.unref(o).styles]
                 }), t.createSlots({
                     _: 2
                 }, [t.unref(o).topSlot ? {
                     name: "top",
-                    fn: t.withCtx(y => [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(t.unref(o).topSlot, P => (t.openBlock(), t.createBlock(Mt, {
-                        component: P,
-                        key: P.id
+                    fn: t.withCtx(w => [(t.openBlock(!0), t.createElementBlock(t.Fragment, null, t.renderList(t.unref(o).topSlot, C => (t.openBlock(), t.createBlock(Mt, {
+                        component: C,
+                        key: C.id
                     }, null, 8, ["component"]))), 128))]),
                     key: "0"
                 } : void 0]), 1040, ["rows", "columns", "visible-columns", "style"])], 8, Ch))
             }
         }),
         Th = t.defineComponent({
             __name: "Icon",
@@ -7761,117 +7765,117 @@
             ripple: {
                 type: [Boolean, Object],
                 default: !0
             }
         };
 
     function $h(e, n, o, l) {
-        const r = t.inject(cl, et);
+        const r = t.inject(dl, et);
         if (r === et) return console.error("QTab/QRouteTab component needs to be child of QTabs"), et;
         const {
             proxy: a
         } = t.getCurrentInstance(), i = t.ref(null), u = t.ref(null), c = t.ref(null), d = t.computed(() => e.disable === !0 || e.ripple === !1 ? !1 : Object.assign({
             keyCodes: [13, 32],
             early: !0
-        }, e.ripple === !0 ? {} : e.ripple)), s = t.computed(() => r.currentModel.value === e.name), h = t.computed(() => "q-tab relative-position self-stretch flex flex-center text-center" + (s.value === !0 ? " q-tab--active" + (r.tabProps.value.activeClass ? " " + r.tabProps.value.activeClass : "") + (r.tabProps.value.activeColor ? ` text-${r.tabProps.value.activeColor}` : "") + (r.tabProps.value.activeBgColor ? ` bg-${r.tabProps.value.activeBgColor}` : "") : " q-tab--inactive") + (e.icon && e.label && r.tabProps.value.inlineLabel === !1 ? " q-tab--full" : "") + (e.noCaps === !0 || r.tabProps.value.noCaps === !0 ? " q-tab--no-caps" : "") + (e.disable === !0 ? " disabled" : " q-focusable q-hoverable cursor-pointer") + (l !== void 0 ? l.linkClass.value : "")), f = t.computed(() => "q-tab__content self-stretch flex-center relative-position q-anchor--skip non-selectable " + (r.tabProps.value.inlineLabel === !0 ? "row no-wrap q-tab__content--inline" : "column") + (e.contentClass !== void 0 ? ` ${e.contentClass}` : "")), m = t.computed(() => e.disable === !0 || r.hasFocus.value === !0 || s.value === !1 && r.hasActiveTab.value === !0 ? -1 : e.tabindex || 0);
+        }, e.ripple === !0 ? {} : e.ripple)), s = t.computed(() => r.currentModel.value === e.name), m = t.computed(() => "q-tab relative-position self-stretch flex flex-center text-center" + (s.value === !0 ? " q-tab--active" + (r.tabProps.value.activeClass ? " " + r.tabProps.value.activeClass : "") + (r.tabProps.value.activeColor ? ` text-${r.tabProps.value.activeColor}` : "") + (r.tabProps.value.activeBgColor ? ` bg-${r.tabProps.value.activeBgColor}` : "") : " q-tab--inactive") + (e.icon && e.label && r.tabProps.value.inlineLabel === !1 ? " q-tab--full" : "") + (e.noCaps === !0 || r.tabProps.value.noCaps === !0 ? " q-tab--no-caps" : "") + (e.disable === !0 ? " disabled" : " q-focusable q-hoverable cursor-pointer") + (l !== void 0 ? l.linkClass.value : "")), f = t.computed(() => "q-tab__content self-stretch flex-center relative-position q-anchor--skip non-selectable " + (r.tabProps.value.inlineLabel === !0 ? "row no-wrap q-tab__content--inline" : "column") + (e.contentClass !== void 0 ? ` ${e.contentClass}` : "")), h = t.computed(() => e.disable === !0 || r.hasFocus.value === !0 || s.value === !1 && r.hasActiveTab.value === !0 ? -1 : e.tabindex || 0);
 
-        function v(y, P) {
-            if (P !== !0 && i.value !== null && i.value.focus(), e.disable === !0) {
-                l !== void 0 && l.hasRouterLink.value === !0 && ve(y);
+        function v(w, C) {
+            if (C !== !0 && i.value !== null && i.value.focus(), e.disable === !0) {
+                l !== void 0 && l.hasRouterLink.value === !0 && ve(w);
                 return
             }
             if (l === void 0) {
                 r.updateModel({
                     name: e.name
-                }), o("click", y);
+                }), o("click", w);
                 return
             }
             if (l.hasRouterLink.value === !0) {
                 const A = (M = {}) => {
                     let V;
-                    const R = M.to === void 0 || tt(M.to, e.to) === !0 ? r.avoidRouteWatcher = gl() : null;
-                    return l.navigateToRouterLink(y, {
+                    const R = M.to === void 0 || tt(M.to, e.to) === !0 ? r.avoidRouteWatcher = pl() : null;
+                    return l.navigateToRouterLink(w, {
                         ...M,
                         returnRouterError: !0
-                    }).catch(T => {
-                        V = T
-                    }).then(T => {
-                        if (R === r.avoidRouteWatcher && (r.avoidRouteWatcher = !1, V === void 0 && (T === void 0 || T.message.startsWith("Avoided redundant navigation") === !0) && r.updateModel({
+                    }).catch(B => {
+                        V = B
+                    }).then(B => {
+                        if (R === r.avoidRouteWatcher && (r.avoidRouteWatcher = !1, V === void 0 && (B === void 0 || B.message.startsWith("Avoided redundant navigation") === !0) && r.updateModel({
                                 name: e.name
-                            })), M.returnRouterError === !0) return V !== void 0 ? Promise.reject(V) : T
+                            })), M.returnRouterError === !0) return V !== void 0 ? Promise.reject(V) : B
                     })
                 };
-                o("click", y, A), y.defaultPrevented !== !0 && A();
+                o("click", w, A), w.defaultPrevented !== !0 && A();
                 return
             }
-            o("click", y)
+            o("click", w)
         }
 
-        function x(y) {
-            ut(y, [13, 32]) ? v(y, !0) : gn(y) !== !0 && y.keyCode >= 35 && y.keyCode <= 40 && y.altKey !== !0 && y.metaKey !== !0 && r.onKbdNavigate(y.keyCode, a.$el) === !0 && ve(y), o("keydown", y)
+        function _(w) {
+            ut(w, [13, 32]) ? v(w, !0) : gn(w) !== !0 && w.keyCode >= 35 && w.keyCode <= 40 && w.altKey !== !0 && w.metaKey !== !0 && r.onKbdNavigate(w.keyCode, a.$el) === !0 && ve(w), o("keydown", w)
         }
 
         function p() {
-            const y = r.tabProps.value.narrowIndicator,
-                P = [],
+            const w = r.tabProps.value.narrowIndicator,
+                C = [],
                 A = t.h("div", {
                     ref: c,
                     class: ["q-tab__indicator", r.tabProps.value.indicatorClass]
                 });
-            e.icon !== void 0 && P.push(t.h(Be, {
+            e.icon !== void 0 && C.push(t.h(Be, {
                 class: "q-tab__icon",
                 name: e.icon
-            })), e.label !== void 0 && P.push(t.h("div", {
+            })), e.label !== void 0 && C.push(t.h("div", {
                 class: "q-tab__label"
-            }, e.label)), e.alert !== !1 && P.push(e.alertIcon !== void 0 ? t.h(Be, {
+            }, e.label)), e.alert !== !1 && C.push(e.alertIcon !== void 0 ? t.h(Be, {
                 class: "q-tab__alert-icon",
                 color: e.alert !== !0 ? e.alert : void 0,
                 name: e.alertIcon
             }) : t.h("div", {
                 class: "q-tab__alert" + (e.alert !== !0 ? ` text-${e.alert}` : "")
-            })), y === !0 && P.push(A);
+            })), w === !0 && C.push(A);
             const M = [t.h("div", {
                 class: "q-focus-helper",
                 tabindex: -1,
                 ref: i
             }), t.h("div", {
                 class: f.value
-            }, Ke(n.default, P))];
-            return y === !1 && M.push(A), M
+            }, Ke(n.default, C))];
+            return w === !1 && M.push(A), M
         }
-        const S = {
+        const k = {
             name: t.computed(() => e.name),
             rootRef: u,
             tabIndicatorRef: c,
             routeData: l
         };
         t.onBeforeUnmount(() => {
-            r.unregisterTab(S)
+            r.unregisterTab(k)
         }), t.onMounted(() => {
-            r.registerTab(S)
+            r.registerTab(k)
         });
 
-        function C(y, P) {
+        function q(w, C) {
             const A = {
                 ref: u,
-                class: h.value,
-                tabindex: m.value,
+                class: m.value,
+                tabindex: h.value,
                 role: "tab",
                 "aria-selected": s.value === !0 ? "true" : "false",
                 "aria-disabled": e.disable === !0 ? "true" : void 0,
                 onClick: v,
-                onKeydown: x,
-                ...P
+                onKeydown: _,
+                ...C
             };
-            return t.withDirectives(t.h(y, A, p()), [
+            return t.withDirectives(t.h(w, A, p()), [
                 [Zn, d.value]
             ])
         }
         return {
-            renderTab: C,
+            renderTab: q,
             $tabs: r
         }
     }
     const Ah = se({
         name: "QTab",
         props: Eh,
         emits: Ph,
@@ -7893,15 +7897,15 @@
         }), e
     }
     const Ea = typeof ResizeObserver < "u",
         $a = Ea === !0 ? {} : {
             style: "display:block;position:absolute;top:0;left:0;right:0;bottom:0;height:100%;width:100%;overflow:hidden;pointer-events:none;z-index:-1;",
             url: "about:blank"
         },
-        Uo = se({
+        Wo = se({
             name: "QResizeObserver",
             props: {
                 debounce: {
                     type: [String, Number],
                     default: 100
                 }
             },
@@ -7946,31 +7950,31 @@
                     }), t.onBeforeUnmount(() => {
                         o !== null && clearTimeout(o), c !== void 0 && (c.disconnect !== void 0 ? c.disconnect() : l && c.unobserve(l))
                     }), Ut
                 } else {
                     let s = function() {
                             o !== null && (clearTimeout(o), o = null), d !== void 0 && (d.removeEventListener !== void 0 && d.removeEventListener("resize", a, Se.passive), d = void 0)
                         },
-                        h = function() {
+                        m = function() {
                             s(), l && l.contentDocument && (d = l.contentDocument.defaultView, d.addEventListener("resize", a, Se.passive), i())
                         };
                     const c = Oh();
                     let d;
                     return t.onMounted(() => {
                         t.nextTick(() => {
-                            l = u.$el, l && h()
+                            l = u.$el, l && m()
                         })
                     }), t.onBeforeUnmount(s), u.trigger = a, () => {
                         if (c.value === !0) return t.h("object", {
                             style: $a.style,
                             tabindex: -1,
                             type: "text/html",
                             data: $a.url,
                             "aria-hidden": "true",
-                            onLoad: h
+                            onLoad: m
                         })
                     }
                 }
             }
         });
 
     function Mh(e, n, o) {
@@ -8025,58 +8029,58 @@
                 } = Gt(), {
                     registerTick: u
                 } = Gt(), {
                     registerTimeout: c,
                     removeTimeout: d
                 } = Xt(), {
                     registerTimeout: s,
-                    removeTimeout: h
-                } = Xt(), f = t.ref(null), m = t.ref(null), v = t.ref(e.modelValue), x = t.ref(!1), p = t.ref(!0), S = t.ref(!1), C = t.ref(!1), y = [], P = t.ref(0), A = t.ref(!1);
+                    removeTimeout: m
+                } = Xt(), f = t.ref(null), h = t.ref(null), v = t.ref(e.modelValue), _ = t.ref(!1), p = t.ref(!0), k = t.ref(!1), q = t.ref(!1), w = [], C = t.ref(0), A = t.ref(!1);
                 let M = null,
                     V = null,
                     R;
-                const T = t.computed(() => ({
+                const B = t.computed(() => ({
                         activeClass: e.activeClass,
                         activeColor: e.activeColor,
                         activeBgColor: e.activeBgColor,
                         indicatorClass: Mh(e.indicatorColor, e.switchIndicator, e.vertical),
                         narrowIndicator: e.narrowIndicator,
                         inlineLabel: e.inlineLabel,
                         noCaps: e.noCaps
                     })),
-                    B = t.computed(() => {
-                        const L = P.value,
+                    P = t.computed(() => {
+                        const L = C.value,
                             W = v.value;
                         for (let E = 0; E < L; E++)
-                            if (y[E].name.value === W) return !0;
+                            if (w[E].name.value === W) return !0;
                         return !1
                     }),
-                    I = t.computed(() => `q-tabs__content--align-${x.value===!0?"left":C.value===!0?"justify":e.align}`),
-                    k = t.computed(() => `q-tabs row no-wrap items-center q-tabs--${x.value===!0?"":"not-"}scrollable q-tabs--${e.vertical===!0?"vertical":"horizontal"} q-tabs__arrows--${e.outsideArrows===!0?"outside":"inside"} q-tabs--mobile-with${e.mobileArrows===!0?"":"out"}-arrows` + (e.dense === !0 ? " q-tabs--dense" : "") + (e.shrink === !0 ? " col-shrink" : "") + (e.stretch === !0 ? " self-stretch" : "")),
+                    I = t.computed(() => `q-tabs__content--align-${_.value===!0?"left":q.value===!0?"justify":e.align}`),
+                    x = t.computed(() => `q-tabs row no-wrap items-center q-tabs--${_.value===!0?"":"not-"}scrollable q-tabs--${e.vertical===!0?"vertical":"horizontal"} q-tabs__arrows--${e.outsideArrows===!0?"outside":"inside"} q-tabs--mobile-with${e.mobileArrows===!0?"":"out"}-arrows` + (e.dense === !0 ? " q-tabs--dense" : "") + (e.shrink === !0 ? " col-shrink" : "") + (e.stretch === !0 ? " self-stretch" : "")),
                     O = t.computed(() => "q-tabs__content scroll--mobile row no-wrap items-center self-stretch hide-scrollbar relative-position " + I.value + (e.contentClass !== void 0 ? ` ${e.contentClass}` : "")),
-                    q = t.computed(() => e.vertical === !0 ? {
+                    T = t.computed(() => e.vertical === !0 ? {
                         container: "height",
                         content: "offsetHeight",
                         scroll: "scrollHeight"
                     } : {
                         container: "width",
                         content: "offsetWidth",
                         scroll: "scrollWidth"
                     }),
                     j = t.computed(() => e.vertical !== !0 && r.lang.rtl === !0),
                     N = t.computed(() => Jt === !1 && j.value === !0);
                 t.watch(j, b), t.watch(() => e.modelValue, L => {
-                    w({
+                    y({
                         name: L,
                         setCurrent: !0,
                         skipEmit: !0
                     })
                 }), t.watch(() => e.outsideArrows, z);
 
-                function w({
+                function y({
                     name: L,
                     setCurrent: W,
                     skipEmit: E
                 }) {
                     v.value !== L && (E !== !0 && e["onUpdate:modelValue"] !== void 0 && o("update:modelValue", L), (W === !0 || e["onUpdate:modelValue"] === void 0) && (J(v.value, L), v.value = L))
                 }
 
@@ -8086,60 +8090,60 @@
                             width: f.value.offsetWidth,
                             height: f.value.offsetHeight
                         })
                     })
                 }
 
                 function G(L) {
-                    if (q.value === void 0 || m.value === null) return;
-                    const W = L[q.value.container],
-                        E = Math.min(m.value[q.value.scroll], Array.prototype.reduce.call(m.value.children, (re, ie) => re + (ie[q.value.content] || 0), 0)),
+                    if (T.value === void 0 || h.value === null) return;
+                    const W = L[T.value.container],
+                        E = Math.min(h.value[T.value.scroll], Array.prototype.reduce.call(h.value.children, (re, ie) => re + (ie[T.value.content] || 0), 0)),
                         Y = W > 0 && E > W;
-                    x.value = Y, Y === !0 && i(b), C.value = W < parseInt(e.breakpoint, 10)
+                    _.value = Y, Y === !0 && i(b), q.value = W < parseInt(e.breakpoint, 10)
                 }
 
                 function J(L, W) {
-                    const E = L != null && L !== "" ? y.find(re => re.name.value === L) : null,
-                        Y = W != null && W !== "" ? y.find(re => re.name.value === W) : null;
+                    const E = L != null && L !== "" ? w.find(re => re.name.value === L) : null,
+                        Y = W != null && W !== "" ? w.find(re => re.name.value === W) : null;
                     if (E && Y) {
                         const re = E.tabIndicatorRef.value,
                             ie = Y.tabIndicatorRef.value;
                         M !== null && (clearTimeout(M), M = null), re.style.transition = "none", re.style.transform = "none", ie.style.transition = "none", ie.style.transform = "none";
                         const ae = re.getBoundingClientRect(),
                             qe = ie.getBoundingClientRect();
                         ie.style.transform = e.vertical === !0 ? `translate3d(0,${ae.top-qe.top}px,0) scale3d(1,${qe.height?ae.height/qe.height:1},1)` : `translate3d(${ae.left-qe.left}px,0,0) scale3d(${qe.width?ae.width/qe.width:1},1,1)`, u(() => {
                             M = setTimeout(() => {
                                 M = null, ie.style.transition = "transform .25s cubic-bezier(.4, 0, .2, 1)", ie.style.transform = "none"
                             }, 70)
                         })
                     }
-                    Y && x.value === !0 && _(Y.rootRef.value)
+                    Y && _.value === !0 && S(Y.rootRef.value)
                 }
 
-                function _(L) {
+                function S(L) {
                     const {
                         left: W,
                         width: E,
                         top: Y,
                         height: re
-                    } = m.value.getBoundingClientRect(), ie = L.getBoundingClientRect();
+                    } = h.value.getBoundingClientRect(), ie = L.getBoundingClientRect();
                     let ae = e.vertical === !0 ? ie.top - Y : ie.left - W;
                     if (ae < 0) {
-                        m.value[e.vertical === !0 ? "scrollTop" : "scrollLeft"] += Math.floor(ae), b();
+                        h.value[e.vertical === !0 ? "scrollTop" : "scrollLeft"] += Math.floor(ae), b();
                         return
                     }
-                    ae += e.vertical === !0 ? ie.height - re : ie.width - E, ae > 0 && (m.value[e.vertical === !0 ? "scrollTop" : "scrollLeft"] += Math.ceil(ae), b())
+                    ae += e.vertical === !0 ? ie.height - re : ie.width - E, ae > 0 && (h.value[e.vertical === !0 ? "scrollTop" : "scrollLeft"] += Math.ceil(ae), b())
                 }
 
                 function b() {
-                    const L = m.value;
+                    const L = h.value;
                     if (L === null) return;
                     const W = L.getBoundingClientRect(),
                         E = e.vertical === !0 ? L.scrollTop : Math.abs(L.scrollLeft);
-                    j.value === !0 ? (p.value = Math.ceil(E + W.width) < L.scrollWidth - 1, S.value = E > 0) : (p.value = E > 0, S.value = e.vertical === !0 ? Math.ceil(E + W.height) < L.scrollHeight : Math.ceil(E + W.width) < L.scrollWidth)
+                    j.value === !0 ? (p.value = Math.ceil(E + W.width) < L.scrollWidth - 1, k.value = E > 0) : (p.value = E > 0, k.value = e.vertical === !0 ? Math.ceil(E + W.height) < L.scrollHeight : Math.ceil(E + W.width) < L.scrollWidth)
                 }
 
                 function H(L) {
                     V !== null && clearInterval(V), V = setInterval(() => {
                         D(L) === !0 && F()
                     }, 5)
                 }
@@ -8153,26 +8157,26 @@
                 }
 
                 function F() {
                     V !== null && (clearInterval(V), V = null)
                 }
 
                 function Z(L, W) {
-                    const E = Array.prototype.filter.call(m.value.children, qe => qe === W || qe.matches && qe.matches(".q-tab.q-focusable") === !0),
+                    const E = Array.prototype.filter.call(h.value.children, qe => qe === W || qe.matches && qe.matches(".q-tab.q-focusable") === !0),
                         Y = E.length;
                     if (Y === 0) return;
-                    if (L === 36) return _(E[0]), E[0].focus(), !0;
-                    if (L === 35) return _(E[Y - 1]), E[Y - 1].focus(), !0;
+                    if (L === 36) return S(E[0]), E[0].focus(), !0;
+                    if (L === 35) return S(E[Y - 1]), E[Y - 1].focus(), !0;
                     const re = L === (e.vertical === !0 ? 38 : 37),
                         ie = L === (e.vertical === !0 ? 40 : 39),
                         ae = re === !0 ? -1 : ie === !0 ? 1 : void 0;
                     if (ae !== void 0) {
                         const qe = j.value === !0 ? -1 : 1,
                             ze = E.indexOf(W) + ae * qe;
-                        return ze >= 0 && ze < Y && (_(E[ze]), E[ze].focus({
+                        return ze >= 0 && ze < Y && (S(E[ze]), E[ze].focus({
                             preventScroll: !0
                         })), !0
                     }
                 }
                 const ue = t.computed(() => N.value === !0 ? {
                     get: L => Math.abs(L.scrollLeft),
                     set: (L, W) => {
@@ -8187,15 +8191,15 @@
                     get: L => L.scrollLeft,
                     set: (L, W) => {
                         L.scrollLeft = W
                     }
                 });
 
                 function D(L) {
-                    const W = m.value,
+                    const W = h.value,
                         {
                             get: E,
                             set: Y
                         } = ue.value;
                     let re = !1,
                         ie = E(W);
                     const ae = L < ie ? -1 : 1;
@@ -8211,15 +8215,15 @@
                 function ke() {
                     let L = null,
                         W = {
                             matchedLen: 0,
                             queryDiff: 9999,
                             hrefLen: 0
                         };
-                    const E = y.filter(ae => ae.routeData !== void 0 && ae.routeData.hasRouterLink.value === !0),
+                    const E = w.filter(ae => ae.routeData !== void 0 && ae.routeData.hasRouterLink.value === !0),
                         {
                             hash: Y,
                             query: re
                         } = l.$route,
                         ie = Object.keys(re).length;
                     for (const ae of E) {
                         const qe = ae.routeData.exact.value === !0;
@@ -8245,127 +8249,127 @@
                             L = ae.name.value, W = Re;
                             continue
                         } else if (Re.matchedLen !== W.matchedLen) continue;
                         if (Re.queryDiff < W.queryDiff) L = ae.name.value, W = Re;
                         else if (Re.queryDiff !== W.queryDiff) continue;
                         Re.hrefLen > W.hrefLen && (L = ae.name.value, W = Re)
                     }
-                    L === null && y.some(ae => ae.routeData === void 0 && ae.name.value === v.value) === !0 || w({
+                    L === null && w.some(ae => ae.routeData === void 0 && ae.name.value === v.value) === !0 || y({
                         name: L,
                         setCurrent: !0
                     })
                 }
 
                 function Ie(L) {
                     if (d(), A.value !== !0 && f.value !== null && L.target && typeof L.target.closest == "function") {
                         const W = L.target.closest(".q-tab");
-                        W && f.value.contains(W) === !0 && (A.value = !0, x.value === !0 && _(W))
+                        W && f.value.contains(W) === !0 && (A.value = !0, _.value === !0 && S(W))
                     }
                 }
 
                 function ce() {
                     c(() => {
                         A.value = !1
                     }, 30)
                 }
 
                 function ye() {
-                    je.avoidRouteWatcher === !1 ? s(ke) : h()
+                    je.avoidRouteWatcher === !1 ? s(ke) : m()
                 }
 
                 function Te() {
                     if (R === void 0) {
                         const L = t.watch(() => l.$route.fullPath, ye);
                         R = () => {
                             L(), R = void 0
                         }
                     }
                 }
 
                 function Ae(L) {
-                    y.push(L), P.value++, z(), L.routeData === void 0 || l.$route === void 0 ? s(() => {
-                        if (x.value === !0) {
+                    w.push(L), C.value++, z(), L.routeData === void 0 || l.$route === void 0 ? s(() => {
+                        if (_.value === !0) {
                             const W = v.value,
-                                E = W != null && W !== "" ? y.find(Y => Y.name.value === W) : null;
-                            E && _(E.rootRef.value)
+                                E = W != null && W !== "" ? w.find(Y => Y.name.value === W) : null;
+                            E && S(E.rootRef.value)
                         }
                     }) : (Te(), L.routeData.hasRouterLink.value === !0 && ye())
                 }
 
                 function Ue(L) {
-                    y.splice(y.indexOf(L), 1), P.value--, z(), R !== void 0 && L.routeData !== void 0 && (y.every(W => W.routeData === void 0) === !0 && R(), ye())
+                    w.splice(w.indexOf(L), 1), C.value--, z(), R !== void 0 && L.routeData !== void 0 && (w.every(W => W.routeData === void 0) === !0 && R(), ye())
                 }
                 const je = {
                     currentModel: v,
-                    tabProps: T,
+                    tabProps: B,
                     hasFocus: A,
-                    hasActiveTab: B,
+                    hasActiveTab: P,
                     registerTab: Ae,
                     unregisterTab: Ue,
                     verifyRouteModel: ye,
-                    updateModel: w,
+                    updateModel: y,
                     onKbdNavigate: Z,
                     avoidRouteWatcher: !1
                 };
-                t.provide(cl, je);
+                t.provide(dl, je);
 
                 function We() {
                     M !== null && clearTimeout(M), F(), R !== void 0 && R()
                 }
                 let Ce;
                 return t.onBeforeUnmount(We), t.onDeactivated(() => {
                     Ce = R !== void 0, We()
                 }), t.onActivated(() => {
                     Ce === !0 && Te(), z()
                 }), () => t.h("div", {
                     ref: f,
-                    class: k.value,
+                    class: x.value,
                     role: "tablist",
                     onFocusin: Ie,
                     onFocusout: ce
-                }, [t.h(Uo, {
+                }, [t.h(Wo, {
                     onResize: G
                 }), t.h("div", {
-                    ref: m,
+                    ref: h,
                     class: O.value,
                     onScroll: b
                 }, we(n.default)), t.h(Be, {
                     class: "q-tabs__arrow q-tabs__arrow--left absolute q-tab__icon" + (p.value === !0 ? "" : " q-tabs__arrow--faded"),
                     name: e.leftIcon || r.iconSet.tabs[e.vertical === !0 ? "up" : "left"],
                     onMousedownPassive: te,
                     onTouchstartPassive: te,
                     onMouseupPassive: F,
                     onMouseleavePassive: F,
                     onTouchendPassive: F
                 }), t.h(Be, {
-                    class: "q-tabs__arrow q-tabs__arrow--right absolute q-tab__icon" + (S.value === !0 ? "" : " q-tabs__arrow--faded"),
+                    class: "q-tabs__arrow q-tabs__arrow--right absolute q-tab__icon" + (k.value === !0 ? "" : " q-tabs__arrow--faded"),
                     name: e.rightIcon || r.iconSet.tabs[e.vertical === !0 ? "down" : "right"],
                     onMousedownPassive: U,
                     onTouchstartPassive: U,
                     onMouseupPassive: F,
                     onMouseleavePassive: F,
                     onTouchendPassive: F
                 })])
             }
         }),
-        Wo = {
+        Ko = {
             left: !0,
             right: !0,
             up: !0,
             down: !0,
             horizontal: !0,
             vertical: !0
         },
-        Ih = Object.keys(Wo);
-    Wo.all = !0;
+        Ih = Object.keys(Ko);
+    Ko.all = !0;
 
     function $n(e) {
         const n = {};
         for (const o of Ih) e[o] === !0 && (n[o] = !0);
-        return Object.keys(n).length === 0 ? Wo : (n.horizontal === !0 ? n.left = n.right = !0 : n.left === !0 && n.right === !0 && (n.horizontal = !0), n.vertical === !0 ? n.up = n.down = !0 : n.up === !0 && n.down === !0 && (n.vertical = !0), n.horizontal === !0 && n.vertical === !0 && (n.all = !0), n)
+        return Object.keys(n).length === 0 ? Ko : (n.horizontal === !0 ? n.left = n.right = !0 : n.left === !0 && n.right === !0 && (n.horizontal = !0), n.vertical === !0 ? n.up = n.down = !0 : n.up === !0 && n.down === !0 && (n.vertical = !0), n.horizontal === !0 && n.vertical === !0 && (n.all = !0), n)
     }
     const zh = ["INPUT", "TEXTAREA"];
 
     function An(e, n) {
         return n.event === void 0 && e.target !== void 0 && e.target.draggable !== !0 && typeof n.handler == "function" && zh.includes(e.target.nodeName.toUpperCase()) === !1 && (e.qClonedBy === void 0 || e.qClonedBy.indexOf(n.uid) === -1)
     }
 
@@ -8387,15 +8391,15 @@
             const r = l.mouseCapture === !0 ? "Capture" : "",
                 a = {
                     handler: n,
                     sensitivity: Lh(o),
                     direction: $n(l),
                     noop: Ut,
                     mouseStart(i) {
-                        An(i, a) && pl(i) && (Qe(a, "temp", [
+                        An(i, a) && bl(i) && (Qe(a, "temp", [
                             [document, "mousemove", "move", `notPassive${r}`],
                             [document, "mouseup", "end", "notPassiveCapture"]
                         ]), a.start(i, !0))
                     },
                     touchStart(i) {
                         if (An(i, a)) {
                             const u = i.target;
@@ -8424,33 +8428,33 @@
                             return
                         }
                         const u = Date.now() - a.event.time;
                         if (u === 0) return;
                         const c = dt(i),
                             d = c.left - a.event.x,
                             s = Math.abs(d),
-                            h = c.top - a.event.y,
-                            f = Math.abs(h);
+                            m = c.top - a.event.y,
+                            f = Math.abs(m);
                         if (a.event.mouse !== !0) {
                             if (s < a.sensitivity[1] && f < a.sensitivity[1]) {
                                 a.end(i);
                                 return
                             }
                         } else if (window.getSelection().toString() !== "") {
                             a.end(i);
                             return
                         } else if (s < a.sensitivity[2] && f < a.sensitivity[2]) return;
-                        const m = s / u,
+                        const h = s / u,
                             v = f / u;
-                        a.direction.vertical === !0 && s < f && s < 100 && v > a.sensitivity[0] && (a.event.dir = h < 0 ? "up" : "down"), a.direction.horizontal === !0 && s > f && f < 100 && m > a.sensitivity[0] && (a.event.dir = d < 0 ? "left" : "right"), a.direction.up === !0 && s < f && h < 0 && s < 100 && v > a.sensitivity[0] && (a.event.dir = "up"), a.direction.down === !0 && s < f && h > 0 && s < 100 && v > a.sensitivity[0] && (a.event.dir = "down"), a.direction.left === !0 && s > f && d < 0 && f < 100 && m > a.sensitivity[0] && (a.event.dir = "left"), a.direction.right === !0 && s > f && d > 0 && f < 100 && m > a.sensitivity[0] && (a.event.dir = "right"), a.event.dir !== !1 ? (ve(i), a.event.mouse === !0 && (document.body.classList.add("no-pointer-events--children"), document.body.classList.add("non-selectable"), no(), a.styleCleanup = x => {
+                        a.direction.vertical === !0 && s < f && s < 100 && v > a.sensitivity[0] && (a.event.dir = m < 0 ? "up" : "down"), a.direction.horizontal === !0 && s > f && f < 100 && h > a.sensitivity[0] && (a.event.dir = d < 0 ? "left" : "right"), a.direction.up === !0 && s < f && m < 0 && s < 100 && v > a.sensitivity[0] && (a.event.dir = "up"), a.direction.down === !0 && s < f && m > 0 && s < 100 && v > a.sensitivity[0] && (a.event.dir = "down"), a.direction.left === !0 && s > f && d < 0 && f < 100 && h > a.sensitivity[0] && (a.event.dir = "left"), a.direction.right === !0 && s > f && d > 0 && f < 100 && h > a.sensitivity[0] && (a.event.dir = "right"), a.event.dir !== !1 ? (ve(i), a.event.mouse === !0 && (document.body.classList.add("no-pointer-events--children"), document.body.classList.add("non-selectable"), no(), a.styleCleanup = _ => {
                             a.styleCleanup = void 0, document.body.classList.remove("non-selectable");
                             const p = () => {
                                 document.body.classList.remove("no-pointer-events--children")
                             };
-                            x === !0 ? setTimeout(p, 50) : p()
+                            _ === !0 ? setTimeout(p, 50) : p()
                         }), a.handler({
                             evt: i,
                             touch: a.event.mouse !== !0,
                             mouse: a.event.mouse,
                             direction: a.event.dir,
                             duration: u,
                             distance: {
@@ -8541,138 +8545,138 @@
             getCacheWithFn: l
         } = Dh();
         let r, a;
         const i = t.ref(null),
             u = t.ref(null);
 
         function c(O) {
-            const q = e.vertical === !0 ? "up" : "left";
-            V((o.$q.lang.rtl === !0 ? -1 : 1) * (O.direction === q ? 1 : -1))
+            const T = e.vertical === !0 ? "up" : "left";
+            V((o.$q.lang.rtl === !0 ? -1 : 1) * (O.direction === T ? 1 : -1))
         }
         const d = t.computed(() => [
                 [Fh, c, void 0, {
                     horizontal: e.vertical !== !0,
                     vertical: e.vertical,
                     mouse: !0
                 }]
             ]),
             s = t.computed(() => e.transitionPrev || `slide-${e.vertical===!0?"down":"right"}`),
-            h = t.computed(() => e.transitionNext || `slide-${e.vertical===!0?"up":"left"}`),
+            m = t.computed(() => e.transitionNext || `slide-${e.vertical===!0?"up":"left"}`),
             f = t.computed(() => `--q-transition-duration: ${e.transitionDuration}ms`),
-            m = t.computed(() => typeof e.modelValue == "string" || typeof e.modelValue == "number" ? e.modelValue : String(e.modelValue)),
+            h = t.computed(() => typeof e.modelValue == "string" || typeof e.modelValue == "number" ? e.modelValue : String(e.modelValue)),
             v = t.computed(() => ({
                 include: e.keepAliveInclude,
                 exclude: e.keepAliveExclude,
                 max: e.keepAliveMax
             })),
-            x = t.computed(() => e.keepAliveInclude !== void 0 || e.keepAliveExclude !== void 0);
-        t.watch(() => e.modelValue, (O, q) => {
-            const j = y(O) === !0 ? P(O) : -1;
-            a !== !0 && M(j === -1 ? 0 : j < P(q) ? -1 : 1), i.value !== j && (i.value = j, n("beforeTransition", O, q), t.nextTick(() => {
-                n("transition", O, q)
+            _ = t.computed(() => e.keepAliveInclude !== void 0 || e.keepAliveExclude !== void 0);
+        t.watch(() => e.modelValue, (O, T) => {
+            const j = w(O) === !0 ? C(O) : -1;
+            a !== !0 && M(j === -1 ? 0 : j < C(T) ? -1 : 1), i.value !== j && (i.value = j, n("beforeTransition", O, T), t.nextTick(() => {
+                n("transition", O, T)
             }))
         });
 
         function p() {
             V(1)
         }
 
-        function S() {
+        function k() {
             V(-1)
         }
 
-        function C(O) {
+        function q(O) {
             n("update:modelValue", O)
         }
 
-        function y(O) {
+        function w(O) {
             return O != null && O !== ""
         }
 
-        function P(O) {
-            return r.findIndex(q => q.props.name === O && q.props.disable !== "" && q.props.disable !== !0)
+        function C(O) {
+            return r.findIndex(T => T.props.name === O && T.props.disable !== "" && T.props.disable !== !0)
         }
 
         function A() {
             return r.filter(O => O.props.disable !== "" && O.props.disable !== !0)
         }
 
         function M(O) {
-            const q = O !== 0 && e.animated === !0 && i.value !== -1 ? "q-transition--" + (O === -1 ? s.value : h.value) : null;
-            u.value !== q && (u.value = q)
+            const T = O !== 0 && e.animated === !0 && i.value !== -1 ? "q-transition--" + (O === -1 ? s.value : m.value) : null;
+            u.value !== T && (u.value = T)
         }
 
-        function V(O, q = i.value) {
-            let j = q + O;
+        function V(O, T = i.value) {
+            let j = T + O;
             for (; j > -1 && j < r.length;) {
                 const N = r[j];
                 if (N !== void 0 && N.props.disable !== "" && N.props.disable !== !0) {
                     M(O), a = !0, n("update:modelValue", N.props.name), setTimeout(() => {
                         a = !1
                     });
                     return
                 }
                 j += O
             }
-            e.infinite === !0 && r.length !== 0 && q !== -1 && q !== r.length && V(O, O === -1 ? r.length : -1)
+            e.infinite === !0 && r.length !== 0 && T !== -1 && T !== r.length && V(O, O === -1 ? r.length : -1)
         }
 
         function R() {
-            const O = P(e.modelValue);
+            const O = C(e.modelValue);
             return i.value !== O && (i.value = O), !0
         }
 
-        function T() {
-            const O = y(e.modelValue) === !0 && R() && r[i.value];
-            return e.keepAlive === !0 ? [t.h(t.KeepAlive, v.value, [t.h(x.value === !0 ? l(m.value, () => ({
+        function B() {
+            const O = w(e.modelValue) === !0 && R() && r[i.value];
+            return e.keepAlive === !0 ? [t.h(t.KeepAlive, v.value, [t.h(_.value === !0 ? l(h.value, () => ({
                 ...Aa,
-                name: m.value
+                name: h.value
             })) : Aa, {
-                key: m.value,
+                key: h.value,
                 style: f.value
             }, () => O)])] : [t.h("div", {
                 class: "q-panel scroll",
                 style: f.value,
-                key: m.value,
+                key: h.value,
                 role: "tabpanel"
             }, [O])]
         }
 
-        function B() {
+        function P() {
             if (r.length !== 0) return e.animated === !0 ? [t.h(t.Transition, {
                 name: u.value
-            }, T)] : T()
+            }, B)] : B()
         }
 
         function I(O) {
-            return r = xi(we(O.default, [])).filter(q => q.props !== null && q.props.slot === void 0 && y(q.props.name) === !0), r.length
+            return r = xi(we(O.default, [])).filter(T => T.props !== null && T.props.slot === void 0 && w(T.props.name) === !0), r.length
         }
 
-        function k() {
+        function x() {
             return r
         }
         return Object.assign(o, {
             next: p,
-            previous: S,
-            goTo: C
+            previous: k,
+            goTo: q
         }), {
             panelIndex: i,
             panelDirectives: d,
             updatePanelsList: I,
             updatePanelIndex: R,
-            getPanelContent: B,
+            getPanelContent: P,
             getEnabledPanels: A,
-            getPanels: k,
-            isValidPanelName: y,
+            getPanels: x,
+            isValidPanelName: w,
             keepAliveProps: v,
-            needsUniqueKeepAliveWrapper: x,
+            needsUniqueKeepAliveWrapper: _,
             goToPanelByOffset: V,
-            goToPanel: C,
+            goToPanel: q,
             nextPanel: p,
-            previousPanel: S
+            previousPanel: k
         }
     }
     const Wh = se({
             name: "QTabPanel",
             props: jh,
             setup(e, {
                 slots: n
@@ -8851,255 +8855,255 @@
             fillMask: [Boolean, String],
             unmaskedValue: Boolean
         };
 
     function Zh(e, n, o, l) {
         let r, a, i, u, c, d;
         const s = t.ref(null),
-            h = t.ref(m());
+            m = t.ref(h());
 
         function f() {
             return e.autogrow === !0 || ["textarea", "text", "search", "url", "tel", "password"].includes(e.type)
         }
-        t.watch(() => e.type + e.autogrow, x), t.watch(() => e.mask, T => {
-            if (T !== void 0) p(h.value, !0);
+        t.watch(() => e.type + e.autogrow, _), t.watch(() => e.mask, B => {
+            if (B !== void 0) p(m.value, !0);
             else {
-                const B = V(h.value);
-                x(), e.modelValue !== B && n("update:modelValue", B)
+                const P = V(m.value);
+                _(), e.modelValue !== P && n("update:modelValue", P)
             }
         }), t.watch(() => e.fillMask + e.reverseFillMask, () => {
-            s.value === !0 && p(h.value, !0)
+            s.value === !0 && p(m.value, !0)
         }), t.watch(() => e.unmaskedValue, () => {
-            s.value === !0 && p(h.value)
+            s.value === !0 && p(m.value)
         });
 
-        function m() {
-            if (x(), s.value === !0) {
-                const T = A(V(e.modelValue));
-                return e.fillMask !== !1 ? R(T) : T
+        function h() {
+            if (_(), s.value === !0) {
+                const B = A(V(e.modelValue));
+                return e.fillMask !== !1 ? R(B) : B
             }
             return e.modelValue
         }
 
-        function v(T) {
-            if (T < r.length) return r.slice(-T);
-            let B = "",
+        function v(B) {
+            if (B < r.length) return r.slice(-B);
+            let P = "",
                 I = r;
-            const k = I.indexOf(xe);
-            if (k > -1) {
-                for (let O = T - I.length; O > 0; O--) B += xe;
-                I = I.slice(0, k) + B + I.slice(k)
+            const x = I.indexOf(xe);
+            if (x > -1) {
+                for (let O = B - I.length; O > 0; O--) P += xe;
+                I = I.slice(0, x) + P + I.slice(x)
             }
             return I
         }
 
-        function x() {
+        function _() {
             if (s.value = e.mask !== void 0 && e.mask.length !== 0 && f(), s.value === !1) {
                 u = void 0, r = "", a = "";
                 return
             }
-            const T = Oa[e.mask] === void 0 ? e.mask : Oa[e.mask],
-                B = typeof e.fillMask == "string" && e.fillMask.length !== 0 ? e.fillMask.slice(0, 1) : "_",
-                I = B.replace(Ra, "\\$&"),
-                k = [],
+            const B = Oa[e.mask] === void 0 ? e.mask : Oa[e.mask],
+                P = typeof e.fillMask == "string" && e.fillMask.length !== 0 ? e.fillMask.slice(0, 1) : "_",
+                I = P.replace(Ra, "\\$&"),
+                x = [],
                 O = [],
-                q = [];
+                T = [];
             let j = e.reverseFillMask === !0,
                 N = "",
-                w = "";
-            T.replace(Xh, (_, b, H, te, U) => {
+                y = "";
+            B.replace(Xh, (S, b, H, te, U) => {
                 if (te !== void 0) {
                     const F = On[te];
-                    q.push(F), w = F.negate, j === !0 && (O.push("(?:" + w + "+)?(" + F.pattern + "+)?(?:" + w + "+)?(" + F.pattern + "+)?"), j = !1), O.push("(?:" + w + "+)?(" + F.pattern + ")?")
-                } else if (H !== void 0) N = "\\" + (H === "\\" ? "" : H), q.push(H), k.push("([^" + N + "]+)?" + N + "?");
+                    T.push(F), y = F.negate, j === !0 && (O.push("(?:" + y + "+)?(" + F.pattern + "+)?(?:" + y + "+)?(" + F.pattern + "+)?"), j = !1), O.push("(?:" + y + "+)?(" + F.pattern + ")?")
+                } else if (H !== void 0) N = "\\" + (H === "\\" ? "" : H), T.push(H), x.push("([^" + N + "]+)?" + N + "?");
                 else {
                     const F = b !== void 0 ? b : U;
-                    N = F === "\\" ? "\\\\\\\\" : F.replace(Ra, "\\\\$&"), q.push(F), k.push("([^" + N + "]+)?" + N + "?")
+                    N = F === "\\" ? "\\\\\\\\" : F.replace(Ra, "\\\\$&"), T.push(F), x.push("([^" + N + "]+)?" + N + "?")
                 }
             });
-            const z = new RegExp("^" + k.join("") + "(" + (N === "" ? "." : "[^" + N + "]") + "+)?" + (N === "" ? "" : "[" + N + "]*") + "$"),
+            const z = new RegExp("^" + x.join("") + "(" + (N === "" ? "." : "[^" + N + "]") + "+)?" + (N === "" ? "" : "[" + N + "]*") + "$"),
                 G = O.length - 1,
-                J = O.map((_, b) => b === 0 && e.reverseFillMask === !0 ? new RegExp("^" + I + "*" + _) : b === G ? new RegExp("^" + _ + "(" + (w === "" ? "." : w) + "+)?" + (e.reverseFillMask === !0 ? "$" : I + "*")) : new RegExp("^" + _));
-            i = q, u = _ => {
-                const b = z.exec(e.reverseFillMask === !0 ? _ : _.slice(0, q.length + 1));
-                b !== null && (_ = b.slice(1).join(""));
+                J = O.map((S, b) => b === 0 && e.reverseFillMask === !0 ? new RegExp("^" + I + "*" + S) : b === G ? new RegExp("^" + S + "(" + (y === "" ? "." : y) + "+)?" + (e.reverseFillMask === !0 ? "$" : I + "*")) : new RegExp("^" + S));
+            i = T, u = S => {
+                const b = z.exec(e.reverseFillMask === !0 ? S : S.slice(0, T.length + 1));
+                b !== null && (S = b.slice(1).join(""));
                 const H = [],
                     te = J.length;
-                for (let U = 0, F = _; U < te; U++) {
+                for (let U = 0, F = S; U < te; U++) {
                     const Z = J[U].exec(F);
                     if (Z === null) break;
                     F = F.slice(Z.shift().length), H.push(...Z)
                 }
-                return H.length !== 0 ? H.join("") : _
-            }, r = q.map(_ => typeof _ == "string" ? _ : xe).join(""), a = r.split(xe).join(B)
+                return H.length !== 0 ? H.join("") : S
+            }, r = T.map(S => typeof S == "string" ? S : xe).join(""), a = r.split(xe).join(P)
         }
 
-        function p(T, B, I) {
-            const k = l.value,
-                O = k.selectionEnd,
-                q = k.value.length - O,
-                j = V(T);
-            B === !0 && x();
+        function p(B, P, I) {
+            const x = l.value,
+                O = x.selectionEnd,
+                T = x.value.length - O,
+                j = V(B);
+            P === !0 && _();
             const N = A(j),
-                w = e.fillMask !== !1 ? R(N) : N,
-                z = h.value !== w;
-            k.value !== w && (k.value = w), z === !0 && (h.value = w), document.activeElement === k && t.nextTick(() => {
-                if (w === a) {
+                y = e.fillMask !== !1 ? R(N) : N,
+                z = m.value !== y;
+            x.value !== y && (x.value = y), z === !0 && (m.value = y), document.activeElement === x && t.nextTick(() => {
+                if (y === a) {
                     const J = e.reverseFillMask === !0 ? a.length : 0;
-                    k.setSelectionRange(J, J, "forward");
+                    x.setSelectionRange(J, J, "forward");
                     return
                 }
                 if (I === "insertFromPaste" && e.reverseFillMask !== !0) {
-                    const J = k.selectionEnd;
-                    let _ = O - 1;
-                    for (let b = c; b <= _ && b < J; b++) r[b] !== xe && _++;
-                    C.right(k, _);
+                    const J = x.selectionEnd;
+                    let S = O - 1;
+                    for (let b = c; b <= S && b < J; b++) r[b] !== xe && S++;
+                    q.right(x, S);
                     return
                 }
                 if (["deleteContentBackward", "deleteContentForward"].indexOf(I) > -1) {
-                    const J = e.reverseFillMask === !0 ? O === 0 ? w.length > N.length ? 1 : 0 : Math.max(0, w.length - (w === a ? 0 : Math.min(N.length, q) + 1)) + 1 : O;
-                    k.setSelectionRange(J, J, "forward");
+                    const J = e.reverseFillMask === !0 ? O === 0 ? y.length > N.length ? 1 : 0 : Math.max(0, y.length - (y === a ? 0 : Math.min(N.length, T) + 1)) + 1 : O;
+                    x.setSelectionRange(J, J, "forward");
                     return
                 }
                 if (e.reverseFillMask === !0)
                     if (z === !0) {
-                        const J = Math.max(0, w.length - (w === a ? 0 : Math.min(N.length, q + 1)));
-                        J === 1 && O === 1 ? k.setSelectionRange(J, J, "forward") : C.rightReverse(k, J)
+                        const J = Math.max(0, y.length - (y === a ? 0 : Math.min(N.length, T + 1)));
+                        J === 1 && O === 1 ? x.setSelectionRange(J, J, "forward") : q.rightReverse(x, J)
                     } else {
-                        const J = w.length - q;
-                        k.setSelectionRange(J, J, "backward")
+                        const J = y.length - T;
+                        x.setSelectionRange(J, J, "backward")
                     }
                 else if (z === !0) {
                     const J = Math.max(0, r.indexOf(xe), Math.min(N.length, O) - 1);
-                    C.right(k, J)
+                    q.right(x, J)
                 } else {
                     const J = O - 1;
-                    C.right(k, J)
+                    q.right(x, J)
                 }
             });
-            const G = e.unmaskedValue === !0 ? V(w) : w;
+            const G = e.unmaskedValue === !0 ? V(y) : y;
             String(e.modelValue) !== G && (e.modelValue !== null || G !== "") && o(G, !0)
         }
 
-        function S(T, B, I) {
-            const k = A(V(T.value));
-            B = Math.max(0, r.indexOf(xe), Math.min(k.length, B)), c = B, T.setSelectionRange(B, I, "forward")
-        }
-        const C = {
-            left(T, B) {
-                const I = r.slice(B - 1).indexOf(xe) === -1;
-                let k = Math.max(0, B - 1);
-                for (; k >= 0; k--)
-                    if (r[k] === xe) {
-                        B = k, I === !0 && B++;
+        function k(B, P, I) {
+            const x = A(V(B.value));
+            P = Math.max(0, r.indexOf(xe), Math.min(x.length, P)), c = P, B.setSelectionRange(P, I, "forward")
+        }
+        const q = {
+            left(B, P) {
+                const I = r.slice(P - 1).indexOf(xe) === -1;
+                let x = Math.max(0, P - 1);
+                for (; x >= 0; x--)
+                    if (r[x] === xe) {
+                        P = x, I === !0 && P++;
                         break
-                    } if (k < 0 && r[B] !== void 0 && r[B] !== xe) return C.right(T, 0);
-                B >= 0 && T.setSelectionRange(B, B, "backward")
+                    } if (x < 0 && r[P] !== void 0 && r[P] !== xe) return q.right(B, 0);
+                P >= 0 && B.setSelectionRange(P, P, "backward")
             },
-            right(T, B) {
-                const I = T.value.length;
-                let k = Math.min(I, B + 1);
-                for (; k <= I; k++)
-                    if (r[k] === xe) {
-                        B = k;
+            right(B, P) {
+                const I = B.value.length;
+                let x = Math.min(I, P + 1);
+                for (; x <= I; x++)
+                    if (r[x] === xe) {
+                        P = x;
                         break
-                    } else r[k - 1] === xe && (B = k);
-                if (k > I && r[B - 1] !== void 0 && r[B - 1] !== xe) return C.left(T, I);
-                T.setSelectionRange(B, B, "forward")
-            },
-            leftReverse(T, B) {
-                const I = v(T.value.length);
-                let k = Math.max(0, B - 1);
-                for (; k >= 0; k--)
-                    if (I[k - 1] === xe) {
-                        B = k;
+                    } else r[x - 1] === xe && (P = x);
+                if (x > I && r[P - 1] !== void 0 && r[P - 1] !== xe) return q.left(B, I);
+                B.setSelectionRange(P, P, "forward")
+            },
+            leftReverse(B, P) {
+                const I = v(B.value.length);
+                let x = Math.max(0, P - 1);
+                for (; x >= 0; x--)
+                    if (I[x - 1] === xe) {
+                        P = x;
                         break
-                    } else if (I[k] === xe && (B = k, k === 0)) break;
-                if (k < 0 && I[B] !== void 0 && I[B] !== xe) return C.rightReverse(T, 0);
-                B >= 0 && T.setSelectionRange(B, B, "backward")
-            },
-            rightReverse(T, B) {
-                const I = T.value.length,
-                    k = v(I),
-                    O = k.slice(0, B + 1).indexOf(xe) === -1;
-                let q = Math.min(I, B + 1);
-                for (; q <= I; q++)
-                    if (k[q - 1] === xe) {
-                        B = q, B > 0 && O === !0 && B--;
+                    } else if (I[x] === xe && (P = x, x === 0)) break;
+                if (x < 0 && I[P] !== void 0 && I[P] !== xe) return q.rightReverse(B, 0);
+                P >= 0 && B.setSelectionRange(P, P, "backward")
+            },
+            rightReverse(B, P) {
+                const I = B.value.length,
+                    x = v(I),
+                    O = x.slice(0, P + 1).indexOf(xe) === -1;
+                let T = Math.min(I, P + 1);
+                for (; T <= I; T++)
+                    if (x[T - 1] === xe) {
+                        P = T, P > 0 && O === !0 && P--;
                         break
-                    } if (q > I && k[B - 1] !== void 0 && k[B - 1] !== xe) return C.leftReverse(T, I);
-                T.setSelectionRange(B, B, "forward")
+                    } if (T > I && x[P - 1] !== void 0 && x[P - 1] !== xe) return q.leftReverse(B, I);
+                B.setSelectionRange(P, P, "forward")
             }
         };
 
-        function y(T) {
-            n("click", T), d = void 0
+        function w(B) {
+            n("click", B), d = void 0
         }
 
-        function P(T) {
-            if (n("keydown", T), gn(T) === !0 || T.altKey === !0) return;
-            const B = l.value,
-                I = B.selectionStart,
-                k = B.selectionEnd;
-            if (T.shiftKey || (d = void 0), T.keyCode === 37 || T.keyCode === 39) {
-                T.shiftKey && d === void 0 && (d = B.selectionDirection === "forward" ? I : k);
-                const O = C[(T.keyCode === 39 ? "right" : "left") + (e.reverseFillMask === !0 ? "Reverse" : "")];
-                if (T.preventDefault(), O(B, d === I ? k : I), T.shiftKey) {
-                    const q = B.selectionStart;
-                    B.setSelectionRange(Math.min(d, q), Math.max(d, q), "forward")
-                }
-            } else T.keyCode === 8 && e.reverseFillMask !== !0 && I === k ? (C.left(B, I), B.setSelectionRange(B.selectionStart, k, "backward")) : T.keyCode === 46 && e.reverseFillMask === !0 && I === k && (C.rightReverse(B, k), B.setSelectionRange(I, B.selectionEnd, "forward"))
-        }
-
-        function A(T) {
-            if (T == null || T === "") return "";
-            if (e.reverseFillMask === !0) return M(T);
-            const B = i;
+        function C(B) {
+            if (n("keydown", B), gn(B) === !0 || B.altKey === !0) return;
+            const P = l.value,
+                I = P.selectionStart,
+                x = P.selectionEnd;
+            if (B.shiftKey || (d = void 0), B.keyCode === 37 || B.keyCode === 39) {
+                B.shiftKey && d === void 0 && (d = P.selectionDirection === "forward" ? I : x);
+                const O = q[(B.keyCode === 39 ? "right" : "left") + (e.reverseFillMask === !0 ? "Reverse" : "")];
+                if (B.preventDefault(), O(P, d === I ? x : I), B.shiftKey) {
+                    const T = P.selectionStart;
+                    P.setSelectionRange(Math.min(d, T), Math.max(d, T), "forward")
+                }
+            } else B.keyCode === 8 && e.reverseFillMask !== !0 && I === x ? (q.left(P, I), P.setSelectionRange(P.selectionStart, x, "backward")) : B.keyCode === 46 && e.reverseFillMask === !0 && I === x && (q.rightReverse(P, x), P.setSelectionRange(I, P.selectionEnd, "forward"))
+        }
+
+        function A(B) {
+            if (B == null || B === "") return "";
+            if (e.reverseFillMask === !0) return M(B);
+            const P = i;
             let I = 0,
-                k = "";
-            for (let O = 0; O < B.length; O++) {
-                const q = T[I],
-                    j = B[O];
-                if (typeof j == "string") k += j, q === j && I++;
-                else if (q !== void 0 && j.regex.test(q)) k += j.transform !== void 0 ? j.transform(q) : q, I++;
-                else return k
+                x = "";
+            for (let O = 0; O < P.length; O++) {
+                const T = B[I],
+                    j = P[O];
+                if (typeof j == "string") x += j, T === j && I++;
+                else if (T !== void 0 && j.regex.test(T)) x += j.transform !== void 0 ? j.transform(T) : T, I++;
+                else return x
             }
-            return k
+            return x
         }
 
-        function M(T) {
-            const B = i,
+        function M(B) {
+            const P = i,
                 I = r.indexOf(xe);
-            let k = T.length - 1,
+            let x = B.length - 1,
                 O = "";
-            for (let q = B.length - 1; q >= 0 && k > -1; q--) {
-                const j = B[q];
-                let N = T[k];
-                if (typeof j == "string") O = j + O, N === j && k--;
+            for (let T = P.length - 1; T >= 0 && x > -1; T--) {
+                const j = P[T];
+                let N = B[x];
+                if (typeof j == "string") O = j + O, N === j && x--;
                 else if (N !== void 0 && j.regex.test(N))
-                    do O = (j.transform !== void 0 ? j.transform(N) : N) + O, k--, N = T[k]; while (I === q && N !== void 0 && j.regex.test(N));
+                    do O = (j.transform !== void 0 ? j.transform(N) : N) + O, x--, N = B[x]; while (I === T && N !== void 0 && j.regex.test(N));
                 else return O
             }
             return O
         }
 
-        function V(T) {
-            return typeof T != "string" || u === void 0 ? typeof T == "number" ? u("" + T) : T : u(T)
+        function V(B) {
+            return typeof B != "string" || u === void 0 ? typeof B == "number" ? u("" + B) : B : u(B)
         }
 
-        function R(T) {
-            return a.length - T.length <= 0 ? T : e.reverseFillMask === !0 && T.length !== 0 ? a.slice(0, -T.length) + T : T + a.slice(T.length)
+        function R(B) {
+            return a.length - B.length <= 0 ? B : e.reverseFillMask === !0 && B.length !== 0 ? a.slice(0, -B.length) + B : B + a.slice(B.length)
         }
         return {
-            innerValue: h,
+            innerValue: m,
             hasMask: s,
-            moveCursorForPaste: S,
+            moveCursorForPaste: k,
             updateMaskValue: p,
-            onMaskedKeydown: P,
-            onMaskedClick: y
+            onMaskedKeydown: C,
+            onMaskedClick: w
         }
     }
 
     function Jh(e, n) {
         function o() {
             const l = e.modelValue;
             try {
@@ -9148,42 +9152,42 @@
                     proxy: l
                 } = t.getCurrentInstance(), {
                     $q: r
                 } = l, a = {};
                 let i = NaN,
                     u, c, d = null,
                     s;
-                const h = t.ref(null),
-                    f = cr(e),
+                const m = t.ref(null),
+                    f = dr(e),
                     {
-                        innerValue: m,
+                        innerValue: h,
                         hasMask: v,
-                        moveCursorForPaste: x,
+                        moveCursorForPaste: _,
                         updateMaskValue: p,
-                        onMaskedKeydown: S,
-                        onMaskedClick: C
-                    } = Zh(e, n, N, h),
-                    y = Jh(e, !0),
-                    P = t.computed(() => Kt(m.value)),
-                    A = dr(q),
+                        onMaskedKeydown: k,
+                        onMaskedClick: q
+                    } = Zh(e, n, N, m),
+                    w = Jh(e, !0),
+                    C = t.computed(() => Kt(h.value)),
+                    A = fr(T),
                     M = Gn(),
                     V = t.computed(() => e.type === "textarea" || e.autogrow === !0),
                     R = t.computed(() => V.value === !0 || ["text", "search", "url", "tel", "password"].includes(e.type)),
-                    T = t.computed(() => {
+                    B = t.computed(() => {
                         const b = {
                             ...M.splitAttrs.listeners.value,
-                            onInput: q,
+                            onInput: T,
                             onPaste: O,
                             onChange: z,
                             onBlur: G,
                             onFocus: De
                         };
-                        return b.onCompositionstart = b.onCompositionupdate = b.onCompositionend = A, v.value === !0 && (b.onKeydown = S, b.onClick = C), e.autogrow === !0 && (b.onAnimationend = j), b
+                        return b.onCompositionstart = b.onCompositionupdate = b.onCompositionend = A, v.value === !0 && (b.onKeydown = k, b.onClick = q), e.autogrow === !0 && (b.onAnimationend = j), b
                     }),
-                    B = t.computed(() => {
+                    P = t.computed(() => {
                         const b = {
                             tabindex: 0,
                             "data-autofocus": e.autofocus === !0 || void 0,
                             rows: e.type === "textarea" ? 6 : void 0,
                             "aria-label": e.label,
                             name: f.value,
                             ...M.splitAttrs.attributes.value,
@@ -9191,49 +9195,49 @@
                             maxlength: e.maxlength,
                             disabled: e.disable === !0,
                             readonly: e.readonly === !0
                         };
                         return V.value === !1 && (b.type = e.type), e.autogrow === !0 && (b.rows = 1), b
                     });
                 t.watch(() => e.type, () => {
-                    h.value && (h.value.value = e.modelValue)
+                    m.value && (m.value.value = e.modelValue)
                 }), t.watch(() => e.modelValue, b => {
                     if (v.value === !0) {
                         if (c === !0 && (c = !1, String(b) === i)) return;
                         p(b)
-                    } else m.value !== b && (m.value = b, e.type === "number" && a.hasOwnProperty("value") === !0 && (u === !0 ? u = !1 : delete a.value));
-                    e.autogrow === !0 && t.nextTick(w)
+                    } else h.value !== b && (h.value = b, e.type === "number" && a.hasOwnProperty("value") === !0 && (u === !0 ? u = !1 : delete a.value));
+                    e.autogrow === !0 && t.nextTick(y)
                 }), t.watch(() => e.autogrow, b => {
-                    b === !0 ? t.nextTick(w) : h.value !== null && o.rows > 0 && (h.value.style.height = "auto")
+                    b === !0 ? t.nextTick(y) : m.value !== null && o.rows > 0 && (m.value.style.height = "auto")
                 }), t.watch(() => e.dense, () => {
-                    e.autogrow === !0 && t.nextTick(w)
+                    e.autogrow === !0 && t.nextTick(y)
                 });
 
                 function I() {
                     hn(() => {
                         const b = document.activeElement;
-                        h.value !== null && h.value !== b && (b === null || b.id !== M.targetUid.value) && h.value.focus({
+                        m.value !== null && m.value !== b && (b === null || b.id !== M.targetUid.value) && m.value.focus({
                             preventScroll: !0
                         })
                     })
                 }
 
-                function k() {
-                    h.value !== null && h.value.select()
+                function x() {
+                    m.value !== null && m.value.select()
                 }
 
                 function O(b) {
                     if (v.value === !0 && e.reverseFillMask !== !0) {
                         const H = b.target;
-                        x(H, H.selectionStart, H.selectionEnd)
+                        _(H, H.selectionStart, H.selectionEnd)
                     }
                     n("paste", b)
                 }
 
-                function q(b) {
+                function T(b) {
                     if (!b || !b.target) return;
                     if (e.type === "file") {
                         n("update:modelValue", b.target.files);
                         return
                     }
                     const H = b.target.value;
                     if (b.target.qComposing === !0) {
@@ -9246,32 +9250,32 @@
                             selectionStart: te,
                             selectionEnd: U
                         } = b.target;
                         te !== void 0 && U !== void 0 && t.nextTick(() => {
                             b.target === document.activeElement && H.indexOf(b.target.value) === 0 && b.target.setSelectionRange(te, U)
                         })
                     }
-                    e.autogrow === !0 && w()
+                    e.autogrow === !0 && y()
                 }
 
                 function j(b) {
-                    n("animationend", b), w()
+                    n("animationend", b), y()
                 }
 
                 function N(b, H) {
                     s = () => {
                         d = null, e.type !== "number" && a.hasOwnProperty("value") === !0 && delete a.value, e.modelValue !== b && i !== b && (i = b, H === !0 && (c = !0), n("update:modelValue", b), t.nextTick(() => {
                             i === b && (i = NaN)
                         })), s = void 0
                     }, e.type === "number" && (u = !0, a.value = b), e.debounce !== void 0 ? (d !== null && clearTimeout(d), a.value = b, d = setTimeout(s, e.debounce)) : s()
                 }
 
-                function w() {
+                function y() {
                     requestAnimationFrame(() => {
-                        const b = h.value;
+                        const b = m.value;
                         if (b !== null) {
                             const H = b.parentNode.style,
                                 {
                                     scrollTop: te
                                 } = b,
                                 {
                                     overflowY: U,
@@ -9285,90 +9289,91 @@
 
                 function z(b) {
                     A(b), d !== null && (clearTimeout(d), d = null), s !== void 0 && s(), n("change", b.target.value)
                 }
 
                 function G(b) {
                     b !== void 0 && De(b), d !== null && (clearTimeout(d), d = null), s !== void 0 && s(), u = !1, c = !1, delete a.value, e.type !== "file" && setTimeout(() => {
-                        h.value !== null && (h.value.value = m.value !== void 0 ? m.value : "")
+                        m.value !== null && (m.value.value = h.value !== void 0 ? h.value : "")
                     })
                 }
 
                 function J() {
-                    return a.hasOwnProperty("value") === !0 ? a.value : m.value !== void 0 ? m.value : ""
+                    return a.hasOwnProperty("value") === !0 ? a.value : h.value !== void 0 ? h.value : ""
                 }
                 t.onBeforeUnmount(() => {
                     G()
                 }), t.onMounted(() => {
-                    e.autogrow === !0 && w()
+                    e.autogrow === !0 && y()
                 }), Object.assign(M, {
-                    innerValue: m,
+                    innerValue: h,
                     fieldClass: t.computed(() => `q-${V.value===!0?"textarea":"input"}` + (e.autogrow === !0 ? " q-textarea--autogrow" : "")),
                     hasShadow: t.computed(() => e.type !== "file" && typeof e.shadowText == "string" && e.shadowText.length !== 0),
-                    inputRef: h,
+                    inputRef: m,
                     emitValue: N,
-                    hasValue: P,
-                    floatingLabel: t.computed(() => P.value === !0 && (e.type !== "number" || isNaN(m.value) === !1) || Kt(e.displayValue)),
+                    hasValue: C,
+                    floatingLabel: t.computed(() => C.value === !0 && (e.type !== "number" || isNaN(h.value) === !1) || Kt(e.displayValue)),
                     getControl: () => t.h(V.value === !0 ? "textarea" : "input", {
-                        ref: h,
+                        ref: m,
                         class: ["q-field__native q-placeholder", e.inputClass],
                         style: e.inputStyle,
+                        ...P.value,
                         ...B.value,
-                        ...T.value,
                         ...e.type !== "file" ? {
                             value: J()
-                        } : y.value
+                        } : w.value
                     }),
                     getShadowControl: () => t.h("div", {
                         class: "q-field__native q-field__shadow absolute-bottom no-pointer-events" + (V.value === !0 ? "" : " text-no-wrap")
                     }, [t.h("span", {
                         class: "invisible"
                     }, J()), t.h("span", e.shadowText)])
                 });
-                const _ = Xn(M);
+                const S = Xn(M);
                 return Object.assign(l, {
                     focus: I,
-                    select: k,
-                    getNativeElement: () => h.value
-                }), Ze(l, "nativeEl", () => h.value), _
+                    select: x,
+                    getNativeElement: () => m.value
+                }), Ze(l, "nativeEl", () => m.value), S
             }
         }),
         tv = {
             class: "pybi-input"
         },
         nv = t.defineComponent({
             __name: "Input",
             props: {
                 model: {}
             },
             setup(e) {
                 const o = e.model,
                     r = t.inject(kn).getFilterHandler(o);
-                t.inject(pr).onResetFilters(() => {
+                t.inject(xo).onResetFilters(() => {
                     i.value = ""
                 });
                 const i = t.ref("");
                 return t.watch(i, u => {
                     if (u === null || u.length === 0) r.removeFilter();
                     else {
+                        u = u.replaceAll("'", "''");
                         const c = o.whereExpr.replaceAll("${}", u);
                         r.addFilter(c)
                     }
                 }), (u, c) => (t.openBlock(), t.createElementBlock("div", tv, [t.createVNode(ev, t.mergeProps({
                     modelValue: i.value,
                     "onUpdate:modelValue": c[0] || (c[0] = d => i.value = d),
                     clearable: "",
                     dense: "",
                     placeholder: `查询[${t.unref(o).updateInfos[0].field}]`
                 }, t.unref(o).props), null, 16, ["modelValue", "placeholder"])]))
             }
         }),
         zv = "",
         ov = Xe(nv, [
-            ["__scopeId", "data-v-56484143"]
+            ["__scopeId", "data-v-0964b155"]
         ]),
         {
             passive: Va
         } = Se,
         lv = ["both", "horizontal", "vertical"],
         rv = se({
             name: "QScrollObserver",
@@ -9407,44 +9412,44 @@
                     r, a;
                 t.watch(() => e.scrollTarget, () => {
                     c(), u()
                 });
 
                 function i() {
                     l !== null && l();
-                    const h = Math.max(0, io(r)),
+                    const m = Math.max(0, io(r)),
                         f = uo(r),
-                        m = {
-                            top: h - o.position.top,
+                        h = {
+                            top: m - o.position.top,
                             left: f - o.position.left
                         };
-                    if (e.axis === "vertical" && m.top === 0 || e.axis === "horizontal" && m.left === 0) return;
-                    const v = Math.abs(m.top) >= Math.abs(m.left) ? m.top < 0 ? "up" : "down" : m.left < 0 ? "left" : "right";
+                    if (e.axis === "vertical" && h.top === 0 || e.axis === "horizontal" && h.left === 0) return;
+                    const v = Math.abs(h.top) >= Math.abs(h.left) ? h.top < 0 ? "up" : "down" : h.left < 0 ? "left" : "right";
                     o.position = {
-                        top: h,
+                        top: m,
                         left: f
-                    }, o.directionChanged = o.direction !== v, o.delta = m, o.directionChanged === !0 && (o.direction = v, o.inflectionPoint = o.position), n("scroll", {
+                    }, o.directionChanged = o.direction !== v, o.delta = h, o.directionChanged === !0 && (o.direction = v, o.inflectionPoint = o.position), n("scroll", {
                         ...o
                     })
                 }
 
                 function u() {
                     r = ao(a, e.scrollTarget), r.addEventListener("scroll", d, Va), d(!0)
                 }
 
                 function c() {
                     r !== void 0 && (r.removeEventListener("scroll", d, Va), r = void 0)
                 }
 
-                function d(h) {
-                    if (h === !0 || e.debounce === 0 || e.debounce === "0") i();
+                function d(m) {
+                    if (m === !0 || e.debounce === 0 || e.debounce === "0") i();
                     else if (l === null) {
-                        const [f, m] = e.debounce ? [setTimeout(i, e.debounce), clearTimeout] : [requestAnimationFrame(i), cancelAnimationFrame];
+                        const [f, h] = e.debounce ? [setTimeout(i, e.debounce), clearTimeout] : [requestAnimationFrame(i), cancelAnimationFrame];
                         l = () => {
-                            m(f), l = null
+                            h(f), l = null
                         }
                     }
                 }
                 const {
                     proxy: s
                 } = t.getCurrentInstance();
                 return t.watch(() => s.$q.lang.rtl, i), t.onMounted(() => {
@@ -9454,15 +9459,15 @@
                 }), Object.assign(s, {
                     trigger: d,
                     getPosition: () => o
                 }), Ut
             }
         });
 
-    function Ko(e, n, o) {
+    function Qo(e, n, o) {
         const l = dt(e);
         let r, a = l.left - n.event.x,
             i = l.top - n.event.y,
             u = Math.abs(a),
             c = Math.abs(i);
         const d = n.direction;
         d.horizontal === !0 && d.vertical !== !0 ? r = a < 0 ? "left" : "right" : d.horizontal !== !0 && d.vertical === !0 ? r = i < 0 ? "up" : "down" : d.up === !0 && i < 0 ? (r = "up", u > c && (d.left === !0 && a < 0 ? r = "left" : d.right === !0 && a > 0 && (r = "right"))) : d.down === !0 && i > 0 ? (r = "down", u > c && (d.left === !0 && a < 0 ? r = "left" : d.right === !0 && a > 0 && (r = "right"))) : d.left === !0 && a < 0 ? (r = "left", u < c && (d.up === !0 && i < 0 ? r = "up" : d.down === !0 && i > 0 && (r = "down"))) : d.right === !0 && a > 0 && (r = "right", u < c && (d.up === !0 && i < 0 ? r = "up" : d.down === !0 && i > 0 && (r = "down")));
@@ -9512,15 +9517,15 @@
                 const r = {
                     uid: "qvtp_" + av++,
                     handler: n,
                     modifiers: o,
                     direction: $n(o),
                     noop: Ut,
                     mouseStart(a) {
-                        An(a, r) && pl(a) && (Qe(r, "temp", [
+                        An(a, r) && bl(a) && (Qe(r, "temp", [
                             [document, "mousemove", "move", "notPassiveCapture"],
                             [document, "mouseup", "end", "passiveCapture"]
                         ]), r.start(a, !0))
                     },
                     touchStart(a) {
                         if (An(a, r)) {
                             const i = a.target;
@@ -9569,51 +9574,51 @@
                             u = i.left - r.event.x,
                             c = i.top - r.event.y;
                         if (u === 0 && c === 0) return;
                         r.lastEvt = a;
                         const d = r.event.mouse === !0,
                             s = () => {
                                 l(a, d);
-                                let m;
-                                o.preserveCursor !== !0 && o.preservecursor !== !0 && (m = document.documentElement.style.cursor || "", document.documentElement.style.cursor = "grabbing"), d === !0 && document.body.classList.add("no-pointer-events--children"), document.body.classList.add("non-selectable"), no(), r.styleCleanup = v => {
-                                    if (r.styleCleanup = void 0, m !== void 0 && (document.documentElement.style.cursor = m), document.body.classList.remove("non-selectable"), d === !0) {
-                                        const x = () => {
+                                let h;
+                                o.preserveCursor !== !0 && o.preservecursor !== !0 && (h = document.documentElement.style.cursor || "", document.documentElement.style.cursor = "grabbing"), d === !0 && document.body.classList.add("no-pointer-events--children"), document.body.classList.add("non-selectable"), no(), r.styleCleanup = v => {
+                                    if (r.styleCleanup = void 0, h !== void 0 && (document.documentElement.style.cursor = h), document.body.classList.remove("non-selectable"), d === !0) {
+                                        const _ = () => {
                                             document.body.classList.remove("no-pointer-events--children")
                                         };
                                         v !== void 0 ? setTimeout(() => {
-                                            x(), v()
-                                        }, 50) : x()
+                                            _(), v()
+                                        }, 50) : _()
                                     } else v !== void 0 && v()
                                 }
                             };
                         if (r.event.detected === !0) {
                             r.event.isFirst !== !0 && l(a, r.event.mouse);
                             const {
-                                payload: m,
+                                payload: h,
                                 synthetic: v
-                            } = Ko(a, r, !1);
-                            m !== void 0 && (r.handler(m) === !1 ? r.end(a) : (r.styleCleanup === void 0 && r.event.isFirst === !0 && s(), r.event.lastX = m.position.left, r.event.lastY = m.position.top, r.event.lastDir = v === !0 ? void 0 : m.direction, r.event.isFirst = !1));
+                            } = Qo(a, r, !1);
+                            h !== void 0 && (r.handler(h) === !1 ? r.end(a) : (r.styleCleanup === void 0 && r.event.isFirst === !0 && s(), r.event.lastX = h.position.left, r.event.lastY = h.position.top, r.event.lastDir = v === !0 ? void 0 : h.direction, r.event.isFirst = !1));
                             return
                         }
                         if (r.direction.all === !0 || d === !0 && (r.modifiers.mouseAllDir === !0 || r.modifiers.mousealldir === !0)) {
                             s(), r.event.detected = !0, r.move(a);
                             return
                         }
-                        const h = Math.abs(u),
+                        const m = Math.abs(u),
                             f = Math.abs(c);
-                        h !== f && (r.direction.horizontal === !0 && h > f || r.direction.vertical === !0 && h < f || r.direction.up === !0 && h < f && c < 0 || r.direction.down === !0 && h < f && c > 0 || r.direction.left === !0 && h > f && u < 0 || r.direction.right === !0 && h > f && u > 0 ? (r.event.detected = !0, r.move(a)) : r.end(a, !0))
+                        m !== f && (r.direction.horizontal === !0 && m > f || r.direction.vertical === !0 && m < f || r.direction.up === !0 && m < f && c < 0 || r.direction.down === !0 && m < f && c > 0 || r.direction.left === !0 && m > f && u < 0 || r.direction.right === !0 && m > f && u > 0 ? (r.event.detected = !0, r.move(a)) : r.end(a, !0))
                     },
                     end(a, i) {
                         if (r.event !== void 0) {
                             if (it(r, "temp"), he.is.firefox === !0 && qt(e, !1), i === !0) r.styleCleanup !== void 0 && r.styleCleanup(), r.event.detected !== !0 && r.initialEvent !== void 0 && r.initialEvent.target.dispatchEvent(r.initialEvent.event);
                             else if (r.event.detected === !0) {
-                                r.event.isFirst === !0 && r.handler(Ko(a === void 0 ? r.lastEvt : a, r).payload);
+                                r.event.isFirst === !0 && r.handler(Qo(a === void 0 ? r.lastEvt : a, r).payload);
                                 const {
                                     payload: u
-                                } = Ko(a === void 0 ? r.lastEvt : a, r, !0), c = () => {
+                                } = Qo(a === void 0 ? r.lastEvt : a, r, !0), c = () => {
                                     r.handler(u)
                                 };
                                 r.styleCleanup !== void 0 ? r.styleCleanup(c) : c()
                             }
                             r.event = void 0, r.initialEvent = void 0, r.lastEvt = void 0
                         }
                     }
@@ -9635,15 +9640,15 @@
             },
             beforeUnmount(e) {
                 const n = e.__qtouchpan;
                 n !== void 0 && (n.event !== void 0 && n.end(), it(n, "main"), it(n, "temp"), he.is.firefox === !0 && qt(e, !1), n.styleCleanup !== void 0 && n.styleCleanup(), delete e.__qtouchpan)
             }
         }),
         Ia = ["vertical", "horizontal"],
-        Qo = {
+        Go = {
             vertical: {
                 offset: "offsetY",
                 scroll: "scrollTop",
                 dir: "down",
                 dist: "y"
             },
             horizontal: {
@@ -9706,215 +9711,215 @@
                         }
                     },
                     {
                         proxy: c
                     } = t.getCurrentInstance(),
                     d = Fe(e, c.$q);
                 let s = null,
-                    h;
+                    m;
                 const f = t.ref(null),
-                    m = t.computed(() => "q-scrollarea" + (d.value === !0 ? " q-scrollarea--dark" : ""));
+                    h = t.computed(() => "q-scrollarea" + (d.value === !0 ? " q-scrollarea--dark" : ""));
                 u.vertical.percentage = t.computed(() => {
-                    const w = u.vertical.size.value - i.vertical.value;
-                    if (w <= 0) return 0;
-                    const z = st(u.vertical.position.value / w, 0, 1);
+                    const y = u.vertical.size.value - i.vertical.value;
+                    if (y <= 0) return 0;
+                    const z = st(u.vertical.position.value / y, 0, 1);
                     return Math.round(z * 1e4) / 1e4
                 }), u.vertical.thumbHidden = t.computed(() => (e.visible === null ? a.value : e.visible) !== !0 && l.value === !1 && r.value === !1 || u.vertical.size.value <= i.vertical.value + 1), u.vertical.thumbStart = t.computed(() => u.vertical.percentage.value * (i.vertical.value - u.vertical.thumbSize.value)), u.vertical.thumbSize = t.computed(() => Math.round(st(i.vertical.value * i.vertical.value / u.vertical.size.value, La(i.vertical.value), i.vertical.value))), u.vertical.style = t.computed(() => ({
                     ...e.thumbStyle,
                     ...e.verticalThumbStyle,
                     top: `${u.vertical.thumbStart.value}px`,
                     height: `${u.vertical.thumbSize.value}px`
                 })), u.vertical.thumbClass = t.computed(() => "q-scrollarea__thumb q-scrollarea__thumb--v absolute-right" + (u.vertical.thumbHidden.value === !0 ? " q-scrollarea__thumb--invisible" : "")), u.vertical.barClass = t.computed(() => "q-scrollarea__bar q-scrollarea__bar--v absolute-right" + (u.vertical.thumbHidden.value === !0 ? " q-scrollarea__bar--invisible" : "")), u.horizontal.percentage = t.computed(() => {
-                    const w = u.horizontal.size.value - i.horizontal.value;
-                    if (w <= 0) return 0;
-                    const z = st(Math.abs(u.horizontal.position.value) / w, 0, 1);
+                    const y = u.horizontal.size.value - i.horizontal.value;
+                    if (y <= 0) return 0;
+                    const z = st(Math.abs(u.horizontal.position.value) / y, 0, 1);
                     return Math.round(z * 1e4) / 1e4
                 }), u.horizontal.thumbHidden = t.computed(() => (e.visible === null ? a.value : e.visible) !== !0 && l.value === !1 && r.value === !1 || u.horizontal.size.value <= i.horizontal.value + 1), u.horizontal.thumbStart = t.computed(() => u.horizontal.percentage.value * (i.horizontal.value - u.horizontal.thumbSize.value)), u.horizontal.thumbSize = t.computed(() => Math.round(st(i.horizontal.value * i.horizontal.value / u.horizontal.size.value, La(i.horizontal.value), i.horizontal.value))), u.horizontal.style = t.computed(() => ({
                     ...e.thumbStyle,
                     ...e.horizontalThumbStyle,
                     [c.$q.lang.rtl === !0 ? "right" : "left"]: `${u.horizontal.thumbStart.value}px`,
                     width: `${u.horizontal.thumbSize.value}px`
                 })), u.horizontal.thumbClass = t.computed(() => "q-scrollarea__thumb q-scrollarea__thumb--h absolute-bottom" + (u.horizontal.thumbHidden.value === !0 ? " q-scrollarea__thumb--invisible" : "")), u.horizontal.barClass = t.computed(() => "q-scrollarea__bar q-scrollarea__bar--h absolute-bottom" + (u.horizontal.thumbHidden.value === !0 ? " q-scrollarea__bar--invisible" : ""));
                 const v = t.computed(() => u.vertical.thumbHidden.value === !0 && u.horizontal.thumbHidden.value === !0 ? e.contentStyle : e.contentActiveStyle),
-                    x = [
-                        [un, w => {
-                            V(w, "vertical")
+                    _ = [
+                        [un, y => {
+                            V(y, "vertical")
                         }, void 0, {
                             vertical: !0,
                             ...za
                         }]
                     ],
                     p = [
-                        [un, w => {
-                            V(w, "horizontal")
+                        [un, y => {
+                            V(y, "horizontal")
                         }, void 0, {
                             horizontal: !0,
                             ...za
                         }]
                     ];
 
-                function S() {
-                    const w = {};
+                function k() {
+                    const y = {};
                     return Ia.forEach(z => {
                         const G = u[z];
-                        w[z + "Position"] = G.position.value, w[z + "Percentage"] = G.percentage.value, w[z + "Size"] = G.size.value, w[z + "ContainerSize"] = i[z].value
-                    }), w
+                        y[z + "Position"] = G.position.value, y[z + "Percentage"] = G.percentage.value, y[z + "Size"] = G.size.value, y[z + "ContainerSize"] = i[z].value
+                    }), y
                 }
-                const C = Un(() => {
-                    const w = S();
-                    w.ref = c, o("scroll", w)
+                const q = Un(() => {
+                    const y = k();
+                    y.ref = c, o("scroll", y)
                 }, 0);
 
-                function y(w, z, G) {
-                    if (Ia.includes(w) === !1) {
+                function w(y, z, G) {
+                    if (Ia.includes(y) === !1) {
                         console.error("[QScrollArea]: wrong first param of setScrollPosition (vertical/horizontal)");
                         return
-                    }(w === "vertical" ? zl : fo)(f.value, z, G)
+                    }(y === "vertical" ? Ll : fo)(f.value, z, G)
                 }
 
-                function P({
-                    height: w,
+                function C({
+                    height: y,
                     width: z
                 }) {
                     let G = !1;
-                    i.vertical.value !== w && (i.vertical.value = w, G = !0), i.horizontal.value !== z && (i.horizontal.value = z, G = !0), G === !0 && I()
+                    i.vertical.value !== y && (i.vertical.value = y, G = !0), i.horizontal.value !== z && (i.horizontal.value = z, G = !0), G === !0 && I()
                 }
 
                 function A({
-                    position: w
+                    position: y
                 }) {
                     let z = !1;
-                    u.vertical.position.value !== w.top && (u.vertical.position.value = w.top, z = !0), u.horizontal.position.value !== w.left && (u.horizontal.position.value = w.left, z = !0), z === !0 && I()
+                    u.vertical.position.value !== y.top && (u.vertical.position.value = y.top, z = !0), u.horizontal.position.value !== y.left && (u.horizontal.position.value = y.left, z = !0), z === !0 && I()
                 }
 
                 function M({
-                    height: w,
+                    height: y,
                     width: z
                 }) {
-                    u.horizontal.size.value !== z && (u.horizontal.size.value = z, I()), u.vertical.size.value !== w && (u.vertical.size.value = w, I())
+                    u.horizontal.size.value !== z && (u.horizontal.size.value = z, I()), u.vertical.size.value !== y && (u.vertical.size.value = y, I())
                 }
 
-                function V(w, z) {
+                function V(y, z) {
                     const G = u[z];
-                    if (w.isFirst === !0) {
+                    if (y.isFirst === !0) {
                         if (G.thumbHidden.value === !0) return;
-                        h = G.position.value, r.value = !0
+                        m = G.position.value, r.value = !0
                     } else if (r.value !== !0) return;
-                    w.isFinal === !0 && (r.value = !1);
-                    const J = Qo[z],
-                        _ = i[z].value,
-                        b = (G.size.value - _) / (_ - G.thumbSize.value),
-                        H = w.distance[J.dist],
-                        te = h + (w.direction === J.dir ? 1 : -1) * H * b;
-                    k(te, z)
+                    y.isFinal === !0 && (r.value = !1);
+                    const J = Go[z],
+                        S = i[z].value,
+                        b = (G.size.value - S) / (S - G.thumbSize.value),
+                        H = y.distance[J.dist],
+                        te = m + (y.direction === J.dir ? 1 : -1) * H * b;
+                    x(te, z)
                 }
 
-                function R(w, z) {
+                function R(y, z) {
                     const G = u[z];
                     if (G.thumbHidden.value !== !0) {
-                        const J = w[Qo[z].offset];
+                        const J = y[Go[z].offset];
                         if (J < G.thumbStart.value || J > G.thumbStart.value + G.thumbSize.value) {
-                            const _ = J - G.thumbSize.value / 2;
-                            k(_ / i[z].value * G.size.value, z)
+                            const S = J - G.thumbSize.value / 2;
+                            x(S / i[z].value * G.size.value, z)
                         }
-                        G.ref.value !== null && G.ref.value.dispatchEvent(new MouseEvent(w.type, w))
+                        G.ref.value !== null && G.ref.value.dispatchEvent(new MouseEvent(y.type, y))
                     }
                 }
 
-                function T(w) {
-                    R(w, "vertical")
+                function B(y) {
+                    R(y, "vertical")
                 }
 
-                function B(w) {
-                    R(w, "horizontal")
+                function P(y) {
+                    R(y, "horizontal")
                 }
 
                 function I() {
                     l.value = !0, s !== null && clearTimeout(s), s = setTimeout(() => {
                         s = null, l.value = !1
-                    }, e.delay), e.onScroll !== void 0 && C()
+                    }, e.delay), e.onScroll !== void 0 && q()
                 }
 
-                function k(w, z) {
-                    f.value[Qo[z].scroll] = w
+                function x(y, z) {
+                    f.value[Go[z].scroll] = y
                 }
                 let O = null;
 
-                function q() {
+                function T() {
                     O !== null && clearTimeout(O), O = setTimeout(() => {
                         O = null, a.value = !0
                     }, c.$q.platform.is.ios ? 50 : 0)
                 }
 
                 function j() {
                     O !== null && (clearTimeout(O), O = null), a.value = !1
                 }
                 let N = null;
-                return t.watch(() => c.$q.lang.rtl, w => {
-                    f.value !== null && fo(f.value, Math.abs(u.horizontal.position.value) * (w === !0 ? -1 : 1))
+                return t.watch(() => c.$q.lang.rtl, y => {
+                    f.value !== null && fo(f.value, Math.abs(u.horizontal.position.value) * (y === !0 ? -1 : 1))
                 }), t.onDeactivated(() => {
                     N = {
                         top: u.vertical.position.value,
                         left: u.horizontal.position.value
                     }
                 }), t.onActivated(() => {
                     if (N === null) return;
-                    const w = f.value;
-                    w !== null && (fo(w, N.left), zl(w, N.top))
-                }), t.onBeforeUnmount(C.cancel), Object.assign(c, {
+                    const y = f.value;
+                    y !== null && (fo(y, N.left), Ll(y, N.top))
+                }), t.onBeforeUnmount(q.cancel), Object.assign(c, {
                     getScrollTarget: () => f.value,
-                    getScroll: S,
+                    getScroll: k,
                     getScrollPosition: () => ({
                         top: u.vertical.position.value,
                         left: u.horizontal.position.value
                     }),
                     getScrollPercentage: () => ({
                         top: u.vertical.percentage.value,
                         left: u.horizontal.percentage.value
                     }),
-                    setScrollPosition: y,
-                    setScrollPercentage(w, z, G) {
-                        y(w, z * (u[w].size.value - i[w].value) * (w === "horizontal" && c.$q.lang.rtl === !0 ? -1 : 1), G)
+                    setScrollPosition: w,
+                    setScrollPercentage(y, z, G) {
+                        w(y, z * (u[y].size.value - i[y].value) * (y === "horizontal" && c.$q.lang.rtl === !0 ? -1 : 1), G)
                     }
                 }), () => t.h("div", {
-                    class: m.value,
-                    onMouseenter: q,
+                    class: h.value,
+                    onMouseenter: T,
                     onMouseleave: j
                 }, [t.h("div", {
                     ref: f,
                     class: "q-scrollarea__container scroll relative-position fit hide-scrollbar",
                     tabindex: e.tabindex !== void 0 ? e.tabindex : void 0
                 }, [t.h("div", {
                     class: "q-scrollarea__content absolute",
                     style: v.value
-                }, Ke(n.default, [t.h(Uo, {
+                }, Ke(n.default, [t.h(Wo, {
                     debounce: 0,
                     onResize: M
                 })])), t.h(rv, {
                     axis: "both",
                     onScroll: A
-                })]), t.h(Uo, {
+                })]), t.h(Wo, {
                     debounce: 0,
-                    onResize: P
+                    onResize: C
                 }), t.h("div", {
                     class: u.vertical.barClass.value,
                     style: [e.barStyle, e.verticalBarStyle],
                     "aria-hidden": "true",
-                    onMousedown: T
+                    onMousedown: B
                 }), t.h("div", {
                     class: u.horizontal.barClass.value,
                     style: [e.barStyle, e.horizontalBarStyle],
                     "aria-hidden": "true",
-                    onMousedown: B
+                    onMousedown: P
                 }), t.withDirectives(t.h("div", {
                     ref: u.vertical.ref,
                     class: u.vertical.thumbClass.value,
                     style: u.vertical.style.value,
                     "aria-hidden": "true"
-                }), x), t.withDirectives(t.h("div", {
+                }), _), t.withDirectives(t.h("div", {
                     ref: u.horizontal.ref,
                     class: u.horizontal.thumbClass.value,
                     style: u.horizontal.style.value,
                     "aria-hidden": "true"
                 }), p)])
             }
         }),
@@ -9933,46 +9938,46 @@
 
     function sv() {
         const {
             props: e,
             proxy: {
                 $q: n
             }
-        } = t.getCurrentInstance(), o = t.inject(sl, et);
+        } = t.getCurrentInstance(), o = t.inject(cl, et);
         if (o === et) return console.error("QPageSticky needs to be child of QLayout"), et;
         const l = t.computed(() => {
-                const h = e.position;
+                const m = e.position;
                 return {
-                    top: h.indexOf("top") > -1,
-                    right: h.indexOf("right") > -1,
-                    bottom: h.indexOf("bottom") > -1,
-                    left: h.indexOf("left") > -1,
-                    vertical: h === "top" || h === "bottom",
-                    horizontal: h === "left" || h === "right"
+                    top: m.indexOf("top") > -1,
+                    right: m.indexOf("right") > -1,
+                    bottom: m.indexOf("bottom") > -1,
+                    left: m.indexOf("left") > -1,
+                    vertical: m === "top" || m === "bottom",
+                    horizontal: m === "left" || m === "right"
                 }
             }),
             r = t.computed(() => o.header.offset),
             a = t.computed(() => o.right.offset),
             i = t.computed(() => o.footer.offset),
             u = t.computed(() => o.left.offset),
             c = t.computed(() => {
-                let h = 0,
+                let m = 0,
                     f = 0;
-                const m = l.value,
+                const h = l.value,
                     v = n.lang.rtl === !0 ? -1 : 1;
-                m.top === !0 && r.value !== 0 ? f = `${r.value}px` : m.bottom === !0 && i.value !== 0 && (f = `${-i.value}px`), m.left === !0 && u.value !== 0 ? h = `${v*u.value}px` : m.right === !0 && a.value !== 0 && (h = `${-v*a.value}px`);
-                const x = {
-                    transform: `translate(${h}, ${f})`
+                h.top === !0 && r.value !== 0 ? f = `${r.value}px` : h.bottom === !0 && i.value !== 0 && (f = `${-i.value}px`), h.left === !0 && u.value !== 0 ? m = `${v*u.value}px` : h.right === !0 && a.value !== 0 && (m = `${-v*a.value}px`);
+                const _ = {
+                    transform: `translate(${m}, ${f})`
                 };
-                return e.offset && (x.margin = `${e.offset[1]}px ${e.offset[0]}px`), m.vertical === !0 ? (u.value !== 0 && (x[n.lang.rtl === !0 ? "right" : "left"] = `${u.value}px`), a.value !== 0 && (x[n.lang.rtl === !0 ? "left" : "right"] = `${a.value}px`)) : m.horizontal === !0 && (r.value !== 0 && (x.top = `${r.value}px`), i.value !== 0 && (x.bottom = `${i.value}px`)), x
+                return e.offset && (_.margin = `${e.offset[1]}px ${e.offset[0]}px`), h.vertical === !0 ? (u.value !== 0 && (_[n.lang.rtl === !0 ? "right" : "left"] = `${u.value}px`), a.value !== 0 && (_[n.lang.rtl === !0 ? "left" : "right"] = `${a.value}px`)) : h.horizontal === !0 && (r.value !== 0 && (_.top = `${r.value}px`), i.value !== 0 && (_.bottom = `${i.value}px`)), _
             }),
             d = t.computed(() => `q-page-sticky row flex-center fixed-${e.position} q-page-sticky--${e.expand===!0?"expand":"shrink"}`);
 
-        function s(h) {
-            const f = we(h.default);
+        function s(m) {
+            const f = we(m.default);
             return t.h("div", {
                 class: d.value,
                 style: c.value
             }, e.expand === !0 ? f : [t.h("div", f)])
         }
         return {
             $layout: o,
@@ -10043,70 +10048,70 @@
                         proxy: {
                             $q: a
                         }
                     } = r,
                     i = Fe(e, a),
                     {
                         preventBodyScroll: u
-                    } = nr(),
+                    } = or(),
                     {
                         registerTimeout: c,
                         removeTimeout: d
                     } = Xt(),
-                    s = t.inject(sl, et);
+                    s = t.inject(cl, et);
                 if (s === et) return console.error("QDrawer needs to be child of QLayout"), et;
-                let h, f = null,
-                    m;
+                let m, f = null,
+                    h;
                 const v = t.ref(e.behavior === "mobile" || e.behavior !== "desktop" && s.totalWidth.value <= e.breakpoint),
-                    x = t.computed(() => e.mini === !0 && v.value !== !0),
-                    p = t.computed(() => x.value === !0 ? e.miniWidth : e.width),
-                    S = t.ref(e.showIfAbove === !0 && v.value === !1 ? !0 : e.modelValue === !0),
-                    C = t.computed(() => e.persistent !== !0 && (v.value === !0 || J.value === !0));
+                    _ = t.computed(() => e.mini === !0 && v.value !== !0),
+                    p = t.computed(() => _.value === !0 ? e.miniWidth : e.width),
+                    k = t.ref(e.showIfAbove === !0 && v.value === !1 ? !0 : e.modelValue === !0),
+                    q = t.computed(() => e.persistent !== !0 && (v.value === !0 || J.value === !0));
 
-                function y(E, Y) {
+                function w(E, Y) {
                     if (V(), E !== !1 && s.animate(), ce(0), v.value === !0) {
                         const re = s.instances[N.value];
                         re !== void 0 && re.belowBreakpoint === !0 && re.hide(!1), ye(1), s.isContainer.value !== !0 && u(!0)
                     } else ye(0), E !== !1 && Te(!1);
                     c(() => {
                         E !== !1 && Te(!0), Y !== !0 && o("show", E)
                     }, Da)
                 }
 
-                function P(E, Y) {
+                function C(E, Y) {
                     R(), E !== !1 && s.animate(), ye(0), ce(I.value * p.value), We(), Y !== !0 ? c(() => {
                         o("hide", E)
                     }, Da) : d()
                 }
                 const {
                     show: A,
                     hide: M
                 } = ro({
-                    showing: S,
-                    hideOnRouteChange: C,
-                    handleShow: y,
-                    handleHide: P
+                    showing: k,
+                    hideOnRouteChange: q,
+                    handleShow: w,
+                    handleHide: C
                 }), {
                     addToHistory: V,
                     removeFromHistory: R
-                } = Xl(S), T = {
+                } = Yl(k), B = {
                     belowBreakpoint: v,
                     hide: M
-                }, B = t.computed(() => e.side === "right"), I = t.computed(() => (a.lang.rtl === !0 ? -1 : 1) * (B.value === !0 ? 1 : -1)), k = t.ref(0), O = t.ref(!1), q = t.ref(!1), j = t.ref(p.value * I.value), N = t.computed(() => B.value === !0 ? "left" : "right"), w = t.computed(() => S.value === !0 && v.value === !1 && e.overlay === !1 ? e.miniToOverlay === !0 ? e.miniWidth : p.value : 0), z = t.computed(() => e.overlay === !0 || e.miniToOverlay === !0 || s.view.value.indexOf(B.value ? "R" : "L") > -1 || a.platform.is.ios === !0 && s.isContainer.value === !0), G = t.computed(() => e.overlay === !1 && S.value === !0 && v.value === !1), J = t.computed(() => e.overlay === !0 && S.value === !0 && v.value === !1), _ = t.computed(() => "fullscreen q-drawer__backdrop" + (S.value === !1 && O.value === !1 ? " hidden" : "")), b = t.computed(() => ({
-                    backgroundColor: `rgba(0,0,0,${k.value*.4})`
-                })), H = t.computed(() => B.value === !0 ? s.rows.value.top[2] === "r" : s.rows.value.top[0] === "l"), te = t.computed(() => B.value === !0 ? s.rows.value.bottom[2] === "r" : s.rows.value.bottom[0] === "l"), U = t.computed(() => {
+                }, P = t.computed(() => e.side === "right"), I = t.computed(() => (a.lang.rtl === !0 ? -1 : 1) * (P.value === !0 ? 1 : -1)), x = t.ref(0), O = t.ref(!1), T = t.ref(!1), j = t.ref(p.value * I.value), N = t.computed(() => P.value === !0 ? "left" : "right"), y = t.computed(() => k.value === !0 && v.value === !1 && e.overlay === !1 ? e.miniToOverlay === !0 ? e.miniWidth : p.value : 0), z = t.computed(() => e.overlay === !0 || e.miniToOverlay === !0 || s.view.value.indexOf(P.value ? "R" : "L") > -1 || a.platform.is.ios === !0 && s.isContainer.value === !0), G = t.computed(() => e.overlay === !1 && k.value === !0 && v.value === !1), J = t.computed(() => e.overlay === !0 && k.value === !0 && v.value === !1), S = t.computed(() => "fullscreen q-drawer__backdrop" + (k.value === !1 && O.value === !1 ? " hidden" : "")), b = t.computed(() => ({
+                    backgroundColor: `rgba(0,0,0,${x.value*.4})`
+                })), H = t.computed(() => P.value === !0 ? s.rows.value.top[2] === "r" : s.rows.value.top[0] === "l"), te = t.computed(() => P.value === !0 ? s.rows.value.bottom[2] === "r" : s.rows.value.bottom[0] === "l"), U = t.computed(() => {
                     const E = {};
                     return s.header.space === !0 && H.value === !1 && (z.value === !0 ? E.top = `${s.header.offset}px` : s.header.space === !0 && (E.top = `${s.header.size}px`)), s.footer.space === !0 && te.value === !1 && (z.value === !0 ? E.bottom = `${s.footer.offset}px` : s.footer.space === !0 && (E.bottom = `${s.footer.size}px`)), E
                 }), F = t.computed(() => {
                     const E = {
                         width: `${p.value}px`,
                         transform: `translateX(${j.value}px)`
                     };
                     return v.value === !0 ? E : Object.assign(E, U.value)
-                }), Z = t.computed(() => "q-drawer__content fit " + (s.isContainer.value !== !0 ? "scroll" : "overflow-auto")), ue = t.computed(() => `q-drawer q-drawer--${e.side}` + (q.value === !0 ? " q-drawer--mini-animate" : "") + (e.bordered === !0 ? " q-drawer--bordered" : "") + (i.value === !0 ? " q-drawer--dark q-dark" : "") + (O.value === !0 ? " no-transition" : S.value === !0 ? "" : " q-layout--prevent-focus") + (v.value === !0 ? " fixed q-drawer--on-top q-drawer--mobile q-drawer--top-padding" : ` q-drawer--${x.value===!0?"mini":"standard"}` + (z.value === !0 || G.value !== !0 ? " fixed" : "") + (e.overlay === !0 || e.miniToOverlay === !0 ? " q-drawer--on-top" : "") + (H.value === !0 ? " q-drawer--top-padding" : ""))), D = t.computed(() => {
+                }), Z = t.computed(() => "q-drawer__content fit " + (s.isContainer.value !== !0 ? "scroll" : "overflow-auto")), ue = t.computed(() => `q-drawer q-drawer--${e.side}` + (T.value === !0 ? " q-drawer--mini-animate" : "") + (e.bordered === !0 ? " q-drawer--bordered" : "") + (i.value === !0 ? " q-drawer--dark q-dark" : "") + (O.value === !0 ? " no-transition" : k.value === !0 ? "" : " q-layout--prevent-focus") + (v.value === !0 ? " fixed q-drawer--on-top q-drawer--mobile q-drawer--top-padding" : ` q-drawer--${_.value===!0?"mini":"standard"}` + (z.value === !0 || G.value !== !0 ? " fixed" : "") + (e.overlay === !0 || e.miniToOverlay === !0 ? " q-drawer--on-top" : "") + (H.value === !0 ? " q-drawer--top-padding" : ""))), D = t.computed(() => {
                     const E = a.lang.rtl === !0 ? e.side : N.value;
                     return [
                         [un, Ue, void 0, {
                             [E]: !0,
                             mouse: !0
                         }]
                     ]
@@ -10129,75 +10134,75 @@
                     ]
                 });
 
                 function Ie() {
                     L(v, e.behavior === "mobile" || e.behavior !== "desktop" && s.totalWidth.value <= e.breakpoint)
                 }
                 t.watch(v, E => {
-                    E === !0 ? (h = S.value, S.value === !0 && M(!1)) : e.overlay === !1 && e.behavior !== "mobile" && h !== !1 && (S.value === !0 ? (ce(0), ye(0), We()) : A(!1))
+                    E === !0 ? (m = k.value, k.value === !0 && M(!1)) : e.overlay === !1 && e.behavior !== "mobile" && m !== !1 && (k.value === !0 ? (ce(0), ye(0), We()) : A(!1))
                 }), t.watch(() => e.side, (E, Y) => {
-                    s.instances[Y] === T && (s.instances[Y] = void 0, s[Y].space = !1, s[Y].offset = 0), s.instances[E] = T, s[E].size = p.value, s[E].space = G.value, s[E].offset = w.value
+                    s.instances[Y] === B && (s.instances[Y] = void 0, s[Y].space = !1, s[Y].offset = 0), s.instances[E] = B, s[E].size = p.value, s[E].space = G.value, s[E].offset = y.value
                 }), t.watch(s.totalWidth, () => {
                     (s.isContainer.value === !0 || document.qScrollPrevented !== !0) && Ie()
                 }), t.watch(() => e.behavior + e.breakpoint, Ie), t.watch(s.isContainer, E => {
-                    S.value === !0 && u(E !== !0), E === !0 && Ie()
+                    k.value === !0 && u(E !== !0), E === !0 && Ie()
                 }), t.watch(s.scrollbarWidth, () => {
-                    ce(S.value === !0 ? 0 : void 0)
-                }), t.watch(w, E => {
+                    ce(k.value === !0 ? 0 : void 0)
+                }), t.watch(y, E => {
                     Ce("offset", E)
                 }), t.watch(G, E => {
                     o("onLayout", E), Ce("space", E)
-                }), t.watch(B, () => {
+                }), t.watch(P, () => {
                     ce()
                 }), t.watch(p, E => {
                     ce(), W(e.miniToOverlay, E)
                 }), t.watch(() => e.miniToOverlay, E => {
                     W(E, p.value)
                 }), t.watch(() => a.lang.rtl, () => {
                     ce()
                 }), t.watch(() => e.mini, () => {
                     e.noMiniAnimation || e.modelValue === !0 && (Ae(), s.animate())
-                }), t.watch(x, E => {
+                }), t.watch(_, E => {
                     o("miniState", E)
                 });
 
                 function ce(E) {
                     E === void 0 ? t.nextTick(() => {
-                        E = S.value === !0 ? 0 : p.value, ce(I.value * E)
-                    }) : (s.isContainer.value === !0 && B.value === !0 && (v.value === !0 || Math.abs(E) === p.value) && (E += I.value * s.scrollbarWidth.value), j.value = E)
+                        E = k.value === !0 ? 0 : p.value, ce(I.value * E)
+                    }) : (s.isContainer.value === !0 && P.value === !0 && (v.value === !0 || Math.abs(E) === p.value) && (E += I.value * s.scrollbarWidth.value), j.value = E)
                 }
 
                 function ye(E) {
-                    k.value = E
+                    x.value = E
                 }
 
                 function Te(E) {
                     const Y = E === !0 ? "remove" : s.isContainer.value !== !0 ? "add" : "";
                     Y !== "" && document.body.classList[Y]("q-body--drawer-toggle")
                 }
 
                 function Ae() {
-                    f !== null && clearTimeout(f), r.proxy && r.proxy.$el && r.proxy.$el.classList.add("q-drawer--mini-animate"), q.value = !0, f = setTimeout(() => {
-                        f = null, q.value = !1, r && r.proxy && r.proxy.$el && r.proxy.$el.classList.remove("q-drawer--mini-animate")
+                    f !== null && clearTimeout(f), r.proxy && r.proxy.$el && r.proxy.$el.classList.add("q-drawer--mini-animate"), T.value = !0, f = setTimeout(() => {
+                        f = null, T.value = !1, r && r.proxy && r.proxy.$el && r.proxy.$el.classList.remove("q-drawer--mini-animate")
                     }, 150)
                 }
 
                 function Ue(E) {
-                    if (S.value !== !1) return;
+                    if (k.value !== !1) return;
                     const Y = p.value,
                         re = st(E.distance.x, 0, Y);
                     if (E.isFinal === !0) {
                         re >= Math.min(75, Y) === !0 ? A() : (s.animate(), ye(0), ce(I.value * Y)), O.value = !1;
                         return
                     }
-                    ce((a.lang.rtl === !0 ? B.value !== !0 : B.value) ? Math.max(Y - re, 0) : Math.min(0, re - Y)), ye(st(re / Y, 0, 1)), E.isFirst === !0 && (O.value = !0)
+                    ce((a.lang.rtl === !0 ? P.value !== !0 : P.value) ? Math.max(Y - re, 0) : Math.min(0, re - Y)), ye(st(re / Y, 0, 1)), E.isFirst === !0 && (O.value = !0)
                 }
 
                 function je(E) {
-                    if (S.value !== !0) return;
+                    if (k.value !== !0) return;
                     const Y = p.value,
                         re = E.direction === e.side,
                         ie = (a.lang.rtl === !0 ? re !== !0 : re) ? st(E.distance.x, 0, Y) : 0;
                     if (E.isFinal === !0) {
                         Math.abs(ie) < Math.min(75, Y) === !0 ? (s.animate(), ye(1), ce(0)) : M(), O.value = !1;
                         return
                     }
@@ -10215,48 +10220,48 @@
                 function L(E, Y) {
                     E.value !== Y && (E.value = Y)
                 }
 
                 function W(E, Y) {
                     Ce("size", E === !0 ? e.miniWidth : Y)
                 }
-                return s.instances[e.side] = T, W(e.miniToOverlay, p.value), Ce("space", G.value), Ce("offset", w.value), e.showIfAbove === !0 && e.modelValue !== !0 && S.value === !0 && e["onUpdate:modelValue"] !== void 0 && o("update:modelValue", !0), t.onMounted(() => {
-                    o("onLayout", G.value), o("miniState", x.value), h = e.showIfAbove === !0;
+                return s.instances[e.side] = B, W(e.miniToOverlay, p.value), Ce("space", G.value), Ce("offset", y.value), e.showIfAbove === !0 && e.modelValue !== !0 && k.value === !0 && e["onUpdate:modelValue"] !== void 0 && o("update:modelValue", !0), t.onMounted(() => {
+                    o("onLayout", G.value), o("miniState", _.value), m = e.showIfAbove === !0;
                     const E = () => {
-                        (S.value === !0 ? y : P)(!1, !0)
+                        (k.value === !0 ? w : C)(!1, !0)
                     };
                     if (s.totalWidth.value !== 0) {
                         t.nextTick(E);
                         return
                     }
-                    m = t.watch(s.totalWidth, () => {
-                        m(), m = void 0, S.value === !1 && e.showIfAbove === !0 && v.value === !1 ? A(!1) : E()
+                    h = t.watch(s.totalWidth, () => {
+                        h(), h = void 0, k.value === !1 && e.showIfAbove === !0 && v.value === !1 ? A(!1) : E()
                     })
                 }), t.onBeforeUnmount(() => {
-                    m !== void 0 && m(), f !== null && (clearTimeout(f), f = null), S.value === !0 && We(), s.instances[e.side] === T && (s.instances[e.side] = void 0, Ce("size", 0), Ce("offset", 0), Ce("space", !1))
+                    h !== void 0 && h(), f !== null && (clearTimeout(f), f = null), k.value === !0 && We(), s.instances[e.side] === B && (s.instances[e.side] = void 0, Ce("size", 0), Ce("offset", 0), Ce("space", !1))
                 }), () => {
                     const E = [];
                     v.value === !0 && (e.noSwipeOpen === !1 && E.push(t.withDirectives(t.h("div", {
                         key: "open",
                         class: `q-drawer__opener fixed-${e.side}`,
                         "aria-hidden": "true"
                     }), D.value)), E.push(cn("div", {
                         ref: "backdrop",
-                        class: _.value,
+                        class: S.value,
                         style: b.value,
                         "aria-hidden": "true",
                         onClick: M
-                    }, void 0, "backdrop", e.noSwipeBackdrop !== !0 && S.value === !0, () => ke.value)));
-                    const Y = x.value === !0 && n.mini !== void 0,
+                    }, void 0, "backdrop", e.noSwipeBackdrop !== !0 && k.value === !0, () => ke.value)));
+                    const Y = _.value === !0 && n.mini !== void 0,
                         re = [t.h("div", {
                             ...l,
                             key: "" + Y,
                             class: [Z.value, l.class]
                         }, Y === !0 ? n.mini() : we(n.default))];
-                    return e.elevated === !0 && S.value === !0 && re.push(t.h("div", {
+                    return e.elevated === !0 && k.value === !0 && re.push(t.h("div", {
                         class: "q-layout__shadow absolute-full overflow-hidden no-pointer-events"
                     })), E.push(cn("aside", {
                         ref: "content",
                         class: ue.value,
                         style: F.value
                     }, re, "contentclose", e.noSwipeClose !== !0 && v.value === !0, () => fe.value)), t.h("div", {
                         class: "q-drawer-container"
@@ -10333,15 +10338,15 @@
         mv = t.defineComponent({
             __name: "Button",
             props: {
                 model: {}
             },
             setup(e) {
                 const o = e.model,
-                    l = t.inject(gr);
+                    l = t.inject(pr);
 
                 function r() {
                     o.action && l.run(o.action.id, o.action.name)
                 }
                 return (a, i) => (t.openBlock(), t.createBlock(pt, t.mergeProps({
                     dense: "",
                     color: "primary"
@@ -10398,28 +10403,28 @@
                     outlined: "",
                     multiple: "",
                     "options-cover": ""
                 }, t.unref(o).props), {
                     option: t.withCtx(({
                         itemProps: d,
                         opt: s,
-                        selected: h,
+                        selected: m,
                         toggleOption: f
-                    }) => [t.createVNode(El, t.normalizeProps(t.guardReactiveProps(d)), {
+                    }) => [t.createVNode($l, t.normalizeProps(t.guardReactiveProps(d)), {
                         default: t.withCtx(() => [t.createVNode(to, null, {
-                            default: t.withCtx(() => [t.createVNode($l, {
+                            default: t.withCtx(() => [t.createVNode(Al, {
                                 innerHTML: s
                             }, null, 8, ["innerHTML"])]),
                             _: 2
                         }, 1024), t.createVNode(to, {
                             side: ""
                         }, {
                             default: t.withCtx(() => [t.createVNode(hv, {
-                                "model-value": h,
-                                "onUpdate:modelValue": m => f(s)
+                                "model-value": m,
+                                "onUpdate:modelValue": h => f(s)
                             }, null, 8, ["model-value", "onUpdate:modelValue"])]),
                             _: 2
                         }, 1024)]),
                         _: 2
                     }, 1040)]),
                     _: 1
                 }, 16, ["modelValue", "options"]))
@@ -10490,114 +10495,114 @@
                     r = pv(e, l);
                 let a = null,
                     i = !1;
                 const u = [t.ref(null), t.ref(p())],
                     c = t.ref(0),
                     d = t.ref(!1),
                     s = t.ref(!1),
-                    h = t.computed(() => `q-img q-img--${e.noNativeMenu===!0?"no-":""}menu`),
+                    m = t.computed(() => `q-img q-img--${e.noNativeMenu===!0?"no-":""}menu`),
                     f = t.computed(() => ({
                         width: e.width,
                         height: e.height
                     })),
-                    m = t.computed(() => `q-img__image ${e.imgClass!==void 0?e.imgClass+" ":""}q-img__image--with${e.noTransition===!0?"out":""}-transition`),
+                    h = t.computed(() => `q-img__image ${e.imgClass!==void 0?e.imgClass+" ":""}q-img__image--with${e.noTransition===!0?"out":""}-transition`),
                     v = t.computed(() => ({
                         ...e.imgStyle,
                         objectFit: e.fit,
                         objectPosition: e.position
                     }));
-                t.watch(() => x(), S);
+                t.watch(() => _(), k);
 
-                function x() {
+                function _() {
                     return e.src || e.srcset || e.sizes ? {
                         src: e.src,
                         srcset: e.srcset,
                         sizes: e.sizes
                     } : null
                 }
 
                 function p() {
                     return e.placeholderSrc !== void 0 ? {
                         src: e.placeholderSrc
                     } : null
                 }
 
-                function S(R) {
+                function k(R) {
                     a !== null && (clearTimeout(a), a = null), s.value = !1, R === null ? (d.value = !1, u[c.value ^ 1].value = p()) : d.value = !0, u[c.value].value = R
                 }
 
-                function C({
+                function q({
                     target: R
                 }) {
-                    i !== !0 && (a !== null && (clearTimeout(a), a = null), l.value = R.naturalHeight === 0 ? .5 : R.naturalWidth / R.naturalHeight, y(R, 1))
+                    i !== !0 && (a !== null && (clearTimeout(a), a = null), l.value = R.naturalHeight === 0 ? .5 : R.naturalWidth / R.naturalHeight, w(R, 1))
                 }
 
-                function y(R, T) {
-                    i === !0 || T === 1e3 || (R.complete === !0 ? P(R) : a = setTimeout(() => {
-                        a = null, y(R, T + 1)
+                function w(R, B) {
+                    i === !0 || B === 1e3 || (R.complete === !0 ? C(R) : a = setTimeout(() => {
+                        a = null, w(R, B + 1)
                     }, 50))
                 }
 
-                function P(R) {
+                function C(R) {
                     i !== !0 && (c.value = c.value ^ 1, u[c.value].value = null, d.value = !1, s.value = !1, o("load", R.currentSrc || R.src))
                 }
 
                 function A(R) {
                     a !== null && (clearTimeout(a), a = null), d.value = !1, s.value = !0, u[c.value].value = null, u[c.value ^ 1].value = p(), o("error", R)
                 }
 
                 function M(R) {
-                    const T = u[R].value,
-                        B = {
+                    const B = u[R].value,
+                        P = {
                             key: "img_" + R,
-                            class: m.value,
+                            class: h.value,
                             style: v.value,
                             crossorigin: e.crossorigin,
                             decoding: e.decoding,
                             referrerpolicy: e.referrerpolicy,
                             height: e.height,
                             width: e.width,
                             loading: e.loading,
                             fetchpriority: e.fetchpriority,
                             "aria-hidden": "true",
                             draggable: e.draggable,
-                            ...T
+                            ...B
                         };
-                    return c.value === R ? (B.class += " q-img__image--waiting", Object.assign(B, {
-                        onLoad: C,
+                    return c.value === R ? (P.class += " q-img__image--waiting", Object.assign(P, {
+                        onLoad: q,
                         onError: A
-                    })) : B.class += " q-img__image--loaded", t.h("div", {
+                    })) : P.class += " q-img__image--loaded", t.h("div", {
                         class: "q-img__container absolute-full",
                         key: "img" + R
-                    }, t.h("img", B))
+                    }, t.h("img", P))
                 }
 
                 function V() {
                     return d.value !== !0 ? t.h("div", {
                         key: "content",
                         class: "q-img__content absolute-full q-anchor--skip"
                     }, we(n[s.value === !0 ? "error" : "default"])) : t.h("div", {
                         key: "loading",
                         class: "q-img__loading absolute-full flex flex-center"
                     }, n.loading !== void 0 ? n.loading() : e.noSpinner === !0 ? void 0 : [t.h(Nn, {
                         color: e.spinnerColor,
                         size: e.spinnerSize
                     })])
                 }
-                return S(x()), t.onBeforeUnmount(() => {
+                return k(_()), t.onBeforeUnmount(() => {
                     i = !0, a !== null && (clearTimeout(a), a = null)
                 }), () => {
                     const R = [];
                     return r.value !== null && R.push(t.h("div", {
                         key: "filler",
                         style: r.value
                     })), s.value !== !0 && (u[0].value !== null && R.push(M(0)), u[1].value !== null && R.push(M(1))), R.push(t.h(t.Transition, {
                         name: "q-transition--fade"
                     }, V)), t.h("div", {
-                        class: h.value,
+                        class: m.value,
                         style: f.value,
                         role: "img",
                         "aria-label": e.alt
                     }, R)
                 }
             }
         });
```

### Comparing `pybi-next-0.5.0b8/pybi/static/sysApp-style.css` & `pybi-next-0.5.0b9/pybi/static/sysApp-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/sysApp.iife.js` & `pybi-next-0.5.0b9/pybi/static/sysApp.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/static/vue.global.prod.min.js` & `pybi-next-0.5.0b9/pybi/static/vue.global.prod.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/template/index.html` & `pybi-next-0.5.0b9/pybi/template/index.html`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/dataSourceUtils.py` & `pybi-next-0.5.0b9/pybi/utils/dataSourceUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/data_gen.py` & `pybi-next-0.5.0b9/pybi/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/dictUtils.py` & `pybi-next-0.5.0b9/pybi/utils/dictUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/echarts_opts_utils.py` & `pybi-next-0.5.0b9/pybi/utils/echarts_opts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/helper.py` & `pybi-next-0.5.0b9/pybi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/markdown2.py` & `pybi-next-0.5.0b9/pybi/utils/markdown2.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/pyecharts_utils.py` & `pybi-next-0.5.0b9/pybi/utils/pyecharts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi/utils/sql.py` & `pybi-next-0.5.0b9/pybi/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/pybi_next.egg-info/SOURCES.txt` & `pybi-next-0.5.0b9/pybi_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybi-next-0.5.0b8/setup.py` & `pybi-next-0.5.0b9/setup.py`

 * *Files identical despite different names*

