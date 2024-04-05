# Comparing `tmp/mrml-0.1.7.tar.gz` & `tmp/mrml-0.1.8.tar.gz`

## Comparing `mrml-0.1.7.tar` & `mrml-0.1.8.tar`

### file list

```diff
@@ -1,271 +1,271 @@
--rw-r--r--   0     1001      127      417 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/Cargo.toml
--rw-r--r--   0     1001      127     6862 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/resources/expected.html
--rw-r--r--   0     1001      127     6862 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/resources/generated.html
--rw-r--r--   0     1001      127     8375 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/src/error.rs
--rw-r--r--   0     1001      127       88 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/src/helper.rs
--rw-r--r--   0     1001      127    16944 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/src/lib.rs
--rw-r--r--   0     1001      127    10088 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/src/stack.rs
--rw-r--r--   0     1001      127     1544 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/html-compare/src/token.rs
--rw-r--r--   0     1001      127      613 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-macros/Cargo.toml
--rw-r--r--   0     1001      127      639 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-macros/CHANGELOG.md
--rw-r--r--   0     1001      127     5175 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-macros/license.md
--rw-r--r--   0     1001      127     5256 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-macros/readme.md
--rw-r--r--   0     1001      127     2825 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-macros/src/children.rs
--rw-r--r--   0     1001      127      171 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-macros/src/lib.rs
--rw-r--r--   0     1001      127     5256 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/readme.md
--rw-r--r--   0     1001      127      481 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/common-macros/Cargo.toml
--rw-r--r--   0     1001      127      720 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/common-macros/CHANGELOG.md
--rw-r--r--   0     1001      127     5175 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/common-macros/license.md
--rw-r--r--   0     1001      127     5256 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/common-macros/readme.md
--rw-r--r--   0     1001      127     4312 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/common-macros/src/lib.rs
--rw-r--r--   0     1001      127     2491 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/Cargo.toml
--rw-r--r--   0     1001      127     5175 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/license.md
--rw-r--r--   0     1001      127      677 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/comment/json.rs
--rw-r--r--   0     1001      127      592 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/comment/mod.rs
--rw-r--r--   0     1001      127      637 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/comment/print.rs
--rw-r--r--   0     1001      127     2059 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/comment/render.rs
--rw-r--r--   0     1001      127     1027 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/helper/condition.rs
--rw-r--r--   0     1001      127      278 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/helper/mod.rs
--rw-r--r--   0     1001      127     3783 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/helper/size.rs
--rw-r--r--   0     1001      127      133 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/helper/sort.rs
--rw-r--r--   0     1001      127     2953 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/helper/spacing.rs
--rw-r--r--   0     1001      127     1198 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/helper/style.rs
--rw-r--r--   0     1001      127     4296 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/helper/tag.rs
--rw-r--r--   0     1001      127     7933 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/lib.rs
--rw-r--r--   0     1001      127      380 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/macros.rs
--rw-r--r--   0     1001      127      423 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion/children.rs
--rw-r--r--   0     1001      127      881 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion/json.rs
--rw-r--r--   0     1001      127     3821 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion/mod.rs
--rw-r--r--   0     1001      127     4853 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion/parse.rs
--rw-r--r--   0     1001      127     1709 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion/print.rs
--rw-r--r--   0     1001      127     5911 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion/render.rs
--rw-r--r--   0     1001      127      507 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/children.rs
--rw-r--r--   0     1001      127     3109 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/json.rs
--rw-r--r--   0     1001      127     1021 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/mod.rs
--rw-r--r--   0     1001      127     4446 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/parse.rs
--rw-r--r--   0     1001      127      608 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/print.rs
--rw-r--r--   0     1001      127     5394 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/render.rs
--rw-r--r--   0     1001      127      938 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/json.rs
--rw-r--r--   0     1001      127      655 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/mod.rs
--rw-r--r--   0     1001      127     1570 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/parse.rs
--rw-r--r--   0     1001      127      239 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/print.rs
--rw-r--r--   0     1001      127     3438 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/render.rs
--rw-r--r--   0     1001      127      930 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/json.rs
--rw-r--r--   0     1001      127      643 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/mod.rs
--rw-r--r--   0     1001      127     2421 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/parse.rs
--rw-r--r--   0     1001      127      242 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/print.rs
--rw-r--r--   0     1001      127     4811 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/render.rs
--rw-r--r--   0     1001      127      555 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes/children.rs
--rw-r--r--   0     1001      127      958 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes/json.rs
--rw-r--r--   0     1001      127      668 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes/mod.rs
--rw-r--r--   0     1001      127     4468 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes/parse.rs
--rw-r--r--   0     1001      127      228 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes/print.rs
--rw-r--r--   0     1001      127      611 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_all/json.rs
--rw-r--r--   0     1001      127      651 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_all/mod.rs
--rw-r--r--   0     1001      127     1251 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_all/parse.rs
--rw-r--r--   0     1001      127      228 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_all/print.rs
--rw-r--r--   0     1001      127     2786 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/json.rs
--rw-r--r--   0     1001      127      634 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/mod.rs
--rw-r--r--   0     1001      127     1941 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/parse.rs
--rw-r--r--   0     1001      127      678 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/print.rs
--rw-r--r--   0     1001      127     2824 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/json.rs
--rw-r--r--   0     1001      127      590 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/mod.rs
--rw-r--r--   0     1001      127     1474 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/parse.rs
--rw-r--r--   0     1001      127      686 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/print.rs
--rw-r--r--   0     1001      127     2846 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_body/children.rs
--rw-r--r--   0     1001      127      816 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_body/json.rs
--rw-r--r--   0     1001      127      652 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_body/mod.rs
--rw-r--r--   0     1001      127    10055 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_body/parse.rs
--rw-r--r--   0     1001      127      683 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_body/print.rs
--rw-r--r--   0     1001      127     3395 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_body/render.rs
--rw-r--r--   0     1001      127     1154 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_breakpoint/json.rs
--rw-r--r--   0     1001      127      934 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_breakpoint/mod.rs
--rw-r--r--   0     1001      127     2074 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_breakpoint/parse.rs
--rw-r--r--   0     1001      127      402 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_breakpoint/print.rs
--rw-r--r--   0     1001      127      828 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_button/json.rs
--rw-r--r--   0     1001      127      643 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_button/mod.rs
--rw-r--r--   0     1001      127     1373 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_button/parse.rs
--rw-r--r--   0     1001      127      702 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_button/print.rs
--rw-r--r--   0     1001      127     7987 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_button/render.rs
--rw-r--r--   0     1001      127      410 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel/children.rs
--rw-r--r--   0     1001      127      817 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel/json.rs
--rw-r--r--   0     1001      127      668 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel/mod.rs
--rw-r--r--   0     1001      127     3987 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel/parse.rs
--rw-r--r--   0     1001      127      532 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel/print.rs
--rw-r--r--   0     1001      127    18955 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel/render.rs
--rw-r--r--   0     1001      127      771 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/json.rs
--rw-r--r--   0     1001      127      589 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/mod.rs
--rw-r--r--   0     1001      127     1077 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/parse.rs
--rw-r--r--   0     1001      127      393 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/print.rs
--rw-r--r--   0     1001      127     7597 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/render.rs
--rw-r--r--   0     1001      127      711 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_column/json.rs
--rw-r--r--   0     1001      127      643 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_column/mod.rs
--rw-r--r--   0     1001      127      981 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_column/parse.rs
--rw-r--r--   0     1001      127      216 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_column/print.rs
--rw-r--r--   0     1001      127    12537 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_column/render.rs
--rw-r--r--   0     1001      127      584 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_divider/json.rs
--rw-r--r--   0     1001      127      576 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_divider/mod.rs
--rw-r--r--   0     1001      127     1026 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_divider/parse.rs
--rw-r--r--   0     1001      127      373 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_divider/print.rs
--rw-r--r--   0     1001      127     4014 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_divider/render.rs
--rw-r--r--   0     1001      127     1268 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_font/json.rs
--rw-r--r--   0     1001      127      902 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_font/mod.rs
--rw-r--r--   0     1001      127     2226 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_font/parse.rs
--rw-r--r--   0     1001      127      498 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_font/print.rs
--rw-r--r--   0     1001      127      705 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_group/json.rs
--rw-r--r--   0     1001      127      641 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_group/mod.rs
--rw-r--r--   0     1001      127      974 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_group/parse.rs
--rw-r--r--   0     1001      127      213 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_group/print.rs
--rw-r--r--   0     1001      127     7454 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_group/render.rs
--rw-r--r--   0     1001      127      795 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_head/children.rs
--rw-r--r--   0     1001      127      679 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_head/json.rs
--rw-r--r--   0     1001      127     2551 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_head/mod.rs
--rw-r--r--   0     1001      127     6345 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_head/parse.rs
--rw-r--r--   0     1001      127     1379 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_head/print.rs
--rw-r--r--   0     1001      127    13408 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_head/render.rs
--rw-r--r--   0     1001      127      699 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_hero/json.rs
--rw-r--r--   0     1001      127      639 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_hero/mod.rs
--rw-r--r--   0     1001      127      967 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_hero/parse.rs
--rw-r--r--   0     1001      127      210 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_hero/print.rs
--rw-r--r--   0     1001      127    12811 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_hero/render.rs
--rw-r--r--   0     1001      127      735 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_image/json.rs
--rw-r--r--   0     1001      127      572 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_image/mod.rs
--rw-r--r--   0     1001      127      988 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_image/parse.rs
--rw-r--r--   0     1001      127      333 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_image/print.rs
--rw-r--r--   0     1001      127     7223 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_image/render.rs
--rw-r--r--   0     1001      127     1437 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/body/json.rs
--rw-r--r--   0     1001      127     3269 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/body/mod.rs
--rw-r--r--   0     1001      127    17724 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/body/parse.rs
--rw-r--r--   0     1001      127     1525 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/body/print.rs
--rw-r--r--   0     1001      127     5043 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/body/render.rs
--rw-r--r--   0     1001      127     2806 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/head/json.rs
--rw-r--r--   0     1001      127     2506 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/head/mod.rs
--rw-r--r--   0     1001      127    15328 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/head/parse.rs
--rw-r--r--   0     1001      127     1717 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/head/print.rs
--rw-r--r--   0     1001      127     5410 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/head/render.rs
--rw-r--r--   0     1001      127     2499 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_include/mod.rs
--rw-r--r--   0     1001      127      396 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar/children.rs
--rw-r--r--   0     1001      127      715 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar/json.rs
--rw-r--r--   0     1001      127      660 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar/mod.rs
--rw-r--r--   0     1001      127     4392 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar/parse.rs
--rw-r--r--   0     1001      127      216 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar/print.rs
--rw-r--r--   0     1001      127     8342 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar/render.rs
--rw-r--r--   0     1001      127      763 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/json.rs
--rw-r--r--   0     1001      127      649 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/mod.rs
--rw-r--r--   0     1001      127     1690 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/parse.rs
--rw-r--r--   0     1001      127      384 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/print.rs
--rw-r--r--   0     1001      127     5198 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/render.rs
--rw-r--r--   0     1001      127      564 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_preview/json.rs
--rw-r--r--   0     1001      127      823 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_preview/mod.rs
--rw-r--r--   0     1001      127     1394 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_preview/parse.rs
--rw-r--r--   0     1001      127      372 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_preview/print.rs
--rw-r--r--   0     1001      127      410 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_raw/children.rs
--rw-r--r--   0     1001      127      727 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_raw/json.rs
--rw-r--r--   0     1001      127      575 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_raw/mod.rs
--rw-r--r--   0     1001      127     5086 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_raw/parse.rs
--rw-r--r--   0     1001      127      207 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_raw/print.rs
--rw-r--r--   0     1001      127     2025 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_raw/render.rs
--rw-r--r--   0     1001      127      717 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_section/json.rs
--rw-r--r--   0     1001      127      735 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_section/mod.rs
--rw-r--r--   0     1001      127     1019 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_section/parse.rs
--rw-r--r--   0     1001      127      219 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_section/print.rs
--rw-r--r--   0     1001      127    19151 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_section/render.rs
--rw-r--r--   0     1001      127      408 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social/children.rs
--rw-r--r--   0     1001      127      742 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social/json.rs
--rw-r--r--   0     1001      127      660 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social/mod.rs
--rw-r--r--   0     1001      127     4410 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social/parse.rs
--rw-r--r--   0     1001      127      216 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social/print.rs
--rw-r--r--   0     1001      127     6990 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social/render.rs
--rw-r--r--   0     1001      127      761 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social_element/json.rs
--rw-r--r--   0     1001      127      695 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social_element/mod.rs
--rw-r--r--   0     1001      127     5938 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social_element/network.rs
--rw-r--r--   0     1001      127     1472 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social_element/parse.rs
--rw-r--r--   0     1001      127      393 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social_element/print.rs
--rw-r--r--   0     1001      127     8511 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_social_element/render.rs
--rw-r--r--   0     1001      127      578 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_spacer/json.rs
--rw-r--r--   0     1001      127      574 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_spacer/mod.rs
--rw-r--r--   0     1001      127      995 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_spacer/parse.rs
--rw-r--r--   0     1001      127      336 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_spacer/print.rs
--rw-r--r--   0     1001      127     1591 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_spacer/render.rs
--rw-r--r--   0     1001      127      684 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_style/json.rs
--rw-r--r--   0     1001      127     1370 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_style/mod.rs
--rw-r--r--   0     1001      127     3091 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_style/parse.rs
--rw-r--r--   0     1001      127      326 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_style/print.rs
--rw-r--r--   0     1001      127      705 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_table/json.rs
--rw-r--r--   0     1001      127      666 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_table/mod.rs
--rw-r--r--   0     1001      127      974 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_table/parse.rs
--rw-r--r--   0     1001      127      213 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_table/print.rs
--rw-r--r--   0     1001      127     3555 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_table/render.rs
--rw-r--r--   0     1001      127      699 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_text/json.rs
--rw-r--r--   0     1001      127      639 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_text/mod.rs
--rw-r--r--   0     1001      127     1168 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_text/parse.rs
--rw-r--r--   0     1001      127      473 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_text/print.rs
--rw-r--r--   0     1001      127     4403 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_text/render.rs
--rw-r--r--   0     1001      127      552 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_title/json.rs
--rw-r--r--   0     1001      127      813 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_title/mod.rs
--rw-r--r--   0     1001      127     1274 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_title/parse.rs
--rw-r--r--   0     1001      127      326 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_title/print.rs
--rw-r--r--   0     1001      127      717 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_wrapper/json.rs
--rw-r--r--   0     1001      127      670 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_wrapper/mod.rs
--rw-r--r--   0     1001      127     1237 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_wrapper/parse.rs
--rw-r--r--   0     1001      127      219 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_wrapper/print.rs
--rw-r--r--   0     1001      127     4516 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mj_wrapper/render.rs
--rw-r--r--   0     1001      127     2651 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mjml/json.rs
--rw-r--r--   0     1001      127     1712 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mjml/mod.rs
--rw-r--r--   0     1001      127    10277 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mjml/parse.rs
--rw-r--r--   0     1001      127      838 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mjml/print.rs
--rw-r--r--   0     1001      127     3767 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/mjml/render.rs
--rw-r--r--   0     1001      127      771 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/node/json.rs
--rw-r--r--   0     1001      127     1012 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/node/mod.rs
--rw-r--r--   0     1001      127     1542 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/node/print.rs
--rw-r--r--   0     1001      127     2612 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/node/render.rs
--rw-r--r--   0     1001      127     2794 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/hash.rs
--rw-r--r--   0     1001      127      141 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/mod.rs
--rw-r--r--   0     1001      127    20701 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/parser/http_loader.rs
--rw-r--r--   0     1001      127     3664 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/parser/loader.rs
--rw-r--r--   0     1001      127     5563 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/parser/local_loader.rs
--rw-r--r--   0     1001      127     2592 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/parser/memory_loader.rs
--rw-r--r--   0     1001      127    17713 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/parser/mod.rs
--rw-r--r--   0     1001      127    10546 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/parser/multi_loader.rs
--rw-r--r--   0     1001      127     1523 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/parser/noop_loader.rs
--rw-r--r--   0     1001      127     1721 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/print.rs
--rw-r--r--   0     1001      127    14010 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/prelude/render.rs
--rw-r--r--   0     1001      127     1393 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/text/json.rs
--rw-r--r--   0     1001      127      442 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/text/mod.rs
--rw-r--r--   0     1001      127      571 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/text/print.rs
--rw-r--r--   0     1001      127      788 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/src/text/render.rs
--rw-r--r--   0     1001      127      655 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/Cargo.toml
--rw-r--r--   0     1001      127      664 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/CHANGELOG.md
--rw-r--r--   0     1001      127     5175 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/license.md
--rw-r--r--   0     1001      127     5256 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/readme.md
--rw-r--r--   0     1001      127    12145 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/src/element.rs
--rw-r--r--   0     1001      127      188 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/src/lib.rs
--rw-r--r--   0     1001      127      638 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/Cargo.toml
--rw-r--r--   0     1001      127      669 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/CHANGELOG.md
--rw-r--r--   0     1001      127     5175 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/license.md
--rw-r--r--   0     1001      127     5256 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/readme.md
--rw-r--r--   0     1001      127     1828 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/attributes.rs
--rw-r--r--   0     1001      127     4215 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/children.rs
--rw-r--r--   0     1001      127     7174 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/element.rs
--rw-r--r--   0     1001      127      957 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/lib.rs
--rw-r--r--   0     1001      127      459 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/css-compare/Cargo.toml
--rw-r--r--   0     1001      127      448 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/css-compare/CHANGELOG.md
--rw-r--r--   0     1001      127    11777 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-core/lib/css-compare/src/lib.rs
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 mrml-0.1.7/packages/mrml-python/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/.gitignore
--rw-r--r--   0     1001      127     1821 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/CHANGELOG.md
--rw-r--r--   0     1001      127     5175 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/license.md
--rw-r--r--   0     1001      127      682 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/readme.md
--rw-r--r--   0     1001      127        8 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/requirements.txt
--rw-r--r--   0     1001      127       31 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/resources/partials/hello-world.mjml
--rw-r--r--   0     1001      127      214 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/resources/with-http-include.mjml
--rw-r--r--   0     1001      127       91 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/resources/with-local-include.mjml
--rw-r--r--   0     1001      127      265 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/resources/with-multi-include.mjml
--rw-r--r--   0     1001      127     7194 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/src/lib.rs
--rw-r--r--   0     1001      127     3515 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/tests/test_loader.py
--rw-r--r--   0     1001      127      499 2024-03-15 18:29:19.000000 mrml-0.1.7/packages/mrml-python/tests/test_main.py
--rw-r--r--   0     1001      127    64821 2024-03-15 18:29:19.000000 mrml-0.1.7/Cargo.lock
--rw-r--r--   0        0        0       62 1970-01-01 00:00:00.000000 mrml-0.1.7/Cargo.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 mrml-0.1.7/pyproject.toml
--rw-r--r--   0     1001      127      682 2024-03-15 18:29:19.000000 mrml-0.1.7/readme.md
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 mrml-0.1.7/PKG-INFO
+-rw-r--r--   0     1001      127      613 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-macros/Cargo.toml
+-rw-r--r--   0     1001      127      639 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-macros/CHANGELOG.md
+-rw-r--r--   0     1001      127     5175 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-macros/license.md
+-rw-r--r--   0     1001      127     5256 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-macros/readme.md
+-rw-r--r--   0     1001      127     2825 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-macros/src/children.rs
+-rw-r--r--   0     1001      127      171 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-macros/src/lib.rs
+-rw-r--r--   0     1001      127     5256 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/readme.md
+-rw-r--r--   0     1001      127      638 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/Cargo.toml
+-rw-r--r--   0     1001      127      669 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/CHANGELOG.md
+-rw-r--r--   0     1001      127     5175 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/license.md
+-rw-r--r--   0     1001      127     5256 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/readme.md
+-rw-r--r--   0     1001      127     1828 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/attributes.rs
+-rw-r--r--   0     1001      127     4215 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/children.rs
+-rw-r--r--   0     1001      127     7174 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/element.rs
+-rw-r--r--   0     1001      127      957 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/lib.rs
+-rw-r--r--   0     1001      127      459 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/css-compare/Cargo.toml
+-rw-r--r--   0     1001      127      448 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/css-compare/CHANGELOG.md
+-rw-r--r--   0     1001      127    11777 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/css-compare/src/lib.rs
+-rw-r--r--   0     1001      127     2491 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/Cargo.toml
+-rw-r--r--   0     1001      127     5175 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/license.md
+-rw-r--r--   0     1001      127      677 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/comment/json.rs
+-rw-r--r--   0     1001      127      592 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/comment/mod.rs
+-rw-r--r--   0     1001      127      637 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/comment/print.rs
+-rw-r--r--   0     1001      127     2059 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/comment/render.rs
+-rw-r--r--   0     1001      127     1027 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/helper/condition.rs
+-rw-r--r--   0     1001      127      278 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/helper/mod.rs
+-rw-r--r--   0     1001      127     3783 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/helper/size.rs
+-rw-r--r--   0     1001      127      133 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/helper/sort.rs
+-rw-r--r--   0     1001      127     2953 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/helper/spacing.rs
+-rw-r--r--   0     1001      127     1198 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/helper/style.rs
+-rw-r--r--   0     1001      127     4296 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/helper/tag.rs
+-rw-r--r--   0     1001      127    10501 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/lib.rs
+-rw-r--r--   0     1001      127      380 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/macros.rs
+-rw-r--r--   0     1001      127      423 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion/children.rs
+-rw-r--r--   0     1001      127      881 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion/json.rs
+-rw-r--r--   0     1001      127     3821 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion/mod.rs
+-rw-r--r--   0     1001      127     5055 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion/parse.rs
+-rw-r--r--   0     1001      127     1709 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion/print.rs
+-rw-r--r--   0     1001      127     5911 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion/render.rs
+-rw-r--r--   0     1001      127      507 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/children.rs
+-rw-r--r--   0     1001      127     3109 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/json.rs
+-rw-r--r--   0     1001      127     1021 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/mod.rs
+-rw-r--r--   0     1001      127     4648 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/parse.rs
+-rw-r--r--   0     1001      127      608 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/print.rs
+-rw-r--r--   0     1001      127     5394 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/render.rs
+-rw-r--r--   0     1001      127      938 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/json.rs
+-rw-r--r--   0     1001      127      655 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/mod.rs
+-rw-r--r--   0     1001      127     1671 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/parse.rs
+-rw-r--r--   0     1001      127      239 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/print.rs
+-rw-r--r--   0     1001      127     3438 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/render.rs
+-rw-r--r--   0     1001      127      930 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/json.rs
+-rw-r--r--   0     1001      127      643 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/mod.rs
+-rw-r--r--   0     1001      127     2623 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/parse.rs
+-rw-r--r--   0     1001      127      242 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/print.rs
+-rw-r--r--   0     1001      127     4811 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/render.rs
+-rw-r--r--   0     1001      127      555 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes/children.rs
+-rw-r--r--   0     1001      127      958 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes/json.rs
+-rw-r--r--   0     1001      127     1968 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes/mod.rs
+-rw-r--r--   0     1001      127     4771 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes/parse.rs
+-rw-r--r--   0     1001      127      228 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes/print.rs
+-rw-r--r--   0     1001      127      611 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_all/json.rs
+-rw-r--r--   0     1001      127      651 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_all/mod.rs
+-rw-r--r--   0     1001      127     1352 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_all/parse.rs
+-rw-r--r--   0     1001      127      228 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_all/print.rs
+-rw-r--r--   0     1001      127     2786 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/json.rs
+-rw-r--r--   0     1001      127      656 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/mod.rs
+-rw-r--r--   0     1001      127     2042 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/parse.rs
+-rw-r--r--   0     1001      127      678 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/print.rs
+-rw-r--r--   0     1001      127     2824 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/json.rs
+-rw-r--r--   0     1001      127      612 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/mod.rs
+-rw-r--r--   0     1001      127     1575 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/parse.rs
+-rw-r--r--   0     1001      127      686 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/print.rs
+-rw-r--r--   0     1001      127     2846 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_body/children.rs
+-rw-r--r--   0     1001      127      816 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_body/json.rs
+-rw-r--r--   0     1001      127      652 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_body/mod.rs
+-rw-r--r--   0     1001      127    10459 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_body/parse.rs
+-rw-r--r--   0     1001      127      683 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_body/print.rs
+-rw-r--r--   0     1001      127     3395 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_body/render.rs
+-rw-r--r--   0     1001      127     1154 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_breakpoint/json.rs
+-rw-r--r--   0     1001      127      934 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_breakpoint/mod.rs
+-rw-r--r--   0     1001      127     2175 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_breakpoint/parse.rs
+-rw-r--r--   0     1001      127      402 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_breakpoint/print.rs
+-rw-r--r--   0     1001      127      828 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_button/json.rs
+-rw-r--r--   0     1001      127      643 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_button/mod.rs
+-rw-r--r--   0     1001      127     1474 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_button/parse.rs
+-rw-r--r--   0     1001      127      702 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_button/print.rs
+-rw-r--r--   0     1001      127     7987 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_button/render.rs
+-rw-r--r--   0     1001      127      410 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel/children.rs
+-rw-r--r--   0     1001      127      817 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel/json.rs
+-rw-r--r--   0     1001      127      668 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel/mod.rs
+-rw-r--r--   0     1001      127     4189 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel/parse.rs
+-rw-r--r--   0     1001      127      532 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel/print.rs
+-rw-r--r--   0     1001      127    18955 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel/render.rs
+-rw-r--r--   0     1001      127      771 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/json.rs
+-rw-r--r--   0     1001      127      589 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/mod.rs
+-rw-r--r--   0     1001      127     1178 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/parse.rs
+-rw-r--r--   0     1001      127      393 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/print.rs
+-rw-r--r--   0     1001      127     7597 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/render.rs
+-rw-r--r--   0     1001      127      711 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_column/json.rs
+-rw-r--r--   0     1001      127      643 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_column/mod.rs
+-rw-r--r--   0     1001      127     1082 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_column/parse.rs
+-rw-r--r--   0     1001      127      216 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_column/print.rs
+-rw-r--r--   0     1001      127    12537 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_column/render.rs
+-rw-r--r--   0     1001      127      584 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_divider/json.rs
+-rw-r--r--   0     1001      127      576 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_divider/mod.rs
+-rw-r--r--   0     1001      127     1127 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_divider/parse.rs
+-rw-r--r--   0     1001      127      373 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_divider/print.rs
+-rw-r--r--   0     1001      127     4014 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_divider/render.rs
+-rw-r--r--   0     1001      127     1268 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_font/json.rs
+-rw-r--r--   0     1001      127     1200 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_font/mod.rs
+-rw-r--r--   0     1001      127     2327 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_font/parse.rs
+-rw-r--r--   0     1001      127      498 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_font/print.rs
+-rw-r--r--   0     1001      127      705 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_group/json.rs
+-rw-r--r--   0     1001      127      641 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_group/mod.rs
+-rw-r--r--   0     1001      127     1075 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_group/parse.rs
+-rw-r--r--   0     1001      127      213 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_group/print.rs
+-rw-r--r--   0     1001      127     7454 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_group/render.rs
+-rw-r--r--   0     1001      127      795 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_head/children.rs
+-rw-r--r--   0     1001      127      679 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_head/json.rs
+-rw-r--r--   0     1001      127     2717 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_head/mod.rs
+-rw-r--r--   0     1001      127     6648 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_head/parse.rs
+-rw-r--r--   0     1001      127     1379 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_head/print.rs
+-rw-r--r--   0     1001      127    20297 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_head/render.rs
+-rw-r--r--   0     1001      127      699 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_hero/json.rs
+-rw-r--r--   0     1001      127      639 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_hero/mod.rs
+-rw-r--r--   0     1001      127     1068 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_hero/parse.rs
+-rw-r--r--   0     1001      127      210 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_hero/print.rs
+-rw-r--r--   0     1001      127    12811 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_hero/render.rs
+-rw-r--r--   0     1001      127      735 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_image/json.rs
+-rw-r--r--   0     1001      127      572 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_image/mod.rs
+-rw-r--r--   0     1001      127     1089 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_image/parse.rs
+-rw-r--r--   0     1001      127      333 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_image/print.rs
+-rw-r--r--   0     1001      127     7223 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_image/render.rs
+-rw-r--r--   0     1001      127     1437 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/body/json.rs
+-rw-r--r--   0     1001      127     3269 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/body/mod.rs
+-rw-r--r--   0     1001      127    18027 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/body/parse.rs
+-rw-r--r--   0     1001      127     1525 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/body/print.rs
+-rw-r--r--   0     1001      127     5043 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/body/render.rs
+-rw-r--r--   0     1001      127     2806 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/head/json.rs
+-rw-r--r--   0     1001      127     2506 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/head/mod.rs
+-rw-r--r--   0     1001      127    15631 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/head/parse.rs
+-rw-r--r--   0     1001      127     1717 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/head/print.rs
+-rw-r--r--   0     1001      127     7495 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/head/render.rs
+-rw-r--r--   0     1001      127     2503 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_include/mod.rs
+-rw-r--r--   0     1001      127      396 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar/children.rs
+-rw-r--r--   0     1001      127      715 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar/json.rs
+-rw-r--r--   0     1001      127      660 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar/mod.rs
+-rw-r--r--   0     1001      127     4594 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar/parse.rs
+-rw-r--r--   0     1001      127      216 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar/print.rs
+-rw-r--r--   0     1001      127     8342 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar/render.rs
+-rw-r--r--   0     1001      127      763 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/json.rs
+-rw-r--r--   0     1001      127      649 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/mod.rs
+-rw-r--r--   0     1001      127     1791 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/parse.rs
+-rw-r--r--   0     1001      127      384 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/print.rs
+-rw-r--r--   0     1001      127     5198 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/render.rs
+-rw-r--r--   0     1001      127      564 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_preview/json.rs
+-rw-r--r--   0     1001      127      823 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_preview/mod.rs
+-rw-r--r--   0     1001      127     1495 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_preview/parse.rs
+-rw-r--r--   0     1001      127      372 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_preview/print.rs
+-rw-r--r--   0     1001      127      410 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_raw/children.rs
+-rw-r--r--   0     1001      127      727 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_raw/json.rs
+-rw-r--r--   0     1001      127      575 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_raw/mod.rs
+-rw-r--r--   0     1001      127     5389 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_raw/parse.rs
+-rw-r--r--   0     1001      127      207 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_raw/print.rs
+-rw-r--r--   0     1001      127     2025 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_raw/render.rs
+-rw-r--r--   0     1001      127      717 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_section/json.rs
+-rw-r--r--   0     1001      127      735 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_section/mod.rs
+-rw-r--r--   0     1001      127     1120 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_section/parse.rs
+-rw-r--r--   0     1001      127      219 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_section/print.rs
+-rw-r--r--   0     1001      127    19151 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_section/render.rs
+-rw-r--r--   0     1001      127      408 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social/children.rs
+-rw-r--r--   0     1001      127      742 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social/json.rs
+-rw-r--r--   0     1001      127      660 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social/mod.rs
+-rw-r--r--   0     1001      127     4612 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social/parse.rs
+-rw-r--r--   0     1001      127      216 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social/print.rs
+-rw-r--r--   0     1001      127     6990 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social/render.rs
+-rw-r--r--   0     1001      127      761 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social_element/json.rs
+-rw-r--r--   0     1001      127      695 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social_element/mod.rs
+-rw-r--r--   0     1001      127     5938 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social_element/network.rs
+-rw-r--r--   0     1001      127     1573 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social_element/parse.rs
+-rw-r--r--   0     1001      127      393 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social_element/print.rs
+-rw-r--r--   0     1001      127     8511 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_social_element/render.rs
+-rw-r--r--   0     1001      127      578 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_spacer/json.rs
+-rw-r--r--   0     1001      127      574 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_spacer/mod.rs
+-rw-r--r--   0     1001      127     1096 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_spacer/parse.rs
+-rw-r--r--   0     1001      127      336 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_spacer/print.rs
+-rw-r--r--   0     1001      127     1591 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_spacer/render.rs
+-rw-r--r--   0     1001      127      684 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_style/json.rs
+-rw-r--r--   0     1001      127     1370 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_style/mod.rs
+-rw-r--r--   0     1001      127     3192 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_style/parse.rs
+-rw-r--r--   0     1001      127      326 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_style/print.rs
+-rw-r--r--   0     1001      127      705 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_table/json.rs
+-rw-r--r--   0     1001      127      666 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_table/mod.rs
+-rw-r--r--   0     1001      127     1075 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_table/parse.rs
+-rw-r--r--   0     1001      127      213 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_table/print.rs
+-rw-r--r--   0     1001      127     3555 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_table/render.rs
+-rw-r--r--   0     1001      127      699 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_text/json.rs
+-rw-r--r--   0     1001      127      639 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_text/mod.rs
+-rw-r--r--   0     1001      127     1269 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_text/parse.rs
+-rw-r--r--   0     1001      127      473 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_text/print.rs
+-rw-r--r--   0     1001      127     4403 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_text/render.rs
+-rw-r--r--   0     1001      127      552 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_title/json.rs
+-rw-r--r--   0     1001      127      813 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_title/mod.rs
+-rw-r--r--   0     1001      127     1375 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_title/parse.rs
+-rw-r--r--   0     1001      127      326 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_title/print.rs
+-rw-r--r--   0     1001      127      717 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_wrapper/json.rs
+-rw-r--r--   0     1001      127      670 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_wrapper/mod.rs
+-rw-r--r--   0     1001      127     1338 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_wrapper/parse.rs
+-rw-r--r--   0     1001      127      219 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_wrapper/print.rs
+-rw-r--r--   0     1001      127     4516 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mj_wrapper/render.rs
+-rw-r--r--   0     1001      127     2651 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mjml/json.rs
+-rw-r--r--   0     1001      127     1712 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mjml/mod.rs
+-rw-r--r--   0     1001      127    10483 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mjml/parse.rs
+-rw-r--r--   0     1001      127      838 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mjml/print.rs
+-rw-r--r--   0     1001      127     3767 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/mjml/render.rs
+-rw-r--r--   0     1001      127      771 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/node/json.rs
+-rw-r--r--   0     1001      127     1012 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/node/mod.rs
+-rw-r--r--   0     1001      127     1542 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/node/print.rs
+-rw-r--r--   0     1001      127     2612 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/node/render.rs
+-rw-r--r--   0     1001      127     2794 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/hash.rs
+-rw-r--r--   0     1001      127      141 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/mod.rs
+-rw-r--r--   0     1001      127    21011 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/parser/http_loader.rs
+-rw-r--r--   0     1001      127     3714 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/parser/loader.rs
+-rw-r--r--   0     1001      127     5664 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/parser/local_loader.rs
+-rw-r--r--   0     1001      127     2638 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/parser/memory_loader.rs
+-rw-r--r--   0     1001      127    17921 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/parser/mod.rs
+-rw-r--r--   0     1001      127    10643 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/parser/multi_loader.rs
+-rw-r--r--   0     1001      127     1574 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/parser/noop_loader.rs
+-rw-r--r--   0     1001      127     1721 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/print.rs
+-rw-r--r--   0     1001      127    14010 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/prelude/render.rs
+-rw-r--r--   0     1001      127     1393 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/text/json.rs
+-rw-r--r--   0     1001      127      442 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/text/mod.rs
+-rw-r--r--   0     1001      127      571 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/text/print.rs
+-rw-r--r--   0     1001      127      788 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-core/src/text/render.rs
+-rw-r--r--   0     1001      127      655 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/Cargo.toml
+-rw-r--r--   0     1001      127      664 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/CHANGELOG.md
+-rw-r--r--   0     1001      127     5175 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/license.md
+-rw-r--r--   0     1001      127     5256 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/readme.md
+-rw-r--r--   0     1001      127    12145 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/src/element.rs
+-rw-r--r--   0     1001      127      188 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/src/lib.rs
+-rw-r--r--   0     1001      127      481 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/common-macros/Cargo.toml
+-rw-r--r--   0     1001      127      720 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/common-macros/CHANGELOG.md
+-rw-r--r--   0     1001      127     5175 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/common-macros/license.md
+-rw-r--r--   0     1001      127     5256 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/common-macros/readme.md
+-rw-r--r--   0     1001      127     4312 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/common-macros/src/lib.rs
+-rw-r--r--   0     1001      127      417 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/Cargo.toml
+-rw-r--r--   0     1001      127     6862 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/resources/expected.html
+-rw-r--r--   0     1001      127     6862 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/resources/generated.html
+-rw-r--r--   0     1001      127     8375 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/src/error.rs
+-rw-r--r--   0     1001      127       88 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/src/helper.rs
+-rw-r--r--   0     1001      127    16944 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/src/lib.rs
+-rw-r--r--   0     1001      127    10088 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/src/stack.rs
+-rw-r--r--   0     1001      127     1544 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-core/lib/html-compare/src/token.rs
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 mrml-0.1.8/packages/mrml-python/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/.gitignore
+-rw-r--r--   0     1001      127     1983 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/CHANGELOG.md
+-rw-r--r--   0     1001      127     5175 2024-03-19 09:51:27.000000 mrml-0.1.8/packages/mrml-python/license.md
+-rw-r--r--   0     1001      127      682 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/readme.md
+-rw-r--r--   0     1001      127        8 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/requirements.txt
+-rw-r--r--   0     1001      127       31 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/resources/partials/hello-world.mjml
+-rw-r--r--   0     1001      127      214 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/resources/with-http-include.mjml
+-rw-r--r--   0     1001      127       91 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/resources/with-local-include.mjml
+-rw-r--r--   0     1001      127      265 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/resources/with-multi-include.mjml
+-rw-r--r--   0     1001      127     7194 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/src/lib.rs
+-rw-r--r--   0     1001      127     3515 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/tests/test_loader.py
+-rw-r--r--   0     1001      127      499 2024-03-19 09:51:28.000000 mrml-0.1.8/packages/mrml-python/tests/test_main.py
+-rw-r--r--   0     1001      127    72382 2024-03-19 09:51:27.000000 mrml-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0       62 1970-01-01 00:00:00.000000 mrml-0.1.8/Cargo.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 mrml-0.1.8/pyproject.toml
+-rw-r--r--   0     1001      127      682 2024-03-19 09:51:28.000000 mrml-0.1.8/readme.md
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 mrml-0.1.8/PKG-INFO
```

### Comparing `mrml-0.1.7/packages/mrml-core/lib/html-compare/resources/expected.html` & `mrml-0.1.8/packages/mrml-core/lib/html-compare/resources/expected.html`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/html-compare/resources/generated.html` & `mrml-0.1.8/packages/mrml-core/lib/html-compare/resources/generated.html`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/html-compare/src/error.rs` & `mrml-0.1.8/packages/mrml-core/lib/html-compare/src/error.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/html-compare/src/lib.rs` & `mrml-0.1.8/packages/mrml-core/lib/html-compare/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/html-compare/src/stack.rs` & `mrml-0.1.8/packages/mrml-core/lib/html-compare/src/stack.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/html-compare/src/token.rs` & `mrml-0.1.8/packages/mrml-core/lib/html-compare/src/token.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-macros/Cargo.toml` & `mrml-0.1.8/packages/mrml-core/lib/mrml-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-macros/CHANGELOG.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-macros/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-macros/license.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-macros/license.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-macros/readme.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-macros/readme.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-macros/src/children.rs` & `mrml-0.1.8/packages/mrml-core/lib/mrml-macros/src/children.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/readme.md` & `mrml-0.1.8/packages/mrml-core/readme.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/common-macros/CHANGELOG.md` & `mrml-0.1.8/packages/mrml-core/lib/common-macros/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/common-macros/license.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/license.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/common-macros/readme.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/readme.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/common-macros/src/lib.rs` & `mrml-0.1.8/packages/mrml-core/lib/common-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/Cargo.toml` & `mrml-0.1.8/packages/mrml-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "mrml"
 description = "Rust implementation of MJML renderer"
 keywords = ["email", "mjml"]
-version = "3.1.0"
+version = "3.1.1"
 authors = ["Jérémie Drouet <jeremie.drouet@gmail.com>"]
 edition = "2018"
 license-file = "license.md"
 repository = "https://github.com/jdrouet/mrml/"
 readme = "readme.md"
 
 include = ["src/*", "Cargo.toml"]
```

### Comparing `mrml-0.1.7/packages/mrml-core/license.md` & `mrml-0.1.8/packages/mrml-core/license.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/comment/json.rs` & `mrml-0.1.8/packages/mrml-core/src/comment/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/comment/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/comment/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/comment/print.rs` & `mrml-0.1.8/packages/mrml-core/src/comment/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/comment/render.rs` & `mrml-0.1.8/packages/mrml-core/src/comment/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/helper/condition.rs` & `mrml-0.1.8/packages/mrml-core/src/helper/condition.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/helper/size.rs` & `mrml-0.1.8/packages/mrml-core/src/helper/size.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/helper/spacing.rs` & `mrml-0.1.8/packages/mrml-core/src/helper/spacing.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/helper/style.rs` & `mrml-0.1.8/packages/mrml-core/src/helper/style.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/helper/tag.rs` & `mrml-0.1.8/packages/mrml-core/src/helper/tag.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/lib.rs` & `mrml-0.1.8/packages/mrml-core/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,121 @@
 //! This project is a reimplementation of the nice [MJML](https://mjml.io/) markup language in Rust.
 //!
-//! [![codecov](https://codecov.io/gh/jolimail/mrml-core/branch/main/graph/badge.svg?token=SIOPR0YWZA)](https://codecov.io/gh/jolimail/mrml-core)
-//! [![.github/workflows/main.yml](https://github.com/jolimail/mrml-core/actions/workflows/main.yml/badge.svg)](https://github.com/jolimail/mrml-core/actions/workflows/main.yml)
-//! [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/jolimail/mrml-core.svg)](http://isitmaintained.com/project/jolimail/mrml-core "Average time to resolve an issue")
-//! [![Percentage of issues still open](http://isitmaintained.com/badge/open/jolimail/mrml-core.svg)](http://isitmaintained.com/project/jolimail/mrml-core "Percentage of issues still open")
-//! [![Maintainability](https://api.codeclimate.com/v1/badges/7ed23ef670d076ab69a4/maintainability)](https://codeclimate.com/github/jolimail/mrml-core/maintainability)
+//! [![.github/workflows/main.yml](https://github.com/jdrouet/mrml/actions/workflows/mrml-core-main.yml/badge.svg)](https://github.com/jdrouet/mrml/actions/workflows/mrml-core-main.yml)
+//! [![codecov](https://codecov.io/gh/jdrouet/mrml/branch/main/graph/badge.svg?token=SIOPR0YWZA)](https://codecov.io/gh/jdrouet/mrml)
+//! [![Maintainability](https://api.codeclimate.com/v1/badges/7ed23ef670d076ab69a4/maintainability)](https://codeclimate.com/github/jdrouet/mrml/maintainability)
+//!
+//! # How to use?
 //!
 //! To use it you can simply update your `Cargo.toml` by adding
 //! ```toml
 //! [dependencies]
-//! mrml = "1.2"
-//! serde = { version = "1.0", features = ["derive"] }
+//! mrml = { version = "3" }
+//! serde = { version = "1", features = ["derive"] }
 //! ```
 //!
 //! And you can then just create a `main.rs` with the following code
 //! ```rust
+//! # #[cfg(feature = "parse")]
+//! # {
 //! let root = mrml::parse("<mjml><mj-body></mj-body></mjml>").expect("parse template");
 //! let opts = mrml::prelude::render::Options::default();
 //! match root.render(&opts) {
 //!     Ok(content) => println!("{}", content),
 //!     Err(_) => println!("couldn't render mjml template"),
 //! };
+//! # }
 //! ```
 //!
+//! ## Using `mj-include`
+//!
 //! You can also use the `mj-include` component by specifying a
-//! [loader](crate::prelude::parse).
+//! [loader](crate::prelude::parser).
 //!
 //! ```rust
+//! # #[cfg(feature = "parse")]
+//! # {
 //! use mrml::prelude::parser::ParserOptions;
 //! use mrml::prelude::parser::memory_loader::MemoryIncludeLoader;
 //!
 //! let loader = MemoryIncludeLoader::from(vec![("partial.mjml", "<mj-button>Hello</mj-button>")]);
 //! let options = ParserOptions {
 //!     include_loader: Box::new(loader),
 //! };
 //! match mrml::parse_with_options("<mjml><mj-head /><mj-body><mj-include path=\"partial.mjml\" /></mj-body></mjml>", &options) {
 //!     Ok(_) => println!("Success!"),
 //!     Err(err) => eprintln!("Something went wrong: {err:?}"),
 //! }
+//! # }
+//! ```
+//!
+//! ## Using `mj-include` with an async loader
+//!
+//! If you want to use the async version to fetch the includes, you've to enable the `async` feature and the required loaders (`http-loader-async-reqwest` in this example).
+//!
+//! ```rust
+//! # #[cfg(all(feature = "parse", feature = "render", feature = "async"))]
+//! # tokio_test::block_on(async {
+//! use mrml::prelude::parser::http_loader::{AsyncReqwestFetcher, HttpIncludeLoader};
+//! use mrml::prelude::parser::memory_loader::MemoryIncludeLoader;
+//! use mrml::prelude::parser::local_loader::LocalIncludeLoader;
+//! use mrml::prelude::parser::multi_loader::MultiIncludeLoader;
+//! use mrml::prelude::parser::noop_loader::NoopIncludeLoader;
+//! use mrml::prelude::parser::loader::AsyncIncludeLoader;
+//! use mrml::prelude::parser::AsyncParserOptions;
+//! use mrml::prelude::render::RenderOptions;
+//! use std::path::PathBuf;
+//! use std::sync::Arc;
+//!
+//! let resolver = MultiIncludeLoader::<Box<dyn AsyncIncludeLoader + Send + Sync + 'static>>::new()
+//!     .with_starts_with("memory://", Box::new(MemoryIncludeLoader::from(vec![("basic.mjml", "<mj-button>Hello</mj-button>")])))
+//!     .with_starts_with("file://", Box::new(LocalIncludeLoader::new(PathBuf::default().join("resources").join("compare").join("success"))))
+//!     .with_starts_with("https://", Box::new(HttpIncludeLoader::<AsyncReqwestFetcher>::allow_all()))
+//!     .with_any(Box::<NoopIncludeLoader>::default());
+//! let parser_options = AsyncParserOptions {
+//!     include_loader: Box::new(resolver),
+//! };
+//! let render_options = RenderOptions::default();
+//! let json = r#"<mjml>
+//! <mj-body>
+//! <mj-include path="file://basic.mjml" />
+//! <mj-include path="memory://basic.mjml" />
+//! </mj-body>
+//! </mjml>"#;
+//! match mrml::async_parse_with_options(json, Arc::new(parser_options)).await {
+//!     Ok(mjml) => match mjml.render(&render_options) {
+//!         Ok(html) => println!("{html}"),
+//!         Err(err) => eprintln!("Couldn't render template: {err:?}"),
+//!     },
+//!     Err(err) => eprintln!("Couldn't parse template: {err:?}"),
+//! }
+//! # })
+//! ```
+//!
+//! ## Using `mrml` in Python
+//!
+//! This crate can also be used in Python. The crate is available with pypi and
+//! you can find some documentation [here](https://pypi.org/project/mrml/).
+//!
+//! ```python
+//! import mrml
+//!
+//! # without options
+//! result = mrml.to_html("<mjml></mjml>")
+//! assert result.startswith("<!doctype html>")
+//!
+//! # with options
+//! parser_options = mrml.ParserOptions(include_loader = mrml.memory_loader({
+//!     'hello-world.mjml': '<mj-text>Hello World!</mj-text>',
+//! }))
+//! result = mrml.to_html("<mjml><mj-body><mj-include path=\"hello-world.mjml\" /></mj-body></mjml>", parser_options = parser_options)
+//! assert result.startswith("<!doctype html>")
 //! ```
 //!
-//! ### Why?
+//! # Why?
 //!
 //! A Node.js server rendering an MJML template takes around **20 MB** of RAM at
 //! startup and **130 MB** under stress test. In Rust, less than **1.7 MB** at
 //! startup and a bit less that **3 MB** under stress test. The Rust version can
 //! also handle twice as many requests per second. You can perform the
 //! benchmarks by running `bash script/run-bench.sh`.
 //!
@@ -98,15 +169,15 @@
 /// Function to parse a raw mjml template with some parsing
 /// [options](crate::prelude::parser::ParserOptions). This function is just an
 /// alias to [the `Mjml::parse_with_options` function](crate::mjml::Mjml).
 ///
 /// You can specify the kind of loader mrml needs to use for loading the content
 /// of [`mj-include`](crate::mj_include) elements.
 ///
-/// You can take a look at the available loaders [here](crate::prelude::parse).
+/// You can take a look at the available loaders [here](crate::prelude::parser).
 ///
 /// ```rust
 /// use mrml::prelude::parser::ParserOptions;
 /// use mrml::prelude::parser::memory_loader::MemoryIncludeLoader;
 ///
 /// let options = ParserOptions {
 ///     include_loader: Box::new(MemoryIncludeLoader::default()),
@@ -135,28 +206,27 @@
 ///
 /// You can take a look at the available loaders [here](crate::prelude::parse).
 ///
 /// ```rust
 /// # tokio_test::block_on(async {
 /// use mrml::prelude::parser::AsyncParserOptions;
 /// use mrml::prelude::parser::memory_loader::MemoryIncludeLoader;
-/// use std::rc::Rc;
 ///
-/// let options = Rc::new(AsyncParserOptions {
+/// let options = std::sync::Arc::new(AsyncParserOptions {
 ///     include_loader: Box::new(MemoryIncludeLoader::default()),
 /// });
 /// match mrml::async_parse_with_options("<mjml><mj-head /><mj-body /></mjml>", options).await {
 ///     Ok(_) => println!("Success!"),
 ///     Err(err) => eprintln!("Something went wrong: {err:?}"),
 /// }
 /// # })
 /// ```
 pub async fn async_parse_with_options<T: AsRef<str>>(
     input: T,
-    opts: std::rc::Rc<crate::prelude::parser::AsyncParserOptions>,
+    opts: std::sync::Arc<crate::prelude::parser::AsyncParserOptions>,
 ) -> Result<mjml::Mjml, prelude::parser::Error> {
     let parser = crate::prelude::parser::AsyncMrmlParser::new(opts);
     let mut cursor = crate::prelude::parser::MrmlCursor::new(input.as_ref());
     parser.parse_root(&mut cursor).await
 }
 
 #[cfg(feature = "parse")]
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion/parse.rs`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,16 @@
                 other => return Err(Error::UnexpectedToken(other.span())),
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjAccordionChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjAccordionChild>, Error> {
         let mut result = Vec::new();
 
@@ -86,15 +87,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAccordion> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjAccordion, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/parse.rs`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,16 @@
                 }
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<MjAccordionElementChildren> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<MjAccordionElementChildren, Error> {
         let mut result = MjAccordionElementChildren::default();
 
@@ -89,15 +90,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAccordionElement> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjAccordionElement, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_element/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_element/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/parse.rs`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAccordionText> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjAccordionText, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_text/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_text/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/parse.rs`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 impl<'opts> ParseChildren<Vec<Text>> for MrmlParser<'opts> {
     fn parse_children(&self, cursor: &mut MrmlCursor<'_>) -> Result<Vec<Text>, Error> {
         parse_children(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<Text>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<Text>, Error> {
         parse_children(cursor)
     }
@@ -48,15 +49,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAccordionTitle> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjAccordionTitle, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_accordion_title/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_accordion_title/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes/children.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes/children.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_all/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-mod children;
+use crate::prelude::hash::Map;
+
 #[cfg(feature = "json")]
 mod json;
 #[cfg(feature = "parse")]
 mod parse;
 #[cfg(feature = "print")]
 mod print;
 
-pub use children::MjAttributesChild;
-
-pub const NAME: &str = "mj-attributes";
+pub const NAME: &str = "mj-all";
 
 #[derive(Debug, Default)]
 #[cfg_attr(feature = "print", derive(mrml_print_macros::MrmlPrintComponent))]
 #[cfg_attr(feature = "print", mrml_print(tag = "NAME"))]
 #[cfg_attr(feature = "json", derive(mrml_json_macros::MrmlJsonComponent))]
 #[cfg_attr(feature = "json", mrml_json(tag = "NAME"))]
-pub struct MjAttributes {
-    children: Vec<MjAttributesChild>,
+pub struct MjAttributesAll {
+    pub attributes: Map<String, String>,
 }
 
-impl MjAttributes {
-    pub fn children(&self) -> &Vec<MjAttributesChild> {
-        &self.children
+impl MjAttributesAll {
+    pub fn attributes(&self) -> &Map<String, String> {
+        &self.attributes
     }
 }
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes/parse.rs`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,16 @@
             MJ_CLASS => MjAttributesChild::MjAttributesClass(self.parse(cursor, tag)?),
             _ => MjAttributesChild::MjAttributesElement(self.parse(cursor, tag)?),
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAttributesChild> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjAttributesChild, Error> {
         Ok(match tag.as_str() {
@@ -55,15 +56,16 @@
                 other => return Err(Error::UnexpectedToken(other.span())),
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjAttributesChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjAttributesChild>, Error> {
         let mut result = Vec::new();
 
@@ -99,15 +101,16 @@
         cursor.assert_element_close()?;
 
         Ok(MjAttributes { children })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAttributes> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjAttributes, Error> {
         let ending = cursor.assert_element_end()?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_all/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_all/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_all/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-use crate::prelude::hash::Map;
-
 #[cfg(feature = "json")]
 mod json;
 #[cfg(feature = "parse")]
 mod parse;
 #[cfg(feature = "print")]
 mod print;
+#[cfg(feature = "render")]
+mod render;
+
+use crate::prelude::hash::Map;
 
-pub const NAME: &str = "mj-all";
+pub const NAME: &str = "mj-carousel-image";
 
 #[derive(Debug, Default)]
 #[cfg_attr(feature = "print", derive(mrml_print_macros::MrmlPrintComponent))]
 #[cfg_attr(feature = "print", mrml_print(tag = "NAME"))]
 #[cfg_attr(feature = "json", derive(mrml_json_macros::MrmlJsonComponent))]
 #[cfg_attr(feature = "json", mrml_json(tag = "NAME"))]
-pub struct MjAttributesAll {
+pub struct MjCarouselImage {
     pub attributes: Map<String, String>,
 }
-
-impl MjAttributesAll {
-    pub fn attributes(&self) -> &Map<String, String> {
-        &self.attributes
-    }
-}
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_all/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_all/parse.rs`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,16 @@
         _tag: StrSpan<'a>,
     ) -> Result<MjAttributesAll, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAttributesAll> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjAttributesAll, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 #[cfg(feature = "print")]
 mod print;
 
 pub const NAME: &str = "mj-class";
 
 #[derive(Debug, Default)]
 pub struct MjAttributesClass {
-    name: String,
-    attributes: Map<String, String>,
+    pub(crate) name: String,
+    pub(crate) attributes: Map<String, String>,
 }
 
 impl MjAttributesClass {
     pub fn name(&self) -> &str {
         &self.name
     }
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/parse.rs`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         tag: StrSpan<'a>,
     ) -> Result<MjAttributesClass, Error> {
         parse(cursor, tag)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAttributesClass> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjAttributesClass, Error> {
         parse(cursor, tag)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_class/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_class/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/mod.rs`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 #[cfg(feature = "parse")]
 mod parse;
 #[cfg(feature = "print")]
 mod print;
 
 #[derive(Debug, Default)]
 pub struct MjAttributesElement {
-    name: String,
-    attributes: Map<String, String>,
+    pub(crate) name: String,
+    pub(crate) attributes: Map<String, String>,
 }
 
 impl MjAttributesElement {
     pub fn new(name: String) -> Self {
         Self {
             name,
             attributes: Map::new(),
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/parse.rs`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         tag: StrSpan<'a>,
     ) -> Result<MjAttributesElement, Error> {
         parse(cursor, tag)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjAttributesElement> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjAttributesElement, Error> {
         parse(cursor, tag)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_attributes_element/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_attributes_element/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_body/children.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_body/children.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_body/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_body/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_body/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_body/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_body/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_body/parse.rs`

 * *Files 17% similar despite different names*

```diff
@@ -72,15 +72,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<Node<MjBodyChild>> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<Node<MjBodyChild>, Error> {
         let tag = tag.to_string();
@@ -131,15 +132,16 @@
             MJ_WRAPPER => Ok(MjBodyChild::MjWrapper(self.parse(cursor, tag)?)),
             _ => Ok(MjBodyChild::Node(self.parse(cursor, tag)?)),
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjBodyChild> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjBodyChild, Error> {
         match tag.as_str() {
@@ -193,15 +195,16 @@
             }
         }
         Ok(result)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjBodyChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjBodyChild>, Error> {
         let mut result = Vec::new();
         while let Some(token) = cursor.next_token() {
@@ -236,15 +239,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjBody> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjBody, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_body/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_body/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_body/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_body/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_breakpoint/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_breakpoint/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_breakpoint/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_breakpoint/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_breakpoint/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_breakpoint/parse.rs`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         _tag: StrSpan<'a>,
     ) -> Result<MjBreakpoint, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjBreakpoint> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjBreakpoint, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_button/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_button/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_button/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_button/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_button/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_button/parse.rs`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjButton> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjButton, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_button/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_button/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_button/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_button/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel/parse.rs`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,16 @@
                 other => return Err(Error::UnexpectedToken(other.span())),
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjCarouselChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjCarouselChild>, Error> {
         let mut result = Vec::new();
 
@@ -82,15 +83,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjCarousel> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjCarousel, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_wrapper/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+use crate::mj_body::MjBodyChild;
+use crate::prelude::hash::Map;
+
 #[cfg(feature = "json")]
 mod json;
 #[cfg(feature = "parse")]
 mod parse;
 #[cfg(feature = "print")]
 mod print;
 #[cfg(feature = "render")]
 mod render;
 
-use crate::prelude::hash::Map;
-
-pub const NAME: &str = "mj-carousel-image";
+pub const NAME: &str = "mj-wrapper";
 
 #[derive(Debug, Default)]
 #[cfg_attr(feature = "print", derive(mrml_print_macros::MrmlPrintComponent))]
-#[cfg_attr(feature = "print", mrml_print(tag = "NAME"))]
+#[cfg_attr(feature = "print", mrml_print(tag = "NAME", indent_children = false))]
 #[cfg_attr(feature = "json", derive(mrml_json_macros::MrmlJsonComponent))]
 #[cfg_attr(feature = "json", mrml_json(tag = "NAME"))]
-pub struct MjCarouselImage {
+pub struct MjWrapper {
     pub attributes: Map<String, String>,
+    pub children: Vec<MjBodyChild>,
 }
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/parse.rs`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         _tag: StrSpan<'a>,
     ) -> Result<MjCarouselImage, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjCarouselImage> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjCarouselImage, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_carousel_image/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_carousel_image/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_column/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_column/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_column/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_column/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_column/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_column/parse.rs`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjColumn> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjColumn, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_column/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_column/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_divider/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_divider/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_divider/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_divider/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_divider/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_divider/parse.rs`

 * *Files 17% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         _tag: StrSpan<'a>,
     ) -> Result<MjDivider, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjDivider> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjDivider, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_divider/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_divider/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_font/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_font/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_font/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_font/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,26 @@
 #[cfg_attr(feature = "print", mrml_print(tag = "NAME"))]
 #[cfg_attr(feature = "json", derive(mrml_json_macros::MrmlJsonComponent))]
 #[cfg_attr(feature = "json", mrml_json(tag = "NAME"))]
 pub struct MjFont {
     pub attributes: MjFontAttributes,
 }
 
+#[cfg(all(test, feature = "render"))]
+impl MjFont {
+    pub(crate) fn new<N: Into<String>, H: Into<String>>(name: N, href: H) -> Self {
+        Self {
+            attributes: MjFontAttributes {
+                name: name.into(),
+                href: href.into(),
+            },
+        }
+    }
+}
+
 impl MjFont {
     pub fn name(&self) -> &str {
         &self.attributes.name
     }
 
     pub fn href(&self) -> &str {
         &self.attributes.href
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_font/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_font/parse.rs`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 impl<'opts> ParseElement<MjFont> for MrmlParser<'opts> {
     fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _: StrSpan<'a>) -> Result<MjFont, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjFont> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _: StrSpan<'a>,
     ) -> Result<MjFont, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_group/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_group/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_group/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_group/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_group/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_text/parse.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 use xmlparser::StrSpan;
 
-use super::MjGroup;
+use super::MjText;
 #[cfg(feature = "async")]
 use crate::prelude::parser::{AsyncMrmlParser, AsyncParseElement};
 use crate::prelude::parser::{Error, MrmlCursor, MrmlParser, ParseElement};
 
-impl<'opts> ParseElement<MjGroup> for MrmlParser<'opts> {
-    fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _tag: StrSpan<'a>) -> Result<MjGroup, Error> {
+impl<'opts> ParseElement<MjText> for MrmlParser<'opts> {
+    fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _tag: StrSpan<'a>) -> Result<MjText, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor)?;
 
-        Ok(MjGroup {
+        Ok(MjText {
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
-impl AsyncParseElement<MjGroup> for AsyncMrmlParser {
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
+impl AsyncParseElement<MjText> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
-    ) -> Result<MjGroup, Error> {
+    ) -> Result<MjText, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
 
-        Ok(MjGroup {
+        Ok(MjText {
             attributes,
             children,
         })
     }
 }
+
+#[cfg(test)]
+mod tests {
+    use crate::mj_text::MjText;
+
+    crate::should_parse!(self_closing, MjText, "<mj-text />");
+    crate::should_parse!(normal, MjText, "<mj-text>Hello World!</mj-text>");
+}
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_group/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_group/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_head/children.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_head/children.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_head/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_head/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_head/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_head/parse.rs`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,16 @@
                 }
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjHeadChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjHeadChild>, Error> {
         use crate::prelude::parser::AsyncParseElement;
 
@@ -82,15 +83,16 @@
         cursor.assert_element_close()?;
 
         Ok(MjHead { children })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjHead> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjHead, Error> {
         let ending = cursor.assert_element_end()?;
@@ -121,15 +123,16 @@
             MJ_TITLE => self.parse(cursor, tag).map(MjHeadChild::MjTitle),
             _ => Err(Error::UnexpectedElement(tag.into())),
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjHeadChild> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjHeadChild, Error> {
         match tag.as_str() {
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_head/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_head/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_hero/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_hero/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_hero/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_hero/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_hero/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_hero/parse.rs`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjHero> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjHero, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_hero/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_hero/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_image/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_image/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_image/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_image/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_image/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_image/parse.rs`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 impl<'opts> ParseElement<MjImage> for MrmlParser<'opts> {
     fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _tag: StrSpan<'a>) -> Result<MjImage, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjImage> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _: StrSpan<'a>,
     ) -> Result<MjImage, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_image/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_image/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/body/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/body/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/body/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/body/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/body/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/body/parse.rs`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
             MJ_WRAPPER => Ok(MjIncludeBodyChild::MjWrapper(self.parse(cursor, tag)?)),
             _ => Err(Error::UnexpectedElement(tag.into())),
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjIncludeBodyChild> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjIncludeBodyChild, Error> {
         match tag.as_str() {
@@ -201,15 +202,16 @@
         }
 
         Ok(result)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjIncludeBodyChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjIncludeBodyChild>, Error> {
         let mut result = Vec::new();
 
@@ -279,15 +281,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl crate::prelude::parser::AsyncParseElement<MjIncludeBody> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjIncludeBody, Error> {
         use crate::prelude::parser::AsyncParseChildren;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/body/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/body/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/body/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/body/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/head/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/head/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/head/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/head/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/head/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/head/parse.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
             MJ_TITLE => self.parse(cursor, tag).map(MjIncludeHeadChild::MjTitle),
             _ => Err(Error::UnexpectedElement(tag.into())),
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjIncludeHeadChild> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjIncludeHeadChild, Error> {
         match tag.as_str() {
@@ -154,15 +155,16 @@
             }
         }
         Ok(result)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjIncludeHeadChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjIncludeHeadChild>, Error> {
         let mut result = Vec::new();
         while let Some(token) = cursor.next_token() {
@@ -232,15 +234,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjIncludeHead> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<MjIncludeHead, Error> {
         let (attributes, children): (MjIncludeHeadAttributes, Vec<MjIncludeHeadChild>) =
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/head/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/head/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_include/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_include/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 pub mod body;
 pub mod head;
 
 pub const NAME: &str = "mj-include";
 
-// #[cfg(all(test, feature = "parser"))]
-#[cfg(test)]
+#[cfg(all(test, feature = "parser", feature = "render"))]
 mod tests {
     use crate::{
         mjml::Mjml,
         prelude::{
             parser::{memory_loader::MemoryIncludeLoader, ParserOptions},
             render::RenderOptions,
         },
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar/parse.rs`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjNavbarChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjNavbarChild>, Error> {
         let mut result = Vec::new();
 
@@ -78,15 +79,16 @@
                 other => return Err(Error::UnexpectedToken(other.span())),
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjNavbar> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjNavbar, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/parse.rs`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjNavbarLink> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjNavbarLink, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_navbar_link/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_navbar_link/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_preview/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_preview/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_preview/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_preview/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_preview/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_preview/parse.rs`

 * *Files 20% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         _tag: StrSpan<'a>,
     ) -> Result<MjPreview, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjPreview> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjPreview, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_raw/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_raw/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_raw/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_raw/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_raw/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_raw/parse.rs`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<Node<MjRawChild>> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<Node<MjRawChild>, Error> {
         let attributes = self.parse_attributes(cursor)?;
@@ -88,15 +89,16 @@
                 other => return Err(Error::UnexpectedToken(other.span())),
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjRawChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjRawChild>, Error> {
         let mut children = Vec::new();
         loop {
@@ -133,15 +135,16 @@
         cursor.assert_element_close()?;
 
         Ok(MjRaw { children })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjRaw> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _: StrSpan<'a>,
     ) -> Result<MjRaw, Error> {
         let ending = cursor.assert_element_end()?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_raw/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_raw/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_section/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_section/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_section/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_section/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_section/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_section/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social/parse.rs`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,16 @@
                 other => return Err(Error::UnexpectedToken(other.span())),
             }
         }
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<Vec<MjSocialChild>> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<Vec<MjSocialChild>, Error> {
         let mut result = Vec::new();
 
@@ -78,15 +79,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjSocial> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<MjSocial, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social_element/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social_element/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social_element/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social_element/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social_element/network.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social_element/network.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social_element/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social_element/parse.rs`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjSocialElement> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _: StrSpan<'a>,
     ) -> Result<MjSocialElement, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_social_element/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_social_element/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_spacer/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_spacer/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_spacer/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_spacer/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_spacer/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_spacer/parse.rs`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 impl<'opts> ParseElement<MjSpacer> for MrmlParser<'opts> {
     fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _tag: StrSpan<'a>) -> Result<MjSpacer, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjSpacer> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _: StrSpan<'a>,
     ) -> Result<MjSpacer, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_spacer/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_spacer/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_style/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_style/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_style/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_style/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_style/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_style/parse.rs`

 * *Files 9% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 impl<'opts> ParseElement<MjStyle> for MrmlParser<'opts> {
     fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _: StrSpan<'a>) -> Result<MjStyle, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjStyle> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _: StrSpan<'a>,
     ) -> Result<MjStyle, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_table/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_table/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_table/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_table/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_table/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_section/parse.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 use xmlparser::StrSpan;
 
-use super::MjTable;
+use super::MjSection;
 #[cfg(feature = "async")]
 use crate::prelude::parser::{AsyncMrmlParser, AsyncParseElement};
 use crate::prelude::parser::{Error, MrmlCursor, MrmlParser, ParseElement};
 
-impl<'opts> ParseElement<MjTable> for MrmlParser<'opts> {
-    fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _tag: StrSpan<'a>) -> Result<MjTable, Error> {
+impl<'opts> ParseElement<MjSection> for MrmlParser<'opts> {
+    fn parse<'a>(
+        &self,
+        cursor: &mut MrmlCursor<'a>,
+        _tag: StrSpan<'a>,
+    ) -> Result<MjSection, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor)?;
 
-        Ok(MjTable {
+        Ok(MjSection {
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
-impl AsyncParseElement<MjTable> for AsyncMrmlParser {
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
+impl AsyncParseElement<MjSection> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
-    ) -> Result<MjTable, Error> {
+    ) -> Result<MjSection, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
 
-        Ok(MjTable {
+        Ok(MjSection {
             attributes,
             children,
         })
     }
 }
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_table/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_table/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_text/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_text/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_text/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_text/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_text/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_wrapper/parse.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 use xmlparser::StrSpan;
 
-use super::MjText;
+use super::MjWrapper;
 #[cfg(feature = "async")]
 use crate::prelude::parser::{AsyncMrmlParser, AsyncParseElement};
 use crate::prelude::parser::{Error, MrmlCursor, MrmlParser, ParseElement};
 
-impl<'opts> ParseElement<MjText> for MrmlParser<'opts> {
-    fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _tag: StrSpan<'a>) -> Result<MjText, Error> {
+impl<'opts> ParseElement<MjWrapper> for MrmlParser<'opts> {
+    fn parse<'a>(
+        &self,
+        cursor: &mut MrmlCursor<'a>,
+        _tag: StrSpan<'a>,
+    ) -> Result<MjWrapper, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor)?;
 
-        Ok(MjText {
+        Ok(MjWrapper {
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
-impl AsyncParseElement<MjText> for AsyncMrmlParser {
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
+impl AsyncParseElement<MjWrapper> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
-    ) -> Result<MjText, Error> {
+    ) -> Result<MjWrapper, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
 
-        Ok(MjText {
+        Ok(MjWrapper {
             attributes,
             children,
         })
     }
 }
 
 #[cfg(test)]
 mod tests {
-    use crate::mj_text::MjText;
+    use crate::mj_wrapper::MjWrapper;
 
-    crate::should_parse!(self_closing, MjText, "<mj-text />");
-    crate::should_parse!(normal, MjText, "<mj-text>Hello World!</mj-text>");
+    crate::should_sync_parse!(
+        parse_br_element,
+        MjWrapper,
+        "<mj-wrapper><h1>hello</h1><br><h2>world</h2></mj-wrapper>"
+    );
 }
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_text/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_text/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_title/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_title/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_title/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_title/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_title/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_title/parse.rs`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 impl<'opts> ParseElement<MjTitle> for MrmlParser<'opts> {
     fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, _: StrSpan<'a>) -> Result<MjTitle, Error> {
         parse(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<MjTitle> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _: StrSpan<'a>,
     ) -> Result<MjTitle, Error> {
         parse(cursor)
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_wrapper/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_wrapper/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mj_wrapper/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mj_wrapper/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mjml/json.rs` & `mrml-0.1.8/packages/mrml-core/src/mjml/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mjml/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/mjml/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mjml/parse.rs` & `mrml-0.1.8/packages/mrml-core/src/mjml/parse.rs`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,16 @@
 impl ParseAttributes<MjmlAttributes> for AsyncMrmlParser {
     fn parse_attributes(&self, cursor: &mut MrmlCursor<'_>) -> Result<MjmlAttributes, Error> {
         parse_attributes(cursor)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseChildren<MjmlChildren> for AsyncMrmlParser {
     async fn async_parse_children<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
     ) -> Result<MjmlChildren, Error> {
         let mut children = MjmlChildren::default();
 
@@ -107,15 +108,16 @@
             attributes,
             children,
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncParseElement<Mjml> for AsyncMrmlParser {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         _tag: StrSpan<'a>,
     ) -> Result<Mjml, Error> {
         let (attributes, children) = self.parse_attributes_and_children(cursor).await?;
@@ -131,15 +133,15 @@
     /// Function to parse a raw mjml template with some parsing
     /// [options](crate::prelude::parser::ParserOptions).
     ///
     /// You can specify the kind of loader mrml needs to use for loading the
     /// content of [`mj-include`](crate::mj_include) elements.
     ///
     /// You can take a look at the available loaders
-    /// [here](crate::prelude::parse).
+    /// [here](crate::prelude::parser).
     ///
     /// ```rust
     /// use mrml::mjml::Mjml;
     /// use mrml::prelude::parser::ParserOptions;
     /// use mrml::prelude::parser::memory_loader::MemoryIncludeLoader;
     ///
     /// let options = ParserOptions {
@@ -158,15 +160,15 @@
         let mut cursor = MrmlCursor::new(value.as_ref());
         parser.parse_root(&mut cursor)
     }
 
     #[cfg(feature = "async")]
     pub async fn async_parse_with_options<T: AsRef<str>>(
         value: T,
-        opts: std::rc::Rc<crate::prelude::parser::AsyncParserOptions>,
+        opts: std::sync::Arc<crate::prelude::parser::AsyncParserOptions>,
     ) -> Result<Self, Error> {
         let parser = AsyncMrmlParser::new(opts);
         let mut cursor = MrmlCursor::new(value.as_ref());
         parser.parse_root(&mut cursor).await
     }
 
     /// Function to parse a raw mjml template using the default parsing
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/mjml/print.rs` & `mrml-0.1.8/packages/mrml-core/src/mjml/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/mjml/render.rs` & `mrml-0.1.8/packages/mrml-core/src/mjml/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/node/json.rs` & `mrml-0.1.8/packages/mrml-core/src/node/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/node/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/node/mod.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/node/print.rs` & `mrml-0.1.8/packages/mrml-core/src/node/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/node/render.rs` & `mrml-0.1.8/packages/mrml-core/src/node/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/hash.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/hash.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/parser/http_loader.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/parser/http_loader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         &self,
         url: &str,
         headers: &HashMap<String, String>,
     ) -> Result<String, IncludeLoaderError>;
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 pub trait AsyncHttpFetcher: Default + Debug {
     async fn async_fetch(
         &self,
         url: &str,
         headers: &HashMap<String, String>,
     ) -> Result<String, IncludeLoaderError>;
 }
@@ -63,15 +64,16 @@
 }
 
 #[cfg(feature = "http-loader-async-reqwest")]
 #[derive(Debug, Default)]
 pub struct AsyncReqwestFetcher(reqwest::Client);
 
 #[cfg(feature = "http-loader-async-reqwest")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncHttpFetcher for AsyncReqwestFetcher {
     async fn async_fetch(
         &self,
         url: &str,
         headers: &HashMap<String, String>,
     ) -> Result<String, IncludeLoaderError> {
         let req = self.0.get(url);
@@ -326,16 +328,17 @@
     fn resolve(&self, path: &str) -> Result<String, IncludeLoaderError> {
         self.check_url(path)?;
         self.fetcher.fetch(path, &self.headers)
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
-impl<F: AsyncHttpFetcher + Sync> AsyncIncludeLoader for HttpIncludeLoader<F> {
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
+impl<F: AsyncHttpFetcher + Sync + Send> AsyncIncludeLoader for HttpIncludeLoader<F> {
     async fn async_resolve(&self, path: &str) -> Result<String, IncludeLoaderError> {
         self.check_url(path)?;
         self.fetcher.async_fetch(path, &self.headers).await
     }
 }
 
 #[cfg(test)]
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/parser/loader.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/parser/loader.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-//! Module containing the trait for implementing an
-//! [`IncludeLoader`](crate::prelude::parser::loader::IncludeLoader).
+//! Module containing the trait for implementing an [`IncludeLoader`].
 
 use std::io::ErrorKind;
 use std::sync::Arc;
 
 #[derive(Debug, Clone)]
 pub struct IncludeLoaderError {
     pub path: String,
@@ -70,15 +69,16 @@
     ///
     /// You can have an example of simple resolve function with the
     /// [`MemoryIncludeLoader`](crate::prelude::parser::memory_loader::MemoryIncludeLoader).
     fn resolve(&self, path: &str) -> Result<String, IncludeLoaderError>;
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 pub trait AsyncIncludeLoader: std::fmt::Debug {
     /// This function is used to fetch the included template using the `path`
     /// attribute.
     ///
     /// You can have an example of simple resolve function with the
     /// [`MemoryIncludeLoader`](crate::prelude::parser::memory_loader::MemoryIncludeLoader).
     async fn async_resolve(&self, path: &str) -> Result<String, IncludeLoaderError>;
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/parser/local_loader.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/parser/local_loader.rs`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,16 @@
                 .with_message("unable to load the template file")
                 .with_cause(Arc::new(err))
         })
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncIncludeLoader for LocalIncludeLoader {
     async fn async_resolve(&self, url: &str) -> Result<String, IncludeLoaderError> {
         let path = self.build_path(url)?;
         std::fs::read_to_string(path).map_err(|err| {
             IncludeLoaderError::new(url, ErrorKind::InvalidData)
                 .with_message("unable to load the template file")
                 .with_cause(Arc::new(err))
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/parser/memory_loader.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/parser/memory_loader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 use super::loader::IncludeLoaderError;
 use crate::prelude::hash::Map;
 #[cfg(feature = "async")]
 use crate::prelude::parser::loader::AsyncIncludeLoader;
 use crate::prelude::parser::loader::IncludeLoader;
 
 #[derive(Debug, Default)]
-/// This struct is a simple
-/// [`IncludeLoader`](crate::prelude::parser::loader::IncludeLoader) where
-/// you can store in a map all files you want to be able to use with
-/// [`mj-include`](crate::mj_include).
+/// This struct is a simple [`IncludeLoader`] where you can store in a map all
+/// files you want to be able to use with [`mj-include`](crate::mj_include).
 ///
 /// # Example
 /// ```rust
 /// use mrml::mj_include::body::MjIncludeBodyKind;
 /// use mrml::prelude::parser::memory_loader::MemoryIncludeLoader;
 /// use mrml::prelude::parser::ParserOptions;
 ///
@@ -68,15 +66,16 @@
             .get(path)
             .cloned()
             .ok_or_else(|| IncludeLoaderError::not_found(path))
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncIncludeLoader for MemoryIncludeLoader {
     async fn async_resolve(&self, path: &str) -> Result<String, IncludeLoaderError> {
         self.0
             .get(path)
             .cloned()
             .ok_or_else(|| IncludeLoaderError::not_found(path))
     }
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/parser/mod.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/parser/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,16 @@
 }
 
 pub(crate) trait ParseElement<E> {
     fn parse<'a>(&self, cursor: &mut MrmlCursor<'a>, tag: StrSpan<'a>) -> Result<E, Error>;
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 pub(crate) trait AsyncParseElement<E> {
     async fn async_parse<'a>(
         &self,
         cursor: &mut MrmlCursor<'a>,
         tag: StrSpan<'a>,
     ) -> Result<E, Error>;
 }
@@ -251,15 +252,16 @@
 }
 
 pub(crate) trait ParseChildren<C> {
     fn parse_children(&self, cursor: &mut MrmlCursor<'_>) -> Result<C, Error>;
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 pub(crate) trait AsyncParseChildren<C> {
     async fn async_parse_children<'a>(&self, cursor: &mut MrmlCursor<'a>) -> Result<C, Error>;
 }
 
 pub struct MrmlCursor<'a> {
     tokenizer: Tokenizer<'a>,
     buffer: Vec<MrmlToken<'a>>,
@@ -407,20 +409,20 @@
         parse_attributes_map(cursor)
     }
 }
 
 #[cfg(feature = "async")]
 #[derive(Default)]
 pub struct AsyncMrmlParser {
-    pub(crate) options: std::rc::Rc<AsyncParserOptions>,
+    pub(crate) options: std::sync::Arc<AsyncParserOptions>,
 }
 
 #[cfg(feature = "async")]
 impl AsyncMrmlParser {
-    pub fn new(options: std::rc::Rc<AsyncParserOptions>) -> Self {
+    pub fn new(options: std::sync::Arc<AsyncParserOptions>) -> Self {
         Self { options }
     }
 }
 
 #[cfg(feature = "async")]
 impl AsyncMrmlParser {
     pub(crate) async fn parse_root<T>(&self, cursor: &mut MrmlCursor<'_>) -> Result<T, Error>
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/parser/multi_loader.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/parser/multi_loader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 use super::loader::IncludeLoaderError;
 #[cfg(feature = "async")]
 use crate::prelude::parser::loader::AsyncIncludeLoader;
 use crate::prelude::parser::loader::IncludeLoader;
 
 #[derive(Debug, Default)]
-/// This struct is a
-/// [`IncludeLoader`](crate::prelude::parser::loader::IncludeLoader) where
-/// you can define a strategy of resolver depending on the path.
+/// This struct is a [`IncludeLoader`] where you can define a strategy of
+/// resolver depending on the path.
 /// That way, you can have a resolver for paths starting with `https://` and
 /// another resolver for local files where the paths start with `file://`.
 /// If no provider match the path, a `NotFound` error will be returned.
 ///
 /// # Example
 /// ```rust
 /// use mrml::mj_include::body::MjIncludeBodyKind;
@@ -53,28 +52,27 @@
 /// use mrml::mj_include::body::MjIncludeBodyKind;
 /// use mrml::prelude::parser::http_loader::{AsyncReqwestFetcher, HttpIncludeLoader};
 /// use mrml::prelude::parser::memory_loader::MemoryIncludeLoader;
 /// use mrml::prelude::parser::multi_loader::{MultiIncludeLoader, MultiIncludeLoaderItem, MultiIncludeLoaderFilter};
 /// use mrml::prelude::parser::noop_loader::NoopIncludeLoader;
 /// use mrml::prelude::parser::loader::AsyncIncludeLoader;
 /// use mrml::prelude::parser::AsyncParserOptions;
-/// use std::rc::Rc;
 ///
 /// let resolver = MultiIncludeLoader::<Box<dyn AsyncIncludeLoader + Send + Sync + 'static>>::new()
 ///     .with_starts_with("https://", Box::new(HttpIncludeLoader::<AsyncReqwestFetcher>::allow_all()))
 ///     .with_any(Box::<NoopIncludeLoader>::default());
 /// let opts = AsyncParserOptions {
 ///     include_loader: Box::new(resolver),
 /// };
 /// let json = r#"<mjml>
 ///   <mj-body>
 ///     <mj-include path="file://basic.mjml" />
 ///   </mj-body>
 /// </mjml>"#;
-/// match mrml::async_parse_with_options(json, Rc::new(opts)).await {
+/// match mrml::async_parse_with_options(json, std::sync::Arc::new(opts)).await {
 ///     Ok(_) => println!("Success!"),
 ///     Err(err) => eprintln!("Couldn't parse template: {err:?}"),
 /// }
 /// # })
 /// ```
 pub struct MultiIncludeLoader<T>(Vec<MultiIncludeLoaderItem<T>>);
 
@@ -84,35 +82,39 @@
     }
 
     fn with_item(mut self, filter: MultiIncludeLoaderFilter, loader: T) -> Self {
         self.0.push(MultiIncludeLoaderItem { filter, loader });
         self
     }
 
+    #[inline]
     pub fn with_any(self, loader: T) -> Self {
         self.with_item(MultiIncludeLoaderFilter::Any, loader)
     }
 
+    #[inline]
     pub fn with_starts_with<S: ToString>(self, starts_with: S, loader: T) -> Self {
         self.with_item(
             MultiIncludeLoaderFilter::StartsWith {
                 value: starts_with.to_string(),
             },
             loader,
         )
     }
 
     fn add_item(&mut self, filter: MultiIncludeLoaderFilter, loader: T) {
         self.0.push(MultiIncludeLoaderItem { filter, loader });
     }
 
+    #[inline]
     pub fn add_any(&mut self, loader: T) {
         self.add_item(MultiIncludeLoaderFilter::Any, loader);
     }
 
+    #[inline]
     pub fn add_starts_with<S: ToString>(&mut self, starts_with: S, loader: T) {
         self.add_item(
             MultiIncludeLoaderFilter::StartsWith {
                 value: starts_with.to_string(),
             },
             loader,
         );
@@ -156,15 +158,16 @@
 }
 
 #[cfg(feature = "async")]
 pub type MultiIncludeLoaderAsync =
     MultiIncludeLoader<Box<dyn AsyncIncludeLoader + Sync + Send + 'static>>;
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncIncludeLoader for MultiIncludeLoaderAsync {
     async fn async_resolve(&self, path: &str) -> Result<String, IncludeLoaderError> {
         let item = self
             .0
             .iter()
             .find(|item| item.filter.matches(path))
             .ok_or_else(|| {
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/parser/noop_loader.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/parser/noop_loader.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 #[cfg(feature = "async")]
 use super::loader::AsyncIncludeLoader;
 use super::loader::IncludeLoaderError;
 use crate::prelude::parser::loader::IncludeLoader;
 
 #[derive(Debug, Default)]
-/// This struct is a simple
-/// [`IncludeLoader`](crate::prelude::parser::loader::IncludeLoader) that
-/// doesn't resolve any template. This is the default loader.
+/// This struct is a simple  [`IncludeLoader`] that doesn't resolve any
+/// template. This is the default loader.
 ///
 /// # Example
 /// ```rust
 /// use mrml::mj_include::body::MjIncludeBodyKind;
 /// use mrml::prelude::parser::noop_loader::NoopIncludeLoader;
 /// use mrml::prelude::parser::ParserOptions;
 ///
@@ -35,13 +34,14 @@
 impl IncludeLoader for NoopIncludeLoader {
     fn resolve(&self, path: &str) -> Result<String, IncludeLoaderError> {
         Err(IncludeLoaderError::not_found(path))
     }
 }
 
 #[cfg(feature = "async")]
-#[async_trait::async_trait(?Send)]
+#[cfg_attr(target_arch = "wasm32", async_trait::async_trait(?Send))]
+#[cfg_attr(not(target_arch = "wasm32"), async_trait::async_trait)]
 impl AsyncIncludeLoader for NoopIncludeLoader {
     async fn async_resolve(&self, path: &str) -> Result<String, IncludeLoaderError> {
         Err(IncludeLoaderError::not_found(path))
     }
 }
```

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/print.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/prelude/render.rs` & `mrml-0.1.8/packages/mrml-core/src/prelude/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/text/json.rs` & `mrml-0.1.8/packages/mrml-core/src/text/json.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/text/print.rs` & `mrml-0.1.8/packages/mrml-core/src/text/print.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/src/text/render.rs` & `mrml-0.1.8/packages/mrml-core/src/text/render.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/Cargo.toml` & `mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/CHANGELOG.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/license.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/license.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/readme.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/readme.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-json-macros/src/element.rs` & `mrml-0.1.8/packages/mrml-core/lib/mrml-json-macros/src/element.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/Cargo.toml` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/CHANGELOG.md` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/license.md` & `mrml-0.1.8/packages/mrml-core/lib/common-macros/license.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/readme.md` & `mrml-0.1.8/packages/mrml-core/lib/common-macros/readme.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/attributes.rs` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/attributes.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/children.rs` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/children.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/element.rs` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/element.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/mrml-print-macros/src/lib.rs` & `mrml-0.1.8/packages/mrml-core/lib/mrml-print-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-core/lib/css-compare/src/lib.rs` & `mrml-0.1.8/packages/mrml-core/lib/css-compare/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-python/Cargo.toml` & `mrml-0.1.8/packages/mrml-python/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "mrml-python"
 description = "Python wrapping on MRML"
 keywords = ["email", "mjml"]
-version = "0.1.7"
+version = "0.1.8"
 authors = ["Jérémie Drouet <jeremie.drouet@gmail.com>"]
 edition = "2021"
 license-file = "license.md"
 repository = "https://github.com/jdrouet/mrml/"
 readme = "readme.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "mrml"
 crate-type = ["cdylib"]
 
 [dependencies]
-mrml = { version = "3.1.0", path = "../mrml-core", features = [
+mrml = { version = "3.1.1", path = "../mrml-core", features = [
   "http-loader-ureq",
   "local-loader",
 ] }
 pyo3 = { version = "0.20.0", features = ["extension-module"] }
```

### Comparing `mrml-0.1.7/packages/mrml-python/.gitignore` & `mrml-0.1.8/packages/mrml-python/.gitignore`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-python/CHANGELOG.md` & `mrml-0.1.8/packages/mrml-python/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.8](https://github.com/jdrouet/mrml/compare/mrml-python-v0.1.7...mrml-python-v0.1.8) - 2024-03-19
+
+### Other
+- updated the following local packages: mrml
+
 ## [0.1.7](https://github.com/jdrouet/mrml/compare/mrml-python-v0.1.6...mrml-python-v0.1.7) - 2024-03-15
 
 ### Other
 - updated the following local packages: mrml
 
 ## [0.1.6](https://github.com/jdrouet/mrml/compare/mrml-python-v0.1.5...mrml-python-v0.1.6) - 2024-03-04
```

### Comparing `mrml-0.1.7/packages/mrml-python/license.md` & `mrml-0.1.8/packages/mrml-python/license.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-python/readme.md` & `mrml-0.1.8/packages/mrml-python/readme.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-python/src/lib.rs` & `mrml-0.1.8/packages/mrml-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/packages/mrml-python/tests/test_loader.py` & `mrml-0.1.8/packages/mrml-python/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/Cargo.lock` & `mrml-0.1.8/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -147,14 +147,96 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "axum"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1236b4b292f6c4d6dc34604bb5120d85c3fe1d1aa596bd5cc52ca054d13e7b9e"
+dependencies = [
+ "async-trait",
+ "axum-core",
+ "axum-macros",
+ "bytes",
+ "futures-util",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "http-body-util",
+ "hyper 1.2.0",
+ "hyper-util",
+ "itoa",
+ "matchit",
+ "memchr",
+ "mime",
+ "percent-encoding",
+ "pin-project-lite",
+ "rustversion",
+ "serde",
+ "serde_json",
+ "serde_path_to_error",
+ "serde_urlencoded",
+ "sync_wrapper",
+ "tokio",
+ "tower",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "axum-core"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a15c63fd72d41492dc4f497196f5da1fb04fb7529e631d73630d1b491e47a2e3"
+dependencies = [
+ "async-trait",
+ "bytes",
+ "futures-util",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "http-body-util",
+ "mime",
+ "pin-project-lite",
+ "rustversion",
+ "sync_wrapper",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "axum-macros"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "00c055ee2d014ae5981ce1016374e8213682aa14d9bf40e48ab48b5f3ef20eaa"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "axum-mrml"
+version = "0.1.0"
+dependencies = [
+ "axum",
+ "mrml",
+ "serde",
+ "serde_json",
+ "tokio",
+ "tower",
+ "tracing",
+ "tracing-subscriber",
+]
+
+[[package]]
 name = "backtrace"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
 dependencies = [
  "addr2line",
  "cc",
@@ -772,15 +854,34 @@
 checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
- "http",
+ "http 0.2.11",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
+name = "h2"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51ee2dd2e4f378392eeff5d51618cd9a63166a2513846bbc55f21cfacd9199d4"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http 1.1.0",
  "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
@@ -859,21 +960,55 @@
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
+name = "http"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
 name = "http-body"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
- "http",
+ "http 0.2.11",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "http-body"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
+dependencies = [
+ "bytes",
+ "http 1.1.0",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http 1.1.0",
+ "http-body 1.0.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -897,43 +1032,79 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
- "h2",
- "http",
- "http-body",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
+name = "hyper"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "h2 0.4.3",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "smallvec",
+ "tokio",
+]
+
+[[package]]
 name = "hyper-rustls"
 version = "0.24.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
- "http",
- "hyper",
+ "http 0.2.11",
+ "hyper 0.14.28",
  "rustls 0.21.10",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
+name = "hyper-util"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+dependencies = [
+ "bytes",
+ "futures-util",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "hyper 1.2.0",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+]
+
+[[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
 name = "idna"
@@ -1057,14 +1228,29 @@
 [[package]]
 name = "log"
 version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
+name = "matchers"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
+dependencies = [
+ "regex-automata 0.1.10",
+]
+
+[[package]]
+name = "matchit"
+version = "0.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0e7465ac9959cc2b1404e8e2367b43684a6d13790fe23056cc8c6c5a6b7bcb94"
+
+[[package]]
 name = "memchr"
 version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memoffset"
@@ -1106,27 +1292,27 @@
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8d3038e23466858569c2d30a537f691fa0d53b51626630ae08262943e3bbb8b"
 dependencies = [
  "assert-json-diff",
  "colored",
  "futures",
- "hyper",
+ "hyper 0.14.28",
  "log",
  "rand",
  "regex",
  "serde_json",
  "serde_urlencoded",
  "similar",
  "tokio",
 ]
 
 [[package]]
 name = "mrml"
-version = "3.1.0"
+version = "3.1.1"
 dependencies = [
  "async-trait",
  "concat-idents",
  "criterion",
  "html-compare",
  "indexmap",
  "itertools 0.12.1",
@@ -1145,15 +1331,15 @@
  "ureq",
  "url",
  "xmlparser",
 ]
 
 [[package]]
 name = "mrml-cli"
-version = "1.5.2"
+version = "1.5.3"
 dependencies = [
  "clap",
  "env_logger",
  "log",
  "mrml",
  "serde",
  "serde_json",
@@ -1198,35 +1384,45 @@
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "mrml-python"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "mrml",
  "pyo3",
 ]
 
 [[package]]
 name = "mrml-wasm"
-version = "1.4.5"
+version = "1.4.6"
 dependencies = [
  "console_error_panic_hook",
  "mrml",
  "serde",
  "serde-wasm-bindgen",
  "tsify",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wasm-bindgen-test",
 ]
 
 [[package]]
+name = "nu-ansi-term"
+version = "0.46.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
+dependencies = [
+ "overload",
+ "winapi",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
@@ -1259,14 +1455,20 @@
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
+name = "overload"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
+
+[[package]]
 name = "parcel_selectors"
 version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05d74befe2d076330d9a58bf9ca2da424568724ab278adf15fb5718253133887"
 dependencies = [
  "bitflags 2.4.2",
  "cssparser",
@@ -1396,14 +1598,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pin-utils"
@@ -1594,36 +1816,45 @@
 version = "1.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata 0.4.5",
- "regex-syntax",
+ "regex-syntax 0.8.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
+dependencies = [
+ "regex-syntax 0.6.29",
+]
 
 [[package]]
 name = "regex-automata"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.8.2",
 ]
 
 [[package]]
 name = "regex-syntax"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "reqwest"
 version = "0.11.24"
@@ -1631,18 +1862,18 @@
 checksum = "c6920094eb85afde5e4a138be3f2de8bbdf28000f0029e72c45025a56b042251"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
- "h2",
- "http",
- "http-body",
- "hyper",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
+ "hyper 0.14.28",
  "hyper-rustls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
  "percent-encoding",
@@ -1750,14 +1981,20 @@
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
+name = "rustversion"
+version = "1.0.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+
+[[package]]
 name = "ryu"
 version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
 
 [[package]]
 name = "same-file"
@@ -1788,17 +2025,17 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.6.3"
@@ -1808,17 +2045,17 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -1830,36 +2067,55 @@
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.113"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_path_to_error"
+version = "0.1.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af99884400da37c88f5e9146b7f1fd0fbcae8f6eec4e9da38b67d05486f814a6"
+dependencies = [
+ "itoa",
+ "serde",
+]
+
+[[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
 dependencies = [
  "form_urlencoded",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "sharded-slab"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
+dependencies = [
+ "lazy_static",
+]
+
+[[package]]
 name = "signal-hook-registry"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
@@ -2011,14 +2267,24 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
+name = "thread_local"
+version = "1.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+]
+
+[[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
@@ -2114,36 +2380,101 @@
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
+name = "tower"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
+dependencies = [
+ "futures-core",
+ "futures-util",
+ "pin-project",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
+ "log",
  "pin-project-lite",
+ "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
+name = "tracing-attributes"
+version = "0.1.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
+ "valuable",
+]
+
+[[package]]
+name = "tracing-log"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
+dependencies = [
+ "log",
+ "once_cell",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-subscriber"
+version = "0.3.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
+dependencies = [
+ "matchers",
+ "nu-ansi-term",
+ "once_cell",
+ "regex",
+ "sharded-slab",
+ "smallvec",
+ "thread_local",
+ "tracing",
+ "tracing-core",
+ "tracing-log",
 ]
 
 [[package]]
 name = "try-lock"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
@@ -2244,14 +2575,20 @@
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
+name = "valuable"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
```

### Comparing `mrml-0.1.7/pyproject.toml` & `mrml-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/readme.md` & `mrml-0.1.8/readme.md`

 * *Files identical despite different names*

### Comparing `mrml-0.1.7/PKG-INFO` & `mrml-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mrml
-Version: 0.1.7
+Version: 0.1.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: license.md
 Summary: A Python wrapper for MRML (Rust port of MJML).
 Keywords: email,mjml
 Author: Jérémie Drouet <jeremie.drouet@gmail.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: mrml Version: 0.1.7 Classifier: Programming
+Metadata-Version: 2.3 Name: mrml Version: 0.1.8 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: license.md Summary: A Python wrapper for MRML (Rust port of
 MJML). Keywords: email,mjml Author: JÃ©rÃ©mie Drouet
 gmail.com> Author-email: JÃ©rÃ©mie Drouet
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: Homepage, https://github.com/jdrouet/
```

