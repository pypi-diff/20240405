# Comparing `tmp/omnix-0.3.1.tar.gz` & `tmp/omnix-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omnix-0.3.1.tar", last modified: Tue Jun 28 08:47:41 2022, max compression
+gzip compressed data, was "dist/omnix-0.3.3.tar", last modified: Fri Apr  5 10:49:40 2024, max compression
```

## Comparing `omnix-0.3.1.tar` & `omnix-0.3.3.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     3755 2022-06-28 08:47:25.000000 omnix-0.3.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     5482 2022-06-28 08:47:41.000000 omnix-0.3.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix.egg-info/
--rw-r--r--   0 root         (0) root         (0)        6 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5482 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       60 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     3761 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-28 08:47:36.000000 omnix-0.3.1/src/omnix.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/models/
--rw-r--r--   0 root         (0) root         (0)     1965 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/models/base.py
--rw-r--r--   0 root         (0) root         (0)     1297 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2645 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/models/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/test/util/
--rw-r--r--   0 root         (0) root         (0)    12169 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/test/util/business.py
--rw-r--r--   0 root         (0) root         (0)     1193 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1193 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/
--rw-r--r--   0 root         (0) root         (0)      338 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/index.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/report/
--rw-r--r--   0 root         (0) root         (0)     2311 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/report/sales.html.tpl
--rw-r--r--   0 root         (0) root         (0)      406 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/report/list.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/partials/
--rw-r--r--   0 root         (0) root         (0)      346 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/footer.html.tpl
--rw-r--r--   0 root         (0) root         (0)        9 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/end_doctype.html.tpl
--rw-r--r--   0 root         (0) root         (0)     5710 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/layout.html.tpl
--rw-r--r--   0 root         (0) root         (0)      680 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/layout_report.html.tpl
--rw-r--r--   0 root         (0) root         (0)      940 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/includes.html.tpl
--rw-r--r--   0 root         (0) root         (0)      237 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/messages.html.tpl
--rw-r--r--   0 root         (0) root         (0)      697 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/layout_simple.html.tpl
--rw-r--r--   0 root         (0) root         (0)       35 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/doctype.html.tpl
--rw-r--r--   0 root         (0) root         (0)       71 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/content_type.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1168 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/layout_media.html.tpl
--rw-r--r--   0 root         (0) root         (0)      679 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/layout_store.html.tpl
--rw-r--r--   0 root         (0) root         (0)      686 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/layout_entity.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1875 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/partials/layout_employee.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/store/
--rw-r--r--   0 root         (0) root         (0)     1570 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/store/sales.html.tpl
--rw-r--r--   0 root         (0) root         (0)      778 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/store/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)      874 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/store/list.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/email/
--rw-r--r--   0 root         (0) root         (0)     3290 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/email/activity.en_us.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1591 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/email/layout.pt_pt.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3310 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/email/activity.pt_pt.html.tpl
--rw-r--r--   0 root         (0) root         (0)      207 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/email/birthday.en_us.html.tpl
--rw-r--r--   0 root         (0) root         (0)      215 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/email/birthday.pt_pt.html.tpl
--rw-r--r--   0 root         (0) root         (0)      717 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/email/macros.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1587 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/email/layout.en_us.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/supplier/
--rw-r--r--   0 root         (0) root         (0)      797 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/supplier/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)      889 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/supplier/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)      480 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/signin.html.tpl
--rw-r--r--   0 root         (0) root         (0)      842 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/error.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/employee/
--rw-r--r--   0 root         (0) root         (0)     4090 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/employee/sales.html.tpl
--rw-r--r--   0 root         (0) root         (0)      812 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/employee/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)      889 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/employee/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)      959 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/about.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/media/
--rw-r--r--   0 root         (0) root         (0)     3043 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/media/edit.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1977 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/media/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)      837 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/media/list.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/customer/
--rw-r--r--   0 root         (0) root         (0)      913 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/customer/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)      889 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/customer/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)     2790 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/top.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/extra/
--rw-r--r--   0 root         (0) root         (0)     1078 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/costs.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1445 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/transfers.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1059 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/images.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3345 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/template.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/extra/browser/
--rw-r--r--   0 root         (0) root         (0)     3538 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/browser/new_media.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1051 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/ctt.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1085 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/prices.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1053 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/media.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3985 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1611 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/metadata.html.tpl
--rw-r--r--   0 root         (0) root         (0)     2016 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/browser.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1093 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/extra/inventory.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/templates/entity/
--rw-r--r--   0 root         (0) root         (0)     1197 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/entity/edit.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1720 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/entity/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)      852 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/templates/entity/list.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/util/
--rw-r--r--   0 root         (0) root         (0)     8670 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/supervisor.py
--rw-r--r--   0 root         (0) root         (0)     3781 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/image.py
--rw-r--r--   0 root         (0) root         (0)     4310 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/ctt.py
--rw-r--r--   0 root         (0) root         (0)     2646 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/format.py
--rw-r--r--   0 root         (0) root         (0)     5890 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/config.py
--rw-r--r--   0 root         (0) root         (0)     4269 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     7380 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/slave.py
--rw-r--r--   0 root         (0) root         (0)     3479 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/logic.py
--rw-r--r--   0 root         (0) root         (0)    34718 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/business.py
--rw-r--r--   0 root         (0) root         (0)     2382 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2182 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/views/api/
--rw-r--r--   0 root         (0) root         (0)     1724 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/api/base.py
--rw-r--r--   0 root         (0) root         (0)     1244 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/views/web/
--rw-r--r--   0 root         (0) root         (0)     3555 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/entity.py
--rw-r--r--   0 root         (0) root         (0)     1777 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/report.py
--rw-r--r--   0 root         (0) root         (0)    10928 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/base.py
--rw-r--r--   0 root         (0) root         (0)     5466 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/employee.py
--rw-r--r--   0 root         (0) root         (0)     3916 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/media.py
--rw-r--r--   0 root         (0) root         (0)    50714 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/extra.py
--rw-r--r--   0 root         (0) root         (0)     2196 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/customer.py
--rw-r--r--   0 root         (0) root         (0)     4471 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/store.py
--rw-r--r--   0 root         (0) root         (0)     2632 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2205 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/supplier.py
--rw-r--r--   0 root         (0) root         (0)     2666 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/web/settings.py
--rw-r--r--   0 root         (0) root         (0)     1275 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/static/css/
--rw-r--r--   0 root         (0) root         (0)     3930 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/static/css/layout.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/static/images/
--rw-r--r--   0 root         (0) root         (0)      129 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/static/images/down.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/static/images/email/
--rw-r--r--   0 root         (0) root         (0)     1177 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/static/images/email/logo.png
--rw-r--r--   0 root         (0) root         (0)      108 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/static/images/equal.png
--rw-r--r--   0 root         (0) root         (0)      127 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/static/images/up.png
--rw-r--r--   0 root         (0) root         (0)     2771 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/static/images/login.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-28 08:47:41.000000 omnix-0.3.1/src/omnix/static/js/
--rw-r--r--   0 root         (0) root         (0)     5109 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/static/js/main.js
--rw-r--r--   0 root         (0) root         (0)     1369 2022-06-28 08:47:25.000000 omnix-0.3.1/src/omnix/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4118 2022-06-28 08:47:25.000000 omnix-0.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-28 08:47:41.000000 omnix-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:49:36.000000 omnix-0.3.3/src/omnix.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3761 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/util/
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/logic.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/image.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/format.py
+-rw-r--r--   0 root         (0) root         (0)    34528 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/business.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/ctt.py
+-rw-r--r--   0 root         (0) root         (0)     5615 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/config.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/slave.py
+-rw-r--r--   0 root         (0) root         (0)     8985 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/supervisor.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/images/
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/down.png
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/equal.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/images/email/
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/email/logo.png
+-rw-r--r--   0 root         (0) root         (0)      127 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/up.png
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/login.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/css/
+-rw-r--r--   0 root         (0) root         (0)     3930 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/css/layout.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/js/
+-rw-r--r--   0 root         (0) root         (0)     5109 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/js/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/error.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      959 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/about.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      338 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/index.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/media/
+-rw-r--r--   0 root         (0) root         (0)     3043 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/media/edit.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      837 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/media/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/media/show.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/extra/
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/ctt.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/costs.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3985 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3345 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/template.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/media.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/images.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/prices.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/inventory.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/transfers.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/browser.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/extra/browser/
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/browser/new_media.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/metadata.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/entity/
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/entity/edit.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      852 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/entity/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/entity/show.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/report/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/report/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/report/sales.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/customer/
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/customer/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      913 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/customer/show.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/doctype.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     5710 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout.html.tpl
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/end_doctype.html.tpl
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/content_type.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      237 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/messages.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      679 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_store.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_simple.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      680 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_report.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      940 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/includes.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_employee.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      686 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_entity.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/footer.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_media.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/supplier/
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/supplier/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/supplier/show.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/email/
+-rw-r--r--   0 root         (0) root         (0)     1591 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/layout.pt_pt.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/birthday.pt_pt.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      717 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/macros.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/layout.en_us.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/activity.en_us.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      207 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/birthday.en_us.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/activity.pt_pt.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/employee/
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/employee/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      812 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/employee/show.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     4090 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/employee/sales.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/signin.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/store/
+-rw-r--r--   0 root         (0) root         (0)      874 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/store/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/store/show.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/store/sales.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/top.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/models/
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/models/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/views/
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/views/web/
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/supplier.py
+-rw-r--r--   0 root         (0) root         (0)    10028 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/base.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/settings.py
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/media.py
+-rw-r--r--   0 root         (0) root         (0)    50263 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/extra.py
+-rw-r--r--   0 root         (0) root         (0)     4169 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/store.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/report.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/customer.py
+-rw-r--r--   0 root         (0) root         (0)     5180 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/employee.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/views/api/
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/api/base.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/test/util/
+-rw-r--r--   0 root         (0) root         (0)      970 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12740 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/test/util/business.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2024-04-05 10:49:28.000000 omnix-0.3.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 10:49:40.000000 omnix-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4118 2024-04-05 10:49:28.000000 omnix-0.3.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-05 10:49:40.000000 omnix-0.3.3/PKG-INFO
```

### Comparing `omnix-0.3.1/setup.py` & `omnix-0.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,58 +18,47 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
-    name = "omnix",
-    version = "0.3.1",
-    author = "Hive Solutions Lda.",
-    author_email = "development@hive.pt",
-    description = "Omnix System",
-    license = "Apache License, Version 2.0",
-    keywords = "omni extensions erp",
-    url = "http://omnix.hive.pt",
-    zip_safe = False,
-    packages = [
+    name="omnix",
+    version="0.3.3",
+    author="Hive Solutions Lda.",
+    author_email="development@hive.pt",
+    description="Omnix System",
+    license="Apache License, Version 2.0",
+    keywords="omni extensions erp",
+    url="http://omnix.hive.pt",
+    zip_safe=False,
+    packages=[
         "omnix",
         "omnix.models",
         "omnix.test",
         "omnix.test.util",
         "omnix.util",
         "omnix.views",
         "omnix.views.api",
-        "omnix.views.web"
+        "omnix.views.web",
     ],
-    test_suite = "omnix.test",
-    package_dir = {
-        "" : os.path.normpath("src")
-    },
-    package_data = {
-        "omnix" : [
+    test_suite="omnix.test",
+    package_dir={"": os.path.normpath("src")},
+    package_data={
+        "omnix": [
             "static/css/*.css",
             "static/images/*.png",
             "static/images/email/*.png",
             "static/js/*.js",
             "templates/*.tpl",
             "templates/customer/*.tpl",
             "templates/email/*.tpl",
@@ -77,41 +66,43 @@
             "templates/entity/*.tpl",
             "templates/extra/*.tpl",
             "templates/extra/browser/*.tpl",
             "templates/media/*.tpl",
             "templates/partials/*.tpl",
             "templates/report/*.tpl",
             "templates/store/*.tpl",
-            "templates/supplier/*.tpl"
+            "templates/supplier/*.tpl",
         ]
     },
-    install_requires = [
+    install_requires=[
         "netius",
         "flask",
         "quorum",
         "pillow",
         "pymongo",
         "redis",
         "pika",
         "xlrd",
-        "omni_api"
+        "omni-api",
     ],
-    classifiers = [
+    classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.7",
     ],
-    long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "r").read(),
-    long_description_content_type = "text/markdown"
+    long_description=open(os.path.join(os.path.dirname(__file__), "README.md"), "rb")
+    .read()
+    .decode("utf-8"),
+    long_description_content_type="text/markdown",
 )
```

### Comparing `omnix-0.3.1/PKG-INFO` & `omnix-0.3.3/src/omnix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnix
-Version: 0.3.1
+Version: 0.3.3
 Summary: Omnix System
 Home-page: http://omnix.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni (x)Extensions](http://omnix.hive.pt)
```

### Comparing `omnix-0.3.1/src/omnix.egg-info/PKG-INFO` & `omnix-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnix
-Version: 0.3.1
+Version: 0.3.3
 Summary: Omnix System
 Home-page: http://omnix.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni (x)Extensions](http://omnix.hive.pt)
```

### Comparing `omnix-0.3.1/src/omnix.egg-info/SOURCES.txt` & `omnix-0.3.3/src/omnix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/models/base.py` & `omnix-0.3.3/src/omnix/models/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,56 +18,34 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
+
 class Base(quorum.Model):
 
-    id = dict(
-        type = int,
-        index = True,
-        increment = True,
-        immutable = True
-    )
-
-    enabled = dict(
-        type = bool,
-        index = True
-    )
+    id = dict(type=int, index=True, increment=True, immutable=True)
+
+    enabled = dict(type=bool, index=True)
 
     def pre_create(self):
         quorum.Model.pre_create(self)
 
         self.enabled = True
 
     def enable(self):
         store = self._get_store()
-        store.update(
-            {"_id" : self._id},
-            {"$set" : {"enabled" : True}}
-        )
+        store.update({"_id": self._id}, {"$set": {"enabled": True}})
 
     def disable(self):
         store = self._get_store()
-        store.update(
-            {"_id" : self._id},
-            {"$set" : {"enabled" : False}}
-        )
+        store.update({"_id": self._id}, {"$set": {"enabled": False}})
```

### Comparing `omnix-0.3.1/src/omnix/models/__init__.py` & `omnix-0.3.3/src/omnix/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,23 +15,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import base
```

### Comparing `omnix-0.3.1/src/omnix/models/settings.py` & `omnix-0.3.3/src/omnix/models/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,73 +18,65 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import flask
 import quorum
 
 from omnix import util
 
 from . import base
 
+
 class Settings(base.Base):
 
     slack_token = quorum.field(
-        index = "hashed",
-        observations = """The OAuth token from Slack that is going
+        index="hashed",
+        observations="""The OAuth token from Slack that is going
         to be used for long term Slack interaction after the OAuth
-        authentication process is completed"""
+        authentication process is completed""",
     )
 
-    slack_channel = quorum.field(
-        index = "hashed"
-    )
+    slack_channel = quorum.field(index="hashed")
 
-    extra = quorum.field(
-        type = dict
-    )
+    extra = quorum.field(type=dict)
 
     @classmethod
     def get_settings(cls, *args, **kwargs):
         return cls.singleton(*args, **kwargs)
 
     @classmethod
     def linked_apis(cls):
         linked = dict()
         settings = cls.get_settings()
-        if settings.slack_token: linked["slack"] = settings.slack_token
+        if settings.slack_token:
+            linked["slack"] = settings.slack_token
         return linked
 
     @classmethod
     def _plural(cls):
         return "Settings"
 
     def get_slack_api(self):
-        try: import slack
-        except ImportError: return None
-        if not self.slack_token: return None
+        try:
+            import slack
+        except ImportError:
+            return None
+        if not self.slack_token:
+            return None
         redirect_url = util.BASE_URL + flask.url_for("oauth_slack")
         access_token = self.slack_token
         return slack.API(
-            client_id = quorum.conf("SLACK_ID"),
-            client_secret = quorum.conf("SLACK_SECRET"),
-            redirect_url = redirect_url,
-            access_token = access_token
+            client_id=quorum.conf("SLACK_ID"),
+            client_secret=quorum.conf("SLACK_SECRET"),
+            redirect_url=redirect_url,
+            access_token=access_token,
         )
```

### Comparing `omnix-0.3.1/src/omnix/test/util/business.py` & `omnix-0.3.3/src/omnix/test/util/business.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,210 +18,298 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import calendar
 import datetime
 import unittest
 
 import omnix
 
+
 class BusinessTest(unittest.TestCase):
 
     def test_get_comparison_day(self):
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 2, day = 28, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 2, day = 28, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "day", offset = -1, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=2, day=28, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=2, day=28, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="day", offset=-1, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 28)
         self.assertEqual(current_v["unit"], "day")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 28)
         self.assertEqual(previous_v["unit"], "day")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 1, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 3, day = 1, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "day", offset = 0, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=1, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=3, day=1, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="day", offset=0, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 1)
         self.assertEqual(current_v["unit"], "day")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 1)
         self.assertEqual(previous_v["unit"], "day")
         self.assertEqual(previous_v["has_global"], True)
 
     def test_get_comparison_day_leap(self):
-        timestamp = calendar.timegm(datetime.datetime(year = 2020, month = 3, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2020, month = 2, day = 29, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2019, month = 2, day = 28, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "day", offset = -1, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2020, month=3, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2020, month=2, day=29, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2019, month=2, day=28, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="day", offset=-1, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 29)
         self.assertEqual(current_v["unit"], "day")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 28)
         self.assertEqual(previous_v["unit"], "day")
         self.assertEqual(previous_v["has_global"], True)
 
     def test_get_comparison_month(self):
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 2, day = 28, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 2, day = 28, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -1, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=2, day=28, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=2, day=28, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-1, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 2)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 2)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 1, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 3, day = 1, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = 0, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=1, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=3, day=1, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=0, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 3)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 3)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 2, day = 25, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 2, day = 25, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -4, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=2, day=25, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=2, day=25, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-4, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 2)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 2)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 4, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 3, day = 31, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 3, day = 31, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -1, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=4, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=3, day=31, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=3, day=31, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-1, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 3)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 3)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 1, day = 2, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 1, day = 1, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 1, day = 1, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -1, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=1, day=2, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=1, day=1, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=1, day=1, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-1, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 1)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 1)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 2, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 1, day = 31, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 1, day = 31, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -1, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=2, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=1, day=31, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=1, day=31, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-1, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 1)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 1)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 2, day = 2, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2018, month = 1, day = 31, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2017, month = 1, day = 31, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -2, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=2, day=2, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2018, month=1, day=31, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2017, month=1, day=31, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-2, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 1)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 1)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
-        timestamp = calendar.timegm(datetime.datetime(year = 2018, month = 1, day = 2, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2017, month = 12, day = 31, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2016, month = 12, day = 31, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -2, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2018, month=1, day=2, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2017, month=12, day=31, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2016, month=12, day=31, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-2, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 12)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
         self.assertEqual(previous_v["span"], 12)
         self.assertEqual(previous_v["unit"], "month")
         self.assertEqual(previous_v["has_global"], True)
 
     def test_get_comparison_month_leap(self):
-        timestamp = calendar.timegm(datetime.datetime(year = 2020, month = 3, day = 1, hour = 4).utctimetuple())
-        current = calendar.timegm(datetime.datetime(year = 2020, month = 2, day = 29, hour = 4).utctimetuple())
-        previous = calendar.timegm(datetime.datetime(year = 2019, month = 2, day = 28, hour = 4).utctimetuple())
-        current_v, previous_v = omnix.calc_comparison(unit = "month", offset = -1, timestamp = timestamp)
+        timestamp = calendar.timegm(
+            datetime.datetime(year=2020, month=3, day=1, hour=4).utctimetuple()
+        )
+        current = calendar.timegm(
+            datetime.datetime(year=2020, month=2, day=29, hour=4).utctimetuple()
+        )
+        previous = calendar.timegm(
+            datetime.datetime(year=2019, month=2, day=28, hour=4).utctimetuple()
+        )
+        current_v, previous_v = omnix.calc_comparison(
+            unit="month", offset=-1, timestamp=timestamp
+        )
 
         self.assertEqual(current_v["date"], current)
         self.assertEqual(current_v["span"], 2)
         self.assertEqual(current_v["unit"], "month")
         self.assertEqual(current_v["has_global"], True)
 
         self.assertEqual(previous_v["date"], previous)
```

### Comparing `omnix-0.3.1/src/omnix/test/util/__init__.py` & `omnix-0.3.3/src/omnix/views/api/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,21 +15,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
+
+from . import base
+
+from .base import log_api
```

### Comparing `omnix-0.3.1/src/omnix/test/__init__.py` & `omnix-0.3.3/src/omnix/views/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,21 +15,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
+
+from . import api
+from . import web
+
+from .api import *
+from .web import *
```

### Comparing `omnix-0.3.1/src/omnix/templates/report/sales.html.tpl` & `omnix-0.3.3/src/omnix/templates/report/sales.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/layout.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/layout.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/layout_report.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/layout_report.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/includes.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/includes.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/layout_simple.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/layout_simple.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/layout_media.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/layout_media.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/layout_store.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/layout_store.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/layout_entity.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/layout_entity.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/partials/layout_employee.html.tpl` & `omnix-0.3.3/src/omnix/templates/partials/layout_employee.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/store/sales.html.tpl` & `omnix-0.3.3/src/omnix/templates/store/sales.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/store/show.html.tpl` & `omnix-0.3.3/src/omnix/templates/store/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/store/list.html.tpl` & `omnix-0.3.3/src/omnix/templates/store/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/email/activity.en_us.html.tpl` & `omnix-0.3.3/src/omnix/templates/email/activity.en_us.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/email/layout.pt_pt.html.tpl` & `omnix-0.3.3/src/omnix/templates/email/layout.pt_pt.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/email/activity.pt_pt.html.tpl` & `omnix-0.3.3/src/omnix/templates/email/activity.pt_pt.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/email/macros.html.tpl` & `omnix-0.3.3/src/omnix/templates/email/macros.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/email/layout.en_us.html.tpl` & `omnix-0.3.3/src/omnix/templates/email/layout.en_us.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/supplier/show.html.tpl` & `omnix-0.3.3/src/omnix/templates/supplier/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/supplier/list.html.tpl` & `omnix-0.3.3/src/omnix/templates/supplier/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/error.html.tpl` & `omnix-0.3.3/src/omnix/templates/error.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/employee/sales.html.tpl` & `omnix-0.3.3/src/omnix/templates/employee/sales.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/employee/show.html.tpl` & `omnix-0.3.3/src/omnix/templates/employee/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/employee/list.html.tpl` & `omnix-0.3.3/src/omnix/templates/employee/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/about.html.tpl` & `omnix-0.3.3/src/omnix/templates/about.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/media/edit.html.tpl` & `omnix-0.3.3/src/omnix/templates/media/edit.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/media/show.html.tpl` & `omnix-0.3.3/src/omnix/templates/media/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/media/list.html.tpl` & `omnix-0.3.3/src/omnix/templates/media/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/customer/show.html.tpl` & `omnix-0.3.3/src/omnix/templates/customer/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/customer/list.html.tpl` & `omnix-0.3.3/src/omnix/templates/customer/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/top.html.tpl` & `omnix-0.3.3/src/omnix/templates/top.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/costs.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/costs.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/transfers.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/transfers.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/images.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/images.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/template.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/template.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/browser/new_media.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/browser/new_media.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/ctt.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/ctt.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/prices.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/prices.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/media.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/media.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/list.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/metadata.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/metadata.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/browser.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/browser.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/extra/inventory.html.tpl` & `omnix-0.3.3/src/omnix/templates/extra/inventory.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/entity/edit.html.tpl` & `omnix-0.3.3/src/omnix/templates/entity/edit.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/entity/show.html.tpl` & `omnix-0.3.3/src/omnix/templates/entity/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/templates/entity/list.html.tpl` & `omnix-0.3.3/src/omnix/templates/entity/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/util/supervisor.py` & `omnix-0.3.3/src/omnix/util/supervisor.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import time
@@ -65,14 +56,15 @@
 before it's considered discarded """
 
 NUMBER_RECORDS = config.RECORD_CHUNK
 """ The maximum number of records that is going to be
 retrieved and set for submission, this value influences
 the performance, mostly under heavy load situations """
 
+
 class Supervisor(threading.Thread):
 
     session_id = None
     connection = None
     channel = None
     queue = None
 
@@ -80,159 +72,185 @@
         threading.Thread.__init__(self)
         self.daemon = True
 
     def stop(self):
         pass
 
     def auth(self):
-        if not config.REMOTE: return
+        if not config.REMOTE:
+            return
 
         username = config.USERNAME
         password = config.PASSWORD
         if username == None or password == None:
             raise RuntimeError("Missing authentication information")
 
-        self.api = logic.get_api(mode = omni.API.DIRECT_MODE)
+        self.api = logic.get_api(mode=omni.API.DIRECT_MODE)
 
-    def connect(self, queue = "default", retry = True):
-        if not config.REMOTE: return
+    def connect(self, queue="default", retry=True):
+        if not config.REMOTE:
+            return
 
         quorum.info("Connecting to the AMQP system")
 
         while True:
             try:
-                self.connection = quorum.get_amqp(force = True)
+                self.connection = quorum.get_amqp(force=True)
                 self.channel = self.connection.channel()
-                self.channel.queue_declare(queue = queue, durable = True)
+                self.channel.queue_declare(queue=queue, durable=True)
                 self.queue = queue
                 break
             except Exception as exception:
-                if not retry: raise
+                if not retry:
+                    raise
                 quorum.error(
-                    "Exception while connecting - %s" % quorum.legacy.UNICODE(exception),
-                    log_trace = True
+                    "Exception while connecting - %s"
+                    % quorum.legacy.UNICODE(exception),
+                    log_trace=True,
                 )
                 quorum.info("Sleeping %d seconds before connect retry" % RETRY_TIMEOUT)
                 time.sleep(RETRY_TIMEOUT)
 
     def disconnect(self):
-        if not config.REMOTE: return
+        if not config.REMOTE:
+            return
 
         quorum.info("Disconnected from the AMQP system")
 
         self.connection.close()
 
-    def reconnect(self, retry = True):
-        if not config.REMOTE: return
-        if not self.connection.is_closed: return
+    def reconnect(self, retry=True):
+        if not config.REMOTE:
+            return
+        if not self.connection.is_closed:
+            return
 
         quorum.info("Re-connecting to the AMQP system")
 
-        self.connect(queue = self.queue, retry = retry)
+        self.connect(queue=self.queue, retry=retry)
 
     def execute(self):
         # in case the current instance is not configured according to
         # the remote rules the queuing operation is ignored, and so
         # the control flow returns immediately
-        if not config.REMOTE: return
+        if not config.REMOTE:
+            return
 
         # creates a values map structure to retrieve the complete
         # set of inbound documents that have not yet been submitted
         # to at for the flush operation
         kwargs = {
-            "session_id" : self.session_id,
-            "filter_string" : "",
-            "start_record" : 0,
-            "number_records" : NUMBER_RECORDS,
-            "sort" : "issue_date:ascending",
-            "filters[]" : [
+            "session_id": self.session_id,
+            "filter_string": "",
+            "start_record": 0,
+            "number_records": NUMBER_RECORDS,
+            "sort": "issue_date:ascending",
+            "filters[]": [
                 "issue_date:greater:1356998400",
                 "submitted_at:equals:2",
-                "document_type:in:1;3"
-            ]
+                "document_type:in:1;3",
+            ],
         }
         documents = self.api.list_signed_documents(**kwargs)
-        valid_documents = [value for value in documents\
-            if value["_class"] in config.AT_SUBMIT_TYPES]
+        valid_documents = [
+            value for value in documents if value["_class"] in config.AT_SUBMIT_TYPES
+        ]
 
         # starts the counter value to zero, so that we're able to count
         # the number of messages that have been successfully queued to
         # the remote queueing mechanism (for debugging)
         count = 0
 
+        # prints a debug message about the number of valid documents that
+        # have been found for submission to the queue
+        quorum.debug(
+            "Found %d valid documents for submission, from a total of %d documents"
+            % (len(valid_documents), len(documents))
+        )
+
         # iterates over all the valid documents that have been found
         # as not submitted and creates a task for their submission
         # then adds the task to the AMQP queue to be processed
         for document in valid_documents:
             try:
                 # tries to run the basic publish operation, this operation
                 # may fail for a variety of reasons including errors in the
                 # underlying library so a reconnection is attempted in case
                 # there's an exception raised under this operation
                 self.channel.basic_publish(
-                    exchange = "",
-                    routing_key = config.QUEUE,
-                    body = json.dumps(document),
-                    properties = quorum.properties_amqp(
-                        delivery_mode = 2,
-                        priority = MESSAGE_RETRIES,
-                        expiration = str(MESSAGE_TIMEOUT * 1000),
-                        timestamp = time.time()
-                    )
+                    exchange="",
+                    routing_key=config.QUEUE,
+                    body=json.dumps(document),
+                    properties=quorum.properties_amqp(
+                        delivery_mode=2,
+                        priority=MESSAGE_RETRIES,
+                        expiration=str(MESSAGE_TIMEOUT * 1000),
+                        timestamp=time.time(),
+                    ),
                 )
                 count += 1
             except Exception as exception:
                 # prints a warning message about the exception that has just occurred
                 # so that it's possible to act on it
                 quorum.warning(
-                    "Exception in publish (will re-connect) - %s" % quorum.legacy.UNICODE(exception),
-                    log_trace = True
+                    "Exception in publish (will re-connect) - %s"
+                    % quorum.legacy.UNICODE(exception),
+                    log_trace=True,
                 )
 
                 # re-tries to connect with the AMQP channels using the currently
                 # pre-defined queue system, this is a fallback of the error
                 self.reconnect()
 
         # prints an information message about the new documents that
         # have been queued for submission by the "slaves"
-        quorum.info("Queued %d (out of %d) documents for submission" % (count, len(valid_documents)))
+        quorum.info(
+            "Queued %d (out of %d) documents for submission"
+            % (count, len(valid_documents))
+        )
 
     def loop(self):
         while True:
-            try: self.execute()
+            try:
+                self.execute()
             except Exception as exception:
                 # prints an error message about the exception that has just occurred
                 # so that it's possible to act on it
                 quorum.error(
                     "Exception while executing - %s" % quorum.legacy.UNICODE(exception),
-                    log_trace = True
+                    log_trace=True,
                 )
 
                 # re-tries to connect with the AMQP channels using the currently
                 # pre-defined queue system, this is a fallback of the error
                 self.reconnect()
 
             try:
-                if self.connection: self.connection.sleep(LOOP_TIMEOUT)
-                else: time.sleep(LOOP_TIMEOUT)
+                if self.connection:
+                    self.connection.sleep(LOOP_TIMEOUT)
+                else:
+                    time.sleep(LOOP_TIMEOUT)
             except Exception as exception:
                 # prints a critical message about the exception that has just occurred
                 # so that it's possible to act on it
                 quorum.critical(
                     "Exception while sleeping - %s" % quorum.legacy.UNICODE(exception),
-                    log_trace = True
+                    log_trace=True,
                 )
 
                 # re-tries to connect with the AMQP channels using the currently
                 # pre-defined queue system, this is a fallback of the error
                 self.reconnect()
 
     def run(self):
         self.auth()
-        self.connect(queue = config.QUEUE)
-        try: self.loop()
-        finally: self.disconnect()
+        self.connect(queue=config.QUEUE)
+        try:
+            self.loop()
+        finally:
+            self.disconnect()
+
 
-def run(count = 1):
+def run(count=1):
     for _index in range(count):
         supervisor = Supervisor()
         supervisor.start()
```

### Comparing `omnix-0.3.1/src/omnix/util/image.py` & `omnix-0.3.3/src/omnix/util/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,26 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
 
 from . import config
 
-def mask_image(base_data, mask_data, format = "png"):
+
+def mask_image(base_data, mask_data, format="png"):
     import PIL.Image
 
     base_file = quorum.legacy.BytesIO(base_data)
     mask_file = quorum.legacy.BytesIO(mask_data)
     out_file = quorum.legacy.BytesIO()
 
     base_image = PIL.Image.open(base_file)
@@ -65,40 +57,38 @@
         ratio_height = float(mask_height) / float(base_height)
 
         ratio = ratio_width if ratio_width < ratio_height else ratio_height
         resize_width = int(base_width * ratio)
         resize_height = int(base_height * ratio)
 
         base_image = base_image.resize(
-            (resize_width, resize_height),
-            PIL.Image.ANTIALIAS
+            (resize_width, resize_height), PIL.Image.ANTIALIAS
         )
     elif config.IMAGE_RESIZE == "crop":
         ratio_width = float(mask_width) / float(base_width)
         ratio_height = float(mask_height) / float(base_height)
 
         ratio = ratio_height if ratio_width < ratio_height else ratio_width
         resize_width = int(base_width * ratio)
         resize_height = int(base_height * ratio)
 
         base_image = base_image.resize(
-            (resize_width, resize_height),
-            PIL.Image.ANTIALIAS
+            (resize_width, resize_height), PIL.Image.ANTIALIAS
         )
 
         center_width = (resize_width - mask_width) / 2.0
         center_height = (resize_height - mask_height) / 2.0
         center_width = int(center_width)
         center_height = int(center_height)
 
         crop_box = (
             center_width,
             center_height,
             mask_width + center_width,
-            mask_height + center_height
+            mask_height + center_height,
         )
         base_image = base_image.crop(crop_box)
 
     base_width, base_height = base_image.size
     center_width = (mask_width - base_width) / 2.0
     center_height = (mask_height - base_height) / 2.0
     center = (int(center_width), int(center_height))
```

### Comparing `omnix-0.3.1/src/omnix/util/ctt.py` & `omnix-0.3.3/src/omnix/util/ctt.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,104 +18,109 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-def encode_ctt(sale_orders, encoding = None):
+
+def encode_ctt(sale_orders, encoding=None):
     lines = []
 
     for sale_order in sale_orders:
         line = dict(
-            reference = sale_order["extended_identifier"][:21],
-            quantity = 1,
-            weight = "100,00",
-            price = "0ue",
-            destiny = sale_order["customer"]["representation"][:60],
-            title = "",
-            name = "",
-            address = sale_order["shipping_address"]["street_name"][:60],
-            town = sale_order["shipping_address"]["zip_code_name"][:50],
-            zip_code_4 = sale_order["shipping_address"]["zip_code"].split("-", 1)[0][:4],
-            zip_code_3 = sale_order["shipping_address"]["zip_code"].split("-", 1)[1][:3],
-            not_applicable_1 = "",
-            observations = "",
-            back = 0,
-            document_code = "",
-            phone_number = (sale_order["customer"]["primary_contact_information"]["phone_number"] or "").replace("+", "00")[:15],
-            saturday = 0,
-            email = (sale_order["customer"]["primary_contact_information"]["email"] or "")[:200],
-            country = "PT",
-            fragile = 0,
-            not_applicable_2 = "",
-            document_collection = "",
-            code_email = "",
-            mobile_phone = (sale_order["customer"]["primary_contact_information"]["mobile_phone_number"] or "").replace("+", "00")[:15],
-            second_delivery = 0,
-            delivery_date = "",
-            return_signed_document = 0,
-            expeditor_instructions = 0,
-            sms = 1,
-            not_applicable_3 = "",
-            printer = "",
-            ticket_machine = "",
-            at_code = ""
+            reference=sale_order["extended_identifier"][:21],
+            quantity=1,
+            weight="100,00",
+            price="0ue",
+            destiny=sale_order["customer"]["representation"][:60],
+            title="",
+            name="",
+            address=sale_order["shipping_address"]["street_name"][:60],
+            town=sale_order["shipping_address"]["zip_code_name"][:50],
+            zip_code_4=sale_order["shipping_address"]["zip_code"].split("-", 1)[0][:4],
+            zip_code_3=sale_order["shipping_address"]["zip_code"].split("-", 1)[1][:3],
+            not_applicable_1="",
+            observations="",
+            back=0,
+            document_code="",
+            phone_number=(
+                sale_order["customer"]["primary_contact_information"]["phone_number"]
+                or ""
+            ).replace("+", "00")[:15],
+            saturday=0,
+            email=(
+                sale_order["customer"]["primary_contact_information"]["email"] or ""
+            )[:200],
+            country="PT",
+            fragile=0,
+            not_applicable_2="",
+            document_collection="",
+            code_email="",
+            mobile_phone=(
+                sale_order["customer"]["primary_contact_information"][
+                    "mobile_phone_number"
+                ]
+                or ""
+            ).replace("+", "00")[:15],
+            second_delivery=0,
+            delivery_date="",
+            return_signed_document=0,
+            expeditor_instructions=0,
+            sms=1,
+            not_applicable_3="",
+            printer="",
+            ticket_machine="",
+            at_code="",
         )
 
-        line = "+".join([
-            line["reference"],
-            str(line["quantity"]),
-            line["weight"],
-            line["price"],
-            line["destiny"],
-            line["title"],
-            line["name"],
-            line["address"],
-            line["town"],
-            line["zip_code_4"],
-            line["zip_code_3"],
-            line["not_applicable_1"],
-            line["observations"],
-            str(line["back"]),
-            line["document_code"],
-            line["phone_number"],
-            str(line["saturday"]),
-            line["email"],
-            line["country"],
-            str(line["fragile"]),
-            line["not_applicable_2"],
-            line["document_collection"],
-            line["code_email"],
-            line["mobile_phone"],
-            str(line["second_delivery"]),
-            line["delivery_date"],
-            str(line["return_signed_document"]),
-            str(line["expeditor_instructions"]),
-            str(line["sms"]),
-            line["not_applicable_3"],
-            line["printer"],
-            line["ticket_machine"],
-            line["at_code"]
-        ])
+        line = "+".join(
+            [
+                line["reference"],
+                str(line["quantity"]),
+                line["weight"],
+                line["price"],
+                line["destiny"],
+                line["title"],
+                line["name"],
+                line["address"],
+                line["town"],
+                line["zip_code_4"],
+                line["zip_code_3"],
+                line["not_applicable_1"],
+                line["observations"],
+                str(line["back"]),
+                line["document_code"],
+                line["phone_number"],
+                str(line["saturday"]),
+                line["email"],
+                line["country"],
+                str(line["fragile"]),
+                line["not_applicable_2"],
+                line["document_collection"],
+                line["code_email"],
+                line["mobile_phone"],
+                str(line["second_delivery"]),
+                line["delivery_date"],
+                str(line["return_signed_document"]),
+                str(line["expeditor_instructions"]),
+                str(line["sms"]),
+                line["not_applicable_3"],
+                line["printer"],
+                line["ticket_machine"],
+                line["at_code"],
+            ]
+        )
 
         lines.append(line)
 
     ctt_data = "\n".join(lines)
-    if encoding: ctt_data = ctt_data.encode(encoding)
+    if encoding:
+        ctt_data = ctt_data.encode(encoding)
 
     return ctt_data
```

### Comparing `omnix-0.3.1/src/omnix/util/format.py` & `omnix-0.3.3/src/omnix/util/format.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,74 +18,56 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import csv
 
 import quorum
 
+
 def csv_file(
-    file,
-    callback,
-    header = False,
-    delimiter = ",",
-    strict = False,
-    encoding = "utf-8"
+    file, callback, header=False, delimiter=",", strict=False, encoding="utf-8"
 ):
     _file_name, mime_type, data = file
     is_csv = mime_type in ("text/csv", "application/vnd.ms-excel")
     if not is_csv and strict:
         raise quorum.OperationalError("Invalid MIME type '%s'" % mime_type)
     data = data.decode(encoding)
     buffer = quorum.legacy.StringIO(data)
-    return csv_import(
-        buffer,
-        callback,
-        header = header,
-        delimiter = delimiter
-    )
+    return csv_import(buffer, callback, header=header, delimiter=delimiter)
+
 
 def csv_import(
-    buffer,
-    callback,
-    header = False,
-    delimiter = ",",
-    quoting = False,
-    encoding = "utf-8"
+    buffer, callback, header=False, delimiter=",", quoting=False, encoding="utf-8"
 ):
     is_unicode = quorum.legacy.PYTHON_3
     if is_unicode:
         data = buffer.read()
         data = data.decode(encoding)
         buffer = quorum.legacy.StringIO(data)
     csv_reader = csv.reader(
         buffer,
-        delimiter = delimiter,
-        quoting = csv.QUOTE_MINIMAL if quoting else csv.QUOTE_NONE
+        delimiter=delimiter,
+        quoting=csv.QUOTE_MINIMAL if quoting else csv.QUOTE_NONE,
     )
-    if header: _header = next(csv_reader)
-    else: _header = []
+    if header:
+        _header = next(csv_reader)
+    else:
+        _header = []
     for line in csv_reader:
-        if not is_unicode: line = [value.decode(encoding) for value in line]
-        callback(line, header = _header)
+        if not is_unicode:
+            line = [value.decode(encoding) for value in line]
+        callback(line, header=_header)
+
 
 def csv_value(name, line, header):
     values = zip(line, header)
     return values[name]
```

### Comparing `omnix-0.3.1/src/omnix/util/config.py` & `omnix-0.3.3/src/omnix/util/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import quorum
@@ -106,58 +97,49 @@
     "documents.signed_document.list",
     "documents.signed_document.submit_invoice_at",
     "analytics.sale_snapshot.list",
     "analytics.employee_snapshot.list",
     "inventory.stock_adjustment.create",
     "inventory.transfer.create",
     "inventory.transactional_merchandise.list",
-    "inventory.transactional_merchandise.update"
+    "inventory.transactional_merchandise.update",
 )
 """ The list of permissions to be used to create the
 scope string for the OAuth value """
 
-AT_SALE_TYPES = (
-    "MoneySaleSlip",
-    "Invoice",
-    "CreditNote",
-    "DebitNote"
-)
+AT_SALE_TYPES = ("MoneySaleSlip", "Invoice", "CreditNote", "DebitNote")
 """ The list containing the complete set of types that
 are considered to be of type sake """
 
-AT_TRANSPORT_TYPES = (
-    "TransportationSlip",
-    "ExpeditionSlip"
-)
+AT_TRANSPORT_TYPES = ("TransportationSlip", "ExpeditionSlip")
 """ The list containing the complete set of types that
 are considered to be of type transport """
 
 AT_SUBMIT_TYPES = AT_SALE_TYPES + AT_TRANSPORT_TYPES
-""" The set of valid types for submission to at, note
+""" The set of valid types for submission to AT, note
 that this range of values should be changed with care """
 
-REMOTE = quorum.conf("REMOTE", False, cast = bool)
-REMOTE = quorum.conf("OMNIX_REMOTE", REMOTE, cast = bool)
+REMOTE = quorum.conf("REMOTE", False, cast=bool)
+REMOTE = quorum.conf("OMNIX_REMOTE", REMOTE, cast=bool)
 BASE_URL = quorum.conf("BASE_URL", "http://localhost:8181")
 REDIRECT_URL = quorum.conf("REDIRECT_URL", REDIRECT_URL)
 CLIENT_ID = quorum.conf("OMNIX_CLIENT_ID", CLIENT_ID)
 CLIENT_SECRET = quorum.conf("OMNIX_CLIENT_SECRET", CLIENT_SECRET)
 SENDER_EMAIL = quorum.conf("SENDER_EMAIL", "Omnix <no-reply@omnix.com>")
 USERNAME = quorum.conf("OMNIX_USERNAME", None)
 PASSWORD = quorum.conf("OMNIX_PASSWORD", None)
-SCHEDULE = quorum.conf("OMNIX_SCHEDULE", True, cast = bool)
-COMMISSION_RATE = quorum.conf("OMNIX_COMMISSION_RATE", 0.01, cast = float)
-COMMISSION_DAY = quorum.conf("OMNIX_COMMISSION_DAY", 26, cast = int)
+SCHEDULE = quorum.conf("OMNIX_SCHEDULE", True, cast=bool)
+COMMISSION_RATE = quorum.conf("OMNIX_COMMISSION_RATE", 0.01, cast=float)
+COMMISSION_DAY = quorum.conf("OMNIX_COMMISSION_DAY", 26, cast=int)
 IMAGE_RESIZE = quorum.conf("OMNIX_IMAGE_RESIZE", "crop")
 LOCALE = quorum.conf("OMNIX_LOCALE", "en_us")
 QUEUE = quorum.conf("OMNIX_QUEUE", "omnix")
-RECORD_CHUNK = quorum.conf("OMNIX_RECORD_CHUNK", 256, cast = int)
+RECORD_CHUNK = quorum.conf("OMNIX_RECORD_CHUNK", 256, cast=int)
 BIRTHDAY_TEMPLATE = quorum.conf(
-    "OMNIX_BIRTHDAY_TEMPLATE",
-    "email/birthday.%s.html.tpl" % LOCALE
+    "OMNIX_BIRTHDAY_TEMPLATE", "email/birthday.%s.html.tpl" % LOCALE
 )
 
 OMNI_URL = REMOTE_URL if REMOTE else LOCAL_URL
 PREFIX = REMOTE_PREFIX if REMOTE else LOCAL_PREFIX
 
 OMNI_URL = quorum.conf("OMNI_URL", OMNI_URL)
 PREFIX = quorum.conf("OMNI_PREFIX", PREFIX)
```

### Comparing `omnix-0.3.1/src/omnix/util/scheduling.py` & `omnix-0.3.3/src/omnix/util/scheduling.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import datetime
@@ -42,74 +33,83 @@
 import omni
 import quorum
 
 from . import logic
 from . import config
 from . import business
 
+
 def load():
-    if not config.SCHEDULE: return
+    if not config.SCHEDULE:
+        return
     quorum.debug("Loading scheduling tasks ...")
     load_slack()
     load_mail()
 
+
 def load_slack():
-    if not config.REMOTE: return
-    sales_time = quorum.daily_work(sales_slack, offset = 14400)
-    previous_time = quorum.daily_work(previous_slack, offset = 18000)
-    week_time = quorum.weekly_work(week_slack, weekday = 0, offset = 14400)
+    if not config.REMOTE:
+        return
+    sales_time = quorum.daily_work(sales_slack, offset=14400)
+    previous_time = quorum.daily_work(previous_slack, offset=18000)
+    week_time = quorum.weekly_work(week_slack, weekday=0, offset=14400)
     sales_date = datetime.datetime.utcfromtimestamp(sales_time)
     previous_date = datetime.datetime.utcfromtimestamp(previous_time)
     week_date = datetime.datetime.utcfromtimestamp(week_time)
     quorum.debug("Scheduled initial daily sales slack task for %s" % sales_date)
-    quorum.debug("Scheduled initial daily previous (sales) slack task for %s" % previous_date)
-    quorum.debug("Scheduled initial weekly previous week (sales) slack task for %s" % week_date)
+    quorum.debug(
+        "Scheduled initial daily previous (sales) slack task for %s" % previous_date
+    )
+    quorum.debug(
+        "Scheduled initial weekly previous week (sales) slack task for %s" % week_date
+    )
+
 
 def load_mail():
-    if not config.REMOTE: return
-    day_time = quorum.daily_work(birthday_mail, offset = 14400)
-    week_time = quorum.weekly_work(activity_mail, weekday = 4, offset = 14400)
-    month_time = quorum.monthly_work(activity_previous, monthday = 26, offset = 14400)
+    if not config.REMOTE:
+        return
+    day_time = quorum.daily_work(birthday_mail, offset=14400)
+    week_time = quorum.weekly_work(activity_mail, weekday=4, offset=14400)
+    month_time = quorum.monthly_work(activity_previous, monthday=26, offset=14400)
     day_date = datetime.datetime.utcfromtimestamp(day_time)
     week_date = datetime.datetime.utcfromtimestamp(week_time)
     month_date = datetime.datetime.utcfromtimestamp(month_time)
     quorum.debug("Scheduled initial daily birthday mail task for %s" % day_date)
     quorum.debug("Scheduled initial weekly activity mail task for %s" % week_date)
     quorum.debug("Scheduled initial monthly activity previous task for %s" % month_date)
 
-def sales_slack(offset = 1):
-    api = logic.get_api(mode = omni.API.DIRECT_MODE)
-    business.slack_sales(api = api, offset = offset)
-
-def previous_slack(offset = 0):
-    api = logic.get_api(mode = omni.API.DIRECT_MODE)
-    business.slack_previous(api = api, offset = offset)
-
-def week_slack(offset = 0, span = 7):
-    api = logic.get_api(mode = omni.API.DIRECT_MODE)
-    business.slack_week(api = api, offset = offset, span = span)
-
-def birthday_mail(month = None, day = None):
-    api = logic.get_api(mode = omni.API.DIRECT_MODE)
-    business.mail_birthday_all(
-        api = api,
-        month = month,
-        day = day,
-        links = False
-    )
+
+def sales_slack(offset=1):
+    api = logic.get_api(mode=omni.API.DIRECT_MODE)
+    business.slack_sales(api=api, offset=offset)
+
+
+def previous_slack(offset=0):
+    api = logic.get_api(mode=omni.API.DIRECT_MODE)
+    business.slack_previous(api=api, offset=offset)
+
+
+def week_slack(offset=0, span=7):
+    api = logic.get_api(mode=omni.API.DIRECT_MODE)
+    business.slack_week(api=api, offset=offset, span=span)
+
+
+def birthday_mail(month=None, day=None):
+    api = logic.get_api(mode=omni.API.DIRECT_MODE)
+    business.mail_birthday_all(api=api, month=month, day=day, links=False)
     quorum.debug("Finished sending birthday emails")
 
-def activity_mail(year = None, month = None):
-    api = logic.get_api(mode = omni.API.DIRECT_MODE)
+
+def activity_mail(year=None, month=None):
+    api = logic.get_api(mode=omni.API.DIRECT_MODE)
     business.mail_activity_all(
-        api = api,
-        year = year,
-        month = month,
-        validate = True,
-        links = False
+        api=api, year=year, month=month, validate=True, links=False
     )
     quorum.debug("Finished sending activity emails")
 
+
 def activity_previous():
     now = datetime.datetime.utcnow()
-    pre_year, pre_month = (now.year - 1, 12) if now.month == 1 else (now.year, now.month - 1)
-    activity_mail(year = pre_year, month = pre_month)
+    pre_year, pre_month = (
+        (now.year - 1, 12) if now.month == 1 else (now.year, now.month - 1)
+    )
+    activity_mail(year=pre_year, month=pre_month)
```

### Comparing `omnix-0.3.1/src/omnix/util/slave.py` & `omnix-0.3.3/src/omnix/util/slave.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
@@ -59,64 +50,67 @@
 considered out dated and is discarded from the
 queue even without processing """
 
 RETRY_TIMEOUT = 30
 """ The timeout to be used in between the retries
 of the operations, as expected """
 
+
 class Slave(threading.Thread):
 
     session_id = None
     connection = None
     channel = None
 
     def __init__(self):
         threading.Thread.__init__(self)
         self.daemon = True
 
     def stop(self):
         pass
 
     def auth(self):
-        if not config.REMOTE: return
+        if not config.REMOTE:
+            return
 
         username = config.USERNAME
         password = config.PASSWORD
         if username == None or password == None:
             raise RuntimeError("Missing authentication information")
 
-        self.api = logic.get_api(mode = omni.API.DIRECT_MODE)
+        self.api = logic.get_api(mode=omni.API.DIRECT_MODE)
 
-    def connect(self, queue = "default"):
-        if not config.REMOTE: return
+    def connect(self, queue="default"):
+        if not config.REMOTE:
+            return
 
         while True:
             try:
                 quorum.debug("Starting loop cycle in slave ...")
-                self.connection = quorum.get_amqp(force = True)
+                self.connection = quorum.get_amqp(force=True)
                 self.channel = self.connection.channel()
-                self.channel.queue_declare(queue = queue, durable = True)
-                self.channel.basic_qos(prefetch_count = 1)
+                self.channel.queue_declare(queue=queue, durable=True)
+                self.channel.basic_qos(prefetch_count=1)
                 self.channel.basic_consume(
-                    queue = queue,
-                    on_message_callback = self.callback
+                    queue=queue, on_message_callback=self.callback
                 )
                 self.channel.start_consuming()
             except Exception as exception:
                 quorum.error(
                     "Exception while executing - %s" % quorum.legacy.UNICODE(exception),
-                    log_trace = True
+                    log_trace=True,
                 )
 
             quorum.info("Sleeping %d seconds before consume retry" % RETRY_TIMEOUT)
 
             time.sleep(RETRY_TIMEOUT)
 
     def disconnect(self):
-        if not config.REMOTE: return
+        if not config.REMOTE:
+            return
 
     def callback(self, channel, method, properties, body):
         # prints a debug message about the callback call for the message, this
         # may be used latter for debugging purposes (as requested)
         quorum.debug("Received callback for message")
 
         # loads the contents of the body that is going to be submitted this
@@ -130,78 +124,77 @@
         representation = document["representation"]
         issue_date = document["issue_date"]
         issue_date_d = datetime.datetime.utcfromtimestamp(issue_date)
         issue_date_s = issue_date_d.strftime("%d %b %Y %H:%M:%S")
 
         # verifies if the document is considered to be outdated (timeout passed)
         # in case it's returns immediately printing a message
-        outdated = not properties.timestamp or\
-            properties.timestamp < time.time() - MESSAGE_TIMEOUT
+        outdated = (
+            not properties.timestamp
+            or properties.timestamp < time.time() - MESSAGE_TIMEOUT
+        )
         if outdated:
-            channel.basic_ack(delivery_tag = method.delivery_tag)
+            channel.basic_ack(delivery_tag=method.delivery_tag)
             quorum.info(
-                "Canceling/Dropping %s - %s (%s)" % (
-                    type,
-                    representation,
-                    issue_date_s
-                )
+                "Canceling/Dropping %s - %s (%s)" % (type, representation, issue_date_s)
             )
             return
 
         # retrieves the current time and uses it to print debug information
         # about the current document submission to at
-        quorum.info(
-            "Submitting %s - %s (%s)" % (
-                type,
-                representation,
-                issue_date_s
-            )
-        )
+        quorum.info("Submitting %s - %s (%s)" % (type, representation, issue_date_s))
 
         # resolves the method for the currently retrieved data type (class)
         # this should raise an exception in case the type is invalid
         api_method = self._resolve_method(type)
 
         try:
             # calls the proper method for the submission of the document
             # described by the provided object id, in case there's a problem
             # in the request an exception should be raised and handled properly
             api_method(object_id)
         except Exception as exception:
-            quorum.error("Exception while submitting document - %s" % quorum.legacy.UNICODE(exception))
+            quorum.error(
+                "Exception while submitting document - %s"
+                % quorum.legacy.UNICODE(exception)
+            )
             retries = properties.priority or 0
             retries -= 1
             properties.priority = retries
             if retries >= 0:
                 self.channel.basic_publish(
-                    exchange = "",
-                    routing_key = config.QUEUE,
-                    body = body,
-                    properties = properties
+                    exchange="",
+                    routing_key=config.QUEUE,
+                    body=body,
+                    properties=properties,
                 )
-                quorum.error("Re-queueing for latter consumption (%d retries pending)" % retries)
-            else: quorum.error("No more retries left, the document will be discarded")
+                quorum.error(
+                    "Re-queueing for latter consumption (%d retries pending)" % retries
+                )
+            else:
+                quorum.error("No more retries left, the document will be discarded")
         else:
             quorum.info("Document submitted with success")
 
         # marks the message as acknowledged in the message queue server
         # and then prints a debug message about the action
-        channel.basic_ack(delivery_tag = method.delivery_tag)
+        channel.basic_ack(delivery_tag=method.delivery_tag)
         quorum.debug("Marked as acknowledged in message queue")
 
     def run(self):
         self.auth()
-        self.connect(queue = config.QUEUE)
+        self.connect(queue=config.QUEUE)
         self.disconnect()
 
     def _resolve_method(self, type):
         if type in config.AT_SALE_TYPES:
             return self.api.submit_invoice_at
         elif type in config.AT_TRANSPORT_TYPES:
             return self.api.submit_transport_at
         else:
             raise RuntimeError("Invalid document type")
 
-def run(count = 1):
+
+def run(count=1):
     for _index in range(count):
         slave = Slave()
         slave.start()
```

### Comparing `omnix-0.3.1/src/omnix/util/logic.py` & `omnix-0.3.3/src/omnix/util/logic.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,90 +18,97 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import omni
 
 import flask
 
 import quorum
 
 from . import config
 
+
 def get_models():
     return omni.models
 
-def get_api(mode = omni.API.OAUTH_MODE):
+
+def get_api(mode=omni.API.OAUTH_MODE):
     access_token = flask.session and flask.session.get("omnix.access_token", None)
     session_id = flask.session and flask.session.get("omnix.session_id", None)
     api = omni.API(
-        base_url = config.OMNI_URL,
-        open_url = config.OMNI_URL,
-        prefix = config.PREFIX,
-        client_id = config.CLIENT_ID,
-        client_secret = config.CLIENT_SECRET,
-        redirect_url = config.REDIRECT_URL,
-        scope = config.SCOPE,
-        access_token = access_token,
-        session_id = session_id,
-        username = config.USERNAME,
-        password = config.PASSWORD,
-        mode = mode
+        base_url=config.OMNI_URL,
+        open_url=config.OMNI_URL,
+        prefix=config.PREFIX,
+        client_id=config.CLIENT_ID,
+        client_secret=config.CLIENT_SECRET,
+        redirect_url=config.REDIRECT_URL,
+        scope=config.SCOPE,
+        access_token=access_token,
+        session_id=session_id,
+        username=config.USERNAME,
+        password=config.PASSWORD,
+        mode=mode,
     )
     api.bind("auth", on_auth)
     return api
 
-def ensure_api(state = None):
+
+def ensure_api(state=None):
     access_token = flask.session.get("omnix.access_token", None)
-    if access_token: return
+    if access_token:
+        return
     api = get_api()
-    return api.oauth_authorize(state = state)
+    return api.oauth_authorize(state=state)
+
 
 def on_auth(contents):
     start_session(contents)
 
+
 def start_session(contents):
-    if not flask.session: return
+    if not flask.session:
+        return
 
     username = contents.get("username", None)
     acl = contents.get("acl", None)
     session_id = contents.get("session_id", None)
     tokens = get_tokens(acl)
 
     flask.session["omnix.base_url"] = config.OMNI_URL
     flask.session["omnix.username"] = username
     flask.session["omnix.acl"] = acl
     flask.session["omnix.session_id"] = session_id
     flask.session["tokens"] = tokens
 
+
 def reset_session():
-    if not flask.session: return
+    if not flask.session:
+        return
 
-    if "omnix.base_url" in flask.session: del flask.session["omnix.base_url"]
-    if "omnix.access_token" in flask.session: del flask.session["omnix.access_token"]
-    if "omnix.username" in flask.session: del flask.session["omnix.username"]
-    if "omnix.acl" in flask.session: del flask.session["omnix.acl"]
-    if "omnix.session_id" in flask.session: del flask.session["omnix.session_id"]
-    if "tokens" in flask.session: del flask.session["tokens"]
+    if "omnix.base_url" in flask.session:
+        del flask.session["omnix.base_url"]
+    if "omnix.access_token" in flask.session:
+        del flask.session["omnix.access_token"]
+    if "omnix.username" in flask.session:
+        del flask.session["omnix.username"]
+    if "omnix.acl" in flask.session:
+        del flask.session["omnix.acl"]
+    if "omnix.session_id" in flask.session:
+        del flask.session["omnix.session_id"]
+    if "tokens" in flask.session:
+        del flask.session["tokens"]
     flask.session.modified = True
 
+
 def get_tokens(acl):
     tokens = acl.keys()
     return quorum.legacy.eager(tokens)
```

### Comparing `omnix-0.3.1/src/omnix/util/business.py` & `omnix-0.3.3/src/omnix/util/business.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import time
@@ -43,78 +34,67 @@
 
 import flask
 import quorum
 
 from . import logic
 from . import config
 
-BIRTHDAY_SUBJECT = dict(
-    en_us = "Happy Birthday",
-    pt_pt = "Feliz Aniversário"
-)
+BIRTHDAY_SUBJECT = dict(en_us="Happy Birthday", pt_pt="Feliz Aniversário")
 
 ACTIVITY_SUBJECT = dict(
-    en_us = "Omni activity report for %s as of %s",
-    pt_pt = "Relatório de atividade Omni para %s em %s"
+    en_us="Omni activity report for %s as of %s",
+    pt_pt="Relatório de atividade Omni para %s em %s",
 )
 
+
 @quorum.ensure_context
-def slack_sales(api = None, channel = None, all = False, offset = 0):
+def slack_sales(api=None, channel=None, all=False, offset=0):
     from omnix import models
 
     # tries to retrieve the reference to the API object
     # and if it fails returns immediately (soft fail)
     api = api or logic.get_api()
     settings = models.Settings.get_settings()
     slack_api = settings.get_slack_api()
-    if not slack_api: return
+    if not slack_api:
+        return
 
     # retrieves the current time and updates it with the delta
     # converting then the value to a string
     current = datetime.datetime.utcfromtimestamp(time.time())
-    delta = datetime.timedelta(days = offset)
+    delta = datetime.timedelta(days=offset)
     target = current - delta
     date_s = target.strftime("%d of %B")
 
     # calculates both the day and the month (time) reference values
     # to be used in the calculus of the comparison values, notice
     # that the day is positioned at the offset value in the month
     # and the month one is positioned at the beginning of the month
     # considered to be of reference (previous n months calculus)
     day_ref = target
-    month_ref = target - datetime.timedelta(days = target.day)
+    month_ref = target - datetime.timedelta(days=target.day)
     day_ref_t = calendar.timegm(day_ref.utctimetuple())
     month_ref_t = calendar.timegm(month_ref.utctimetuple())
 
     # retrieves the complete set of sales according to the
     # default value and then sorts the received object identifiers
     # according to their names and in case the
     contents = api.stats_sales(
-        date = time.time() - offset * 86400,
-        unit = "day",
-        span = 1,
-        has_global = True
+        date=time.time() - offset * 86400, unit="day", span=1, has_global=True
     )
     object_ids = quorum.legacy.keys(contents)
     object_ids.sort()
-    if not all: object_ids = ["-1"]
+    if not all:
+        object_ids = ["-1"]
 
     # retrieves the comparison values from both the day level and
     # the month level, so that it's possible to compare both the
     # current month and the current year against the previous ones
-    day_comparison = get_comparison(
-        api = api,
-        unit = "day",
-        timestamp = day_ref_t
-    )
-    month_comparison = get_comparison(
-        api = api,
-        unit = "month",
-        timestamp = month_ref_t
-    )
+    day_comparison = get_comparison(api=api, unit="day", timestamp=day_ref_t)
+    month_comparison = get_comparison(api=api, unit="month", timestamp=month_ref_t)
 
     # in case the month in calculus is the first one then an empty
     # result is going to be forced as this is the case for the
     # first month of the year (only day comparison is relevant)
     if target.month == 1:
         month_comparison = empty_results(month_comparison)
 
@@ -131,617 +111,626 @@
 
     # iterates over the complete set of "stores" to try to find
     # the one to be considered the best selling one and creates
     # the best value string for it
     for object_id, values in quorum.legacy.iteritems(contents):
         store_name = values["name"]
         store_net_price_vat = values["net_price_vat"][-1]
-        if not store_net_price_vat > value: continue
-        if object_id == "-1": continue
+        if not store_net_price_vat > value:
+            continue
+        if object_id == "-1":
+            continue
         value = store_net_price_vat
         best_value = "<%s|%s>" % (
-            flask.url_for("sales_stores", id = object_id, _external = True),
-            store_name
+            flask.url_for("sales_stores", id=object_id, _external=True),
+            store_name,
         )
 
     # iterates over the complete set of object identifiers for which
     # a message is meant to be displayed and sends it using Slack API
     for object_id in object_ids:
         values = contents[object_id]
         name = values["name"]
         name = name.capitalize()
         text = "Sales report for %s" % date_s
         values = dict(
-            number_entries = values["number_entries"][-1],
-            net_price_vat = values["net_price_vat"][-1],
-            net_average_sale = values["net_price_vat"][-1] / (values["net_number_sales"][-1] or 1.0),
-            net_number_sales = values["net_number_sales"][-1]
+            number_entries=values["number_entries"][-1],
+            net_price_vat=values["net_price_vat"][-1],
+            net_average_sale=values["net_price_vat"][-1]
+            / (values["net_number_sales"][-1] or 1.0),
+            net_number_sales=values["net_number_sales"][-1],
         )
         slack_api.post_message_chat(
             channel or settings.slack_channel or "general",
             None,
-            attachments = [
+            attachments=[
                 dict(
-                    fallback = text,
-                    color = "#36a64f",
-                    title = text,
-                    title_link = flask.url_for("sales_stores", id = object_id, _external = True),
-                    test = text,
-                    mrkdwn_in = ["text", "pretext", "fields"],
-                    fields = [
+                    fallback=text,
+                    color="#36a64f",
+                    title=text,
+                    title_link=flask.url_for(
+                        "sales_stores", id=object_id, _external=True
+                    ),
+                    test=text,
+                    mrkdwn_in=["text", "pretext", "fields"],
+                    fields=[
                         dict(
-                            title = "Store Name",
-                            value = "<%s|%s>" % (
-                                flask.url_for("sales_stores", id = object_id, _external = True),
-                                name
+                            title="Store Name",
+                            value="<%s|%s>"
+                            % (
+                                flask.url_for(
+                                    "sales_stores", id=object_id, _external=True
+                                ),
+                                name,
                             ),
-                            short = True
+                            short=True,
                         ),
+                        dict(title="Best Store", value=best_value, short=True),
                         dict(
-                            title = "Best Store",
-                            value = best_value,
-                            short = True
+                            title="Number Entries",
+                            value="%d x" % values["number_entries"],
+                            short=True,
                         ),
                         dict(
-                            title = "Number Entries",
-                            value = "%d x" % values["number_entries"],
-                            short = True
+                            title="Number Sales",
+                            value="%d x" % values["net_number_sales"],
+                            short=True,
                         ),
                         dict(
-                            title = "Number Sales",
-                            value = "%d x" % values["net_number_sales"],
-                            short = True
+                            title="Average Sale",
+                            value="%.2f EUR" % values["net_average_sale"],
+                            short=True,
                         ),
                         dict(
-                            title = "Average Sale",
-                            value = "%.2f EUR" % values["net_average_sale"],
-                            short = True
+                            title="Total Sales",
+                            value="*%.2f EUR*" % values["net_price_vat"],
+                            short=True,
+                            mrkdwn=True,
                         ),
-                        dict(
-                            title = "Total Sales",
-                            value = "*%.2f EUR*" % values["net_price_vat"],
-                            short = True,
-                            mrkdwn = True
-                        )
-                    ]
+                    ],
                 )
-            ]
+            ],
         )
 
         reports = (
             dict(
-                text = "Month to date report for %s" % date_s,
-                comparison = day_comparison
+                text="Month to date report for %s" % date_s, comparison=day_comparison
             ),
             dict(
-                text = "Year to date report for %s" % date_s,
-                comparison = month_comparison
-            )
+                text="Year to date report for %s" % date_s, comparison=month_comparison
+            ),
         )
 
         for report in reports:
             text, comparison = report["text"], report["comparison"]
             slack_api.post_message_chat(
                 channel or settings.slack_channel or "general",
                 None,
-                attachments = [
+                attachments=[
                     dict(
-                        fallback = text,
-                        color = "#36a64f",
-                        title = text,
-                        title_link = flask.url_for("sales_stores", id = object_id, _external = True),
-                        test = text,
-                        mrkdwn_in = ["text", "pretext", "fields"],
-                        fields = [
+                        fallback=text,
+                        color="#36a64f",
+                        title=text,
+                        title_link=flask.url_for(
+                            "sales_stores", id=object_id, _external=True
+                        ),
+                        test=text,
+                        mrkdwn_in=["text", "pretext", "fields"],
+                        fields=[
                             dict(
-                                title = "Store Name",
-                                value = "<%s|%s>" % (
-                                    flask.url_for("sales_stores", id = object_id, _external = True),
-                                    name
+                                title="Store Name",
+                                value="<%s|%s>"
+                                % (
+                                    flask.url_for(
+                                        "sales_stores", id=object_id, _external=True
+                                    ),
+                                    name,
                                 ),
-                                short = True
+                                short=True,
                             ),
                             dict(
-                                title = "Number Entries",
-                                value = "%d x / %+d x (%+.2f %%)" % (
+                                title="Number Entries",
+                                value="%d x / %+d x (%+.2f %%)"
+                                % (
                                     comparison[object_id]["number_entries"]["current"],
                                     comparison[object_id]["number_entries"]["diff"],
-                                    comparison[object_id]["number_entries"]["percentage"]
+                                    comparison[object_id]["number_entries"][
+                                        "percentage"
+                                    ],
                                 ),
-                                short = True
+                                short=True,
                             ),
                             dict(
-                                title = "Number Sales",
-                                value = "%d x / %+d x (%+.2f %%)" % (
-                                    comparison[object_id]["net_number_sales"]["current"],
+                                title="Number Sales",
+                                value="%d x / %+d x (%+.2f %%)"
+                                % (
+                                    comparison[object_id]["net_number_sales"][
+                                        "current"
+                                    ],
                                     comparison[object_id]["net_number_sales"]["diff"],
-                                    comparison[object_id]["net_number_sales"]["percentage"]
+                                    comparison[object_id]["net_number_sales"][
+                                        "percentage"
+                                    ],
                                 ),
-                                short = True
+                                short=True,
                             ),
                             dict(
-                                title = "Average Sale",
-                                value = "%.2f EUR / %+.2f EUR (%+.2f %%)" % (
-                                    comparison[object_id]["net_average_sale"]["current"],
+                                title="Average Sale",
+                                value="%.2f EUR / %+.2f EUR (%+.2f %%)"
+                                % (
+                                    comparison[object_id]["net_average_sale"][
+                                        "current"
+                                    ],
                                     comparison[object_id]["net_average_sale"]["diff"],
-                                    comparison[object_id]["net_average_sale"]["percentage"]
+                                    comparison[object_id]["net_average_sale"][
+                                        "percentage"
+                                    ],
                                 ),
-                                short = True
+                                short=True,
                             ),
                             dict(
-                                title = "Total Sales",
-                                value = "*%.2f EUR / %+.2f EUR (%+.2f %%)*" % (
+                                title="Total Sales",
+                                value="*%.2f EUR / %+.2f EUR (%+.2f %%)*"
+                                % (
                                     comparison[object_id]["net_price_vat"]["current"],
                                     comparison[object_id]["net_price_vat"]["diff"],
-                                    comparison[object_id]["net_price_vat"]["percentage"]
+                                    comparison[object_id]["net_price_vat"][
+                                        "percentage"
+                                    ],
                                 ),
-                                short = False,
-                                mrkdwn = True
-                            )
-                        ]
+                                short=False,
+                                mrkdwn=True,
+                            ),
+                        ],
                     )
-                ]
+                ],
             )
 
+
 @quorum.ensure_context
-def slack_previous(api = None, channel = None, all = False, offset = 0):
+def slack_previous(api=None, channel=None, all=False, offset=0):
     from omnix import models
 
     # tries to retrieve the reference to the API object
     # and if it fails returns immediately (soft fail)
     api = api or logic.get_api()
     settings = models.Settings.get_settings()
     slack_api = settings.get_slack_api()
-    if not slack_api: return
+    if not slack_api:
+        return
 
     current = datetime.datetime.utcfromtimestamp(time.time())
     previous = datetime.datetime(
         current.year - 1,
         current.month,
         current.day,
-        hour = current.hour,
-        minute = current.minute,
-        second = current.second
+        hour=current.hour,
+        minute=current.minute,
+        second=current.second,
     )
     previous_t = previous.utctimetuple()
     previous_t = calendar.timegm(previous_t)
 
     contents = api.stats_sales(
-        date = previous_t - offset * 86400,
-        unit = "day",
-        span = 1,
-        has_global = True
+        date=previous_t - offset * 86400, unit="day", span=1, has_global=True
     )
 
     # starts both the best (sales) value and the numeric value
     # for this same best value, these values should start with
     # the lower possible values (to be overriden)
     best_value, value = None, -1.0
 
     # iterates over the complete set of "stores" to try to find
     # the one to be considered the best selling one and creates
     # the best value string for it
     for object_id, values in quorum.legacy.iteritems(contents):
         store_name = values["name"]
         store_net_price_vat = values["net_price_vat"][-1]
-        if not store_net_price_vat > value: continue
-        if object_id == "-1": continue
+        if not store_net_price_vat > value:
+            continue
+        if object_id == "-1":
+            continue
         value = store_net_price_vat
         best_value = "<%s|%s>" % (
-            flask.url_for("sales_stores", id = object_id, _external = True),
-            store_name
+            flask.url_for("sales_stores", id=object_id, _external=True),
+            store_name,
         )
 
     # unpacks the contents of the API call and creates some of the
     # global values to be used in the Slack message creation
     values = contents["-1"]
     name = values["name"]
     name = name.capitalize()
     text = "Previous period sales for %s" % previous.strftime("%d, %B of %Y")
 
     values = dict(
-        number_entries = values["number_entries"][-1],
-        net_price_vat = values["net_price_vat"][-1],
-        net_average_sale = values["net_price_vat"][-1] / (values["net_number_sales"][-1] or 1.0),
-        net_number_sales = values["net_number_sales"][-1]
+        number_entries=values["number_entries"][-1],
+        net_price_vat=values["net_price_vat"][-1],
+        net_average_sale=values["net_price_vat"][-1]
+        / (values["net_number_sales"][-1] or 1.0),
+        net_number_sales=values["net_number_sales"][-1],
     )
 
     slack_api.post_message_chat(
         channel or settings.slack_channel or "general",
         None,
-        attachments = [
+        attachments=[
             dict(
-                fallback = text,
-                color = "#36a64f",
-                title = text,
-                title_link = flask.url_for("sales_stores", id = object_id, _external = True),
-                test = text,
-                mrkdwn_in = ["text", "pretext", "fields"],
-                fields = [
+                fallback=text,
+                color="#36a64f",
+                title=text,
+                title_link=flask.url_for("sales_stores", id=object_id, _external=True),
+                test=text,
+                mrkdwn_in=["text", "pretext", "fields"],
+                fields=[
                     dict(
-                        title = "Store Name",
-                        value = "<%s|%s>" % (
-                            flask.url_for("sales_stores", id = object_id, _external = True),
-                            name
+                        title="Store Name",
+                        value="<%s|%s>"
+                        % (
+                            flask.url_for("sales_stores", id=object_id, _external=True),
+                            name,
                         ),
-                        short = True
+                        short=True,
                     ),
+                    dict(title="Best Store", value=best_value, short=True),
                     dict(
-                        title = "Best Store",
-                        value = best_value,
-                        short = True
+                        title="Number Entries",
+                        value="%d x" % values["number_entries"],
+                        short=True,
                     ),
                     dict(
-                        title = "Number Entries",
-                        value = "%d x" % values["number_entries"],
-                        short = True
+                        title="Number Sales",
+                        value="%d x" % values["net_number_sales"],
+                        short=True,
                     ),
                     dict(
-                        title = "Number Sales",
-                        value = "%d x" % values["net_number_sales"],
-                        short = True
+                        title="Average Sale",
+                        value="%.2f EUR" % values["net_average_sale"],
+                        short=True,
                     ),
                     dict(
-                        title = "Average Sale",
-                        value = "%.2f EUR" % values["net_average_sale"],
-                        short = True
+                        title="Total Sales",
+                        value="*%.2f EUR*" % values["net_price_vat"],
+                        short=True,
+                        mrkdwn=True,
                     ),
-                    dict(
-                        title = "Total Sales",
-                        value = "*%.2f EUR*" % values["net_price_vat"],
-                        short = True,
-                        mrkdwn = True
-                    )
-                ]
+                ],
             )
-        ]
+        ],
     )
 
+
 @quorum.ensure_context
-def slack_week(api = None, channel = None, all = False, offset = 0, span = 7):
+def slack_week(api=None, channel=None, all=False, offset=0, span=7):
     from omnix import models
 
     # tries to retrieve the reference to the API object
     # and if it fails returns immediately (soft fail)
     api = api or logic.get_api()
     settings = models.Settings.get_settings()
     slack_api = settings.get_slack_api()
-    if not slack_api: return
+    if not slack_api:
+        return
 
     current = datetime.datetime.utcfromtimestamp(time.time())
     previous = datetime.datetime(
         current.year - 1,
         current.month,
         current.day,
-        hour = current.hour,
-        minute = current.minute,
-        second = current.second
+        hour=current.hour,
+        minute=current.minute,
+        second=current.second,
     )
     previous_t = previous.utctimetuple()
     previous_t = calendar.timegm(previous_t)
 
     contents = api.stats_sales(
-        date = previous_t + (span - offset - 1) * 86400,
-        unit = "day",
-        span = span,
-        has_global = True
+        date=previous_t + (span - offset - 1) * 86400,
+        unit="day",
+        span=span,
+        has_global=True,
     )
 
     values = contents["-1"]
     name = values["name"]
     name = name.capitalize()
     text = "Weekly sales for %d" % previous.year
 
     fields = []
     curent_t = previous_t - offset * 86400
 
-    for amount, number_sales in zip(values["net_price_vat"], values["net_number_sales"]):
+    for amount, number_sales in zip(
+        values["net_price_vat"], values["net_number_sales"]
+    ):
         fields.append(
             dict(
-                title = "Sales for %s" % (datetime.datetime.utcfromtimestamp(curent_t).strftime("%d of %B")),
-                value = "%.2f EUR (%d x)" % (amount, number_sales),
-                short = False,
-                mrkdwn = True
+                title="Sales for %s"
+                % (datetime.datetime.utcfromtimestamp(curent_t).strftime("%d of %B")),
+                value="%.2f EUR (%d x)" % (amount, number_sales),
+                short=False,
+                mrkdwn=True,
             )
         )
         curent_t += 86400
 
     slack_api.post_message_chat(
         channel or settings.slack_channel or "general",
         None,
-        attachments = [
+        attachments=[
             dict(
-                fallback = text,
-                color = "#36a64f",
-                title = text,
-                test = text,
-                mrkdwn_in = ["text", "pretext", "fields"],
-                fields = fields
+                fallback=text,
+                color="#36a64f",
+                title=text,
+                test=text,
+                mrkdwn_in=["text", "pretext", "fields"],
+                fields=fields,
             )
-        ]
+        ],
     )
 
+
 @quorum.ensure_context
-def mail_birthday_all(
-    api = None,
-    month = None,
-    day = None,
-    validate = False,
-    links = True
-):
+def mail_birthday_all(api=None, month=None, day=None, validate=False, links=True):
     api = api or logic.get_api()
     has_date = month and day
     if not has_date:
         current = datetime.datetime.utcnow()
         month, day = current.month, current.day
     birth_day = "%02d/%02d" % (month, day)
     employees = api.list_employees(
-        object = dict(limit = -1),
-        **{
-            "filters[]" : [
-                "birth_day:equals:%s" % birth_day
-            ]
-        }
+        object=dict(limit=-1), **{"filters[]": ["birth_day:equals:%s" % birth_day]}
     )
     for employee in employees:
-        try: mail_birthday(
-            api = api,
-            id = employee["object_id"],
-            links = links
-        )
-        except quorum.OperationalError: pass
+        try:
+            mail_birthday(api=api, id=employee["object_id"], links=links)
+        except quorum.OperationalError:
+            pass
+
 
 @quorum.ensure_context
-def mail_activity_all(
-    api = None,
-    year = None,
-    month = None,
-    validate = False,
-    links = True
-):
+def mail_activity_all(api=None, year=None, month=None, validate=False, links=True):
     api = api or logic.get_api()
-    employees = api.list_employees(object = dict(limit = -1))
+    employees = api.list_employees(object=dict(limit=-1))
     for employee in employees:
-        try: mail_activity(
-            api = api,
-            id = employee["object_id"],
-            year = year,
-            month = month,
-            validate = validate,
-            links = links
-        )
-        except quorum.OperationalError: pass
+        try:
+            mail_activity(
+                api=api,
+                id=employee["object_id"],
+                year=year,
+                month=month,
+                validate=validate,
+                links=links,
+            )
+        except quorum.OperationalError:
+            pass
+
 
 @quorum.ensure_context
-def mail_birthday(api = None, id = None, links = True):
+def mail_birthday(api=None, id=None, links=True):
     api = api or logic.get_api()
     employee = api.get_employee(id) if id else api.self_employee()
 
     name = employee.get("full_name", None)
     working = employee.get("working", None)
     contact_information = employee.get("primary_contact_information", {})
     email = contact_information.get("email", None)
 
-    if not name: raise quorum.OperationalError("No name defined")
-    if not email: raise quorum.OperationalError("No email defined")
-    if not working == 1: raise quorum.OperationalError("No longer working")
+    if not name:
+        raise quorum.OperationalError("No name defined")
+    if not email:
+        raise quorum.OperationalError("No email defined")
+    if not working == 1:
+        raise quorum.OperationalError("No longer working")
 
     quorum.debug("Sending birthday email to %s <%s>" % (name, email))
     quorum.send_mail(
-        subject = BIRTHDAY_SUBJECT[config.LOCALE],
-        sender = config.SENDER_EMAIL,
-        receivers = ["%s <%s>" % (name, email)],
-        rich = config.BIRTHDAY_TEMPLATE,
-        context = dict(
-            settings = dict(
-                logo = True,
-                links = links
-            ),
-            base_url = config.BASE_URL,
-            omnix_base_url = config.OMNI_URL,
-            commission_rate = config.COMMISSION_RATE
-        )
+        subject=BIRTHDAY_SUBJECT[config.LOCALE],
+        sender=config.SENDER_EMAIL,
+        receivers=["%s <%s>" % (name, email)],
+        rich=config.BIRTHDAY_TEMPLATE,
+        context=dict(
+            settings=dict(logo=True, links=links),
+            base_url=config.BASE_URL,
+            omnix_base_url=config.OMNI_URL,
+            commission_rate=config.COMMISSION_RATE,
+        ),
     )
 
+
 @quorum.ensure_context
-def mail_activity(
-    api = None,
-    id = None,
-    year = None,
-    month = None,
-    validate = False,
-    links = True
-):
+def mail_activity(api=None, id=None, year=None, month=None, validate=False, links=True):
     api = api or logic.get_api()
     employee = api.get_employee(id) if id else api.self_employee()
 
     name = employee.get("full_name", None)
     working = employee.get("working", None)
     contact_information = employee.get("primary_contact_information", {})
     email = contact_information.get("email", None)
 
-    if not name: raise quorum.OperationalError("No name defined")
-    if not email: raise quorum.OperationalError("No email defined")
-    if not working == 1: raise quorum.OperationalError("No longer working")
+    if not name:
+        raise quorum.OperationalError("No name defined")
+    if not email:
+        raise quorum.OperationalError("No email defined")
+    if not working == 1:
+        raise quorum.OperationalError("No longer working")
 
     now = datetime.datetime.utcnow()
     now_s = now.strftime("%B %d %Y")
 
-    operations,\
-    target_s,\
-    sales_total,\
-    sales_s,\
-    returns_s,\
-    _previous_month,\
-    _previous_year,\
-    _next_month,\
-    _next_year,\
-    _has_next = get_sales(api = api, id = id, year = year, month = month)
+    (
+        operations,
+        target_s,
+        sales_total,
+        sales_s,
+        returns_s,
+        _previous_month,
+        _previous_year,
+        _next_month,
+        _next_year,
+        _has_next,
+    ) = get_sales(api=api, id=id, year=year, month=month)
 
-    if validate and not operations: return
+    if validate and not operations:
+        return
 
     quorum.debug("Sending activity email to %s <%s>" % (name, email))
     quorum.send_mail(
-        subject = ACTIVITY_SUBJECT[config.LOCALE] % (target_s, now_s),
-        sender = config.SENDER_EMAIL,
-        receivers = ["%s <%s>" % (name, email)],
-        rich = "email/activity.%s.html.tpl" % config.LOCALE,
-        context = dict(
-            settings = dict(
-                logo = True,
-                links = links
-            ),
-            target = target_s,
-            operations = operations,
-            sales_total = sales_total,
-            sales_count = len(sales_s),
-            returns_count = len(returns_s),
-            base_url = config.BASE_URL,
-            omnix_base_url = config.OMNI_URL,
-            commission_rate = config.COMMISSION_RATE
-        )
+        subject=ACTIVITY_SUBJECT[config.LOCALE] % (target_s, now_s),
+        sender=config.SENDER_EMAIL,
+        receivers=["%s <%s>" % (name, email)],
+        rich="email/activity.%s.html.tpl" % config.LOCALE,
+        context=dict(
+            settings=dict(logo=True, links=links),
+            target=target_s,
+            operations=operations,
+            sales_total=sales_total,
+            sales_count=len(sales_s),
+            returns_count=len(returns_s),
+            base_url=config.BASE_URL,
+            omnix_base_url=config.OMNI_URL,
+            commission_rate=config.COMMISSION_RATE,
+        ),
     )
 
-def get_date(year = None, month = None, pivot = config.FIRST_DAY):
+
+def get_date(year=None, month=None, pivot=config.FIRST_DAY):
     now = datetime.datetime.utcnow()
     year = year or now.year
     month = month or now.month
 
     has_next = int("%04d%02d" % (year, month)) < int("%04d%02d" % (now.year, now.month))
 
-    previous_month, previous_year = (month - 1, year) if not month == 1 else (12, year - 1)
+    previous_month, previous_year = (
+        (month - 1, year) if not month == 1 else (12, year - 1)
+    )
     next_month, next_year = (month + 1, year) if not month == 12 else (1, year + 1)
 
-    start_month, start_year = (month, year) if now.day >= pivot else (previous_month, previous_year)
-    if pivot == config.FIRST_DAY: end_month, end_year = start_month, start_year
-    else: end_month, end_year = (start_month + 1, start_year) if not start_month == 12 else (1, start_year + 1)
-
-    start = datetime.datetime(
-        year = start_year,
-        month = start_month,
-        day = pivot
-    )
-    end = datetime.datetime(
-        year = end_year,
-        month = end_month,
-        day = pivot
+    start_month, start_year = (
+        (month, year) if now.day >= pivot else (previous_month, previous_year)
     )
+    if pivot == config.FIRST_DAY:
+        end_month, end_year = start_month, start_year
+    else:
+        end_month, end_year = (
+            (start_month + 1, start_year)
+            if not start_month == 12
+            else (1, start_year + 1)
+        )
+
+    start = datetime.datetime(year=start_year, month=start_month, day=pivot)
+    end = datetime.datetime(year=end_year, month=end_month, day=pivot)
 
     start_t = calendar.timegm(start.utctimetuple())
     end_t = calendar.timegm(end.utctimetuple())
 
-    target = datetime.datetime(year = end_year, month = end_month, day = 1)
+    target = datetime.datetime(year=end_year, month=end_month, day=1)
     target = target.strftime("%B %Y")
 
     return (
         target,
         month,
         year,
         start_t,
         end_t,
         previous_month,
         previous_year,
         next_month,
         next_year,
-        has_next
+        has_next,
     )
 
-def get_top(api = None, year = None, month = None):
+
+def get_top(api=None, year=None, month=None):
     api = api or logic.get_api()
 
-    target, \
-    month, \
-    year, \
-    start_t, \
-    _end_t, \
-    previous_month, \
-    previous_year, \
-    next_month, \
-    next_year, \
-    has_next = get_date(year = year, month = month)
-
-    stats = api.stats_employee(
-        date = start_t,
-        unit = "month",
-        span = 1,
-        has_global = True
-    )
+    (
+        target,
+        month,
+        year,
+        start_t,
+        _end_t,
+        previous_month,
+        previous_year,
+        next_month,
+        next_year,
+        has_next,
+    ) = get_date(year=year, month=month)
+
+    stats = api.stats_employee(date=start_t, unit="month", span=1, has_global=True)
 
     top_employees = []
     for object_id, values in stats.items():
         values = values["-1"]
         values["object_id"] = object_id
         values["amount_price_vat"] = values["amount_price_vat"][0]
         values["number_sales"] = values["number_sales"][0]
         top_employees.append(values)
 
-    top_employees.sort(
-        reverse = True,
-        key = lambda value: value["amount_price_vat"]
-    )
+    top_employees.sort(reverse=True, key=lambda value: value["amount_price_vat"])
 
     return (
         top_employees,
         target,
         previous_month,
         previous_year,
         next_month,
         next_year,
-        has_next
+        has_next,
     )
 
-def get_sales(api = None, id = None, year = None, month = None):
+
+def get_sales(api=None, id=None, year=None, month=None):
     api = api or logic.get_api()
 
-    target, \
-    month, \
-    year, \
-    start_t, \
-    end_t, \
-    previous_month, \
-    previous_year, \
-    next_month, \
-    next_year, \
-    has_next = get_date(year = year, month = month, pivot = config.COMMISSION_DAY)
+    (
+        target,
+        month,
+        year,
+        start_t,
+        end_t,
+        previous_month,
+        previous_year,
+        next_month,
+        next_year,
+        has_next,
+    ) = get_date(year=year, month=month, pivot=config.COMMISSION_DAY)
 
     kwargs = {
-        "filter_string" : "",
-        "start_record" : 0,
-        "number_records" : -1,
-        "sort" : "date:descending",
-        "filters[]" : [
-            "date:greater:" + str(start_t),
-            "date:lesser:" + str(end_t)
-        ]
+        "filter_string": "",
+        "start_record": 0,
+        "number_records": -1,
+        "sort": "date:descending",
+        "filters[]": ["date:greater:" + str(start_t), "date:lesser:" + str(end_t)],
     }
-    if id: kwargs["filters[]"].append("primary_seller:equals:" + str(id))
+    if id:
+        kwargs["filters[]"].append("primary_seller:equals:" + str(id))
     sales = api.list_sales(**kwargs) if id else api.self_sales(**kwargs)
 
     kwargs = {
-        "filter_string" : "",
-        "start_record" : 0,
-        "number_records" : -1,
-        "sort" : "date:descending",
-        "filters[]" : [
-            "date:greater:" + str(start_t),
-            "date:lesser:" + str(end_t)
-        ]
+        "filter_string": "",
+        "start_record": 0,
+        "number_records": -1,
+        "sort": "date:descending",
+        "filters[]": ["date:greater:" + str(start_t), "date:lesser:" + str(end_t)],
     }
 
-    if id: kwargs["filters[]"].append("primary_return_processor:equals:" + str(id))
+    if id:
+        kwargs["filters[]"].append("primary_return_processor:equals:" + str(id))
     returns = api.list_returns(**kwargs) if id else api.self_returns(**kwargs)
 
     operations = returns + sales
 
     sorter = lambda item: item["date"]
-    operations.sort(key = sorter, reverse = True)
+    operations.sort(key=sorter, reverse=True)
 
     sales_total = 0
-    for sale in sales: sales_total += sale["price"]["value"]
-    for _return in returns: sales_total -= _return["price"]["value"]
+    for sale in sales:
+        sales_total += sale["price"]["value"]
+    for _return in returns:
+        sales_total -= _return["price"]["value"]
 
     for operation in operations:
         date = operation["date"]
         date_t = datetime.datetime.utcfromtimestamp(date)
         operation["date_f"] = date_t.strftime("%b %d, %Y")
 
     return (
@@ -750,33 +739,33 @@
         sales_total,
         sales,
         returns,
         previous_month,
         previous_year,
         next_month,
         next_year,
-        has_next
+        has_next,
     )
 
-def get_comparison(api = None, unit = "day", offset = 0, timestamp = None):
+
+def get_comparison(api=None, unit="day", offset=0, timestamp=None):
     from omnix import models
 
     # tries to retrieve the reference to the API object
     # and if it fails returns immediately (soft fail)
     api = api or logic.get_api()
     settings = models.Settings.get_settings()
     slack_api = settings.get_slack_api()
-    if not slack_api: return
+    if not slack_api:
+        return
 
     # retrieves both the current and the previous dictionary
     # set of arguments to be passed to the API requests
     current_args, previous_args = calc_comparison(
-        unit = unit,
-        offset = offset,
-        timestamp = timestamp
+        unit=unit, offset=offset, timestamp=timestamp
     )
 
     # retrieves both the current and the previous values so that
     # they can be properly compared, notice the proper span
     current_v = api.stats_sales(**current_args)
     previous_v = api.stats_sales(**previous_args)
 
@@ -785,40 +774,41 @@
     results = dict()
 
     for object_id in quorum.legacy.keys(current_v):
         current_i = current_v.get(object_id, {})
         previous_i = previous_v.get(object_id, {})
 
         result = dict(
-            number_entries = dict(
-                current = sum(current_i.get("number_entries", [])),
-                previous = sum(previous_i.get("number_entries", []))
+            number_entries=dict(
+                current=sum(current_i.get("number_entries", [])),
+                previous=sum(previous_i.get("number_entries", [])),
             ),
-            net_price_vat = dict(
-                current = sum(current_i.get("net_price_vat", [])),
-                previous = sum(previous_i.get("net_price_vat", []))
+            net_price_vat=dict(
+                current=sum(current_i.get("net_price_vat", [])),
+                previous=sum(previous_i.get("net_price_vat", [])),
+            ),
+            net_number_sales=dict(
+                current=sum(current_i.get("net_number_sales", [])),
+                previous=sum(previous_i.get("net_number_sales", [])),
             ),
-            net_number_sales = dict(
-                current = sum(current_i.get("net_number_sales", [])),
-                previous = sum(previous_i.get("net_number_sales", []))
-            )
         )
 
         # sets the current object identifier result in the map
         # of results (for latter usage)
         results[object_id] = result
 
     # runs the post-processing calculus operations on the results
     # so that the calculated attributes get correctly processed
     calc_extra(results)
     calc_results(results)
 
     return results
 
-def sum_results(first, second, calc = True):
+
+def sum_results(first, second, calc=True):
     """
     Sums the results of the first comparison dictionary
     with the second one.
 
     The function should return a dictionary compliant with
     the structure of the input ones.
 
@@ -858,15 +848,16 @@
 
     if calc:
         calc_extra(result)
         calc_results(result)
 
     return result
 
-def empty_results(input, calc = True):
+
+def empty_results(input, calc=True):
     """
     Generates an empty results dictionary taking as reference the
     input dictionary structure.
 
     The resulting dictionary should conform with the expected input
     specification.
 
@@ -899,93 +890,89 @@
 
     if calc:
         calc_extra(result)
         calc_results(result)
 
     return result
 
-def calc_comparison(unit = "day", offset = 0, timestamp = None):
+
+def calc_comparison(unit="day", offset=0, timestamp=None):
     # tries to retrieve the proper timestamp value falling back
     # to the current time in case nothing is provided
     timestamp = timestamp or time.time()
 
     # retrieves the current time and updates it with the delta
     # converting then the value to a string
     if unit == "day":
-        current = datetime.datetime.utcfromtimestamp(
-            timestamp + offset * 86400
-        )
+        current = datetime.datetime.utcfromtimestamp(timestamp + offset * 86400)
     if unit == "month":
-        now = datetime.datetime.utcfromtimestamp(
-            timestamp + offset * 86400
-        )
+        now = datetime.datetime.utcfromtimestamp(timestamp + offset * 86400)
         current = datetime.datetime(
             now.year,
             now.month,
             now.day,
-            hour = now.hour,
-            minute = now.minute,
-            second = now.second
+            hour=now.hour,
+            minute=now.minute,
+            second=now.second,
         )
     current_t = current.utctimetuple()
     current_t = calendar.timegm(current_t)
 
     try:
         # calculates the previous period timestamp by removing one
         # complete year from the current time
         previous = datetime.datetime(
             current.year - 1,
             current.month,
             current.day,
-            hour = current.hour,
-            minute = current.minute,
-            second = current.second
+            hour=current.hour,
+            minute=current.minute,
+            second=current.second,
         )
     except ValueError:
         # in case the value error assumes that's because of a leap
         # year invalid date range and decrements the day by one
         previous = datetime.datetime(
             current.year - 1,
             current.month,
             current.day - 1,
-            hour = current.hour,
-            minute = current.minute,
-            second = current.second
+            hour=current.hour,
+            minute=current.minute,
+            second=current.second,
         )
     previous_t = previous.utctimetuple()
     previous_t = calendar.timegm(previous_t)
 
     # tries to retrieve the proper span value according to the
     # requested unit of comparison
-    if unit == "day": span_c, span_p = current.day, previous.day
-    if unit == "month": span_c, span_p = current.month, previous.month
+    if unit == "day":
+        span_c, span_p = current.day, previous.day
+    if unit == "month":
+        span_c, span_p = current.month, previous.month
 
     # return a tuple containing both the current and previous values,
     # to be evaluated from the outside as expected, possible to be used
     # to pass then to a remote API request
-    return dict(
-        date = current_t,
-        unit = unit,
-        span = span_c,
-        has_global = True
-    ), dict(
-        date = previous_t,
-        unit = unit,
-        span = span_p,
-        has_global = True
+    return dict(date=current_t, unit=unit, span=span_c, has_global=True), dict(
+        date=previous_t, unit=unit, span=span_p, has_global=True
     )
 
+
 def calc_extra(results):
     for result in quorum.legacy.itervalues(results):
         result["net_average_sale"] = dict(
-            current = result["net_price_vat"]["current"] /\
-                (result["net_number_sales"]["current"] or 1.0),
-            previous = result["net_price_vat"]["previous"] /\
-                (result["net_number_sales"]["previous"] or 1.0)
+            current=result["net_price_vat"]["current"]
+            / (result["net_number_sales"]["current"] or 1.0),
+            previous=result["net_price_vat"]["previous"]
+            / (result["net_number_sales"]["previous"] or 1.0),
         )
 
+
 def calc_results(results):
     for result in quorum.legacy.itervalues(results):
         for values in quorum.legacy.itervalues(result):
             values["diff"] = values["current"] - values["previous"]
-            values["percentage"] = float(values["diff"]) /\
-                (float(values["previous"]) or float(values["diff"]) or 1.0) * 100.0
+            values["percentage"] = (
+                float(values["diff"])
+                / (float(values["previous"]) or float(values["diff"]) or 1.0)
+                * 100.0
+            )
```

### Comparing `omnix-0.3.1/src/omnix/main.py` & `omnix-0.3.3/src/omnix/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,60 +18,54 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-import flask #@UnusedImport
+import flask  # @UnusedImport
 import datetime
 
 import quorum
 
 import omnix.models
 
 MONGO_DATABASE = "omnix"
 """ The default database to be used for the connection with
 the MongoDB database """
 
 SECRET_KEY = "zhsga32ki5kvv7ymq8nolbleg248fzn1"
 """ The "secret" key to be at the internal encryption
 processes handled by flask (eg: sessions) """
 
+
 @quorum.onrun
 def onrun():
     import omnix.util
+
     omnix.util.run_slave(1)
     omnix.util.run_supervisor()
     omnix.util.load_scheduling()
 
+
 app = quorum.load(
-    name = __name__,
-    secret_key = SECRET_KEY,
-    mongo_database = MONGO_DATABASE,
-    logger = "omnix.debug",
-    models = omnix.models,
-    PERMANENT_SESSION_LIFETIME = datetime.timedelta(31),
-    MAX_CONTENT_LENGTH = 1024 ** 3
+    name=__name__,
+    secret_key=SECRET_KEY,
+    mongo_database=MONGO_DATABASE,
+    logger="omnix.debug",
+    models=omnix.models,
+    PERMANENT_SESSION_LIFETIME=datetime.timedelta(31),
+    MAX_CONTENT_LENGTH=1024**3,
 )
 
-import omnix.views #@UnusedImport
+import omnix.views  # @UnusedImport
 
 if __name__ == "__main__":
-    quorum.run(server = "netius")
+    quorum.run(server="netius")
 else:
     __path__ = []
```

### Comparing `omnix-0.3.1/src/omnix/views/api/base.py` & `omnix-0.3.3/src/omnix/views/api/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,36 +18,26 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from omnix.main import app
 from omnix.main import quorum
 
-@app.route("/api/log.json", methods = ("GET",), json = True)
-@quorum.ensure("base.admin", json = True)
+
+@app.route("/api/log.json", methods=("GET",), json=True)
+@quorum.ensure("base.admin", json=True)
 def log_api():
     memory_handler = quorum.get_handler("memory")
 
-    count = quorum.get_field("count", None, cast = int)
+    count = quorum.get_field("count", None, cast=int)
     level = quorum.get_field("level", None)
 
-    return dict(
-        messages = memory_handler.get_latest(count = count, level = level)
-    )
+    return dict(messages=memory_handler.get_latest(count=count, level=level))
```

### Comparing `omnix-0.3.1/src/omnix/views/api/__init__.py` & `omnix-0.3.3/src/omnix/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
-from . import base
-
-from .base import log_api
+from . import models
+from . import util
+from . import views
+from . import main
+
+from .models import *
+from .util import *
+from .views import *
+from .main import app
```

### Comparing `omnix-0.3.1/src/omnix/views/web/entity.py` & `omnix-0.3.3/src/omnix/views/web/entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,95 +18,89 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/entities", methods = ("GET",))
+
+@app.route("/entities", methods=("GET",))
 @quorum.ensure("foundation.root_entity.list")
 def list_entities():
-    return flask.render_template(
-        "entity/list.html.tpl",
-        link = "entities"
-    )
+    return flask.render_template("entity/list.html.tpl", link="entities")
+
 
-@app.route("/entities.json", methods = ("GET",), json = True)
+@app.route("/entities.json", methods=("GET",), json=True)
 @quorum.ensure("foundation.root_entity.list")
 def list_entities_json():
     api = util.get_api()
     object = quorum.get_object()
     return api.list_entities(**object)
 
-@app.route("/entities/<int:id>", methods = ("GET",))
+
+@app.route("/entities/<int:id>", methods=("GET",))
 @quorum.ensure("foundation.root_entity.show")
 def show_entities(id):
     api = util.get_api()
     entity = api.get_entity(id)
     metadata = entity.get("metadata", None)
     entity["metadata_s"] = _metadata_s(metadata)
     return flask.render_template(
-        "entity/show.html.tpl",
-        link = "entities",
-        sub_link = "info",
-        entity = entity
+        "entity/show.html.tpl", link="entities", sub_link="info", entity=entity
     )
 
-@app.route("/entities/<int:id>/edit", methods = ("GET",))
+
+@app.route("/entities/<int:id>/edit", methods=("GET",))
 @quorum.ensure("foundation.root_entity.update")
 def edit_entities(id):
     api = util.get_api()
     entity = api.get_entity(id)
     metadata = entity.get("metadata", None)
     entity["metadata_s"] = _metadata_s(metadata)
     return flask.render_template(
         "entity/edit.html.tpl",
-        link = "entities",
-        sub_link = "edit",
-        entity = entity,
-        errors = dict()
+        link="entities",
+        sub_link="edit",
+        entity=entity,
+        errors=dict(),
     )
 
-@app.route("/entities/<int:id>/update", methods = ("POST",))
+
+@app.route("/entities/<int:id>/update", methods=("POST",))
 @quorum.ensure("foundation.root_entity.update")
 def update_entities(id):
     models = util.get_models()
     api = util.get_api()
     object = quorum.get_object()
-    for name, value in object.items(): object[name] = None if value == "" else value
-    entity = models.Entity.new(model = object, build = False, fill = False)
-    api.update_entity(id, payload = dict(root_entity = entity.model))
-    return flask.redirect(
-        flask.url_for("show_entities", id = id)
-    )
+    for name, value in object.items():
+        object[name] = None if value == "" else value
+    entity = models.Entity.new(model=object, build=False, fill=False)
+    api.update_entity(id, payload=dict(root_entity=entity.model))
+    return flask.redirect(flask.url_for("show_entities", id=id))
+
 
 def _metadata_s(metadata):
-    return json.dumps(
-        metadata,
-        ensure_ascii = False,
-        indent = 4,
-        separators = (",", " : "),
-        sort_keys = True
-    ) if not metadata == None else None
+    return (
+        json.dumps(
+            metadata,
+            ensure_ascii=False,
+            indent=4,
+            separators=(",", " : "),
+            sort_keys=True,
+        )
+        if not metadata == None
+        else None
+    )
```

### Comparing `omnix-0.3.1/src/omnix/views/web/base.py` & `omnix-0.3.3/src/omnix/views/web/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import datetime
@@ -42,184 +33,154 @@
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/", methods = ("GET",))
-@app.route("/index", methods = ("GET",))
+
+@app.route("/", methods=("GET",))
+@app.route("/index", methods=("GET",))
 @quorum.ensure("base")
 def index():
-    return flask.render_template(
-        "index.html.tpl",
-        link = "home"
-    )
+    return flask.render_template("index.html.tpl", link="home")
+
 
-@app.route("/signin", methods = ("GET",))
+@app.route("/signin", methods=("GET",))
 def signin():
     next = quorum.get_field("next", None)
-    return flask.render_template(
-        "signin.html.tpl",
-        next = next
-    )
+    return flask.render_template("signin.html.tpl", next=next)
+
 
-@app.route("/signin", methods = ("POST",))
+@app.route("/signin", methods=("POST",))
 def login():
     next = quorum.get_field("next", None)
-    url = util.ensure_api(state = next)
-    if url: return flask.redirect(url)
-    return flask.redirect(
-        next or flask.url_for("index")
-    )
+    url = util.ensure_api(state=next)
+    if url:
+        return flask.redirect(url)
+    return flask.redirect(next or flask.url_for("index"))
+
 
-@app.route("/signin_do", methods = ("GET",))
+@app.route("/signin_do", methods=("GET",))
 def do_login():
     next = quorum.get_field("next", None)
-    url = util.ensure_api(state = next)
-    if url: return flask.redirect(url)
-    return flask.redirect(
-        next or flask.url_for("index")
-    )
+    url = util.ensure_api(state=next)
+    if url:
+        return flask.redirect(url)
+    return flask.redirect(next or flask.url_for("index"))
+
 
-@app.route("/logout", methods = ("GET",))
+@app.route("/logout", methods=("GET",))
 def logout():
     next = quorum.get_field("next", None)
     util.reset_session()
-    return flask.redirect(
-        next or flask.url_for("index")
-    )
+    return flask.redirect(next or flask.url_for("index"))
+
 
-@app.route("/about", methods = ("GET",))
+@app.route("/about", methods=("GET",))
 @quorum.ensure("base")
 def about():
     access_token = flask.session.get("omnix.access_token", None)
     session_id = flask.session.get("omnix.session_id", None)
 
     return flask.render_template(
-        "about.html.tpl",
-        link = "about",
-        access_token = access_token,
-        session_id = session_id
+        "about.html.tpl", link="about", access_token=access_token, session_id=session_id
     )
 
-@app.route("/reset", methods = ("GET",))
+
+@app.route("/reset", methods=("GET",))
 def reset():
     util.reset_session()
 
-    return flask.redirect(
-        flask.url_for("index")
-    )
+    return flask.redirect(flask.url_for("index"))
 
-@app.route("/flush_slack", methods = ("GET",))
-@app.route("/flush_slack_sales", methods = ("GET",))
+
+@app.route("/flush_slack", methods=("GET",))
+@app.route("/flush_slack_sales", methods=("GET",))
 @quorum.ensure("base.admin")
 def flush_slack_sales():
     channel = quorum.get_field("channel", None)
-    offset = quorum.get_field("offset", 0, cast = int)
+    offset = quorum.get_field("offset", 0, cast=int)
 
-    util.slack_sales(channel = channel, offset = offset)
+    util.slack_sales(channel=channel, offset=offset)
+
+    return flask.redirect(flask.url_for("index", message="Slack events have been sent"))
 
-    return flask.redirect(
-        flask.url_for(
-            "index",
-             message = "Slack events have been sent"
-        )
-    )
 
-@app.route("/flush_slack_previous", methods = ("GET",))
+@app.route("/flush_slack_previous", methods=("GET",))
 @quorum.ensure("base.admin")
 def flush_slack_previous():
     channel = quorum.get_field("channel", None)
-    offset = quorum.get_field("offset", 0, cast = int)
+    offset = quorum.get_field("offset", 0, cast=int)
 
-    util.slack_previous(channel = channel, offset = offset)
+    util.slack_previous(channel=channel, offset=offset)
 
-    return flask.redirect(
-        flask.url_for(
-            "index",
-             message = "Slack events have been sent"
-        )
-    )
+    return flask.redirect(flask.url_for("index", message="Slack events have been sent"))
 
 
-@app.route("/flush_slack_week", methods = ("GET",))
+@app.route("/flush_slack_week", methods=("GET",))
 @quorum.ensure("base.admin")
 def flush_slack_week():
     channel = quorum.get_field("channel", None)
-    offset = quorum.get_field("offset", 0, cast = int)
-    span = quorum.get_field("span", 7, cast = int)
+    offset = quorum.get_field("offset", 0, cast=int)
+    span = quorum.get_field("span", 7, cast=int)
 
-    util.slack_week(channel = channel, offset = offset, span = span)
+    util.slack_week(channel=channel, offset=offset, span=span)
+
+    return flask.redirect(flask.url_for("index", message="Slack events have been sent"))
 
-    return flask.redirect(
-        flask.url_for(
-            "index",
-             message = "Slack events have been sent"
-        )
-    )
 
-@app.route("/flush_birthday", methods = ("GET",))
+@app.route("/flush_birthday", methods=("GET",))
 @quorum.ensure("base.admin")
 def flush_birthday():
-    month = quorum.get_field("month", None, cast = int)
-    day = quorum.get_field("day", None, cast = int)
+    month = quorum.get_field("month", None, cast=int)
+    day = quorum.get_field("day", None, cast=int)
 
-    util.mail_birthday_all(
-        month = month,
-        day = day,
-        links = False
-    )
+    util.mail_birthday_all(month=month, day=day, links=False)
 
     return flask.redirect(
-        flask.url_for(
-            "index",
-            message = "Birthday emails have been sent"
-        )
+        flask.url_for("index", message="Birthday emails have been sent")
     )
 
-@app.route("/flush_activity", methods = ("GET",))
+
+@app.route("/flush_activity", methods=("GET",))
 @quorum.ensure("base.admin")
 def flush_activity():
-    util.mail_activity_all(
-        validate = True,
-        links = False
-    )
+    util.mail_activity_all(validate=True, links=False)
 
     return flask.redirect(
-        flask.url_for(
-            "index",
-            message = "Activity emails have been sent"
-        )
+        flask.url_for("index", message="Activity emails have been sent")
     )
 
-@app.route("/flush_at", methods = ("GET",))
+
+@app.route("/flush_at", methods=("GET",))
 @quorum.ensure("base.admin")
 def flush_at():
     # creates a values map structure to retrieve the complete
     # set of inbound documents that have not yet been submitted
     # to at for the flush operation
     kwargs = {
-        "filter_string" : "",
-        "start_record" : 0,
-        "number_records" : 1000,
-        "sort" : "issue_date:ascending",
-        "filters[]" : [
+        "filter_string": "",
+        "start_record": 0,
+        "number_records": 1000,
+        "sort": "issue_date:ascending",
+        "filters[]": [
             "issue_date:greater:1356998400",
             "submitted_at:equals:2",
-            "document_type:equals:3"
-        ]
+            "document_type:equals:3",
+        ],
     }
     api = util.get_api()
     documents = api.list_signed_documents(**kwargs)
 
     # filters the result set retrieved so that only the valid at
     # "submittable" documents are present in the sequence
-    valid_documents = [value for value in documents\
-        if value["_class"] in util.AT_SUBMIT_TYPES]
+    valid_documents = [
+        value for value in documents if value["_class"] in util.AT_SUBMIT_TYPES
+    ]
 
     # "calculates" the total set of valid documents present in the
     # valid documents and starts the index counter
     total = len(valid_documents)
     index = 1
 
     # iterates over the complete set of valid documents to be sent
@@ -231,45 +192,41 @@
         issue_date = document["issue_date"]
         issue_date_d = datetime.datetime.utcfromtimestamp(issue_date)
         issue_date_s = issue_date_d.strftime("%d %b %Y %H:%M:%S")
 
         # retrieves the current time and uses it to print debug information
         # about the current document submission to at
         quorum.info(
-            "Submitting %s - %s (%s) [%d/%d]" % (
-                type,
-                representation,
-                issue_date_s,
-                index,
-                total
-            )
+            "Submitting %s - %s (%s) [%d/%d]"
+            % (type, representation, issue_date_s, index, total)
         )
 
         try:
             # starts the submission process for the invoice, taking into
             # account that the document id to be submitted is the one that
             # has been extracted from the (signed) document structure
             api.submit_invoice_at(object_id)
         except Exception as exception:
-            quorum.error("Exception while submitting document - %s" % quorum.legacy.UNICODE(exception))
+            quorum.error(
+                "Exception while submitting document - %s"
+                % quorum.legacy.UNICODE(exception)
+            )
         else:
             quorum.info("Document submitted with success")
 
         # increments the index counter, because one more document
         # as been processed (submitted or failed)
         index += 1
 
     return flask.redirect(
-        flask.url_for(
-            "index",
-            message = "Signed documents have been sent to AT"
-        )
+        flask.url_for("index", message="Signed documents have been sent to AT")
     )
 
-@app.route("/oauth", methods = ("GET",))
+
+@app.route("/oauth", methods=("GET",))
 def oauth():
     # retrieves the reference to the current API object, so that
     # it may be used for the retrieval of the access token from
     # the currently received code value
     api = util.get_api()
 
     # retrieves the code value provided that is going to be used
@@ -278,81 +235,76 @@
     code = quorum.get_field("code", None)
     state = quorum.get_field("state", None)
 
     # tries to retrieve the error field an in case it exists raises
     # an error indicating the OAuth based problem
     error = quorum.get_field("error", None)
     error_description = quorum.get_field("error_description", None)
-    if error: raise RuntimeError("%s - %s" % (error, error_description))
+    if error:
+        raise RuntimeError("%s - %s" % (error, error_description))
 
     # creates the access token URL for the API usage and sends the
     # appropriate attributes for the retrieval of the access token,
     # then stores it in the current session
     access_token = api.oauth_access(code)
     flask.session["omnix.access_token"] = access_token
 
     # ensures that a correct session value exists in session, creating
     # a new session in case that's required, this ensures that the acl
     # exists for the current user that is logging in
     api.oauth_session()
 
-    return flask.redirect(
-        state or flask.url_for("index")
-    )
+    return flask.redirect(state or flask.url_for("index"))
+
 
-@app.route("/top", methods = ("GET",))
+@app.route("/top", methods=("GET",))
 @quorum.ensure("base.admin")
 def top():
-    year = quorum.get_field("year", None, cast = int)
-    month = quorum.get_field("month", None, cast = int)
+    year = quorum.get_field("year", None, cast=int)
+    month = quorum.get_field("month", None, cast=int)
 
-    top_employees,\
-    target_s, \
-    previous_month,\
-    previous_year,\
-    next_month,\
-    next_year,\
-    has_next = util.get_top(year = year, month = month)
+    (
+        top_employees,
+        target_s,
+        previous_month,
+        previous_year,
+        next_month,
+        next_year,
+        has_next,
+    ) = util.get_top(year=year, month=month)
 
     return flask.render_template(
         "top.html.tpl",
-        link = "top",
-        title = target_s,
-        top_employees = top_employees,
-        previous = (previous_month, previous_year),
-        next = (next_month, next_year),
-        has_next = has_next
+        link="top",
+        title=target_s,
+        top_employees=top_employees,
+        previous=(previous_month, previous_year),
+        next=(next_month, next_year),
+        has_next=has_next,
     )
 
+
 @app.errorhandler(404)
 def handler_404(error):
     return flask.Response(
-        flask.render_template(
-            "error.html.tpl",
-            error = "404 - Page not found"
-        ),
-        status = 404
+        flask.render_template("error.html.tpl", error="404 - Page not found"),
+        status=404,
     )
 
+
 @app.errorhandler(413)
 def handler_413(error):
     return flask.Response(
-        flask.render_template(
-            "error.html.tpl",
-            error = "412 - Precondition failed"
-        ),
-        status = 413
+        flask.render_template("error.html.tpl", error="412 - Precondition failed"),
+        status=413,
     )
 
+
 @app.errorhandler(Exception)
 def handler_exception(error):
     formatted = traceback.format_exc()
     lines = formatted.splitlines() if quorum.is_devel() else []
 
     return flask.Response(
-        flask.render_template(
-            "error.html.tpl",
-            error = str(error),
-            traceback = lines
-        ),
-        status = 500
+        flask.render_template("error.html.tpl", error=str(error), traceback=lines),
+        status=500,
     )
```

### Comparing `omnix-0.3.1/src/omnix/views/web/employee.py` & `omnix-0.3.3/src/omnix/views/web/employee.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,161 +18,158 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/employees", methods = ("GET",))
+
+@app.route("/employees", methods=("GET",))
 @quorum.ensure("foundation.employee.list")
 def list_employees():
-    return flask.render_template(
-        "employee/list.html.tpl",
-        link = "employees"
-    )
+    return flask.render_template("employee/list.html.tpl", link="employees")
+
 
-@app.route("/employees.json", methods = ("GET",), json = True)
+@app.route("/employees.json", methods=("GET",), json=True)
 @quorum.ensure("foundation.employee.list")
 def list_employees_json():
     api = util.get_api()
     object = quorum.get_object()
     return api.list_employees(**object)
 
-@app.route("/employees/self", methods = ("GET",))
+
+@app.route("/employees/self", methods=("GET",))
 @quorum.ensure("foundation.employee.show.self")
 def show_employee():
     api = util.get_api()
     employee = api.self_employee()
     return flask.render_template(
         "employee/show.html.tpl",
-        link = "employees",
-        sub_link = "info",
-        is_self = True,
-        employee = employee
+        link="employees",
+        sub_link="info",
+        is_self=True,
+        employee=employee,
     )
 
-@app.route("/employees/self/sales", methods = ("GET",))
+
+@app.route("/employees/self/sales", methods=("GET",))
 @quorum.ensure(("sales.sale_transaction.list.self", "sales.customer_return.list.self"))
 def sales_employee():
-    year = quorum.get_field("year", None, cast = int)
-    month = quorum.get_field("month", None, cast = int)
+    year = quorum.get_field("year", None, cast=int)
+    month = quorum.get_field("month", None, cast=int)
 
     api = util.get_api()
     employee = api.self_employee()
 
-    operations,\
-    target,\
-    sales_total,\
-    sales,\
-    returns,\
-    previous_month,\
-    previous_year,\
-    next_month,\
-    next_year,\
-    has_next = util.get_sales(year = year, month = month)
+    (
+        operations,
+        target,
+        sales_total,
+        sales,
+        returns,
+        previous_month,
+        previous_year,
+        next_month,
+        next_year,
+        has_next,
+    ) = util.get_sales(year=year, month=month)
 
     return flask.render_template(
         "employee/sales.html.tpl",
-        link = "employees",
-        sub_link = "sales",
-        is_self = True,
-        employee = employee,
-        operations = operations,
-        commission_rate = util.COMMISSION_RATE,
-        title = target,
-        sales_total = sales_total,
-        sales_count = len(sales),
-        returns_count = len(returns),
-        previous = (previous_month, previous_year),
-        next = (next_month, next_year),
-        has_next = has_next
+        link="employees",
+        sub_link="sales",
+        is_self=True,
+        employee=employee,
+        operations=operations,
+        commission_rate=util.COMMISSION_RATE,
+        title=target,
+        sales_total=sales_total,
+        sales_count=len(sales),
+        returns_count=len(returns),
+        previous=(previous_month, previous_year),
+        next=(next_month, next_year),
+        has_next=has_next,
     )
 
-@app.route("/employees/self/mail", methods = ("GET",))
+
+@app.route("/employees/self/mail", methods=("GET",))
 @quorum.ensure("foundation.employee.show.self")
 def mail_employee():
-    year = quorum.get_field("year", None, cast = int)
-    month = quorum.get_field("month", None, cast = int)
+    year = quorum.get_field("year", None, cast=int)
+    month = quorum.get_field("month", None, cast=int)
 
-    util.mail_activity(year = year, month = month)
+    util.mail_activity(year=year, month=month)
 
     return show_employee()
 
-@app.route("/employees/<int:id>", methods = ("GET",))
+
+@app.route("/employees/<int:id>", methods=("GET",))
 @quorum.ensure("foundation.employee.show")
 def show_employees(id):
     api = util.get_api()
     employee = api.get_employee(id)
     return flask.render_template(
-        "employee/show.html.tpl",
-        link = "employees",
-        sub_link = "info",
-        employee = employee
+        "employee/show.html.tpl", link="employees", sub_link="info", employee=employee
     )
 
-@app.route("/employees/<int:id>/sales", methods = ("GET",))
+
+@app.route("/employees/<int:id>/sales", methods=("GET",))
 @quorum.ensure(("sales.sale_transaction.list", "sales.customer_return.list"))
 def sales_employees(id):
-    year = quorum.get_field("year", None, cast = int)
-    month = quorum.get_field("month", None, cast = int)
+    year = quorum.get_field("year", None, cast=int)
+    month = quorum.get_field("month", None, cast=int)
 
     api = util.get_api()
     employee = api.get_employee(id)
 
-    operations,\
-    target_s,\
-    sales_total,\
-    sales_s,\
-    returns_s,\
-    previous_month,\
-    previous_year,\
-    next_month,\
-    next_year,\
-    has_next = util.get_sales(id = id, year = year, month = month)
+    (
+        operations,
+        target_s,
+        sales_total,
+        sales_s,
+        returns_s,
+        previous_month,
+        previous_year,
+        next_month,
+        next_year,
+        has_next,
+    ) = util.get_sales(id=id, year=year, month=month)
 
     return flask.render_template(
         "employee/sales.html.tpl",
-        link = "employees",
-        sub_link = "sales",
-        is_self = False,
-        employee = employee,
-        operations = operations,
-        commission_rate = util.COMMISSION_RATE,
-        title = target_s,
-        sales_total = sales_total,
-        sales_count = len(sales_s),
-        returns_count = len(returns_s),
-        previous = (previous_month, previous_year),
-        next = (next_month, next_year),
-        has_next = has_next
+        link="employees",
+        sub_link="sales",
+        is_self=False,
+        employee=employee,
+        operations=operations,
+        commission_rate=util.COMMISSION_RATE,
+        title=target_s,
+        sales_total=sales_total,
+        sales_count=len(sales_s),
+        returns_count=len(returns_s),
+        previous=(previous_month, previous_year),
+        next=(next_month, next_year),
+        has_next=has_next,
     )
 
-@app.route("/employees/<int:id>/mail", methods = ("GET",))
+
+@app.route("/employees/<int:id>/mail", methods=("GET",))
 @quorum.ensure("foundation.employee.show")
 def mail_employees(id):
-    year = quorum.get_field("year", None, cast = int)
-    month = quorum.get_field("month", None, cast = int)
+    year = quorum.get_field("year", None, cast=int)
+    month = quorum.get_field("month", None, cast=int)
 
-    util.mail_activity(id = id, year = year, month = month)
+    util.mail_activity(id=id, year=year, month=month)
 
     return show_employees(id)
```

### Comparing `omnix-0.3.1/src/omnix/views/web/media.py` & `omnix-0.3.3/src/omnix/views/web/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,107 +18,89 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import mimetypes
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/media", methods = ("GET",))
+
+@app.route("/media", methods=("GET",))
 @quorum.ensure("foundation.media.list")
 def list_media():
-    return flask.render_template(
-        "media/list.html.tpl",
-        link = "media"
-    )
+    return flask.render_template("media/list.html.tpl", link="media")
+
 
-@app.route("/media.json", methods = ("GET",), json = True)
+@app.route("/media.json", methods=("GET",), json=True)
 @quorum.ensure("foundation.media.list")
 def list_media_json():
     api = util.get_api()
     object = quorum.get_object()
     return api.list_media(**object)
 
-@app.route("/media/<int:id>", methods = ("GET",))
+
+@app.route("/media/<int:id>", methods=("GET",))
 @quorum.ensure("foundation.media.show")
 def show_media(id):
     api = util.get_api()
     media = api.info_media(id)
     media["image_url"] = api.get_media_url(media["secret"])
     return flask.render_template(
-        "media/show.html.tpl",
-        link = "media",
-        sub_link = "info",
-        media = media
+        "media/show.html.tpl", link="media", sub_link="info", media=media
     )
 
-@app.route("/media/<int:id>/edit", methods = ("GET",))
+
+@app.route("/media/<int:id>/edit", methods=("GET",))
 @quorum.ensure("foundation.media.update")
 def edit_media(id):
     api = util.get_api()
     media = api.info_media(id)
     return flask.render_template(
-        "media/edit.html.tpl",
-        link = "media",
-        sub_link = "edit",
-        media = media,
-        errors = dict()
+        "media/edit.html.tpl", link="media", sub_link="edit", media=media, errors=dict()
     )
 
-@app.route("/media/<int:id>/update", methods = ("POST",))
+
+@app.route("/media/<int:id>/update", methods=("POST",))
 @quorum.ensure("foundation.media.update")
 def update_media(id):
     api = util.get_api()
-    position = quorum.get_field("position", None, cast = int)
+    position = quorum.get_field("position", None, cast=int)
     label = quorum.get_field("label", None) or None
-    visibility = quorum.get_field("visibility", None, cast = int)
+    visibility = quorum.get_field("visibility", None, cast=int)
     description = quorum.get_field("description", None) or None
     media_file = quorum.get_field("media_file", None)
     image_type = mimetypes.guess_type(media_file.filename)[0]
     mime_type = image_type if image_type else "image/unknown"
     media = dict(
-        position = position,
-        label = label,
-        visibility = visibility,
-        description = description
+        position=position, label=label, visibility=visibility, description=description
     )
-    payload = dict(media = media)
+    payload = dict(media=media)
     if media_file:
-        try: data = media_file.stream.read()
-        finally: media_file.close()
+        try:
+            data = media_file.stream.read()
+        finally:
+            media_file.close()
         media["mime_type"] = mime_type
         payload["data"] = data
     media = api.update_media(id, payload)
-    return flask.redirect(
-        flask.url_for("show_media", id = media["object_id"])
-    )
+    return flask.redirect(flask.url_for("show_media", id=media["object_id"]))
+
 
-@app.route("/media/<int:id>/delete", methods = ("GET",))
+@app.route("/media/<int:id>/delete", methods=("GET",))
 @quorum.ensure("foundation.media.delete")
 def delete_media(id):
     api = util.get_api()
     api.delete_media(id)
-    return flask.redirect(
-        flask.url_for("list_media")
-    )
+    return flask.redirect(flask.url_for("list_media"))
```

### Comparing `omnix-0.3.1/src/omnix/views/web/extra.py` & `omnix-0.3.3/src/omnix/views/web/extra.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
@@ -46,67 +37,66 @@
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/extras", methods = ("GET",))
+
+@app.route("/extras", methods=("GET",))
 @quorum.ensure("base.user")
 def list_extras():
-    return flask.render_template(
-        "extra/list.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/list.html.tpl", link="extras")
 
-@app.route("/extras/media", methods = ("GET",))
+
+@app.route("/extras/media", methods=("GET",))
 @quorum.ensure("foundation.root_entity.set_media")
 def media_extras():
-    return flask.render_template(
-        "extra/media.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/media.html.tpl", link="extras")
+
 
-@app.route("/extras/media", methods = ("POST",))
+@app.route("/extras/media", methods=("POST",))
 @quorum.ensure("inventory.transactional_merchandise.update")
 def do_media_extras():
     # retrieves the reference to the (Omni) API object that
     # is going to be used for the operations of updating of
     # the merchandise in bulk (multiple operations at a time)
     api = util.get_api()
 
     # tries to retrieve the media file from the current
     # form in case it's not available renders the current
     # template with an error message
     media_file = quorum.get_field("media_file", None)
     if media_file == None or not media_file.filename:
         return flask.render_template(
-            "extra/media.html.tpl",
-            link = "extras",
-            error = "No file defined"
+            "extra/media.html.tpl", link="extras", error="No file defined"
         )
 
     # creates a temporary file path for the storage of the file
     # and then saves it into that directory, closing the same
     # file afterwards, as it has been properly saved
     fd, file_path = tempfile.mkstemp()
-    try: media_file.save(file_path)
-    finally: media_file.close()
+    try:
+        media_file.save(file_path)
+    finally:
+        media_file.close()
 
     try:
         # creates a new temporary directory that is going to be used
         # in the extraction of the media zip file
         temp_path = tempfile.mkdtemp()
         try:
             # creates the zip file reference with the current file path
             # and then extracts the complete set of contents to the "target"
             # temporary path closing the zip file afterwards
             zip = zipfile.ZipFile(file_path)
-            try: zip.extractall(temp_path)
-            finally: zip.close()
+            try:
+                zip.extractall(temp_path)
+            finally:
+                zip.close()
 
             # iterates over the complete set of names in the temporary path
             # to try to upload the media to the target data source, note that
             # only the media files are considered and the base name of them
             # are going to be validation for existence in the data source
             for name in os.listdir(temp_path):
                 # splits the file name into base name and extension and validates
@@ -115,143 +105,150 @@
                 if not extension.lower() in (".png", ".jpg", ".jpeg"):
                     quorum.info("Skipping, '%s' not a valid media file" % name)
                     continue
 
                 # splits the base value of the file name so that it's possible to
                 # extract the proper position of the image if that's required
                 base_s = base.rsplit("_", 1)
-                if len(base_s) > 1: position = int(base_s[1])
-                else: position = 1
+                if len(base_s) > 1:
+                    position = int(base_s[1])
+                else:
+                    position = 1
 
                 # tries to "cast" the base file name value as an integer and in case
                 # it's possible assumes that this value is the object identifier
-                try: object_id = int(base_s[0])
-                except Exception: object_id = None
+                try:
+                    object_id = int(base_s[0])
+                except Exception:
+                    object_id = None
 
                 # in case no object id was retrieved from the base file name value
                 # a secondary strategy is used, so that the merchandise database
                 # is searched using the base string value as the company product code
                 if not object_id:
                     # creates the keyword arguments map so that the the merchandise
                     # with the provided company product code is retrieved
                     kwargs = {
-                        "start_record" : 0,
-                        "number_records" : 1,
-                        "filters[]" : [
-                            "company_product_code:equals:%s" % base_s[0]
-                        ]
+                        "start_record": 0,
+                        "number_records": 1,
+                        "filters[]": ["company_product_code:equals:%s" % base_s[0]],
                     }
 
                     # runs the list merchandise operation in order to try to find a
                     # merchandise entity for the requested (unique) product code in
                     # case there's at least one merchandise its object id is used
-                    try: merchandise = api.list_merchandise(**kwargs)
-                    except Exception: merchandise = []
-                    if merchandise: object_id = merchandise[0]["object_id"]
+                    try:
+                        merchandise = api.list_merchandise(**kwargs)
+                    except Exception:
+                        merchandise = []
+                    if merchandise:
+                        object_id = merchandise[0]["object_id"]
 
                 # in case no object id was retrieved must skip the current loop
                 # with a proper information message (as expected)
                 if not object_id:
-                    quorum.info("Skipping, could not resolve Object ID id for '%s'" % base)
+                    quorum.info(
+                        "Skipping, could not resolve Object ID id for '%s'" % base
+                    )
                     continue
 
                 # prints a logging message about the upload of media file that
                 # is going to be performed for the current entity
                 quorum.debug(
-                    "Adding media file for entity '%d' in position '%d'" %\
-                    (object_id, position)
+                    "Adding media file for entity '%d' in position '%d'"
+                    % (object_id, position)
                 )
 
                 # creates the target temporary media path from the temporary directory
                 # path and then "read" the complete set of contents from it closing the
                 # file afterwards (no more reading allowed)
                 media_path = os.path.join(temp_path, name)
                 media_file = open(media_path, "rb")
-                try: contents = media_file.read()
-                finally: media_file.close()
+                try:
+                    contents = media_file.read()
+                finally:
+                    media_file.close()
 
                 # tries to guess the proper image type for the image located at the
                 # provided path and the uses this value to construct the mime type
                 image_type = imghdr.what(media_path)
                 mime_type = "image/" + image_type if image_type else "image/unknown"
 
                 # sets/updates the media for the associated root entity using the
                 # data extracted from the file and the information in its name
                 api.set_media_entity(
                     object_id,
                     contents,
-                    position = position,
-                    mime_type = mime_type,
-                    engine = "fs",
-                    thumbnails = True
+                    position=position,
+                    mime_type=mime_type,
+                    engine="fs",
+                    thumbnails=True,
                 )
         finally:
             # removes the temporary path as it's no longer going to be
             # required for the operation (errors are ignored)
-            shutil.rmtree(temp_path, ignore_errors = True)
+            shutil.rmtree(temp_path, ignore_errors=True)
     finally:
         # closes the temporary file descriptor and removes the temporary
         # file (avoiding any memory leaks)
         os.close(fd)
         os.remove(file_path)
 
     # redirects the user back to the media list page with a success
     # message indicating that everything went as expected
     return flask.redirect(
-        flask.url_for(
-            "media_extras",
-            message = "Media file processed with success"
-        )
+        flask.url_for("media_extras", message="Media file processed with success")
     )
 
-@app.route("/extras/images", methods = ("GET",))
+
+@app.route("/extras/images", methods=("GET",))
 @quorum.ensure("inventory.transactional_merchandise.update")
 def images_extras():
-    return flask.render_template(
-        "extra/images.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/images.html.tpl", link="extras")
 
-@app.route("/extras/images", methods = ("POST",))
+
+@app.route("/extras/images", methods=("POST",))
 @quorum.ensure("inventory.transactional_merchandise.update")
 def do_images_extras():
     # retrieves the reference to the (Omni) API object that
     # is going to be used for the operations of updating of
     # the merchandise in bulk (multiple operations at a time)
     api = util.get_api()
 
     # tries to retrieve the images file from the current
     # form in case it's not available renders the current
     # template with an error message
     images_file = quorum.get_field("images_file", None)
     if images_file == None or not images_file.filename:
         return flask.render_template(
-            "extra/images.html.tpl",
-            link = "extras",
-            error = "No file defined"
+            "extra/images.html.tpl", link="extras", error="No file defined"
         )
 
     # creates a temporary file path for the storage of the file
     # and then saves it into that directory, closing the same
     # file afterwards, as it has been properly saved
     fd, file_path = tempfile.mkstemp()
-    try: images_file.save(file_path)
-    finally: images_file.close()
+    try:
+        images_file.save(file_path)
+    finally:
+        images_file.close()
 
     try:
         # creates a new temporary directory that is going to be used
         # in the extraction of the images zip file
         temp_path = tempfile.mkdtemp()
         try:
             # creates the zip file reference with the current file path
             # and then extracts the complete set of contents to the "target"
             # temporary path closing the zip file afterwards
             zip = zipfile.ZipFile(file_path)
-            try: zip.extractall(temp_path)
-            finally: zip.close()
+            try:
+                zip.extractall(temp_path)
+            finally:
+                zip.close()
 
             # iterates over the complete set of names in the temporary path
             # to try to upload the image to the target data source, note that
             # only the image files are considered and the base name of them
             # are going to be validation for existence in the data source
             for name in os.listdir(temp_path):
                 # splits the file name into base name and extension and validates
@@ -260,19 +257,17 @@
                 if not extension.lower() in (".png", ".jpg", ".jpeg"):
                     quorum.info("Skipping, '%s' not a valid image file" % name)
                     continue
 
                 # creates the keyword arguments map so that the the merchandise
                 # with the provided company product code is retrieved
                 kwargs = {
-                    "start_record" : 0,
-                    "number_records" : 1,
-                    "filters[]" : [
-                        "company_product_code:equals:%s" % base
-                    ]
+                    "start_record": 0,
+                    "number_records": 1,
+                    "filters[]": ["company_product_code:equals:%s" % base],
                 }
 
                 # creates the URL for the merchandise retrieval and runs the get
                 # operation with the provided filter so that the target merchandise
                 # is retrieved for object id validation
                 merchandise = api.list_merchandise(**kwargs)
 
@@ -292,102 +287,100 @@
                 object_id = entity["object_id"]
 
                 # creates the target temporary image path from the temporary directory
                 # path and then "read" the complete set of contents from it closing the
                 # file afterwards (no more reading allowed)
                 image_path = os.path.join(temp_path, name)
                 image_file = open(image_path, "rb")
-                try: contents = image_file.read()
-                finally: image_file.close()
+                try:
+                    contents = image_file.read()
+                finally:
+                    image_file.close()
 
                 # creates the image (file) tuple with both the name of the file and the
                 # contents if it (multipart standard)
                 image_tuple = (name, contents)
 
                 # creates the multipart data map with both the object id and the image
                 # file parameters that are going to be used in the encoding
                 data_m = {
-                    "object_id" : object_id,
-                    "transactional_merchandise[_parameters][image_file]" : image_tuple
+                    "object_id": object_id,
+                    "transactional_merchandise[_parameters][image_file]": image_tuple,
                 }
 
                 # uses the "resolved" items structure in the operation to
                 # the Omni API so that the images for them get updated
                 api.update_merchandise(object_id, data_m)
         finally:
             # removes the temporary path as it's no longer going to be
             # required for the operation (errors are ignored)
-            shutil.rmtree(temp_path, ignore_errors = True)
+            shutil.rmtree(temp_path, ignore_errors=True)
     finally:
         # closes the temporary file descriptor and removes the temporary
         # file (avoiding any memory leaks)
         os.close(fd)
         os.remove(file_path)
 
     # redirects the user back to the images list page with a success
     # message indicating that everything went as expected
     return flask.redirect(
-        flask.url_for(
-            "images_extras",
-            message = "Images file processed with success"
-        )
+        flask.url_for("images_extras", message="Images file processed with success")
     )
 
-@app.route("/extras/metadata", methods = ("GET",))
+
+@app.route("/extras/metadata", methods=("GET",))
 @quorum.ensure("foundation.root_entity.update")
 def metadata_extras():
-    return flask.render_template(
-        "extra/metadata.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/metadata.html.tpl", link="extras")
 
-@app.route("/extras/metadata", methods = ("POST",))
+
+@app.route("/extras/metadata", methods=("POST",))
 @quorum.ensure("foundation.root_entity.update")
 def do_metadata_extras():
     # retrieves the reference to the API object that is going
     # to be used for the updating of prices operation
     api = util.get_api()
 
     # tries to retrieve the metadata file from the current
     # form in case it's not available renders the current
     # template with an error message
     metadata_file = quorum.get_field("metadata_file", None)
     if metadata_file == None or not metadata_file.filename:
         return flask.render_template(
-            "extra/metadata.html.tpl",
-            link = "extras",
-            error = "No file defined"
+            "extra/metadata.html.tpl", link="extras", error="No file defined"
         )
 
     # retrieves the value of the custom field that control if
     # the importing will be performed using a dynamic approach
     # meaning that no static values will be retrieved and instead
     # the header will be used for dynamic retrieval
-    custom = quorum.get_field("custom", False, cast = bool)
+    custom = quorum.get_field("custom", False, cast=bool)
 
     # check if the CSV file to uploaded is separated by the comma
     # character or if instead it used the semicolon
-    comma = quorum.get_field("comma", False, cast = bool)
+    comma = quorum.get_field("comma", False, cast=bool)
 
     # creates a temporary file path for the storage of the file
     # and then saves it into that directory
     fd, file_path = tempfile.mkstemp()
     metadata_file.save(file_path)
 
     # creates the file object that is going to be used in the
     # reading of the CSV file (underlying object)
     file = open(file_path, "rb")
-    try: data = file.read()
-    finally: file.close()
+    try:
+        data = file.read()
+    finally:
+        file.close()
 
     # constructs the bytes based buffer object from the data that
     # has just been loaded from the file
     buffer = quorum.legacy.BytesIO(data)
 
-    def callback(line, header = None):
+    def callback(line, header=None):
         # in case the custom metadata mode is enabled then a special work
         # model is set where all of the columns are going to be used dynamically
         # for the update of the metadata map of the object
         if custom:
             # creates a zip of tuples with the header to line value association
             # and uses them to build a proper dictionary
             zipped = zip(header, line)
@@ -413,50 +406,56 @@
             ean = update.pop("ean", None)
 
         # otherwise this is a "normal" update and the "typical" metadata
         # fields are the one to be updated
         else:
             # unpacks the current "metadata" line into its components as
             # expected by the specification
-            base,\
-            name,\
-            _retail_price,\
-            compare_price,\
-            discount,\
-            characteristics,\
-            material,\
-            category,\
-            collection,\
-            brand,\
-            season,\
-            gender,\
-            description,\
-            order,\
-            discountable,\
-            orderable,\
-            sku_field,\
-            upc,\
-            ean = line[:19]
+            (
+                base,
+                name,
+                _retail_price,
+                compare_price,
+                discount,
+                characteristics,
+                material,
+                category,
+                collection,
+                brand,
+                season,
+                gender,
+                description,
+                order,
+                discountable,
+                orderable,
+                sku_field,
+                upc,
+                ean,
+            ) = line[:19]
 
             # verifies if the initials part of the CSV line exists and
             # if that's the case processes it properly
             if len(line) >= 22:
                 initials, initials_min, initials_max = line[19:22]
             else:
                 initials, initials_min, initials_max = "", "", ""
 
             # normalizes the various values that have been extracted from the line
             # so they are properly represented for importing
             name = name or None
             compare_price = (compare_price and compare_price.strip()) or None
             discount = (discount and discount.strip()) or None
-            characteristics = [value.strip() for value in characteristics.split(";") if value.strip()]
+            characteristics = [
+                value.strip() for value in characteristics.split(";") if value.strip()
+            ]
             material = [value.strip() for value in material.split(";") if value.strip()]
             category = [value.strip() for value in category.split(";") if value.strip()]
-            collection = [value.strip() for value in collection.split(";") if value.strip()]
+            collection = [
+                value.strip() for value in collection.split(";") if value.strip()
+            ]
             brand = brand or None
             season = season or None
             gender = gender or None
             description = description or None
             order = (order and order.strip()) or None
             discountable = discountable or None
             orderable = orderable or None
@@ -465,81 +464,100 @@
             ean = ean or None
             initials = initials or None
             initials_min = initials_min or None
             initials_max = initials_max or None
 
             # verifies and strips the various possible string values so that they
             # represent a valid not trailed value
-            if name: name = name.strip()
-            if compare_price: compare_price = float(compare_price)
-            if brand: brand = brand.strip()
-            if season: season = season.strip()
-            if gender: gender = gender.strip()
-            if description: description = description.strip()
-            if order: order = int(order)
-            if discountable: discountable = discountable == "1"
-            if orderable: orderable = orderable == "1"
-            if sku_field: sku_field = sku_field.strip()
-            if discount: discount = float(discount)
-            if upc: upc = upc.strip()
-            if ean: ean = ean.strip()
-            if initials: initials = initials == "1"
-            if initials_min: initials_min = int(initials_min)
-            if initials_max: initials_max = int(initials_max)
+            if name:
+                name = name.strip()
+            if compare_price:
+                compare_price = float(compare_price)
+            if brand:
+                brand = brand.strip()
+            if season:
+                season = season.strip()
+            if gender:
+                gender = gender.strip()
+            if description:
+                description = description.strip()
+            if order:
+                order = int(order)
+            if discountable:
+                discountable = discountable == "1"
+            if orderable:
+                orderable = orderable == "1"
+            if sku_field:
+                sku_field = sku_field.strip()
+            if discount:
+                discount = float(discount)
+            if upc:
+                upc = upc.strip()
+            if ean:
+                ean = ean.strip()
+            if initials:
+                initials = initials == "1"
+            if initials_min:
+                initials_min = int(initials_min)
+            if initials_max:
+                initials_max = int(initials_max)
 
             # creates the map that is going to hold the complete set of features
             # and populates the features according to their existence
             features = dict()
             if initials:
-                features["initials"] = dict(min = initials_min, max = initials_max)
+                features["initials"] = dict(min=initials_min, max=initials_max)
 
             # creates the update dictionary that is going to be used in the updating
             # of the "product" metadata (this is considered to be a delta dictionary)
             update = dict(
-                compare_price = compare_price,
-                discount = discount,
-                characteristics = characteristics,
-                features = features,
-                material = material,
-                category = category,
-                collection = collection,
-                brand = brand,
-                season = season,
-                gender = gender,
-                order = order,
-                discountable = discountable,
-                orderable = orderable,
-                sku_field = sku_field
+                compare_price=compare_price,
+                discount=discount,
+                characteristics=characteristics,
+                features=features,
+                material=material,
+                category=category,
+                collection=collection,
+                brand=brand,
+                season=season,
+                gender=gender,
+                order=order,
+                discountable=discountable,
+                orderable=orderable,
+                sku_field=sku_field,
             )
 
         # tries to "cast" the base value as an integer and in case
         # it's possible assumes that this value is the object identifier
-        try: object_id = int(base)
-        except Exception: object_id = None
+        try:
+            object_id = int(base)
+        except Exception:
+            object_id = None
 
         # in case no object id was retrieved from the base name value
         # a secondary strategy is used, so that the merchandise database
         # is searched using the base string value as the company product code
         if not object_id:
             # creates the keyword arguments map so that the the merchandise
             # with the provided company product code is retrieved
             kwargs = {
-                "start_record" : 0,
-                "number_records" : 1,
-                "filters[]" : [
-                    "company_product_code:equals:%s" % base
-                ]
+                "start_record": 0,
+                "number_records": 1,
+                "filters[]": ["company_product_code:equals:%s" % base],
             }
 
             # runs the list merchandise operation in order to try to find a
             # merchandise entity for the requested (unique) product code in
             # case there's at least one merchandise its object id is used
-            try: merchandise = api.list_merchandise(**kwargs)
-            except Exception: merchandise = []
-            if merchandise: object_id = merchandise[0]["object_id"]
+            try:
+                merchandise = api.list_merchandise(**kwargs)
+            except Exception:
+                merchandise = []
+            if merchandise:
+                object_id = merchandise[0]["object_id"]
 
         # in case no object id was retrieved must skip the current loop
         # with a proper information message (as expected)
         if not object_id:
             quorum.info("Skipping, could not resolve Object ID for '%s'" % base)
             return
 
@@ -555,231 +573,221 @@
         # updates the metadata dictionary with the new values that are going
         # to be used for the updating of the entity, note that the previous
         # metadata values are leveraged and not overwritten with this strategy
         metadata.update(update)
 
         # creates the model structure to be updated and then runs the
         # proper execution of the metadata import
-        model = dict(metadata = metadata)
-        if name: model["name"] = name
-        if description: model["description"] = description
-        if upc: model["upc"] = upc
-        if ean: model["ean"] = ean
-        api.update_entity(object_id, payload = dict(root_entity = model))
+        model = dict(metadata=metadata)
+        if name:
+            model["name"] = name
+        if description:
+            model["description"] = description
+        if upc:
+            model["upc"] = upc
+        if ean:
+            model["ean"] = ean
+        api.update_entity(object_id, payload=dict(root_entity=model))
 
     try:
         # start the CSV import operation that is going to import the
         # various lines of the CSV in the buffer and for each of them
         # call the function passed as callback
         util.csv_import(
-            buffer,
-            callback,
-            header = True,
-            delimiter = "," if comma else ";",
-            quoting = True
+            buffer, callback, header=True, delimiter="," if comma else ";", quoting=True
         )
     finally:
         # closes the temporary file descriptor and removes the temporary
         # file (avoiding any memory leaks)
         os.close(fd)
         os.remove(file_path)
 
     # redirects the user back to the metadata list page with a success
     # message indicating that everything went ok
     return flask.redirect(
-        flask.url_for(
-            "metadata_extras",
-            message = "Metadata file processed with success"
-        )
+        flask.url_for("metadata_extras", message="Metadata file processed with success")
     )
 
-@app.route("/extras/prices", methods = ("GET",))
+
+@app.route("/extras/prices", methods=("GET",))
 @quorum.ensure("inventory.transactional_merchandise.update")
 def prices_extras():
-    return flask.render_template(
-        "extra/prices.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/prices.html.tpl", link="extras")
 
-@app.route("/extras/prices", methods = ("POST",))
+
+@app.route("/extras/prices", methods=("POST",))
 @quorum.ensure("inventory.transactional_merchandise.update")
 def do_prices_extras():
     # retrieves the reference to the API object that is going
     # to be used for the updating of prices operation
     api = util.get_api()
 
     # tries to retrieve the prices file from the current
     # form in case it's not available renders the current
     # template with an error message
     prices_file = quorum.get_field("prices_file", None)
     if prices_file == None or not prices_file.filename:
         return flask.render_template(
-            "extra/prices.html.tpl",
-            link = "extras",
-            error = "No file defined"
+            "extra/prices.html.tpl", link="extras", error="No file defined"
         )
 
     # creates a temporary file path for the storage of the file
     # and then saves it into that directory
     fd, file_path = tempfile.mkstemp()
     prices_file.save(file_path)
 
     try:
         # parses the temporary file containing the spreadsheet according
         # to the provided set of keys (to create the correct structures)
         items = quorum.xlsx_to_map(
             file_path,
-            keys = ("company_product_code", "retail_price"),
-            types = (quorum.legacy.UNICODE, None)
+            keys=("company_product_code", "retail_price"),
+            types=(quorum.legacy.UNICODE, None),
         )
     finally:
         # closes the temporary file descriptor and removes the temporary
         # file (avoiding any memory leaks)
         os.close(fd)
         os.remove(file_path)
 
     # iterates over the complete set of items to make sure that they
     # all comply with the expected structure
     for index, item in enumerate(items):
         quorum.verify(
             item["company_product_code"],
-            message = "No key for value at index %d, please verify" % index
+            message="No key for value at index %d, please verify" % index,
         )
         quorum.verify(
             not item["retail_price"] in (None, ""),
-            message = "No retail price for code '%s', please verify" % item["company_product_code"]
+            message="No retail price for code '%s', please verify"
+            % item["company_product_code"],
         )
 
     # uses the "resolved" items structure in the put operation to
     # the Omni API so that the prices for them get updated
     api.prices_merchandise(items)
 
     # redirects the user back to the prices list page with a success
     # message indicating that everything went ok
     return flask.redirect(
-        flask.url_for(
-            "prices_extras",
-            message = "Prices file processed with success"
-        )
+        flask.url_for("prices_extras", message="Prices file processed with success")
     )
 
-@app.route("/extras/costs", methods = ("GET",))
+
+@app.route("/extras/costs", methods=("GET",))
 @quorum.ensure("inventory.transactional_merchandise.update")
 def costs_extras():
-    return flask.render_template(
-        "extra/costs.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/costs.html.tpl", link="extras")
+
 
-@app.route("/extras/costs", methods = ("POST",))
+@app.route("/extras/costs", methods=("POST",))
 @quorum.ensure("inventory.transactional_merchandise.update")
 def do_costs_extras():
     # retrieves the reference to the API object that is going
     # to be used for the updating of costs operation
     api = util.get_api()
 
     # tries to retrieve the costs file from the current
     # form in case it's not available renders the current
     # template with an error message
     costs_file = quorum.get_field("costs_file", None)
     if costs_file == None or not costs_file.filename:
         return flask.render_template(
-            "extra/costs.html.tpl",
-            link = "extras",
-            error = "No file defined"
+            "extra/costs.html.tpl", link="extras", error="No file defined"
         )
 
     # creates a temporary file path for the storage of the file
     # and then saves it into that directory
     fd, file_path = tempfile.mkstemp()
     costs_file.save(file_path)
 
     try:
         # parses the temporary file containing the spreadsheet according
         # to the provided set of keys (to create the correct structures)
         items = quorum.xlsx_to_map(
             file_path,
-            keys = ("company_product_code", "cost"),
-            types = (quorum.legacy.UNICODE, None)
+            keys=("company_product_code", "cost"),
+            types=(quorum.legacy.UNICODE, None),
         )
     finally:
         # closes the temporary file descriptor and removes the temporary
         # file (avoiding any memory leaks)
         os.close(fd)
         os.remove(file_path)
 
     # iterates over the complete set of items to make sure that they
     # all comply with the expected structure
     for index, item in enumerate(items):
         quorum.verify(
             item["company_product_code"],
-            message = "No key for value at index %d, please verify" % index
+            message="No key for value at index %d, please verify" % index,
         )
         quorum.verify(
             not item["cost"] in (None, ""),
-            message = "No cost value for code '%s', please verify" % item["company_product_code"]
+            message="No cost value for code '%s', please verify"
+            % item["company_product_code"],
         )
 
     # uses the "resolved" items structure in the put operation to
     # the Omni API so that the costs for them get updated
     api.costs_merchandise(items)
 
     # redirects the user back to the costs list page with a success
     # message indicating that everything went ok
     return flask.redirect(
-        flask.url_for(
-            "costs_extras",
-            message = "Costs file processed with success"
-        )
+        flask.url_for("costs_extras", message="Costs file processed with success")
     )
 
-@app.route("/extras/inventory", methods = ("GET",))
-@quorum.ensure((
-    "inventory.stock_adjustment.create",
-    "inventory.transactional_merchandise.list",
-    "foundation.store.list"
-))
-def inventory_extras():
-    return flask.render_template(
-        "extra/inventory.html.tpl",
-        link = "extras"
+
+@app.route("/extras/inventory", methods=("GET",))
+@quorum.ensure(
+    (
+        "inventory.stock_adjustment.create",
+        "inventory.transactional_merchandise.list",
+        "foundation.store.list",
     )
+)
+def inventory_extras():
+    return flask.render_template("extra/inventory.html.tpl", link="extras")
 
-@app.route("/extras/inventory", methods = ("POST",))
-@quorum.ensure((
-    "inventory.stock_adjustment.create",
-    "inventory.transactional_merchandise.list",
-    "foundation.store.list"
-))
+
+@app.route("/extras/inventory", methods=("POST",))
+@quorum.ensure(
+    (
+        "inventory.stock_adjustment.create",
+        "inventory.transactional_merchandise.list",
+        "foundation.store.list",
+    )
+)
 def do_inventory_extras():
     # retrieves the reference to the API object that is going
     # to be used for the updating of prices operation
     api = util.get_api()
 
     # tries to retrieve the inventory file from the current
     # form in case it's not available renders the current
     # template with an error message
     inventory_file = quorum.get_field("inventory_file", None)
     if inventory_file == None or not inventory_file.filename:
         return flask.render_template(
-            "extra/inventory.html.tpl",
-            link = "extras",
-            error = "No file defined"
+            "extra/inventory.html.tpl", link="extras", error="No file defined"
         )
 
     # creates a temporary file path for the storage of the file
     # and then saves it into that directory
     fd, file_path = tempfile.mkstemp()
     inventory_file.save(file_path)
 
     # creates the file object that is going to be used in the
     # reading of the CSV file (underlying object)
     file = open(file_path, "rb")
-    try: data = file.read()
-    finally: file.close()
+    try:
+        data = file.read()
+    finally:
+        file.close()
 
     # constructs the bytes based buffer object from the data that
     # has just been loaded from the file
     buffer = quorum.legacy.BytesIO(data)
 
     # creates the maps that are going to be used to cache the
     # resolution processes for both the stores and the merchandise
@@ -792,195 +800,196 @@
 
     def get_adjustment():
         return state.get("adjustment", None)
 
     def new_adjustment(target_id):
         flush_adjustment()
         adjustment = dict(
-            adjustment_target = dict(
-                object_id = target_id
-            ),
-            stock_adjustment_lines = []
+            adjustment_target=dict(object_id=target_id), stock_adjustment_lines=[]
         )
         state["adjustment"] = adjustment
         return adjustment
 
     def flush_adjustment():
         adjustment = get_adjustment()
         state["adjustment"] = None
-        if not adjustment: return
-        payload = dict(stock_adjustment = adjustment)
+        if not adjustment:
+            return
+        payload = dict(stock_adjustment=adjustment)
         stock_adjustment = api.create_stock_adjustment(payload)
         store_id = adjustment["adjustment_target"]["object_id"]
         stock_adjustment_id = stock_adjustment["object_id"]
         quorum.debug(
-            "Created stock adjustment '%d' for store '%d'" %\
-            (stock_adjustment_id, store_id)
+            "Created stock adjustment '%d' for store '%d'"
+            % (stock_adjustment_id, store_id)
         )
         return stock_adjustment
 
-    def add_adjustment_line(merchandise_id, quantity = -1):
+    def add_adjustment_line(merchandise_id, quantity=-1):
         adjustment = get_adjustment()
-        if not adjustment: raise quorum.OperationalError(
-            "No adjustment in context"
-        )
+        if not adjustment:
+            raise quorum.OperationalError("No adjustment in context")
         lines = adjustment["stock_adjustment_lines"]
         line = dict(
-            stock_on_hand_delta = quantity,
-            merchandise = dict(
-                object_id = merchandise_id
-            )
+            stock_on_hand_delta=quantity, merchandise=dict(object_id=merchandise_id)
         )
         lines.append(line)
 
     def get_store_id(store_code):
         object_id = stores_map.get(store_code, None)
-        if object_id: return object_id
+        if object_id:
+            return object_id
 
         kwargs = {
-            "start_record" : 0,
-            "number_records" : 1,
-            "filters[]" : [
-                "store_code:equals:%s" % store_code
-            ]
+            "start_record": 0,
+            "number_records": 1,
+            "filters[]": ["store_code:equals:%s" % store_code],
         }
 
-        try: stores = api.list_stores(**kwargs)
-        except Exception: stores = []
-        if stores: object_id = stores[0]["object_id"]
+        try:
+            stores = api.list_stores(**kwargs)
+        except Exception:
+            stores = []
+        if stores:
+            object_id = stores[0]["object_id"]
 
         stores_map[store_code] = object_id
         return object_id
 
     def get_merchandise_id(company_product_code):
         # tries to retrieve the object id of the merchandise from the
         # cache and in case it succeeds returns it immediately
         object_id = merchandise_map.get(company_product_code, None)
-        if object_id: return object_id
+        if object_id:
+            return object_id
 
         # creates the map containing the (filter) keyword arguments that
         # are going to be send to the list merchandise operation
         kwargs = {
-            "start_record" : 0,
-            "number_records" : 1,
-            "filters[]" : [
-                "company_product_code:equals:%s" % company_product_code
-            ]
+            "start_record": 0,
+            "number_records": 1,
+            "filters[]": ["company_product_code:equals:%s" % company_product_code],
         }
 
         # runs the list merchandise operation in order to try to find a
         # merchandise entity for the requested (unique) product code in
         # case there's at least one merchandise its object id is used
-        try: merchandise = api.list_merchandise(**kwargs)
-        except Exception: merchandise = []
-        if merchandise: object_id = merchandise[0]["object_id"]
+        try:
+            merchandise = api.list_merchandise(**kwargs)
+        except Exception:
+            merchandise = []
+        if merchandise:
+            object_id = merchandise[0]["object_id"]
 
         # updates the (cache) map for the merchandise with the reference
         # new object id to company product code reference and then returns
         # the object id of the merchandise to the caller method
         merchandise_map[company_product_code] = object_id
         return object_id
 
-    def callback(line, header = None):
+    def callback(line, header=None):
         code, quantity, _date, _time = line[:4]
 
         code = code.strip()
         quantity = quantity.strip()
         quantity = int(quantity)
         quantity = quantity * -1
 
         is_store = len(code) < 4
-        if is_store: store_id = get_store_id(code)
-        else: merchandise_id = get_merchandise_id(code)
+        if is_store:
+            store_id = get_store_id(code)
+        else:
+            merchandise_id = get_merchandise_id(code)
 
         if is_store:
-            if store_id: new_adjustment(store_id)
-            else: flush_adjustment()
+            if store_id:
+                new_adjustment(store_id)
+            else:
+                flush_adjustment()
         elif merchandise_id:
-            try: add_adjustment_line(
-                merchandise_id,
-                quantity = quantity
-            )
-            except Exception: pass
+            try:
+                add_adjustment_line(merchandise_id, quantity=quantity)
+            except Exception:
+                pass
 
     try:
         # start the CSV import operation that is going to import the
         # various lines of the CSV in the buffer and for each of them
         # call the function passed as callback
-        util.csv_import(buffer, callback, delimiter = ";")
+        util.csv_import(buffer, callback, delimiter=";")
         flush_adjustment()
     finally:
         # closes the temporary file descriptor and removes the temporary
         # file (avoiding any memory leaks)
         os.close(fd)
         os.remove(file_path)
 
     # redirects the user back to the inventory list page with a success
     # message indicating that everything went ok
     return flask.redirect(
         flask.url_for(
-            "inventory_extras",
-            message = "Inventory file processed with success"
+            "inventory_extras", message="Inventory file processed with success"
         )
     )
 
-@app.route("/extras/transfers", methods = ("GET",))
-@quorum.ensure((
-    "inventory.transfer.create",
-    "inventory.transactional_merchandise.list",
-    "foundation.store.list"
-))
-def transfers_extras():
-    return flask.render_template(
-        "extra/transfers.html.tpl",
-        link = "extras"
+
+@app.route("/extras/transfers", methods=("GET",))
+@quorum.ensure(
+    (
+        "inventory.transfer.create",
+        "inventory.transactional_merchandise.list",
+        "foundation.store.list",
     )
+)
+def transfers_extras():
+    return flask.render_template("extra/transfers.html.tpl", link="extras")
 
-@app.route("/extras/transfers", methods = ("POST",))
-@quorum.ensure((
-    "inventory.transfer.create",
-    "inventory.transactional_merchandise.list",
-    "foundation.store.list"
-))
+
+@app.route("/extras/transfers", methods=("POST",))
+@quorum.ensure(
+    (
+        "inventory.transfer.create",
+        "inventory.transactional_merchandise.list",
+        "foundation.store.list",
+    )
+)
 def do_transfers_extras():
     # retrieves the reference to the API object that is going
     # to be used for the updating of prices operation
     api = util.get_api()
 
     # tries to retrieve the origin value from the provided set
     # of fields and in case it's not defined re-renders the template
-    origin = quorum.get_field("origin", None, cast = int)
+    origin = quorum.get_field("origin", None, cast=int)
     if not origin:
         return flask.render_template(
-            "extra/transfers.html.tpl",
-            link = "extras",
-            error = "No origin defined"
+            "extra/transfers.html.tpl", link="extras", error="No origin defined"
         )
 
     # tries to retrieve the transfers file from the current
     # form in case it's not available renders the current
     # template with an error message
     transfers_file = quorum.get_field("transfers_file", None)
     if transfers_file == None or not transfers_file.filename:
         return flask.render_template(
-            "extra/transfers.html.tpl",
-            link = "extras",
-            error = "No file defined"
+            "extra/transfers.html.tpl", link="extras", error="No file defined"
         )
 
     # creates a temporary file path for the storage of the file
     # and then saves it into that directory
     fd, file_path = tempfile.mkstemp()
     transfers_file.save(file_path)
 
     # creates the file object that is going to be used in the
     # reading of the CSV file (underlying object)
     file = open(file_path, "rb")
-    try: data = file.read()
-    finally: file.close()
+    try:
+        data = file.read()
+    finally:
+        file.close()
 
     # constructs the bytes based buffer object from the data that
     # has just been loaded from the file
     buffer = quorum.legacy.BytesIO(data)
 
     # creates the maps that are going to be used to cache the
     # resolution processes for both the stores and the merchandise
@@ -990,215 +999,203 @@
     # creates the map that is going to hold the complete state
     # to be used in the process of the various transfers (context)
     state = dict()
 
     def get_transfer():
         return state.get("transfer", None)
 
-    def new_transfer(target_id, workflow_state = 6):
+    def new_transfer(target_id, workflow_state=6):
         flush_transfer()
         transfer = dict(
-            origin = dict(
-                object_id = origin
-            ),
-            destination = dict(
-                object_id = target_id
-            ),
-            transfer_lines = [],
-            _parameters = dict(
-                target_workflow_state = workflow_state
-            )
+            origin=dict(object_id=origin),
+            destination=dict(object_id=target_id),
+            transfer_lines=[],
+            _parameters=dict(target_workflow_state=workflow_state),
         )
         state["transfer"] = transfer
         return transfer
 
     def flush_transfer():
         transfer = get_transfer()
         state["transfer"] = None
-        if not transfer: return
-        payload = dict(transfer = transfer)
+        if not transfer:
+            return
+        payload = dict(transfer=transfer)
         transfer = api.create_transfer(payload)
         transfer_id = transfer["object_id"]
-        quorum.debug(
-            "Created stock transfer '%d'" % transfer_id
-        )
+        quorum.debug("Created stock transfer '%d'" % transfer_id)
         return transfer
 
-    def add_transfer_line(merchandise_id, quantity = 1):
+    def add_transfer_line(merchandise_id, quantity=1):
         transfer = get_transfer()
-        if not transfer: raise quorum.OperationalError(
-            "No transfer in context"
-        )
+        if not transfer:
+            raise quorum.OperationalError("No transfer in context")
         lines = transfer["transfer_lines"]
-        line = dict(
-            quantity = quantity,
-            merchandise = dict(
-                object_id = merchandise_id
-            )
-        )
+        line = dict(quantity=quantity, merchandise=dict(object_id=merchandise_id))
         lines.append(line)
 
     def get_store_id(store_code):
         object_id = stores_map.get(store_code, None)
-        if object_id: return object_id
+        if object_id:
+            return object_id
 
         kwargs = {
-            "start_record" : 0,
-            "number_records" : 1,
-            "filters[]" : [
-                "store_code:equals:%s" % store_code
-            ]
+            "start_record": 0,
+            "number_records": 1,
+            "filters[]": ["store_code:equals:%s" % store_code],
         }
 
-        try: stores = api.list_stores(**kwargs)
-        except Exception: stores = []
-        if stores: object_id = stores[0]["object_id"]
+        try:
+            stores = api.list_stores(**kwargs)
+        except Exception:
+            stores = []
+        if stores:
+            object_id = stores[0]["object_id"]
 
         stores_map[store_code] = object_id
         return object_id
 
     def get_merchandise_id(company_product_code):
         # tries to retrieve the object id of the merchandise from the
         # cache and in case it succeeds returns it immediately
         object_id = merchandise_map.get(company_product_code, None)
-        if object_id: return object_id
+        if object_id:
+            return object_id
 
         # creates the map containing the (filter) keyword arguments that
         # are going to be send to the list merchandise operation
         kwargs = {
-            "start_record" : 0,
-            "number_records" : 1,
-            "filters[]" : [
-                "company_product_code:equals:%s" % company_product_code
-            ]
+            "start_record": 0,
+            "number_records": 1,
+            "filters[]": ["company_product_code:equals:%s" % company_product_code],
         }
 
         # runs the list merchandise operation in order to try to find a
         # merchandise entity for the requested (unique) product code in
         # case there's at least one merchandise its object id is used
-        try: merchandise = api.list_merchandise(**kwargs)
-        except Exception: merchandise = []
-        if merchandise: object_id = merchandise[0]["object_id"]
+        try:
+            merchandise = api.list_merchandise(**kwargs)
+        except Exception:
+            merchandise = []
+        if merchandise:
+            object_id = merchandise[0]["object_id"]
 
         # updates the (cache) map for the merchandise with the reference
         # new object id to company product code reference and then returns
         # the object id of the merchandise to the caller method
         merchandise_map[company_product_code] = object_id
         return object_id
 
-    def callback(line, header = None):
+    def callback(line, header=None):
         code, quantity, _date, _time = line[:4]
 
         code = code.strip()
         quantity = quantity.strip()
         quantity = int(quantity)
 
         is_store = len(code) < 4
-        if is_store: store_id = get_store_id(code)
-        else: merchandise_id = get_merchandise_id(code)
+        if is_store:
+            store_id = get_store_id(code)
+        else:
+            merchandise_id = get_merchandise_id(code)
 
         if is_store:
-            if store_id: new_transfer(store_id)
-            else: flush_transfer()
+            if store_id:
+                new_transfer(store_id)
+            else:
+                flush_transfer()
         elif merchandise_id:
-            try: add_transfer_line(
-                merchandise_id,
-                quantity = quantity
-            )
-            except Exception: pass
+            try:
+                add_transfer_line(merchandise_id, quantity=quantity)
+            except Exception:
+                pass
 
     try:
         # start the CSV import operation that is going to import the
         # various lines of the CSV in the buffer and for each of them
         # call the function passed as callback
-        util.csv_import(buffer, callback, delimiter = ";")
+        util.csv_import(buffer, callback, delimiter=";")
         flush_transfer()
     finally:
         # closes the temporary file descriptor and removes the temporary
         # file (avoiding any memory leaks)
         os.close(fd)
         os.remove(file_path)
 
     # redirects the user back to the transfers list page with a success
     # message indicating that everything went ok
     return flask.redirect(
         flask.url_for(
-            "transfers_extras",
-            message = "Transfers file processed with success"
+            "transfers_extras", message="Transfers file processed with success"
         )
     )
 
-@app.route("/extras/ctt", methods = ("GET",))
+
+@app.route("/extras/ctt", methods=("GET",))
 @quorum.ensure("sales.sale_order.list")
 def ctt_extras():
-    return flask.render_template(
-        "extra/ctt.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/ctt.html.tpl", link="extras")
+
 
-@app.route("/extras/ctt", methods = ("POST",))
+@app.route("/extras/ctt", methods=("POST",))
 @quorum.ensure("sales.sale_order.list")
 def do_ctt_extras():
     api = util.get_api()
-    sale_orders = api.list_sale_orders(**{
-        "start_record" : 0,
-        "number_records" : -1,
-        "eager[]" : [
-            "customer",
-            "customer.primary_contact_information",
-            "shipping_address"
-        ],
-        "filters[]" : [
-            "workflow_state:equals:5",
-            "shipping_type:equals:2"
-        ]
-    })
-
-    out_data = util.encode_ctt(sale_orders, encoding = "Cp1252")
-
-    return flask.Response(
-        out_data,
-        mimetype = "binary/octet-stream"
+    sale_orders = api.list_sale_orders(
+        **{
+            "start_record": 0,
+            "number_records": -1,
+            "eager[]": [
+                "customer",
+                "customer.primary_contact_information",
+                "shipping_address",
+            ],
+            "filters[]": ["workflow_state:equals:5", "shipping_type:equals:2"],
+        }
     )
 
-@app.route("/extras/template", methods = ("GET",))
+    out_data = util.encode_ctt(sale_orders, encoding="Cp1252")
+
+    return flask.Response(out_data, mimetype="binary/octet-stream")
+
+
+@app.route("/extras/template", methods=("GET",))
 @quorum.ensure("base.user")
 def template_extras():
-    return flask.render_template(
-        "extra/template.html.tpl",
-        link = "extras"
-    )
+    return flask.render_template("extra/template.html.tpl", link="extras")
 
-@app.route("/extras/template", methods = ("POST",))
+
+@app.route("/extras/template", methods=("POST",))
 @quorum.ensure("foundation.system_company.show.self")
 def do_template_extras():
     object = quorum.get_object()
     mask_name = object.get("mask_name", None)
     format = object.get("format", "png")
     base_file = object.get("base_file", None)
     base_data = base_file.read()
 
     mask_name = "mask_" + mask_name if mask_name else "mask"
     mask_name = mask_name.lower()
     mask_name = mask_name.replace(" ", "_")
 
     api = util.get_api()
-    try: mask_data = api.public_media_system_company(label = mask_name)
-    except Exception: mask_data = None
-    if not mask_data: raise quorum.OperationalError("No mask defined")
+    try:
+        mask_data = api.public_media_system_company(label=mask_name)
+    except Exception:
+        mask_data = None
+    if not mask_data:
+        raise quorum.OperationalError("No mask defined")
 
-    out_data = util.mask_image(base_data, mask_data, format = format)
+    out_data = util.mask_image(base_data, mask_data, format=format)
     mimetype = mimetypes.guess_type("_." + format)[0]
 
-    return flask.Response(
-        out_data,
-        mimetype = mimetype or "application/octet-stream"
-    )
+    return flask.Response(out_data, mimetype=mimetype or "application/octet-stream")
+
 
-@app.route("/extras/mask", methods = ("POST",))
+@app.route("/extras/mask", methods=("POST",))
 @quorum.ensure("foundation.root_entity.set_media")
 def do_mask_extras():
     object = quorum.get_object()
     mask_name = object.get("mask_name", None)
     mask_file = object.get("mask_file", None)
 
     mask_name = "mask_" + mask_name if mask_name else "mask"
@@ -1209,106 +1206,101 @@
     system_company = api.self_system_company()
 
     data = mask_file.read()
     mime_type = mask_file.content_type
     api.set_media_entity(
         system_company["object_id"],
         mask_name,
-        data = data,
-        mime_type = mime_type,
-        visibility = 2
+        data=data,
+        mime_type=mime_type,
+        visibility=2,
     )
 
     return flask.redirect(
-        flask.url_for(
-            "template_extras",
-            message = "Mask file uploaded with success"
-        )
+        flask.url_for("template_extras", message="Mask file uploaded with success")
     )
 
-@app.route("/extras/browser", methods = ("GET",))
+
+@app.route("/extras/browser", methods=("GET",))
 @quorum.ensure("foundation.root_entity.show_media")
 def browser_extras():
-    object_id = quorum.get_field("id", None, cast = int)
+    object_id = quorum.get_field("id", None, cast=int)
     return flask.render_template(
-        "extra/browser.html.tpl",
-        link = "extras",
-        object_id = object_id
+        "extra/browser.html.tpl", link="extras", object_id=object_id
     )
 
-@app.route("/extras/browser", methods = ("POST",), json = True)
+
+@app.route("/extras/browser", methods=("POST",), json=True)
 @quorum.ensure("foundation.root_entity.show_media")
 def do_browser():
-    object_id = quorum.get_field("object_id", None, cast = int)
+    object_id = quorum.get_field("object_id", None, cast=int)
     api = util.get_api()
     entity = api.get_entity(object_id)
     media = api.info_media_entity(object_id)
     media_info = []
     for item in media:
         mitem = dict(
-            object_id = item["object_id"],
-            label = item["label"],
-            position = item["position"],
-            dimensions = item["dimensions"],
-            image_url = api.get_media_url(item["secret"])
+            object_id=item["object_id"],
+            label=item["label"],
+            position=item["position"],
+            dimensions=item["dimensions"],
+            image_url=api.get_media_url(item["secret"]),
         )
         media_info.append(mitem)
-    media_info.sort(key = _media_sorter)
+    media_info.sort(key=_media_sorter)
     entity["media"] = media_info
     return entity
 
-@app.route("/extras/browser/new_media/<int:id>", methods = ("GET",))
+
+@app.route("/extras/browser/new_media/<int:id>", methods=("GET",))
 @quorum.ensure("foundation.root_entity.set_media")
 def new_media_browser(id):
     return flask.render_template(
         "extra/browser/new_media.html.tpl",
-        link = "extras",
-        object_id = id,
-        media = dict(),
-        errors = dict()
+        link="extras",
+        object_id=id,
+        media=dict(),
+        errors=dict(),
     )
 
-@app.route("/extras/browser/new_media/<int:id>", methods = ("POST",))
+
+@app.route("/extras/browser/new_media/<int:id>", methods=("POST",))
 @quorum.ensure("foundation.root_entity.set_media")
 def create_media_browser(id):
     api = util.get_api()
     engine = quorum.get_field("engine", None) or None
-    position = quorum.get_field("position", None, cast = int)
+    position = quorum.get_field("position", None, cast=int)
     label = quorum.get_field("label", None) or None
-    visibility = quorum.get_field("visibility", None, cast = int)
+    visibility = quorum.get_field("visibility", None, cast=int)
     description = quorum.get_field("description", None) or None
-    thumbnails = quorum.get_field("thumbnails", False, cast = bool)
+    thumbnails = quorum.get_field("thumbnails", False, cast=bool)
     media_file = quorum.get_field("media_file", None)
     image_type = mimetypes.guess_type(media_file.filename)[0]
     mime_type = image_type if image_type else "image/unknown"
-    try: data = media_file.stream.read()
-    finally: media_file.close()
+    try:
+        data = media_file.stream.read()
+    finally:
+        media_file.close()
     api.set_media_entity(
         id,
         data,
-        engine = engine,
-        position = position,
-        label = label,
-        mime_type = mime_type,
-        visibility = visibility,
-        description = description,
-        thumbnails = thumbnails
-    )
-    return flask.redirect(
-        flask.url_for("browser_extras", id = id)
+        engine=engine,
+        position=position,
+        label=label,
+        mime_type=mime_type,
+        visibility=visibility,
+        description=description,
+        thumbnails=thumbnails,
     )
+    return flask.redirect(flask.url_for("browser_extras", id=id))
 
-@app.route("/extras/browser/clear_media/<int:id>", methods = ("GET",))
+
+@app.route("/extras/browser/clear_media/<int:id>", methods=("GET",))
 @quorum.ensure("foundation.root_entity.clear_media")
 def clear_media_browser(id):
     api = util.get_api()
     api.clear_media_entity(id)
-    return flask.redirect(
-        flask.url_for("browser_extras", id = id)
-    )
+    return flask.redirect(flask.url_for("browser_extras", id=id))
+
 
 def _media_sorter(item):
-    return (
-        item["label"] or "",
-        item["position"] or 0,
-        item["dimensions"] or ""
-    )
+    return (item["label"] or "", item["position"] or 0, item["dimensions"] or "")
```

### Comparing `omnix-0.3.1/src/omnix/views/web/customer.py` & `omnix-0.3.3/src/omnix/views/web/customer.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,53 +18,42 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/customers", methods = ("GET",))
+
+@app.route("/customers", methods=("GET",))
 @quorum.ensure("customers.customer_person.list")
 def list_customers():
-    return flask.render_template(
-        "customer/list.html.tpl",
-        link = "customers"
-    )
+    return flask.render_template("customer/list.html.tpl", link="customers")
 
-@app.route("/customers.json", methods = ("GET",), json = True)
+
+@app.route("/customers.json", methods=("GET",), json=True)
 @quorum.ensure("customers.customer_person.list")
 def list_customers_json():
     api = util.get_api()
     object = quorum.get_object()
     return api.list_persons(**object)
 
-@app.route("/customers/<int:id>", methods = ("GET",))
+
+@app.route("/customers/<int:id>", methods=("GET",))
 @quorum.ensure("customers.customer_person.show")
 def show_customers(id):
     api = util.get_api()
     customer = api.get_person(id)
     return flask.render_template(
-        "customer/show.html.tpl",
-        link = "customers",
-        customer = customer
+        "customer/show.html.tpl", link="customers", customer=customer
     )
```

### Comparing `omnix-0.3.1/src/omnix/views/web/store.py` & `omnix-0.3.3/src/omnix/views/web/store.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,130 +18,122 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import datetime
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/stores", methods = ("GET",))
+
+@app.route("/stores", methods=("GET",))
 @quorum.ensure("foundation.store.list")
 def list_stores():
-    return flask.render_template(
-        "store/list.html.tpl",
-        link = "stores"
-    )
+    return flask.render_template("store/list.html.tpl", link="stores")
+
 
-@app.route("/stores.json", methods = ("GET",), json = True)
+@app.route("/stores.json", methods=("GET",), json=True)
 @quorum.ensure("foundation.store.list")
 def list_stores_json():
     api = util.get_api()
     object = quorum.get_object()
     return api.list_stores(**object)
 
-@app.route("/stores/<id>", methods = ("GET",))
+
+@app.route("/stores/<id>", methods=("GET",))
 @quorum.ensure("foundation.store.show")
 def show_stores(id):
     api = util.get_api()
     id = int(id)
     is_global = id == -1
     store = _global() if is_global else api.get_store(id)
     return flask.render_template(
-        "store/show.html.tpl",
-        link = "stores",
-        sub_link = "info",
-        store = store
+        "store/show.html.tpl", link="stores", sub_link="info", store=store
     )
 
-@app.route("/stores/<id>/sales", methods = ("GET",))
+
+@app.route("/stores/<id>/sales", methods=("GET",))
 @quorum.ensure(("foundation.store.show", "analytics.sale_snapshot.list"))
 def sales_stores(id):
     api = util.get_api()
 
     id = int(id)
     is_global = id == -1
 
     now = datetime.datetime.utcnow()
     current_day = datetime.datetime(now.year, now.month, now.day)
 
     store = _global() if is_global else api.get_store(id)
 
     contents = api.stats_sales(
-        unit = "day",
-        store_id = None if is_global else id,
-        has_global = True
+        unit="day", store_id=None if is_global else id, has_global=True
     )
     stats = contents[str(id)]
     current = dict(
-        net_price_vat = stats["net_price_vat"][-1],
-        net_number_sales = stats["net_number_sales"][-1],
-        date = current_day
+        net_price_vat=stats["net_price_vat"][-1],
+        net_number_sales=stats["net_number_sales"][-1],
+        date=current_day,
     )
 
     days = []
 
     count = len(stats["net_price_vat"]) - 1
     count_r = range(count)
     count_r = list(count_r)
     count_r.reverse()
     _current_day = current_day
     for index in count_r:
         _current_day -= datetime.timedelta(1)
         day = dict(
-            net_price_vat = stats["net_price_vat"][index],
-            net_number_sales = stats["net_number_sales"][index],
-            date = _current_day
+            net_price_vat=stats["net_price_vat"][index],
+            net_number_sales=stats["net_number_sales"][index],
+            date=_current_day,
         )
         days.append(day)
 
     previous_s = days[0] if days else dict()
-    current["amount_delta"] = current["net_price_vat"] -\
-        previous_s.get("net_price_vat", 0)
-    current["number_delta"] = current["net_number_sales"] -\
-        previous_s.get("net_number_sales", 0)
-
-    if current["amount_delta"] == 0: current["amount_direction"] = "equal"
-    elif current["amount_delta"] > 0: current["amount_direction"] = "up"
-    else: current["amount_direction"] = "down"
-
-    if current["number_delta"] == 0: current["number_direction"] = "equal"
-    elif current["number_delta"] > 0: current["number_direction"] = "up"
-    else: current["number_direction"] = "down"
+    current["amount_delta"] = current["net_price_vat"] - previous_s.get(
+        "net_price_vat", 0
+    )
+    current["number_delta"] = current["net_number_sales"] - previous_s.get(
+        "net_number_sales", 0
+    )
+
+    if current["amount_delta"] == 0:
+        current["amount_direction"] = "equal"
+    elif current["amount_delta"] > 0:
+        current["amount_direction"] = "up"
+    else:
+        current["amount_direction"] = "down"
+
+    if current["number_delta"] == 0:
+        current["number_direction"] = "equal"
+    elif current["number_delta"] > 0:
+        current["number_direction"] = "up"
+    else:
+        current["number_direction"] = "down"
 
     return flask.render_template(
         "store/sales.html.tpl",
-        link = "stores",
-        sub_link = "sales",
-        store = store,
-        stats = stats,
-        current = current,
-        days = days
+        link="stores",
+        sub_link="sales",
+        store=store,
+        stats=stats,
+        current=current,
+        days=days,
     )
 
+
 def _global():
-    return dict(
-        object_id = -1,
-        name = "Global",
-        primary_contact_information = dict()
-    )
+    return dict(object_id=-1, name="Global", primary_contact_information=dict())
```

### Comparing `omnix-0.3.1/src/omnix/views/web/supplier.py` & `omnix-0.3.3/src/omnix/views/web/supplier.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,53 +18,42 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from omnix import util
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/suppliers", methods = ("GET",))
+
+@app.route("/suppliers", methods=("GET",))
 @quorum.ensure("foundation.supplier_company.list")
 def list_suppliers():
-    return flask.render_template(
-        "supplier/list.html.tpl",
-        link = "suppliers"
-    )
+    return flask.render_template("supplier/list.html.tpl", link="suppliers")
 
-@app.route("/suppliers.json", methods = ("GET",), json = True)
+
+@app.route("/suppliers.json", methods=("GET",), json=True)
 @quorum.ensure("foundation.supplier_company.list")
 def list_suppliers_json():
     api = util.get_api()
     object = quorum.get_object()
     return api.list_companies(**object)
 
-@app.route("/suppliers/<int:id>", methods = ("GET",))
+
+@app.route("/suppliers/<int:id>", methods=("GET",))
 @quorum.ensure("foundation.supplier_company.show")
 def show_suppliers(id):
     api = util.get_api()
     supplier = api.get_company(id)
     return flask.render_template(
-        "supplier/show.html.tpl",
-        link = "suppliers",
-        supplier = supplier
+        "supplier/show.html.tpl", link="suppliers", supplier=supplier
     )
```

### Comparing `omnix-0.3.1/src/omnix/views/web/settings.py` & `omnix-0.3.3/src/omnix/views/web/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,67 +18,59 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Omnix System. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
 __copyright__ = "Copyright (c) 2008-2022 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from omnix import util
 from omnix import models
 
 from omnix.main import app
 from omnix.main import flask
 from omnix.main import quorum
 
-@app.route("/settings/slack/ensure", methods = ("GET",))
+
+@app.route("/settings/slack/ensure", methods=("GET",))
 @quorum.ensure("base.admin")
 def ensure_slack():
     next = quorum.get_field("next")
     api = _get_slack_api()
-    return flask.redirect(
-        api.oauth_authorize(state = next)
-    )
+    return flask.redirect(api.oauth_authorize(state=next))
 
-@app.route("/settings/slack/oauth", methods = ("GET",))
+
+@app.route("/settings/slack/oauth", methods=("GET",))
 @quorum.ensure("base.admin")
 def oauth_slack():
     code = quorum.get_field("code")
     state = quorum.get_field("state")
     next = state
     api = _get_slack_api()
     access_token = api.oauth_access(code)
     settings = models.Settings.get_settings()
     settings.slack_token = access_token
     settings.slack_channel = api.channel
     settings.save()
-    return flask.redirect(
-       next or flask.url_for("index")
-    )
+    return flask.redirect(next or flask.url_for("index"))
 
-def _get_slack_api(scope = None):
+
+def _get_slack_api(scope=None):
     import slack
+
     kwargs = dict()
     redirect_url = util.BASE_URL + flask.url_for("oauth_slack")
     access_token = flask.session and flask.session.get("slack.access_token", None)
-    if scope: kwargs["scope"] = scope
+    if scope:
+        kwargs["scope"] = scope
     return slack.API(
-        client_id = quorum.conf("SLACK_ID"),
-        client_secret = quorum.conf("SLACK_SECRET"),
-        redirect_url = redirect_url,
-        access_token = access_token,
+        client_id=quorum.conf("SLACK_ID"),
+        client_secret=quorum.conf("SLACK_SECRET"),
+        redirect_url=redirect_url,
+        access_token=access_token,
         **kwargs
     )
```

### Comparing `omnix-0.3.1/src/omnix/static/css/layout.css` & `omnix-0.3.3/src/omnix/static/css/layout.css`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/static/images/email/logo.png` & `omnix-0.3.3/src/omnix/static/images/email/logo.png`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/static/images/login.png` & `omnix-0.3.3/src/omnix/static/images/login.png`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/src/omnix/static/js/main.js` & `omnix-0.3.3/src/omnix/static/js/main.js`

 * *Files identical despite different names*

### Comparing `omnix-0.3.1/README.md` & `omnix-0.3.3/README.md`

 * *Files identical despite different names*

