# Comparing `tmp/aws_service_screener-2.0.2a2.tar.gz` & `tmp/aws_service_screener-2.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_service_screener-2.0.2a2.tar", max compression
+gzip compressed data, was "aws_service_screener-2.0.2a3.tar", max compression
```

## Comparing `aws_service_screener-2.0.2a2.tar` & `aws_service_screener-2.0.2a3.tar`

### file list

```diff
@@ -1,316 +1,316 @@
--rw-r--r--   0        0        0    10142 2024-04-03 06:56:08.275195 aws_service_screener-2.0.2a2/LICENSE
--rwxr-xr-x   0        0        0     6237 2024-04-03 06:56:08.275783 aws_service_screener-2.0.2a2/README.md
--rw-r--r--   0        0        0     1284 2024-04-03 06:56:08.274112 aws_service_screener-2.0.2a2/aws_service_screener/CreateService.py
--rw-r--r--   0        0        0     1928 2024-04-04 06:43:18.073637 aws_service_screener-2.0.2a2/aws_service_screener/DocLinkValidity.py
--rw-r--r--   0        0        0     4044 2024-04-03 06:56:08.276068 aws_service_screener-2.0.2a2/aws_service_screener/RuleCount.py
--rw-r--r--   0        0        0     8183 2024-04-04 06:44:10.460535 aws_service_screener-2.0.2a2/aws_service_screener/Screener.py
--rw-r--r--   0        0        0        0 2024-04-03 07:23:50.580521 aws_service_screener-2.0.2a2/aws_service_screener/__fork/tail.txt
--rw-r--r--   0        0        0        7 2024-04-03 06:56:08.276828 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/.gitignore
--rw-r--r--   0        0        0     1081 2024-04-03 06:56:08.277048 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/LICENCE.md
--rw-r--r--   0        0        0  1382975 2024-04-03 06:56:08.280923 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/css/adminlte.min.css
--rw-r--r--   0        0        0     2637 2024-04-03 06:56:08.285084 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/AdminLTELogo.png
--rw-r--r--   0        0        0     2391 2024-04-03 06:56:08.285270 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/aws.png
--rw-r--r--   0        0        0   123766 2024-04-03 06:56:08.285958 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.jpg
--rw-r--r--   0        0        0    43676 2024-04-03 06:56:08.286257 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.png
--rw-r--r--   0        0        0      339 2024-04-03 06:56:08.286450 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/default-150x150.png
--rw-r--r--   0        0        0     1139 2024-04-03 06:56:08.286646 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/icons.png
--rw-r--r--   0        0        0      942 2024-04-03 06:56:08.286888 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/.eslintrc.json
--rw-r--r--   0        0        0    99945 2024-04-03 06:56:08.287646 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js
--rw-r--r--   0        0        0   171653 2024-04-03 06:56:08.288815 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js.map
--rw-r--r--   0        0        0    44244 2024-04-03 06:56:08.289171 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js
--rw-r--r--   0        0        0   129651 2024-04-03 06:56:08.289486 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js.map
--rw-r--r--   0        0        0    22240 2024-04-03 06:56:08.289713 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/demo.js
--rw-r--r--   0        0        0    84378 2024-04-03 06:56:08.290404 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   173077 2024-04-03 06:56:08.291348 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/chart.js/Chart.min.js
--rw-r--r--   0        0        0   448232 2024-04-03 06:56:08.302255 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.js
--rw-r--r--   0        0        0    87956 2024-04-03 06:56:08.304038 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.min.js
--rw-r--r--   0        0        0     8428 2024-04-03 06:56:08.291858 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.css
--rw-r--r--   0        0        0     7496 2024-04-03 06:56:08.292112 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.min.css
--rw-r--r--   0        0        0     4706 2024-04-03 06:56:08.292891 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.js
--rw-r--r--   0        0        0     4520 2024-04-03 06:56:08.293210 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.min.js
--rw-r--r--   0        0        0    10415 2024-04-03 06:56:08.293624 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.css
--rw-r--r--   0        0        0     9000 2024-04-03 06:56:08.293941 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.min.css
--rw-r--r--   0        0        0     2041 2024-04-03 06:56:08.294355 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.js
--rw-r--r--   0        0        0     1443 2024-04-03 06:56:08.294712 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.min.js
--rw-r--r--   0        0        0     6131 2024-04-03 06:56:08.294974 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.js
--rw-r--r--   0        0        0     3198 2024-04-03 06:56:08.295253 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.min.js
--rw-r--r--   0        0        0    44471 2024-04-03 06:56:08.295745 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.js
--rw-r--r--   0        0        0    25103 2024-04-03 06:56:08.296505 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.min.js
--rw-r--r--   0        0        0     5333 2024-04-03 06:56:08.296882 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.js
--rw-r--r--   0        0        0     2514 2024-04-03 06:56:08.297178 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.min.js
--rw-r--r--   0        0        0    60730 2024-04-03 06:56:08.297768 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.js
--rw-r--r--   0        0        0    25183 2024-04-03 06:56:08.298206 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.min.js
--rw-r--r--   0        0        0     5091 2024-04-03 06:56:08.298685 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.css
--rw-r--r--   0        0        0     4301 2024-04-03 06:56:08.298907 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.min.css
--rw-r--r--   0        0        0    40599 2024-04-03 06:56:08.299383 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.js
--rw-r--r--   0        0        0    16849 2024-04-03 06:56:08.299793 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.min.js
--rw-r--r--   0        0        0     1997 2024-04-03 06:56:08.300118 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.js
--rw-r--r--   0        0        0     3661 2024-04-03 06:56:08.300406 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.min.js
--rw-r--r--   0        0        0    73625 2024-04-03 06:56:08.304643 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.css
--rw-r--r--   0        0        0    59344 2024-04-03 06:56:08.305015 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.min.css
--rw-r--r--   0        0        0      732 2024-04-03 06:56:08.305211 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.css
--rw-r--r--   0        0        0      675 2024-04-03 06:56:08.305453 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.min.css
--rw-r--r--   0        0        0    71990 2024-04-03 06:56:08.306103 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.css
--rw-r--r--   0        0        0    57912 2024-04-03 06:56:08.306614 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.min.css
--rw-r--r--   0        0        0      734 2024-04-03 06:56:08.306857 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.css
--rw-r--r--   0        0        0      677 2024-04-03 06:56:08.307135 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.min.css
--rw-r--r--   0        0        0      727 2024-04-03 06:56:08.307390 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.css
--rw-r--r--   0        0        0      669 2024-04-03 06:56:08.307583 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.min.css
--rw-r--r--   0        0        0     8077 2024-04-03 06:56:08.307782 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.css
--rw-r--r--   0        0        0     6359 2024-04-03 06:56:08.307947 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.min.css
--rw-r--r--   0        0        0    41312 2024-04-03 06:56:08.308190 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.css
--rw-r--r--   0        0        0    26702 2024-04-03 06:56:08.308620 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.min.css
--rw-r--r--   0        0        0   134346 2024-04-03 06:56:08.310346 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.eot
--rw-r--r--   0        0        0   747545 2024-04-03 06:56:08.313956 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.svg
--rw-r--r--   0        0        0   134040 2024-04-03 06:56:08.315427 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    90060 2024-04-03 06:56:08.316187 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff
--rw-r--r--   0        0        0    76764 2024-04-03 06:56:08.316763 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    34034 2024-04-03 06:56:08.317519 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.eot
--rw-r--r--   0        0        0   144714 2024-04-03 06:56:08.318696 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.svg
--rw-r--r--   0        0        0    33736 2024-04-03 06:56:08.319302 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    16276 2024-04-03 06:56:08.319839 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff
--rw-r--r--   0        0        0    13276 2024-04-03 06:56:08.320181 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   203030 2024-04-03 06:56:08.323786 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.eot
--rw-r--r--   0        0        0   918991 2024-04-03 06:56:08.328886 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.svg
--rw-r--r--   0        0        0   202744 2024-04-03 06:56:08.341995 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   101652 2024-04-03 06:56:08.342791 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0    78196 2024-04-03 06:56:08.344104 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    12505 2024-04-03 06:56:08.344800 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/icheck-bootstrap/icheck-bootstrap.min.css
--rw-r--r--   0        0        0   288579 2024-04-03 06:56:08.349324 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/jquery/jquery.js
--rw-r--r--   0        0        0    20020 2024-04-03 06:56:08.351376 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/css/OverlayScrollbars.min.css
--rw-r--r--   0        0        0    42602 2024-04-03 06:56:08.353692 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/js/jquery.overlayScrollbars.min.js
--rw-r--r--   0        0        0    17358 2024-04-03 06:56:08.354464 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.css
--rw-r--r--   0        0        0    14966 2024-04-03 06:56:08.354867 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.min.css
--rw-r--r--   0        0        0      866 2024-04-03 06:56:08.355685 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/af.js
--rw-r--r--   0        0        0      905 2024-04-03 06:56:08.355962 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ar.js
--rw-r--r--   0        0        0      721 2024-04-03 06:56:08.356293 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/az.js
--rw-r--r--   0        0        0      968 2024-04-03 06:56:08.356609 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bg.js
--rw-r--r--   0        0        0     1291 2024-04-03 06:56:08.356879 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bn.js
--rw-r--r--   0        0        0      965 2024-04-03 06:56:08.357168 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bs.js
--rw-r--r--   0        0        0     1802 2024-04-03 06:56:08.357426 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/build.txt
--rw-r--r--   0        0        0      900 2024-04-03 06:56:08.357721 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ca.js
--rw-r--r--   0        0        0     1292 2024-04-03 06:56:08.357983 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/cs.js
--rw-r--r--   0        0        0      828 2024-04-03 06:56:08.358941 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/da.js
--rw-r--r--   0        0        0      866 2024-04-03 06:56:08.359279 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/de.js
--rw-r--r--   0        0        0     1017 2024-04-03 06:56:08.359717 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/dsb.js
--rw-r--r--   0        0        0     1182 2024-04-03 06:56:08.360022 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/el.js
--rw-r--r--   0        0        0      844 2024-04-03 06:56:08.360329 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/en.js
--rw-r--r--   0        0        0      922 2024-04-03 06:56:08.360817 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/es.js
--rw-r--r--   0        0        0      801 2024-04-03 06:56:08.361139 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/et.js
--rw-r--r--   0        0        0      868 2024-04-03 06:56:08.362358 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/eu.js
--rw-r--r--   0        0        0     1023 2024-04-03 06:56:08.362678 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fa.js
--rw-r--r--   0        0        0      803 2024-04-03 06:56:08.363227 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fi.js
--rw-r--r--   0        0        0      924 2024-04-03 06:56:08.363580 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fr.js
--rw-r--r--   0        0        0      924 2024-04-03 06:56:08.363932 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/gl.js
--rw-r--r--   0        0        0      984 2024-04-03 06:56:08.364211 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/he.js
--rw-r--r--   0        0        0     1175 2024-04-03 06:56:08.364896 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hi.js
--rw-r--r--   0        0        0      852 2024-04-03 06:56:08.365303 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hr.js
--rw-r--r--   0        0        0     1018 2024-04-03 06:56:08.365652 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hsb.js
--rw-r--r--   0        0        0      831 2024-04-03 06:56:08.366120 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hu.js
--rw-r--r--   0        0        0     1028 2024-04-03 06:56:08.366410 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hy.js
--rw-r--r--   0        0        0      768 2024-04-03 06:56:08.366776 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/id.js
--rw-r--r--   0        0        0      807 2024-04-03 06:56:08.367447 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/is.js
--rw-r--r--   0        0        0      897 2024-04-03 06:56:08.367804 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/it.js
--rw-r--r--   0        0        0      862 2024-04-03 06:56:08.368128 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ja.js
--rw-r--r--   0        0        0     1195 2024-04-03 06:56:08.368446 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ka.js
--rw-r--r--   0        0        0     1088 2024-04-03 06:56:08.368737 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/km.js
--rw-r--r--   0        0        0      855 2024-04-03 06:56:08.369044 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ko.js
--rw-r--r--   0        0        0      944 2024-04-03 06:56:08.369350 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lt.js
--rw-r--r--   0        0        0      900 2024-04-03 06:56:08.369635 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lv.js
--rw-r--r--   0        0        0     1038 2024-04-03 06:56:08.369971 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/mk.js
--rw-r--r--   0        0        0      811 2024-04-03 06:56:08.370338 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ms.js
--rw-r--r--   0        0        0      778 2024-04-03 06:56:08.370603 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nb.js
--rw-r--r--   0        0        0     1357 2024-04-03 06:56:08.370945 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ne.js
--rw-r--r--   0        0        0      904 2024-04-03 06:56:08.371332 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nl.js
--rw-r--r--   0        0        0      947 2024-04-03 06:56:08.371731 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pl.js
--rw-r--r--   0        0        0     1049 2024-04-03 06:56:08.372074 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ps.js
--rw-r--r--   0        0        0      876 2024-04-03 06:56:08.372457 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt-BR.js
--rw-r--r--   0        0        0      878 2024-04-03 06:56:08.372733 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt.js
--rw-r--r--   0        0        0      938 2024-04-03 06:56:08.373542 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ro.js
--rw-r--r--   0        0        0     1171 2024-04-03 06:56:08.373888 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ru.js
--rw-r--r--   0        0        0     1306 2024-04-03 06:56:08.374196 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sk.js
--rw-r--r--   0        0        0      925 2024-04-03 06:56:08.374466 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sl.js
--rw-r--r--   0        0        0      903 2024-04-03 06:56:08.374734 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sq.js
--rw-r--r--   0        0        0     1109 2024-04-03 06:56:08.375015 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr-Cyrl.js
--rw-r--r--   0        0        0      980 2024-04-03 06:56:08.376266 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr.js
--rw-r--r--   0        0        0      786 2024-04-03 06:56:08.376792 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sv.js
--rw-r--r--   0        0        0     1074 2024-04-03 06:56:08.377834 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/th.js
--rw-r--r--   0        0        0      771 2024-04-03 06:56:08.378568 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tk.js
--rw-r--r--   0        0        0      775 2024-04-03 06:56:08.378885 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tr.js
--rw-r--r--   0        0        0     1156 2024-04-03 06:56:08.379156 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/uk.js
--rw-r--r--   0        0        0      796 2024-04-03 06:56:08.379398 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/vi.js
--rw-r--r--   0        0        0      768 2024-04-03 06:56:08.379677 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-CN.js
--rw-r--r--   0        0        0      707 2024-04-03 06:56:08.379918 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-TW.js
--rw-r--r--   0        0        0   173566 2024-04-03 06:56:08.380849 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.js
--rw-r--r--   0        0        0    79172 2024-04-03 06:56:08.382426 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.min.js
--rw-r--r--   0        0        0   153589 2024-04-03 06:56:08.383701 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.js
--rw-r--r--   0        0        0    70851 2024-04-03 06:56:08.384483 aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.min.js
--rw-r--r--   0        0        0      658 2024-04-04 06:43:14.502120 aws_service_screener-2.0.2a2/aws_service_screener/constants.py
--rw-r--r--   0        0        0      399 2024-04-03 06:56:08.385151 aws_service_screener-2.0.2a2/aws_service_screener/crossAccounts.sample.json
--rw-r--r--   0        0        0      418 2024-04-04 03:25:06.992938 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/FTR.py
--rw-r--r--   0        0        0      225 2024-04-04 03:24:28.500915 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/FTRPageBuilder.py
--rw-r--r--   0        0        0     1064 2024-04-03 07:13:49.778355 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-312.pyc
--rw-r--r--   0        0        0      769 2024-04-03 07:23:19.927246 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-39.pyc
--rw-r--r--   0        0        0     3166 2024-04-03 06:56:08.386522 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/map.json
--rw-r--r--   0        0        0     4887 2024-04-04 03:25:14.366928 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/Framework.py
--rw-r--r--   0        0        0     8928 2024-04-04 03:22:53.875133 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FrameworkPageBuilder.py
--rw-r--r--   0        0        0      401 2024-04-04 03:24:26.632654 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/.~c9_invoke_T7uTi.py
--rw-r--r--   0        0        0      936 2024-04-04 03:24:25.840688 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/MSR.py
--rw-r--r--   0        0        0      225 2024-04-04 03:24:25.150045 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/MSRPageBuilder.py
--rw-r--r--   0        0        0      230 2024-04-03 06:56:08.389995 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/README.md
--rw-r--r--   0        0        0     1739 2024-04-03 07:13:49.786617 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-312.pyc
--rw-r--r--   0        0        0     1253 2024-04-03 07:23:19.932440 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-39.pyc
--rw-r--r--   0        0        0     3769 2024-04-03 06:56:08.390329 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/map.json
--rw-r--r--   0        0        0      418 2024-04-04 03:24:24.491532 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/SSB.py
--rw-r--r--   0        0        0      225 2024-04-04 03:24:23.714161 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/SSBPageBuilder.py
--rw-r--r--   0        0        0     1064 2024-04-03 07:13:49.782605 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-312.pyc
--rw-r--r--   0        0        0      769 2024-04-03 07:23:19.930174 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-39.pyc
--rw-r--r--   0        0        0     3022 2024-04-03 06:56:08.391405 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/map.json
--rw-r--r--   0        0        0      420 2024-04-04 03:24:22.879011 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/WAFS.py
--rw-r--r--   0        0        0      246 2024-04-04 03:24:21.731471 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/WAFSPageBuilder.py
--rw-r--r--   0        0        0     1074 2024-04-03 07:13:49.784295 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-312.pyc
--rw-r--r--   0        0        0      779 2024-04-03 07:23:19.931200 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-39.pyc
--rw-r--r--   0        0        0     4321 2024-04-03 06:56:08.393288 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/map.json
--rw-r--r--   0        0        0     6344 2024-04-03 07:13:49.780725 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/Framework.cpython-312.pyc
--rw-r--r--   0        0        0     4091 2024-04-03 07:23:19.929148 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/Framework.cpython-39.pyc
--rw-r--r--   0        0        0    12116 2024-04-03 07:13:49.776696 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-312.pyc
--rw-r--r--   0        0        0     8235 2024-04-03 07:23:19.926339 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-39.pyc
--rw-r--r--   0        0        0    21098 2024-04-03 06:56:08.393669 aws_service_screener-2.0.2a2/aws_service_screener/frameworks/api.json
--rw-r--r--   0        0        0      191 2024-04-03 06:56:08.394469 aws_service_screener-2.0.2a2/aws_service_screener/info.json
--rw-r--r--   0        0        0    10992 2024-04-04 06:41:23.044965 aws_service_screener-2.0.2a2/aws_service_screener/main.py
--rwxr-xr-x   0        0        0     5818 2024-04-03 06:56:08.396324 aws_service_screener-2.0.2a2/aws_service_screener/reporter.md
--rw-r--r--   0        0        0     6148 2024-04-03 06:56:08.397550 aws_service_screener-2.0.2a2/aws_service_screener/services/.DS_Store
--rw-r--r--   0        0        0     1238 2024-04-04 06:43:17.140786 aws_service_screener-2.0.2a2/aws_service_screener/services/Cloudwatch.py
--rw-r--r--   0        0        0     4065 2024-04-04 06:43:15.855134 aws_service_screener-2.0.2a2/aws_service_screener/services/Evaluator.py
--rw-r--r--   0        0        0    30268 2024-04-04 06:43:13.324659 aws_service_screener-2.0.2a2/aws_service_screener/services/PageBuilder.py
--rw-r--r--   0        0        0    12595 2024-04-04 06:43:36.935738 aws_service_screener-2.0.2a2/aws_service_screener/services/Reporter.py
--rw-r--r--   0        0        0     3585 2024-04-04 06:43:27.237315 aws_service_screener-2.0.2a2/aws_service_screener/services/Service.py
--rw-r--r--   0        0        0     1663 2024-04-03 07:13:49.758209 aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Cloudwatch.cpython-312.pyc
--rw-r--r--   0        0        0     1252 2024-04-03 07:23:19.911843 aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Cloudwatch.cpython-39.pyc
--rw-r--r--   0        0        0    38925 2024-04-03 07:13:49.769944 aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/PageBuilder.cpython-312.pyc
--rw-r--r--   0        0        0    24688 2024-04-03 07:23:19.920696 aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/PageBuilder.cpython-39.pyc
--rw-r--r--   0        0        0    13320 2024-04-03 07:13:49.762194 aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Reporter.cpython-312.pyc
--rw-r--r--   0        0        0     6990 2024-04-03 07:23:19.914700 aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Reporter.cpython-39.pyc
--rw-r--r--   0        0        0     1977 2024-04-03 06:56:08.400472 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudfront/Cloudfront.py
--rw-r--r--   0        0        0     4833 2024-04-03 06:56:08.400787 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudfront/cloudfront.reporter.json
--rw-r--r--   0        0        0     2929 2024-04-03 06:56:08.401370 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudfront/drivers/cloudfrontDist.py
--rw-r--r--   0        0        0     3176 2024-04-03 06:56:08.402116 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/Cloudtrail.py
--rw-r--r--   0        0        0       40 2024-04-03 06:56:08.402377 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/README.md
--rw-r--r--   0        0        0    13808 2024-04-03 06:56:08.402722 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/cloudtrail.reporter.json
--rw-r--r--   0        0        0     1235 2024-04-03 06:56:08.403129 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/drivers/CloudtrailAccount.py
--rw-r--r--   0        0        0     5443 2024-04-03 06:56:08.403404 aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/drivers/CloudtrailCommon.py
--rw-r--r--   0        0        0     8708 2024-04-04 03:21:56.829424 aws_service_screener-2.0.2a2/aws_service_screener/services/dashboard/DashboardPageBuilder.py
--rw-r--r--   0        0        0    10171 2024-04-03 07:13:49.773186 aws_service_screener-2.0.2a2/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-312.pyc
--rw-r--r--   0        0        0     6797 2024-04-03 07:23:19.924057 aws_service_screener-2.0.2a2/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-39.pyc
--rw-r--r--   0        0        0     3859 2024-04-03 06:56:08.404469 aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/Dynamodb.py
--rw-r--r--   0        0        0      292 2024-04-03 06:56:08.404923 aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/drivers/DateTimeEncoder.py
--rw-r--r--   0        0        0    21159 2024-04-03 06:56:08.405306 aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/drivers/DynamoDbCommon.py
--rw-r--r--   0        0        0     6613 2024-04-03 06:56:08.405672 aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/drivers/DynamoDbGeneric.py
--rw-r--r--   0        0        0    15863 2024-04-03 06:56:08.406076 aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/dynamodb.reporter.json
--rw-r--r--   0        0        0    15205 2024-04-03 06:56:08.406726 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/Ec2.py
--rw-r--r--   0        0        0     4606 2024-04-03 06:56:08.407258 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2AutoScaling.py
--rw-r--r--   0        0        0      536 2024-04-03 06:56:08.407555 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2CompOpt.py
--rw-r--r--   0        0        0     1766 2024-04-03 06:56:08.410006 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2CostExplorerRecs.py
--rw-r--r--   0        0        0      444 2024-04-03 06:56:08.410397 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2EIP.py
--rw-r--r--   0        0        0      816 2024-04-03 06:56:08.410732 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2EbsSnapshot.py
--rw-r--r--   0        0        0     4893 2024-04-03 06:56:08.411046 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2EbsVolume.py
--rw-r--r--   0        0        0     1642 2024-04-03 06:56:08.411341 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2ElbClassic.py
--rw-r--r--   0        0        0     2897 2024-04-03 06:56:08.411619 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2ElbCommon.py
--rw-r--r--   0        0        0    10126 2024-04-03 06:56:08.412024 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2Instance.py
--rw-r--r--   0        0        0     6156 2024-04-03 06:56:08.412551 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2SecGroup.py
--rw-r--r--   0        0        0    27940 2024-04-03 06:56:08.412919 aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/ec2.reporter.json
--rw-r--r--   0        0        0     1344 2024-04-03 06:56:08.413639 aws_service_screener-2.0.2a2/aws_service_screener/services/efs/Efs.py
--rw-r--r--   0        0        0      108 2024-04-03 06:56:08.413983 aws_service_screener-2.0.2a2/aws_service_screener/services/efs/README.md
--rw-r--r--   0        0        0     1184 2024-04-03 06:56:08.414741 aws_service_screener-2.0.2a2/aws_service_screener/services/efs/drivers/EfsDriver.py
--rw-r--r--   0        0        0     1485 2024-04-03 06:56:08.415034 aws_service_screener-2.0.2a2/aws_service_screener/services/efs/efs.reporter.json
--rw-r--r--   0        0        0     2127 2024-04-03 06:56:08.415463 aws_service_screener-2.0.2a2/aws_service_screener/services/eks/Eks.py
--rw-r--r--   0        0        0       35 2024-04-03 06:56:08.415952 aws_service_screener-2.0.2a2/aws_service_screener/services/eks/README.md
--rw-r--r--   0        0        0     9087 2024-04-03 06:56:08.417555 aws_service_screener-2.0.2a2/aws_service_screener/services/eks/drivers/EksCommon.py
--rw-r--r--   0        0        0     3715 2024-04-03 06:56:08.417915 aws_service_screener-2.0.2a2/aws_service_screener/services/eks/eks.reporter.json
--rw-r--r--   0        0        0     8150 2024-04-03 06:56:08.418508 aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/Elasticache.py
--rw-r--r--   0        0        0     2619 2024-04-03 06:56:08.419071 aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheCommon.py
--rw-r--r--   0        0        0      699 2024-04-03 06:56:08.419741 aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheMemcached.py
--rw-r--r--   0        0        0      728 2024-04-03 06:56:08.420098 aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheRedis.py
--rw-r--r--   0        0        0     1192 2024-04-03 06:56:08.420493 aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheReplicationGroup.py
--rw-r--r--   0        0        0     7097 2024-04-03 06:56:08.420850 aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/elasticache.reporter.json
--rw-r--r--   0        0        0      445 2024-04-03 06:56:08.421153 aws_service_screener-2.0.2a2/aws_service_screener/services/general.reporter.json
--rw-r--r--   0        0        0      916 2024-04-03 06:56:08.421596 aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/Guardduty.py
--rw-r--r--   0        0        0    12019 2024-04-03 06:56:08.421956 aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/GuarddutypageBuilder.py
--rw-r--r--   0        0        0       89 2024-04-03 06:56:08.422282 aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/README.md
--rw-r--r--   0        0        0     5159 2024-04-03 06:56:08.424470 aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/drivers/GuarddutyDriver.py
--rw-r--r--   0        0        0      950 2024-04-03 06:56:08.424836 aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/guardduty.reporter.json
--rw-r--r--   0        0        0     6886 2024-04-03 06:56:08.425972 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/Iam.py
--rw-r--r--   0        0        0       84 2024-04-03 06:56:08.426271 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/README.md
--rw-r--r--   0        0        0     8483 2024-04-03 06:56:08.426772 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamAccount.py
--rw-r--r--   0        0        0     3794 2024-04-03 06:56:08.427305 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamCommon.py
--rw-r--r--   0        0        0     1048 2024-04-03 06:56:08.427639 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamGroup.py
--rw-r--r--   0        0        0     2272 2024-04-03 06:56:08.427928 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamRole.py
--rw-r--r--   0        0        0     3785 2024-04-03 06:56:08.428254 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamUser.py
--rw-r--r--   0        0        0    24518 2024-04-03 06:56:08.428548 aws_service_screener-2.0.2a2/aws_service_screener/services/iam/iam.reporter.json
--rw-r--r--   0        0        0     2129 2024-04-03 06:56:08.429042 aws_service_screener-2.0.2a2/aws_service_screener/services/kms/Kms.py
--rw-r--r--   0        0        0     3435 2024-04-03 06:56:08.429553 aws_service_screener-2.0.2a2/aws_service_screener/services/kms/drivers/KmsCommon.py
--rw-r--r--   0        0        0     1329 2024-04-03 06:56:08.429846 aws_service_screener-2.0.2a2/aws_service_screener/services/kms/kms.reporter.json
--rw-r--r--   0        0        0     2773 2024-04-03 06:56:08.430268 aws_service_screener-2.0.2a2/aws_service_screener/services/lambda_/Lambda.py
--rw-r--r--   0        0        0      125 2024-04-03 06:56:08.430546 aws_service_screener-2.0.2a2/aws_service_screener/services/lambda_/README.md
--rw-r--r--   0        0        0     8185 2024-04-03 06:56:08.431002 aws_service_screener-2.0.2a2/aws_service_screener/services/lambda_/drivers/LambdaCommon.py
--rw-r--r--   0        0        0     8167 2024-04-03 06:56:08.431306 aws_service_screener-2.0.2a2/aws_service_screener/services/lambda_/lambda.reporter.json
--rw-r--r--   0        0        0     1863 2024-04-03 06:56:08.431955 aws_service_screener-2.0.2a2/aws_service_screener/services/opensearch/Opensearch.py
--rw-r--r--   0        0        0       82 2024-04-03 06:56:08.432729 aws_service_screener-2.0.2a2/aws_service_screener/services/opensearch/README.md
--rw-r--r--   0        0        0    10966 2024-04-03 06:56:08.433230 aws_service_screener-2.0.2a2/aws_service_screener/services/opensearch/drivers/OpensearchCommon.py
--rw-r--r--   0        0        0    16303 2024-04-03 06:56:08.433636 aws_service_screener-2.0.2a2/aws_service_screener/services/opensearch/opensearch.reporter.json
--rw-r--r--   0        0        0      102 2024-04-03 06:56:08.434098 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/README.md
--rw-r--r--   0        0        0     6476 2024-04-03 06:56:08.434469 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/Rds.py
--rw-r--r--   0        0        0    25380 2024-04-03 06:56:08.435042 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsCommon.py
--rw-r--r--   0        0        0     4201 2024-04-03 06:56:08.435462 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsMssql.py
--rw-r--r--   0        0        0     3101 2024-04-03 06:56:08.435707 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsMysql.py
--rw-r--r--   0        0        0      826 2024-04-03 06:56:08.435937 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsMysqlAurora.py
--rw-r--r--   0        0        0     4077 2024-04-03 06:56:08.436203 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsPostgres.py
--rw-r--r--   0        0        0      237 2024-04-03 06:56:08.436639 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsPostgresAurora.py
--rw-r--r--   0        0        0     1498 2024-04-03 06:56:08.436953 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsSecretsManager.py
--rw-r--r--   0        0        0      928 2024-04-03 06:56:08.437237 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsSecretsVsDB.py
--rw-r--r--   0        0        0     2348 2024-04-03 06:56:08.437596 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsSecurityGroup.py
--rw-r--r--   0        0        0    64958 2024-04-03 06:56:08.438422 aws_service_screener-2.0.2a2/aws_service_screener/services/rds/rds.reporter.json
--rw-r--r--   0        0        0     6148 2024-04-03 06:56:08.439030 aws_service_screener-2.0.2a2/aws_service_screener/services/s3/.DS_Store
--rw-r--r--   0        0        0     4330 2024-04-03 06:56:08.439331 aws_service_screener-2.0.2a2/aws_service_screener/services/s3/S3.py
--rw-r--r--   0        0        0     5469 2024-04-03 06:56:08.439742 aws_service_screener-2.0.2a2/aws_service_screener/services/s3/drivers/S3Bucket.py
--rw-r--r--   0        0        0     1422 2024-04-03 06:56:08.440148 aws_service_screener-2.0.2a2/aws_service_screener/services/s3/drivers/S3Control.py
--rw-r--r--   0        0        0      705 2024-04-03 06:56:08.440385 aws_service_screener-2.0.2a2/aws_service_screener/services/s3/drivers/S3Macie.py
--rw-r--r--   0        0        0     9004 2024-04-03 06:56:08.440747 aws_service_screener-2.0.2a2/aws_service_screener/services/s3/s3.reporter.json
--rw-r--r--   0        0        0      580 2024-04-03 06:56:08.442043 aws_service_screener-2.0.2a2/aws_service_screener/templates/breadcrumb.template.html
--rw-r--r--   0        0        0       15 2024-04-03 06:56:08.442367 aws_service_screener-2.0.2a2/aws_service_screener/templates/footer.postjs.template.html
--rw-r--r--   0        0        0      916 2024-04-03 06:56:08.442648 aws_service_screener-2.0.2a2/aws_service_screener/templates/footer.prejs.template.html
--rw-r--r--   0        0        0     1798 2024-04-03 06:56:08.442933 aws_service_screener-2.0.2a2/aws_service_screener/templates/header.postcss.template.html
--rw-r--r--   0        0        0      182 2024-04-03 06:56:08.443218 aws_service_screener-2.0.2a2/aws_service_screener/templates/header.precss.template.html
--rw-r--r--   0        0        0      387 2024-04-03 06:56:08.443801 aws_service_screener-2.0.2a2/aws_service_screener/templates/sidebar.postcustom.template.html
--rw-r--r--   0        0        0     1266 2024-04-03 06:56:08.444141 aws_service_screener-2.0.2a2/aws_service_screener/templates/sidebar.precustom.template.html
--rw-r--r--   0        0        0     6148 2024-04-03 06:56:08.444808 aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/.DS_Store
--rw-r--r--   0        0        0     5884 2024-04-03 06:56:08.445185 aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/README.md
--rw-r--r--   0        0        0     1324 2024-04-03 06:56:08.445502 aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/crossAccountRoleCF.yml
--rw-r--r--   0        0        0   126803 2024-04-03 06:56:08.447366 aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/static/images/p1-architecture-diagram.png
--rw-r--r--   0        0        0    48532 2024-04-03 06:56:08.448536 aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/static/images/p2-cloudshell.png
--rw-r--r--   0        0        0   156668 2024-04-03 06:56:08.449945 aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/static/images/p3-report.png
--rw-r--r--   0        0        0     3314 2024-04-03 06:56:08.450543 aws_service_screener-2.0.2a2/aws_service_screener/utils/ArguParser.py
--rw-r--r--   0        0        0     3289 2024-04-04 03:11:41.428755 aws_service_screener-2.0.2a2/aws_service_screener/utils/AwsRegionSelector.py
--rw-r--r--   0        0        0     2784 2024-04-04 03:08:36.616950 aws_service_screener-2.0.2a2/aws_service_screener/utils/CfnTrail.py
--rw-r--r--   0        0        0     5086 2024-04-04 03:04:28.098536 aws_service_screener-2.0.2a2/aws_service_screener/utils/Config.py
--rw-r--r--   0        0        0     6409 2024-04-04 03:11:39.993780 aws_service_screener-2.0.2a2/aws_service_screener/utils/CrossAccountsValidator.py
--rw-r--r--   0        0        0     8073 2024-04-04 03:11:47.983030 aws_service_screener-2.0.2a2/aws_service_screener/utils/ExcelBuilder.py
--rw-r--r--   0        0        0     3052 2024-04-03 06:56:08.453050 aws_service_screener-2.0.2a2/aws_service_screener/utils/Policy.py
--rw-r--r--   0        0        0     2259 2024-04-03 06:56:08.453405 aws_service_screener-2.0.2a2/aws_service_screener/utils/RuleReader.py
--rw-r--r--   0        0        0     3543 2024-04-04 03:11:45.199952 aws_service_screener-2.0.2a2/aws_service_screener/utils/Tools.py
--rw-r--r--   0        0        0     2913 2024-04-03 07:13:49.715389 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ArguParser.cpython-312.pyc
--rw-r--r--   0        0        0     2071 2024-04-03 07:23:19.887254 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ArguParser.cpython-39.pyc
--rw-r--r--   0        0        0     4156 2024-04-03 07:13:49.753096 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-312.pyc
--rw-r--r--   0        0        0     2806 2024-04-03 07:23:19.907871 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-39.pyc
--rw-r--r--   0        0        0     4527 2024-04-03 07:13:49.722593 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CfnTrail.cpython-312.pyc
--rw-r--r--   0        0        0     3027 2024-04-03 07:23:19.890810 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CfnTrail.cpython-39.pyc
--rw-r--r--   0        0        0     6093 2024-04-03 07:13:49.708317 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Config.cpython-312.pyc
--rw-r--r--   0        0        0     4262 2024-04-03 07:23:19.885076 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Config.cpython-39.pyc
--rw-r--r--   0        0        0     8336 2024-04-03 07:13:49.750752 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-312.pyc
--rw-r--r--   0        0        0     5385 2024-04-03 07:23:19.906327 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-39.pyc
--rw-r--r--   0        0        0    11358 2024-04-03 07:13:49.790612 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-312.pyc
--rw-r--r--   0        0        0     6742 2024-04-03 07:23:19.935144 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-39.pyc
--rw-r--r--   0        0        0     5749 2024-04-03 07:13:49.725901 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Tools.cpython-312.pyc
--rw-r--r--   0        0        0     4043 2024-04-03 07:23:19.892415 aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Tools.cpython-39.pyc
--rw-r--r--   0        0        0      600 2024-04-04 06:44:19.191640 aws_service_screener-2.0.2a2/pyproject.toml
--rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 aws_service_screener-2.0.2a2/PKG-INFO
+-rw-r--r--   0        0        0    10142 2024-04-03 06:56:08.275195 aws_service_screener-2.0.2a3/LICENSE
+-rwxr-xr-x   0        0        0     6237 2024-04-03 06:56:08.275783 aws_service_screener-2.0.2a3/README.md
+-rw-r--r--   0        0        0     1284 2024-04-03 06:56:08.274112 aws_service_screener-2.0.2a3/aws_service_screener/CreateService.py
+-rw-r--r--   0        0        0     1928 2024-04-04 06:43:18.073637 aws_service_screener-2.0.2a3/aws_service_screener/DocLinkValidity.py
+-rw-r--r--   0        0        0     4044 2024-04-03 06:56:08.276068 aws_service_screener-2.0.2a3/aws_service_screener/RuleCount.py
+-rw-r--r--   0        0        0     8183 2024-04-04 06:44:10.460535 aws_service_screener-2.0.2a3/aws_service_screener/Screener.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:23:50.580521 aws_service_screener-2.0.2a3/aws_service_screener/__fork/tail.txt
+-rw-r--r--   0        0        0        7 2024-04-03 06:56:08.276828 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/.gitignore
+-rw-r--r--   0        0        0     1081 2024-04-03 06:56:08.277048 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/LICENCE.md
+-rw-r--r--   0        0        0  1382975 2024-04-03 06:56:08.280923 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/css/adminlte.min.css
+-rw-r--r--   0        0        0     2637 2024-04-03 06:56:08.285084 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/AdminLTELogo.png
+-rw-r--r--   0        0        0     2391 2024-04-03 06:56:08.285270 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/aws.png
+-rw-r--r--   0        0        0   123766 2024-04-03 06:56:08.285958 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.jpg
+-rw-r--r--   0        0        0    43676 2024-04-03 06:56:08.286257 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.png
+-rw-r--r--   0        0        0      339 2024-04-03 06:56:08.286450 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/default-150x150.png
+-rw-r--r--   0        0        0     1139 2024-04-03 06:56:08.286646 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/icons.png
+-rw-r--r--   0        0        0      942 2024-04-03 06:56:08.286888 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/.eslintrc.json
+-rw-r--r--   0        0        0    99945 2024-04-03 06:56:08.287646 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js
+-rw-r--r--   0        0        0   171653 2024-04-03 06:56:08.288815 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js.map
+-rw-r--r--   0        0        0    44244 2024-04-03 06:56:08.289171 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js
+-rw-r--r--   0        0        0   129651 2024-04-03 06:56:08.289486 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js.map
+-rw-r--r--   0        0        0    22240 2024-04-03 06:56:08.289713 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/demo.js
+-rw-r--r--   0        0        0    84378 2024-04-03 06:56:08.290404 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   173077 2024-04-03 06:56:08.291348 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/chart.js/Chart.min.js
+-rw-r--r--   0        0        0   448232 2024-04-03 06:56:08.302255 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.js
+-rw-r--r--   0        0        0    87956 2024-04-03 06:56:08.304038 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.min.js
+-rw-r--r--   0        0        0     8428 2024-04-03 06:56:08.291858 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.css
+-rw-r--r--   0        0        0     7496 2024-04-03 06:56:08.292112 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.min.css
+-rw-r--r--   0        0        0     4706 2024-04-03 06:56:08.292891 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.js
+-rw-r--r--   0        0        0     4520 2024-04-03 06:56:08.293210 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.min.js
+-rw-r--r--   0        0        0    10415 2024-04-03 06:56:08.293624 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.css
+-rw-r--r--   0        0        0     9000 2024-04-03 06:56:08.293941 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.min.css
+-rw-r--r--   0        0        0     2041 2024-04-03 06:56:08.294355 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.js
+-rw-r--r--   0        0        0     1443 2024-04-03 06:56:08.294712 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.min.js
+-rw-r--r--   0        0        0     6131 2024-04-03 06:56:08.294974 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.js
+-rw-r--r--   0        0        0     3198 2024-04-03 06:56:08.295253 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.min.js
+-rw-r--r--   0        0        0    44471 2024-04-03 06:56:08.295745 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.js
+-rw-r--r--   0        0        0    25103 2024-04-03 06:56:08.296505 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.min.js
+-rw-r--r--   0        0        0     5333 2024-04-03 06:56:08.296882 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.js
+-rw-r--r--   0        0        0     2514 2024-04-03 06:56:08.297178 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.min.js
+-rw-r--r--   0        0        0    60730 2024-04-03 06:56:08.297768 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.js
+-rw-r--r--   0        0        0    25183 2024-04-03 06:56:08.298206 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.min.js
+-rw-r--r--   0        0        0     5091 2024-04-03 06:56:08.298685 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.css
+-rw-r--r--   0        0        0     4301 2024-04-03 06:56:08.298907 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.min.css
+-rw-r--r--   0        0        0    40599 2024-04-03 06:56:08.299383 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.js
+-rw-r--r--   0        0        0    16849 2024-04-03 06:56:08.299793 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.min.js
+-rw-r--r--   0        0        0     1997 2024-04-03 06:56:08.300118 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.js
+-rw-r--r--   0        0        0     3661 2024-04-03 06:56:08.300406 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.min.js
+-rw-r--r--   0        0        0    73625 2024-04-03 06:56:08.304643 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.css
+-rw-r--r--   0        0        0    59344 2024-04-03 06:56:08.305015 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.min.css
+-rw-r--r--   0        0        0      732 2024-04-03 06:56:08.305211 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.css
+-rw-r--r--   0        0        0      675 2024-04-03 06:56:08.305453 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.min.css
+-rw-r--r--   0        0        0    71990 2024-04-03 06:56:08.306103 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.css
+-rw-r--r--   0        0        0    57912 2024-04-03 06:56:08.306614 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.min.css
+-rw-r--r--   0        0        0      734 2024-04-03 06:56:08.306857 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.css
+-rw-r--r--   0        0        0      677 2024-04-03 06:56:08.307135 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.min.css
+-rw-r--r--   0        0        0      727 2024-04-03 06:56:08.307390 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.css
+-rw-r--r--   0        0        0      669 2024-04-03 06:56:08.307583 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.min.css
+-rw-r--r--   0        0        0     8077 2024-04-03 06:56:08.307782 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.css
+-rw-r--r--   0        0        0     6359 2024-04-03 06:56:08.307947 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.min.css
+-rw-r--r--   0        0        0    41312 2024-04-03 06:56:08.308190 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.css
+-rw-r--r--   0        0        0    26702 2024-04-03 06:56:08.308620 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.min.css
+-rw-r--r--   0        0        0   134346 2024-04-03 06:56:08.310346 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   747545 2024-04-03 06:56:08.313956 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   134040 2024-04-03 06:56:08.315427 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    90060 2024-04-03 06:56:08.316187 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    76764 2024-04-03 06:56:08.316763 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    34034 2024-04-03 06:56:08.317519 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   144714 2024-04-03 06:56:08.318696 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    33736 2024-04-03 06:56:08.319302 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    16276 2024-04-03 06:56:08.319839 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    13276 2024-04-03 06:56:08.320181 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   203030 2024-04-03 06:56:08.323786 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   918991 2024-04-03 06:56:08.328886 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   202744 2024-04-03 06:56:08.341995 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   101652 2024-04-03 06:56:08.342791 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    78196 2024-04-03 06:56:08.344104 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    12505 2024-04-03 06:56:08.344800 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/icheck-bootstrap/icheck-bootstrap.min.css
+-rw-r--r--   0        0        0   288579 2024-04-03 06:56:08.349324 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/jquery/jquery.js
+-rw-r--r--   0        0        0    20020 2024-04-03 06:56:08.351376 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/css/OverlayScrollbars.min.css
+-rw-r--r--   0        0        0    42602 2024-04-03 06:56:08.353692 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/js/jquery.overlayScrollbars.min.js
+-rw-r--r--   0        0        0    17358 2024-04-03 06:56:08.354464 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.css
+-rw-r--r--   0        0        0    14966 2024-04-03 06:56:08.354867 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.min.css
+-rw-r--r--   0        0        0      866 2024-04-03 06:56:08.355685 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/af.js
+-rw-r--r--   0        0        0      905 2024-04-03 06:56:08.355962 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ar.js
+-rw-r--r--   0        0        0      721 2024-04-03 06:56:08.356293 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/az.js
+-rw-r--r--   0        0        0      968 2024-04-03 06:56:08.356609 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bg.js
+-rw-r--r--   0        0        0     1291 2024-04-03 06:56:08.356879 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bn.js
+-rw-r--r--   0        0        0      965 2024-04-03 06:56:08.357168 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bs.js
+-rw-r--r--   0        0        0     1802 2024-04-03 06:56:08.357426 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/build.txt
+-rw-r--r--   0        0        0      900 2024-04-03 06:56:08.357721 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ca.js
+-rw-r--r--   0        0        0     1292 2024-04-03 06:56:08.357983 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/cs.js
+-rw-r--r--   0        0        0      828 2024-04-03 06:56:08.358941 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/da.js
+-rw-r--r--   0        0        0      866 2024-04-03 06:56:08.359279 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/de.js
+-rw-r--r--   0        0        0     1017 2024-04-03 06:56:08.359717 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/dsb.js
+-rw-r--r--   0        0        0     1182 2024-04-03 06:56:08.360022 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/el.js
+-rw-r--r--   0        0        0      844 2024-04-03 06:56:08.360329 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/en.js
+-rw-r--r--   0        0        0      922 2024-04-03 06:56:08.360817 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/es.js
+-rw-r--r--   0        0        0      801 2024-04-03 06:56:08.361139 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/et.js
+-rw-r--r--   0        0        0      868 2024-04-03 06:56:08.362358 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/eu.js
+-rw-r--r--   0        0        0     1023 2024-04-03 06:56:08.362678 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fa.js
+-rw-r--r--   0        0        0      803 2024-04-03 06:56:08.363227 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fi.js
+-rw-r--r--   0        0        0      924 2024-04-03 06:56:08.363580 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fr.js
+-rw-r--r--   0        0        0      924 2024-04-03 06:56:08.363932 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/gl.js
+-rw-r--r--   0        0        0      984 2024-04-03 06:56:08.364211 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/he.js
+-rw-r--r--   0        0        0     1175 2024-04-03 06:56:08.364896 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hi.js
+-rw-r--r--   0        0        0      852 2024-04-03 06:56:08.365303 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hr.js
+-rw-r--r--   0        0        0     1018 2024-04-03 06:56:08.365652 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hsb.js
+-rw-r--r--   0        0        0      831 2024-04-03 06:56:08.366120 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hu.js
+-rw-r--r--   0        0        0     1028 2024-04-03 06:56:08.366410 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hy.js
+-rw-r--r--   0        0        0      768 2024-04-03 06:56:08.366776 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/id.js
+-rw-r--r--   0        0        0      807 2024-04-03 06:56:08.367447 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/is.js
+-rw-r--r--   0        0        0      897 2024-04-03 06:56:08.367804 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/it.js
+-rw-r--r--   0        0        0      862 2024-04-03 06:56:08.368128 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ja.js
+-rw-r--r--   0        0        0     1195 2024-04-03 06:56:08.368446 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ka.js
+-rw-r--r--   0        0        0     1088 2024-04-03 06:56:08.368737 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/km.js
+-rw-r--r--   0        0        0      855 2024-04-03 06:56:08.369044 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ko.js
+-rw-r--r--   0        0        0      944 2024-04-03 06:56:08.369350 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lt.js
+-rw-r--r--   0        0        0      900 2024-04-03 06:56:08.369635 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lv.js
+-rw-r--r--   0        0        0     1038 2024-04-03 06:56:08.369971 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/mk.js
+-rw-r--r--   0        0        0      811 2024-04-03 06:56:08.370338 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ms.js
+-rw-r--r--   0        0        0      778 2024-04-03 06:56:08.370603 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nb.js
+-rw-r--r--   0        0        0     1357 2024-04-03 06:56:08.370945 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ne.js
+-rw-r--r--   0        0        0      904 2024-04-03 06:56:08.371332 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nl.js
+-rw-r--r--   0        0        0      947 2024-04-03 06:56:08.371731 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pl.js
+-rw-r--r--   0        0        0     1049 2024-04-03 06:56:08.372074 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ps.js
+-rw-r--r--   0        0        0      876 2024-04-03 06:56:08.372457 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt-BR.js
+-rw-r--r--   0        0        0      878 2024-04-03 06:56:08.372733 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt.js
+-rw-r--r--   0        0        0      938 2024-04-03 06:56:08.373542 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ro.js
+-rw-r--r--   0        0        0     1171 2024-04-03 06:56:08.373888 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ru.js
+-rw-r--r--   0        0        0     1306 2024-04-03 06:56:08.374196 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sk.js
+-rw-r--r--   0        0        0      925 2024-04-03 06:56:08.374466 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sl.js
+-rw-r--r--   0        0        0      903 2024-04-03 06:56:08.374734 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sq.js
+-rw-r--r--   0        0        0     1109 2024-04-03 06:56:08.375015 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr-Cyrl.js
+-rw-r--r--   0        0        0      980 2024-04-03 06:56:08.376266 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr.js
+-rw-r--r--   0        0        0      786 2024-04-03 06:56:08.376792 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sv.js
+-rw-r--r--   0        0        0     1074 2024-04-03 06:56:08.377834 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/th.js
+-rw-r--r--   0        0        0      771 2024-04-03 06:56:08.378568 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tk.js
+-rw-r--r--   0        0        0      775 2024-04-03 06:56:08.378885 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tr.js
+-rw-r--r--   0        0        0     1156 2024-04-03 06:56:08.379156 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/uk.js
+-rw-r--r--   0        0        0      796 2024-04-03 06:56:08.379398 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/vi.js
+-rw-r--r--   0        0        0      768 2024-04-03 06:56:08.379677 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-CN.js
+-rw-r--r--   0        0        0      707 2024-04-03 06:56:08.379918 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-TW.js
+-rw-r--r--   0        0        0   173566 2024-04-03 06:56:08.380849 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.js
+-rw-r--r--   0        0        0    79172 2024-04-03 06:56:08.382426 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.min.js
+-rw-r--r--   0        0        0   153589 2024-04-03 06:56:08.383701 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.js
+-rw-r--r--   0        0        0    70851 2024-04-03 06:56:08.384483 aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.min.js
+-rw-r--r--   0        0        0      658 2024-04-04 06:43:14.502120 aws_service_screener-2.0.2a3/aws_service_screener/constants.py
+-rw-r--r--   0        0        0      399 2024-04-03 06:56:08.385151 aws_service_screener-2.0.2a3/aws_service_screener/crossAccounts.sample.json
+-rw-r--r--   0        0        0      418 2024-04-04 03:25:06.992938 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/FTR.py
+-rw-r--r--   0        0        0      225 2024-04-04 03:24:28.500915 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/FTRPageBuilder.py
+-rw-r--r--   0        0        0     1064 2024-04-03 07:13:49.778355 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-312.pyc
+-rw-r--r--   0        0        0      769 2024-04-03 07:23:19.927246 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-39.pyc
+-rw-r--r--   0        0        0     3166 2024-04-03 06:56:08.386522 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/map.json
+-rw-r--r--   0        0        0     4887 2024-04-04 03:25:14.366928 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/Framework.py
+-rw-r--r--   0        0        0     8928 2024-04-04 03:22:53.875133 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FrameworkPageBuilder.py
+-rw-r--r--   0        0        0      401 2024-04-04 03:24:26.632654 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/.~c9_invoke_T7uTi.py
+-rw-r--r--   0        0        0      936 2024-04-04 03:24:25.840688 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/MSR.py
+-rw-r--r--   0        0        0      225 2024-04-04 03:24:25.150045 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/MSRPageBuilder.py
+-rw-r--r--   0        0        0      230 2024-04-03 06:56:08.389995 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/README.md
+-rw-r--r--   0        0        0     1739 2024-04-03 07:13:49.786617 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-312.pyc
+-rw-r--r--   0        0        0     1253 2024-04-03 07:23:19.932440 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-39.pyc
+-rw-r--r--   0        0        0     3769 2024-04-03 06:56:08.390329 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/map.json
+-rw-r--r--   0        0        0      418 2024-04-04 03:24:24.491532 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/SSB.py
+-rw-r--r--   0        0        0      225 2024-04-04 03:24:23.714161 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/SSBPageBuilder.py
+-rw-r--r--   0        0        0     1064 2024-04-03 07:13:49.782605 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-312.pyc
+-rw-r--r--   0        0        0      769 2024-04-03 07:23:19.930174 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-39.pyc
+-rw-r--r--   0        0        0     3022 2024-04-03 06:56:08.391405 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/map.json
+-rw-r--r--   0        0        0      420 2024-04-04 03:24:22.879011 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/WAFS.py
+-rw-r--r--   0        0        0      246 2024-04-04 03:24:21.731471 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/WAFSPageBuilder.py
+-rw-r--r--   0        0        0     1074 2024-04-03 07:13:49.784295 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-312.pyc
+-rw-r--r--   0        0        0      779 2024-04-03 07:23:19.931200 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-39.pyc
+-rw-r--r--   0        0        0     4321 2024-04-03 06:56:08.393288 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/map.json
+-rw-r--r--   0        0        0     6344 2024-04-03 07:13:49.780725 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/Framework.cpython-312.pyc
+-rw-r--r--   0        0        0     4091 2024-04-03 07:23:19.929148 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/Framework.cpython-39.pyc
+-rw-r--r--   0        0        0    12116 2024-04-03 07:13:49.776696 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-312.pyc
+-rw-r--r--   0        0        0     8235 2024-04-03 07:23:19.926339 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-39.pyc
+-rw-r--r--   0        0        0    21098 2024-04-03 06:56:08.393669 aws_service_screener-2.0.2a3/aws_service_screener/frameworks/api.json
+-rw-r--r--   0        0        0      191 2024-04-03 06:56:08.394469 aws_service_screener-2.0.2a3/aws_service_screener/info.json
+-rw-r--r--   0        0        0    10992 2024-04-04 06:41:23.044965 aws_service_screener-2.0.2a3/aws_service_screener/main.py
+-rwxr-xr-x   0        0        0     5818 2024-04-03 06:56:08.396324 aws_service_screener-2.0.2a3/aws_service_screener/reporter.md
+-rw-r--r--   0        0        0     6148 2024-04-03 06:56:08.397550 aws_service_screener-2.0.2a3/aws_service_screener/services/.DS_Store
+-rw-r--r--   0        0        0     1238 2024-04-04 06:43:17.140786 aws_service_screener-2.0.2a3/aws_service_screener/services/Cloudwatch.py
+-rw-r--r--   0        0        0     4065 2024-04-04 06:43:15.855134 aws_service_screener-2.0.2a3/aws_service_screener/services/Evaluator.py
+-rw-r--r--   0        0        0    30268 2024-04-04 06:43:13.324659 aws_service_screener-2.0.2a3/aws_service_screener/services/PageBuilder.py
+-rw-r--r--   0        0        0    12595 2024-04-04 06:43:36.935738 aws_service_screener-2.0.2a3/aws_service_screener/services/Reporter.py
+-rw-r--r--   0        0        0     3585 2024-04-04 06:43:27.237315 aws_service_screener-2.0.2a3/aws_service_screener/services/Service.py
+-rw-r--r--   0        0        0     1663 2024-04-03 07:13:49.758209 aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Cloudwatch.cpython-312.pyc
+-rw-r--r--   0        0        0     1252 2024-04-03 07:23:19.911843 aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Cloudwatch.cpython-39.pyc
+-rw-r--r--   0        0        0    38925 2024-04-03 07:13:49.769944 aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/PageBuilder.cpython-312.pyc
+-rw-r--r--   0        0        0    24688 2024-04-03 07:23:19.920696 aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/PageBuilder.cpython-39.pyc
+-rw-r--r--   0        0        0    13320 2024-04-03 07:13:49.762194 aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Reporter.cpython-312.pyc
+-rw-r--r--   0        0        0     6990 2024-04-03 07:23:19.914700 aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Reporter.cpython-39.pyc
+-rw-r--r--   0        0        0     1977 2024-04-03 06:56:08.400472 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudfront/Cloudfront.py
+-rw-r--r--   0        0        0     4833 2024-04-03 06:56:08.400787 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudfront/cloudfront.reporter.json
+-rw-r--r--   0        0        0     2929 2024-04-03 06:56:08.401370 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudfront/drivers/cloudfrontDist.py
+-rw-r--r--   0        0        0     3176 2024-04-03 06:56:08.402116 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/Cloudtrail.py
+-rw-r--r--   0        0        0       40 2024-04-03 06:56:08.402377 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/README.md
+-rw-r--r--   0        0        0    13808 2024-04-03 06:56:08.402722 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/cloudtrail.reporter.json
+-rw-r--r--   0        0        0     1235 2024-04-03 06:56:08.403129 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/drivers/CloudtrailAccount.py
+-rw-r--r--   0        0        0     5443 2024-04-03 06:56:08.403404 aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/drivers/CloudtrailCommon.py
+-rw-r--r--   0        0        0     8708 2024-04-04 03:21:56.829424 aws_service_screener-2.0.2a3/aws_service_screener/services/dashboard/DashboardPageBuilder.py
+-rw-r--r--   0        0        0    10171 2024-04-03 07:13:49.773186 aws_service_screener-2.0.2a3/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-312.pyc
+-rw-r--r--   0        0        0     6797 2024-04-03 07:23:19.924057 aws_service_screener-2.0.2a3/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-39.pyc
+-rw-r--r--   0        0        0     3859 2024-04-03 06:56:08.404469 aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/Dynamodb.py
+-rw-r--r--   0        0        0      292 2024-04-03 06:56:08.404923 aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/drivers/DateTimeEncoder.py
+-rw-r--r--   0        0        0    21159 2024-04-03 06:56:08.405306 aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/drivers/DynamoDbCommon.py
+-rw-r--r--   0        0        0     6613 2024-04-03 06:56:08.405672 aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/drivers/DynamoDbGeneric.py
+-rw-r--r--   0        0        0    15863 2024-04-03 06:56:08.406076 aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/dynamodb.reporter.json
+-rw-r--r--   0        0        0    15205 2024-04-03 06:56:08.406726 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/Ec2.py
+-rw-r--r--   0        0        0     4606 2024-04-03 06:56:08.407258 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2AutoScaling.py
+-rw-r--r--   0        0        0      536 2024-04-03 06:56:08.407555 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2CompOpt.py
+-rw-r--r--   0        0        0     1766 2024-04-03 06:56:08.410006 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2CostExplorerRecs.py
+-rw-r--r--   0        0        0      444 2024-04-03 06:56:08.410397 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2EIP.py
+-rw-r--r--   0        0        0      816 2024-04-03 06:56:08.410732 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2EbsSnapshot.py
+-rw-r--r--   0        0        0     4893 2024-04-03 06:56:08.411046 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2EbsVolume.py
+-rw-r--r--   0        0        0     1642 2024-04-03 06:56:08.411341 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2ElbClassic.py
+-rw-r--r--   0        0        0     2897 2024-04-03 06:56:08.411619 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2ElbCommon.py
+-rw-r--r--   0        0        0    10126 2024-04-03 06:56:08.412024 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2Instance.py
+-rw-r--r--   0        0        0     6156 2024-04-03 06:56:08.412551 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2SecGroup.py
+-rw-r--r--   0        0        0    27940 2024-04-03 06:56:08.412919 aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/ec2.reporter.json
+-rw-r--r--   0        0        0     1344 2024-04-03 06:56:08.413639 aws_service_screener-2.0.2a3/aws_service_screener/services/efs/Efs.py
+-rw-r--r--   0        0        0      108 2024-04-03 06:56:08.413983 aws_service_screener-2.0.2a3/aws_service_screener/services/efs/README.md
+-rw-r--r--   0        0        0     1184 2024-04-03 06:56:08.414741 aws_service_screener-2.0.2a3/aws_service_screener/services/efs/drivers/EfsDriver.py
+-rw-r--r--   0        0        0     1485 2024-04-03 06:56:08.415034 aws_service_screener-2.0.2a3/aws_service_screener/services/efs/efs.reporter.json
+-rw-r--r--   0        0        0     2127 2024-04-03 06:56:08.415463 aws_service_screener-2.0.2a3/aws_service_screener/services/eks/Eks.py
+-rw-r--r--   0        0        0       35 2024-04-03 06:56:08.415952 aws_service_screener-2.0.2a3/aws_service_screener/services/eks/README.md
+-rw-r--r--   0        0        0     9087 2024-04-03 06:56:08.417555 aws_service_screener-2.0.2a3/aws_service_screener/services/eks/drivers/EksCommon.py
+-rw-r--r--   0        0        0     3715 2024-04-03 06:56:08.417915 aws_service_screener-2.0.2a3/aws_service_screener/services/eks/eks.reporter.json
+-rw-r--r--   0        0        0     8150 2024-04-03 06:56:08.418508 aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/Elasticache.py
+-rw-r--r--   0        0        0     2619 2024-04-03 06:56:08.419071 aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheCommon.py
+-rw-r--r--   0        0        0      699 2024-04-03 06:56:08.419741 aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheMemcached.py
+-rw-r--r--   0        0        0      728 2024-04-03 06:56:08.420098 aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheRedis.py
+-rw-r--r--   0        0        0     1192 2024-04-03 06:56:08.420493 aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheReplicationGroup.py
+-rw-r--r--   0        0        0     7097 2024-04-03 06:56:08.420850 aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/elasticache.reporter.json
+-rw-r--r--   0        0        0      445 2024-04-03 06:56:08.421153 aws_service_screener-2.0.2a3/aws_service_screener/services/general.reporter.json
+-rw-r--r--   0        0        0      916 2024-04-03 06:56:08.421596 aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/Guardduty.py
+-rw-r--r--   0        0        0    12019 2024-04-03 06:56:08.421956 aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/GuarddutypageBuilder.py
+-rw-r--r--   0        0        0       89 2024-04-03 06:56:08.422282 aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/README.md
+-rw-r--r--   0        0        0     5159 2024-04-03 06:56:08.424470 aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/drivers/GuarddutyDriver.py
+-rw-r--r--   0        0        0      950 2024-04-03 06:56:08.424836 aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/guardduty.reporter.json
+-rw-r--r--   0        0        0     6886 2024-04-03 06:56:08.425972 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/Iam.py
+-rw-r--r--   0        0        0       84 2024-04-03 06:56:08.426271 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/README.md
+-rw-r--r--   0        0        0     8483 2024-04-03 06:56:08.426772 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamAccount.py
+-rw-r--r--   0        0        0     3794 2024-04-03 06:56:08.427305 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamCommon.py
+-rw-r--r--   0        0        0     1048 2024-04-03 06:56:08.427639 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamGroup.py
+-rw-r--r--   0        0        0     2272 2024-04-03 06:56:08.427928 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamRole.py
+-rw-r--r--   0        0        0     3785 2024-04-03 06:56:08.428254 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamUser.py
+-rw-r--r--   0        0        0    24518 2024-04-03 06:56:08.428548 aws_service_screener-2.0.2a3/aws_service_screener/services/iam/iam.reporter.json
+-rw-r--r--   0        0        0     2129 2024-04-03 06:56:08.429042 aws_service_screener-2.0.2a3/aws_service_screener/services/kms/Kms.py
+-rw-r--r--   0        0        0     3435 2024-04-03 06:56:08.429553 aws_service_screener-2.0.2a3/aws_service_screener/services/kms/drivers/KmsCommon.py
+-rw-r--r--   0        0        0     1329 2024-04-03 06:56:08.429846 aws_service_screener-2.0.2a3/aws_service_screener/services/kms/kms.reporter.json
+-rw-r--r--   0        0        0     2773 2024-04-03 06:56:08.430268 aws_service_screener-2.0.2a3/aws_service_screener/services/lambda_/Lambda.py
+-rw-r--r--   0        0        0      125 2024-04-03 06:56:08.430546 aws_service_screener-2.0.2a3/aws_service_screener/services/lambda_/README.md
+-rw-r--r--   0        0        0     8185 2024-04-03 06:56:08.431002 aws_service_screener-2.0.2a3/aws_service_screener/services/lambda_/drivers/LambdaCommon.py
+-rw-r--r--   0        0        0     8167 2024-04-03 06:56:08.431306 aws_service_screener-2.0.2a3/aws_service_screener/services/lambda_/lambda.reporter.json
+-rw-r--r--   0        0        0     1863 2024-04-03 06:56:08.431955 aws_service_screener-2.0.2a3/aws_service_screener/services/opensearch/Opensearch.py
+-rw-r--r--   0        0        0       82 2024-04-03 06:56:08.432729 aws_service_screener-2.0.2a3/aws_service_screener/services/opensearch/README.md
+-rw-r--r--   0        0        0    10966 2024-04-03 06:56:08.433230 aws_service_screener-2.0.2a3/aws_service_screener/services/opensearch/drivers/OpensearchCommon.py
+-rw-r--r--   0        0        0    16303 2024-04-03 06:56:08.433636 aws_service_screener-2.0.2a3/aws_service_screener/services/opensearch/opensearch.reporter.json
+-rw-r--r--   0        0        0      102 2024-04-03 06:56:08.434098 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/README.md
+-rw-r--r--   0        0        0     6476 2024-04-03 06:56:08.434469 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/Rds.py
+-rw-r--r--   0        0        0    25380 2024-04-03 06:56:08.435042 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsCommon.py
+-rw-r--r--   0        0        0     4201 2024-04-03 06:56:08.435462 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsMssql.py
+-rw-r--r--   0        0        0     3101 2024-04-03 06:56:08.435707 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsMysql.py
+-rw-r--r--   0        0        0      826 2024-04-03 06:56:08.435937 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsMysqlAurora.py
+-rw-r--r--   0        0        0     4077 2024-04-03 06:56:08.436203 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsPostgres.py
+-rw-r--r--   0        0        0      237 2024-04-03 06:56:08.436639 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsPostgresAurora.py
+-rw-r--r--   0        0        0     1498 2024-04-03 06:56:08.436953 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsSecretsManager.py
+-rw-r--r--   0        0        0      928 2024-04-03 06:56:08.437237 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsSecretsVsDB.py
+-rw-r--r--   0        0        0     2348 2024-04-03 06:56:08.437596 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsSecurityGroup.py
+-rw-r--r--   0        0        0    64958 2024-04-03 06:56:08.438422 aws_service_screener-2.0.2a3/aws_service_screener/services/rds/rds.reporter.json
+-rw-r--r--   0        0        0     6148 2024-04-03 06:56:08.439030 aws_service_screener-2.0.2a3/aws_service_screener/services/s3/.DS_Store
+-rw-r--r--   0        0        0     4330 2024-04-03 06:56:08.439331 aws_service_screener-2.0.2a3/aws_service_screener/services/s3/S3.py
+-rw-r--r--   0        0        0     5469 2024-04-03 06:56:08.439742 aws_service_screener-2.0.2a3/aws_service_screener/services/s3/drivers/S3Bucket.py
+-rw-r--r--   0        0        0     1422 2024-04-03 06:56:08.440148 aws_service_screener-2.0.2a3/aws_service_screener/services/s3/drivers/S3Control.py
+-rw-r--r--   0        0        0      705 2024-04-03 06:56:08.440385 aws_service_screener-2.0.2a3/aws_service_screener/services/s3/drivers/S3Macie.py
+-rw-r--r--   0        0        0     9004 2024-04-03 06:56:08.440747 aws_service_screener-2.0.2a3/aws_service_screener/services/s3/s3.reporter.json
+-rw-r--r--   0        0        0      580 2024-04-03 06:56:08.442043 aws_service_screener-2.0.2a3/aws_service_screener/templates/breadcrumb.template.html
+-rw-r--r--   0        0        0       15 2024-04-03 06:56:08.442367 aws_service_screener-2.0.2a3/aws_service_screener/templates/footer.postjs.template.html
+-rw-r--r--   0        0        0      916 2024-04-03 06:56:08.442648 aws_service_screener-2.0.2a3/aws_service_screener/templates/footer.prejs.template.html
+-rw-r--r--   0        0        0     1798 2024-04-03 06:56:08.442933 aws_service_screener-2.0.2a3/aws_service_screener/templates/header.postcss.template.html
+-rw-r--r--   0        0        0      182 2024-04-03 06:56:08.443218 aws_service_screener-2.0.2a3/aws_service_screener/templates/header.precss.template.html
+-rw-r--r--   0        0        0      387 2024-04-03 06:56:08.443801 aws_service_screener-2.0.2a3/aws_service_screener/templates/sidebar.postcustom.template.html
+-rw-r--r--   0        0        0     1266 2024-04-03 06:56:08.444141 aws_service_screener-2.0.2a3/aws_service_screener/templates/sidebar.precustom.template.html
+-rw-r--r--   0        0        0     6148 2024-04-03 06:56:08.444808 aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/.DS_Store
+-rw-r--r--   0        0        0     5884 2024-04-03 06:56:08.445185 aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/README.md
+-rw-r--r--   0        0        0     1324 2024-04-03 06:56:08.445502 aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/crossAccountRoleCF.yml
+-rw-r--r--   0        0        0   126803 2024-04-03 06:56:08.447366 aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/static/images/p1-architecture-diagram.png
+-rw-r--r--   0        0        0    48532 2024-04-03 06:56:08.448536 aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/static/images/p2-cloudshell.png
+-rw-r--r--   0        0        0   156668 2024-04-03 06:56:08.449945 aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/static/images/p3-report.png
+-rw-r--r--   0        0        0     3314 2024-04-03 06:56:08.450543 aws_service_screener-2.0.2a3/aws_service_screener/utils/ArguParser.py
+-rw-r--r--   0        0        0     3289 2024-04-04 03:11:41.428755 aws_service_screener-2.0.2a3/aws_service_screener/utils/AwsRegionSelector.py
+-rw-r--r--   0        0        0     2784 2024-04-04 03:08:36.616950 aws_service_screener-2.0.2a3/aws_service_screener/utils/CfnTrail.py
+-rw-r--r--   0        0        0     5086 2024-04-04 03:04:28.098536 aws_service_screener-2.0.2a3/aws_service_screener/utils/Config.py
+-rw-r--r--   0        0        0     6409 2024-04-04 03:11:39.993780 aws_service_screener-2.0.2a3/aws_service_screener/utils/CrossAccountsValidator.py
+-rw-r--r--   0        0        0     8073 2024-04-04 03:11:47.983030 aws_service_screener-2.0.2a3/aws_service_screener/utils/ExcelBuilder.py
+-rw-r--r--   0        0        0     3052 2024-04-03 06:56:08.453050 aws_service_screener-2.0.2a3/aws_service_screener/utils/Policy.py
+-rw-r--r--   0        0        0     2259 2024-04-03 06:56:08.453405 aws_service_screener-2.0.2a3/aws_service_screener/utils/RuleReader.py
+-rw-r--r--   0        0        0     3543 2024-04-04 03:11:45.199952 aws_service_screener-2.0.2a3/aws_service_screener/utils/Tools.py
+-rw-r--r--   0        0        0     2913 2024-04-03 07:13:49.715389 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ArguParser.cpython-312.pyc
+-rw-r--r--   0        0        0     2071 2024-04-03 07:23:19.887254 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ArguParser.cpython-39.pyc
+-rw-r--r--   0        0        0     4156 2024-04-03 07:13:49.753096 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-312.pyc
+-rw-r--r--   0        0        0     2806 2024-04-03 07:23:19.907871 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-39.pyc
+-rw-r--r--   0        0        0     4527 2024-04-03 07:13:49.722593 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CfnTrail.cpython-312.pyc
+-rw-r--r--   0        0        0     3027 2024-04-03 07:23:19.890810 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CfnTrail.cpython-39.pyc
+-rw-r--r--   0        0        0     6093 2024-04-03 07:13:49.708317 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Config.cpython-312.pyc
+-rw-r--r--   0        0        0     4262 2024-04-03 07:23:19.885076 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Config.cpython-39.pyc
+-rw-r--r--   0        0        0     8336 2024-04-03 07:13:49.750752 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-312.pyc
+-rw-r--r--   0        0        0     5385 2024-04-03 07:23:19.906327 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-39.pyc
+-rw-r--r--   0        0        0    11358 2024-04-03 07:13:49.790612 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-312.pyc
+-rw-r--r--   0        0        0     6742 2024-04-03 07:23:19.935144 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-39.pyc
+-rw-r--r--   0        0        0     5749 2024-04-03 07:13:49.725901 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Tools.cpython-312.pyc
+-rw-r--r--   0        0        0     4043 2024-04-03 07:23:19.892415 aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Tools.cpython-39.pyc
+-rw-r--r--   0        0        0      646 2024-04-05 03:26:20.154182 aws_service_screener-2.0.2a3/pyproject.toml
+-rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 aws_service_screener-2.0.2a3/PKG-INFO
```

### Comparing `aws_service_screener-2.0.2a2/LICENSE` & `aws_service_screener-2.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/README.md` & `aws_service_screener-2.0.2a3/README.md`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/CreateService.py` & `aws_service_screener-2.0.2a3/aws_service_screener/CreateService.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/DocLinkValidity.py` & `aws_service_screener-2.0.2a3/aws_service_screener/DocLinkValidity.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/RuleCount.py` & `aws_service_screener-2.0.2a3/aws_service_screener/RuleCount.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/Screener.py` & `aws_service_screener-2.0.2a3/aws_service_screener/Screener.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/LICENCE.md` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/LICENCE.md`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/css/adminlte.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/css/adminlte.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/AdminLTELogo.png` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/AdminLTELogo.png`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/aws.png` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/aws.png`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.jpg` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.jpg`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.png` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/boxed-bg.png`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/img/icons.png` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/img/icons.png`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/.eslintrc.json` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js.map` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.js.map`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js.map` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/adminlte.min.js.map`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/dist/js/demo.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/dist/js/demo.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/bootstrap/js/bootstrap.bundle.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/chart.js/Chart.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/css/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-bs4/js/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/css/buttons.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.colVis.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/buttons.print.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-buttons/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/css/responsive.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/datatables-responsive/js/responsive.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.eot` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.svg` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.ttf` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff2` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.eot` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.svg` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.ttf` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff2` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.eot` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.svg` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.ttf` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff2` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/icheck-bootstrap/icheck-bootstrap.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/icheck-bootstrap/icheck-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/jquery/jquery.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/css/OverlayScrollbars.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/css/OverlayScrollbars.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/js/jquery.overlayScrollbars.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/overlayScrollbars/js/jquery.overlayScrollbars.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.min.css` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/af.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ar.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/az.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bg.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bn.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bs.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/build.txt` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/build.txt`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ca.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/cs.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/da.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/de.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/dsb.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/el.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/en.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/es.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/et.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/eu.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fa.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fi.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fr.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/gl.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/he.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hi.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hr.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hsb.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hu.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hy.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/id.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/is.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/it.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ja.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ka.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/km.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ko.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lt.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lv.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/mk.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ms.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nb.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ne.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nl.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pl.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ps.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt-BR.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ro.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ru.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sk.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sl.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sq.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr-Cyrl.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sv.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/th.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tk.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tr.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/uk.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/vi.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-CN.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-TW.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.min.js` & `aws_service_screener-2.0.2a3/aws_service_screener/adminlte/aws/res/plugins/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/constants.py` & `aws_service_screener-2.0.2a3/aws_service_screener/constants.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/__pycache__/FTR.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FTR/map.json` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FTR/map.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/Framework.py` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/Framework.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/FrameworkPageBuilder.py` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/FrameworkPageBuilder.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/MSR.py` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/MSR.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/__pycache__/MSR.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/MSR/map.json` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/MSR/map.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/__pycache__/SSB.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/SSB/map.json` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/SSB/map.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/__pycache__/WAFS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/WAFS/map.json` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/WAFS/map.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/Framework.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/Framework.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/Framework.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/Framework.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/__pycache__/FrameworkPageBuilder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/frameworks/api.json` & `aws_service_screener-2.0.2a3/aws_service_screener/frameworks/api.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/main.py` & `aws_service_screener-2.0.2a3/aws_service_screener/main.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/reporter.md` & `aws_service_screener-2.0.2a3/aws_service_screener/reporter.md`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/.DS_Store` & `aws_service_screener-2.0.2a3/aws_service_screener/services/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/Cloudwatch.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/Cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/Evaluator.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/Evaluator.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/PageBuilder.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/PageBuilder.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/Reporter.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/Reporter.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/Service.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/Service.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Cloudwatch.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Cloudwatch.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Cloudwatch.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Cloudwatch.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/PageBuilder.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/PageBuilder.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/PageBuilder.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/PageBuilder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Reporter.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Reporter.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/__pycache__/Reporter.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/__pycache__/Reporter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/cloudfront/Cloudfront.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/cloudfront/Cloudfront.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/cloudfront/cloudfront.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/cloudfront/cloudfront.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/cloudfront/drivers/cloudfrontDist.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/cloudfront/drivers/cloudfrontDist.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/Cloudtrail.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/Cloudtrail.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/cloudtrail.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/cloudtrail.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/drivers/CloudtrailAccount.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/drivers/CloudtrailAccount.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/cloudtrail/drivers/CloudtrailCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/cloudtrail/drivers/CloudtrailCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/dashboard/DashboardPageBuilder.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/dashboard/DashboardPageBuilder.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/services/dashboard/__pycache__/DashboardPageBuilder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/Dynamodb.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/Dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/drivers/DynamoDbCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/drivers/DynamoDbCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/drivers/DynamoDbGeneric.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/drivers/DynamoDbGeneric.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/dynamodb/dynamodb.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/dynamodb/dynamodb.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/Ec2.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/Ec2.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2AutoScaling.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2AutoScaling.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2CompOpt.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2CompOpt.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2CostExplorerRecs.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2CostExplorerRecs.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2EbsSnapshot.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2EbsSnapshot.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2EbsVolume.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2EbsVolume.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2ElbClassic.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2ElbClassic.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2ElbCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2ElbCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2Instance.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2Instance.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/drivers/Ec2SecGroup.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/drivers/Ec2SecGroup.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/ec2/ec2.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/ec2/ec2.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/efs/Efs.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/efs/Efs.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/efs/drivers/EfsDriver.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/efs/drivers/EfsDriver.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/efs/efs.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/efs/efs.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/eks/Eks.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/eks/Eks.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/eks/drivers/EksCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/eks/drivers/EksCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/eks/eks.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/eks/eks.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/Elasticache.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/Elasticache.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheMemcached.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheMemcached.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheRedis.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheRedis.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/drivers/ElasticacheReplicationGroup.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/drivers/ElasticacheReplicationGroup.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/elasticache/elasticache.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/elasticache/elasticache.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/Guardduty.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/Guardduty.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/GuarddutypageBuilder.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/GuarddutypageBuilder.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/drivers/GuarddutyDriver.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/drivers/GuarddutyDriver.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/guardduty/guardduty.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/guardduty/guardduty.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/iam/Iam.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/iam/Iam.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamAccount.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamAccount.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamGroup.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamGroup.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamRole.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamRole.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/iam/drivers/IamUser.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/iam/drivers/IamUser.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/iam/iam.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/iam/iam.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/kms/Kms.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/kms/Kms.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/kms/drivers/KmsCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/kms/drivers/KmsCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/kms/kms.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/kms/kms.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/lambda_/Lambda.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/lambda_/Lambda.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/lambda_/drivers/LambdaCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/lambda_/drivers/LambdaCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/lambda_/lambda.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/lambda_/lambda.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/opensearch/Opensearch.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/opensearch/Opensearch.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/opensearch/drivers/OpensearchCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/opensearch/drivers/OpensearchCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/opensearch/opensearch.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/opensearch/opensearch.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/Rds.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/Rds.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsCommon.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsCommon.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsMssql.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsMssql.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsMysql.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsMysql.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsMysqlAurora.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsMysqlAurora.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsPostgres.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsPostgres.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsSecretsManager.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsSecretsManager.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsSecretsVsDB.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsSecretsVsDB.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/drivers/RdsSecurityGroup.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/drivers/RdsSecurityGroup.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/rds/rds.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/rds/rds.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/s3/.DS_Store` & `aws_service_screener-2.0.2a3/aws_service_screener/services/s3/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/s3/S3.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/s3/S3.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/s3/drivers/S3Bucket.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/s3/drivers/S3Bucket.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/s3/drivers/S3Control.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/s3/drivers/S3Control.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/s3/drivers/S3Macie.py` & `aws_service_screener-2.0.2a3/aws_service_screener/services/s3/drivers/S3Macie.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/services/s3/s3.reporter.json` & `aws_service_screener-2.0.2a3/aws_service_screener/services/s3/s3.reporter.json`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/templates/breadcrumb.template.html` & `aws_service_screener-2.0.2a3/aws_service_screener/templates/breadcrumb.template.html`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/templates/footer.prejs.template.html` & `aws_service_screener-2.0.2a3/aws_service_screener/templates/footer.prejs.template.html`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/templates/header.postcss.template.html` & `aws_service_screener-2.0.2a3/aws_service_screener/templates/header.postcss.template.html`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/templates/sidebar.precustom.template.html` & `aws_service_screener-2.0.2a3/aws_service_screener/templates/sidebar.precustom.template.html`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/.DS_Store` & `aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/README.md` & `aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/README.md`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/crossAccountRoleCF.yml` & `aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/crossAccountRoleCF.yml`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/static/images/p1-architecture-diagram.png` & `aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/static/images/p1-architecture-diagram.png`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/static/images/p2-cloudshell.png` & `aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/static/images/p2-cloudshell.png`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/usecases/crossAccounts/static/images/p3-report.png` & `aws_service_screener-2.0.2a3/aws_service_screener/usecases/crossAccounts/static/images/p3-report.png`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/ArguParser.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/ArguParser.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/AwsRegionSelector.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/AwsRegionSelector.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/CfnTrail.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/CfnTrail.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/Config.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/Config.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/CrossAccountsValidator.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/CrossAccountsValidator.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/ExcelBuilder.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/ExcelBuilder.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/Policy.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/Policy.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/RuleReader.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/RuleReader.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/Tools.py` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ArguParser.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ArguParser.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ArguParser.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ArguParser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/AwsRegionSelector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CfnTrail.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CfnTrail.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CfnTrail.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CfnTrail.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Config.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Config.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Config.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/CrossAccountsValidator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/ExcelBuilder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Tools.cpython-312.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Tools.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/aws_service_screener/utils/__pycache__/Tools.cpython-39.pyc` & `aws_service_screener-2.0.2a3/aws_service_screener/utils/__pycache__/Tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aws_service_screener-2.0.2a2/pyproject.toml` & `aws_service_screener-2.0.2a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-service-screener"
-version = "2.0.2-alpha2"
+version = "2.0.2-alpha3"
 description = "An open source guidance tool for AWS environments"
 authors = ["AWS <aws-gh-ss@amazon.com>"]
 license = "Apache 2.0 license"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -19,8 +19,9 @@
 black = "^24.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-aws-screen = 'aws_service_screener.main:main'
+screener = 'aws_service_screener.main:main'
+aws-screener = 'aws_service_screener.main:main'
```

### Comparing `aws_service_screener-2.0.2a2/PKG-INFO` & `aws_service_screener-2.0.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-service-screener
-Version: 2.0.2a2
+Version: 2.0.2a3
 Summary: An open source guidance tool for AWS environments
 License: Apache 2.0 license
 Author: AWS
 Author-email: aws-gh-ss@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

