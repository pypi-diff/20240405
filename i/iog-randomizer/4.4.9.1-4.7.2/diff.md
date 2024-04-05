# Comparing `tmp/iog-randomizer-4.4.9.1.tar.gz` & `tmp/iog-randomizer-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iog-randomizer-4.4.9.1.tar", last modified: Sun Apr  9 04:47:14 2023, max compression
+gzip compressed data, was "iog-randomizer-4.7.2.tar", last modified: Fri Apr  5 03:09:04 2024, max compression
```

## Comparing `iog-randomizer-4.4.9.1.tar` & `iog-randomizer-4.7.2.tar`

### file list

```diff
@@ -1,174 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/
--rw-rw-rw-   0        0        0     1233 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/LICENSE
--rw-rw-rw-   0        0        0      188 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    16459 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.547349 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/
--rw-rw-rw-   0        0        0      188 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6261 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 04:47:13.000000 iog-randomizer-4.4.9.1/iog_randomizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.609862 iog-randomizer-4.4.9.1/randomizer/
--rw-rw-rw-   0        0        0       25 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.109746 iog-randomizer-4.4.9.1/randomizer/bin/
--rw-rw-rw-   0        0        0       84 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/00f49a_roominit.bin
--rw-rw-rw-   0        0        0     2048 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/00f500_redjewel.bin
--rw-rw-rw-   0        0        0      448 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/00fdf0_pi.bin
--rw-rw-rw-   0        0        0       40 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01a7c2_babel.bin
--rw-rw-rw-   0        0        0      256 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01aade_roomrewards.bin
--rw-rw-rw-   0        0        0      440 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemies_z3.bin
--rw-rw-rw-   0        0        0      440 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesadvanced.bin
--rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesbeginner.bin
--rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesexpert.bin
--rw-rw-rw-   0        0        0      440 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesintermediate.bin
--rw-rw-rw-   0        0        0      440 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01abf0_enemiesohko.bin
--rw-rw-rw-   0        0        0      224 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/01afa6_chests.bin
--rw-rw-rw-   0        0        0     2863 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01dabf_startmenu.bin
--rw-rw-rw-   0        0        0     1210 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01e132_itemdesc.bin
--rw-rw-rw-   0        0        0      478 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/01fd24_acquisition.bin
--rw-rw-rw-   0        0        0       98 2021-03-25 16:40:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/02f0c0_firebird.bin
--rw-rw-rw-   0        0        0     1784 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/02f130_enemystats.bin
--rw-rw-rw-   0        0        0     1784 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/02f130_enemystats_z3.bin
--rw-rw-rw-   0        0        0      109 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03881d_item05.bin
--rw-rw-rw-   0        0        0      157 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/038bf5_item09.bin
--rw-rw-rw-   0        0        0      220 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/038f17_item0d.bin
--rw-rw-rw-   0        0        0       53 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/03950c_item16.bin
--rw-rw-rw-   0        0        0       36 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/03983d_item19.bin
--rw-rw-rw-   0        0        0      268 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/039d09_item25.bin
--rw-rw-rw-   0        0        0       81 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/039f5d_item28.bin
--rw-rw-rw-   0        0        0      686 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03b401_mapchoices.bin
--rw-rw-rw-   0        0        0      368 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03b955_mapdest.bin
--rw-rw-rw-   0        0        0      135 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03f779_statupgrades.bin
--rw-rw-rw-   0        0        0       79 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03fd70_rjm.bin
--rw-rw-rw-   0        0        0      134 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/03fdc0_startmenu.bin
--rw-rw-rw-   0        0        0       74 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/03ff90_copd4.bin
--rw-rw-rw-   0        0        0       70 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/048a94_teacher.bin
--rw-rw-rw-   0        0        0      399 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/04b9a5_seaside.bin
--rw-rw-rw-   0        0        0       78 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04c4fb_edward.bin
--rw-rw-rw-   0        0        0       57 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/04c6af_edward2.bin
--rw-rw-rw-   0        0        0       95 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04d1a0_castleguard.bin
--rw-rw-rw-   0        0        0      256 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/04e2a3_itory.bin
--rw-rw-rw-   0        0        0      238 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04e5ff_lilly.bin
--rw-rw-rw-   0        0        0      220 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/04fb50_tutorial.bin
--rw-rw-rw-   0        0        0     2048 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/058100_redjewel.bin
--rw-rw-rw-   0        0        0      175 2020-02-26 04:14:01.000000 iog-randomizer-4.4.9.1/randomizer/bin/0584a9_goldship.bin
--rw-rw-rw-   0        0        0      122 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/05cf85_freejia.bin
--rw-rw-rw-   0        0        0      184 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/05d7e2_trappedlaborer.bin
--rw-rw-rw-   0        0        0      479 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/05d89a_neilscottage.bin
--rw-rw-rw-   0        0        0      248 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/05e647_nazca.bin
--rw-rw-rw-   0        0        0      338 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/05f356_skygarden.bin
--rw-rw-rw-   0        0        0       42 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/069739_mudoor.bin
--rw-rw-rw-   0        0        0      462 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/0699dc_mu.bin
--rw-rw-rw-   0        0        0       46 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/06ba36_angelsign.bin
--rw-rw-rw-   0        0        0     1867 2022-11-06 21:34:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/06dd30_collectioncheck.bin
--rw-rw-rw-   0        0        0       88 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/06e500_vampchange.bin
--rw-rw-rw-   0        0        0       37 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/078569_watermia1.bin
--rw-rw-rw-   0        0        0      173 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/0786c1_watermia2.bin
--rw-rw-rw-   0        0        0      145 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/079237_russianglass.bin
--rw-rw-rw-   0        0        0      192 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/07b59e_necklace.bin
--rw-rw-rw-   0        0        0       80 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/07c432_euro1.bin
--rw-rw-rw-   0        0        0      572 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/07c4d0_euro2.bin
--rw-rw-rw-   0        0        0       86 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/07e517_euroitem.bin
--rw-rw-rw-   0        0        0      352 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/088fc4_natives.bin
--rw-rw-rw-   0        0        0      113 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/089a31_ankorwat.bin
--rw-rw-rw-   0        0        0      115 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/089abf_ankorwat.bin
--rw-rw-rw-   0        0        0      163 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08b010_snakegame.bin
--rw-rw-rw-   0        0        0     1136 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08cec9_jeweler.bin
--rw-rw-rw-   0        0        0      811 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/08db07_darkspace.bin
--rw-rw-rw-   0        0        0       80 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08fd30_forcechange.bin
--rw-rw-rw-   0        0        0       87 2021-04-20 04:45:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/08fd80_jeweler2.bin
--rw-rw-rw-   0        0        0       87 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/08fd80_jeweler2_rjm.bin
--rw-rw-rw-   0        0        0      375 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09ca02_incaship.bin
--rw-rw-rw-   0        0        0      253 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09d0f5_moontribe.bin
--rw-rw-rw-   0        0        0      302 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09d11e_moontribe.bin
--rw-rw-rw-   0        0        0      130 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/09d30f_moontribe.bin
--rw-rw-rw-   0        0        0       88 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/0aff99_viperchange.bin
--rw-rw-rw-   0        0        0      317 2023-04-09 03:38:21.000000 iog-randomizer-4.4.9.1/randomizer/bin/0bfd00_switches.bin
--rw-rw-rw-   0        0        0      434 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/bin/0bfe40_infdeath.bin
--rw-rw-rw-   0        0        0      211 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/0ce099_babel.bin
--rw-rw-rw-   0        0        0    12286 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/0d8000_mapdata.bin
--rw-rw-rw-   0        0        0      112 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9.1/randomizer/bin/0f8fa4_fluteless.bin
--rw-rw-rw-   0        0        0       68 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/108ea3_multijewel.bin
--rw-rw-rw-   0        0        0     1531 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/193d25_ishtarpuzzle.bin
--rw-rw-rw-   0        0        0     1257 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/1a5a37_angelmap.bin
--rw-rw-rw-   0        0        0      481 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/1d42a2_incatile.bin
--rw-rw-rw-   0        0        0      486 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/1e28a5_mupassage.bin
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/__init__.py
--rw-rw-rw-   0        0        0     1024 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/incamapblank.bin
--rw-rw-rw-   0        0        0     4096 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/ishtarmapblank.bin
--rw-rw-rw-   0        0        0       57 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/bin/item_get_blank.bin
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.500513 iog-randomizer-4.4.9.1/randomizer/bin/plugins/
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.234717 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/
--rw-rw-rw-   0        0        0        4 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00800f_BrkVector.bin
--rw-rw-rw-   0        0        0      472 2020-02-26 04:14:02.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/008476_FasterInterrupts.bin
--rw-rw-rw-   0        0        0       34 2023-02-07 15:44:11.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/008ffd_FasterCop23.bin
--rw-rw-rw-   0        0        0       15 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00b125_PageAlignedActorFinder.bin
--rw-rw-rw-   0        0        0      174 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00bce1_FasterCometShimmerThinkers.bin
--rw-rw-rw-   0        0        0       46 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00f3d7_FasterOrbiters.bin
--rw-rw-rw-   0        0        0      229 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/00fd00_LibsAndMisc.bin
--rw-rw-rw-   0        0        0       12 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0281da_FasterMultiplication.bin
--rw-rw-rw-   0        0        0       12 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0281ee_FasterDivision.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/02a5e8_HereBeDragons_RemoveNops.bin
--rw-rw-rw-   0        0        0        1 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03c84b_FasterRenderingFragment.bin
--rw-rw-rw-   0        0        0      193 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03c854_FasterRendering.bin
--rw-rw-rw-   0        0        0      125 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03ca5f_FasterAnimating.bin
--rw-rw-rw-   0        0        0       27 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03cde4_HereBeDragons_PageAlignActorIds.bin
--rw-rw-rw-   0        0        0       15 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/03f745_PageAlignActorIdsHelper.bin
--rw-rw-rw-   0        0        0     1362 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/07e9fc_ApocalypseGaiaAssets2.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c313_PageAlignPyramidSmasher8.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c3b2_PageAlignPyramidSmasher7.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:03.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c49c_PageAlignPyramidSmasher3.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c556_PageAlignPyramidSmasher5.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c567_PageAlignPyramidSmasher6.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c5da_PageAlignPyramidSmasher1.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c5ef_PageAlignPyramidSmasher2.bin
--rw-rw-rw-   0        0        0        2 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/08c61c_PageAlignPyramidSmasher4.bin
--rw-rw-rw-   0        0        0     4114 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/09aa6e_ApocalypseGaiaCode.bin
--rw-rw-rw-   0        0        0     1783 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/09f790_ApocalypseGaiaAssets1.bin
--rw-rw-rw-   0        0        0        7 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0aa36e_FasterMakePlayerImmune.bin
--rw-rw-rw-   0        0        0        4 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0acbf2_FixVanillaGardenWormBug.bin
--rw-rw-rw-   0        0        0      530 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0afd87_PushAndUpdateAGAssets.bin
--rw-rw-rw-   0        0        0        9 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0ceac7_CometThinkerTableFragment.bin
--rw-rw-rw-   0        0        0      470 2020-02-26 04:14:04.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0ceb74_CometThinkers.bin
--rw-rw-rw-   0        0        0     1837 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/0ceeaa_CometAndDarkGaiaCode.bin
--rw-rw-rw-   0        0        0        1 2020-02-26 04:14:05.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/AG/1f2ce7_SetCometBg2HeightTo2.bin
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:13.516109 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.250339 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/
--rw-rw-rw-   0        0        0    16384 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/1a8000.bin
--rw-rw-rw-   0        0        0     5120 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/bagu/1b8000.bin
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.265959 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/freet/
--rw-rw-rw-   0        0        0     2356 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/freet/1a820a.bin
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.281581 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/
--rw-rw-rw-   0        0        0    32768 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1a8000.bin
--rw-rw-rw-   0        0        0    32768 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1b8000.bin
--rw-rw-rw-   0        0        0    16384 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/invisible/1c8000.bin
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.281581 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/solar/
--rw-rw-rw-   0        0        0    69280 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/solar/1a8000.bin
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.297202 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/sye/
--rw-rw-rw-   0        0        0    69280 2021-03-25 16:08:24.000000 iog-randomizer-4.4.9.1/randomizer/bin/plugins/sprites/sye/1a8000.bin
--rw-rw-rw-   0        0        0   331576 2023-04-09 03:38:21.000000 iog-randomizer-4.4.9.1/randomizer/classes.py
--rw-rw-rw-   0        0        0    68771 2021-04-20 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/constants.py
--rw-rw-rw-   0        0        0      191 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/errors.py
--rw-rw-rw-   0        0        0   200866 2023-04-09 04:45:25.000000 iog-randomizer-4.4.9.1/randomizer/iogr_rom.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.297202 iog-randomizer-4.4.9.1/randomizer/models/
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/randomizer/models/enums/
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/__init__.py
--rw-rw-rw-   0        0        0      113 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/difficulty.py
--rw-rw-rw-   0        0        0      129 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/enemizer.py
--rw-rw-rw-   0        0        0      107 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/entrance_shuffle.py
--rw-rw-rw-   0        0        0      128 2020-02-26 04:14:06.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/goal.py
--rw-rw-rw-   0        0        0      121 2021-03-25 16:41:36.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/level.py
--rw-rw-rw-   0        0        0      101 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/logic.py
--rw-rw-rw-   0        0        0      174 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/sprites.py
--rw-rw-rw-   0        0        0      128 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/start_location.py
--rw-rw-rw-   0        0        0      118 2021-09-13 18:24:28.000000 iog-randomizer-4.4.9.1/randomizer/models/enums/statue_req.py
--rw-rw-rw-   0        0        0     2097 2023-04-09 03:38:21.000000 iog-randomizer-4.4.9.1/randomizer/models/randomizer_data.py
--rw-rw-rw-   0        0        0      818 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/patch.py
--rw-rw-rw-   0        0        0     4190 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/quintet_comp.py
--rw-rw-rw-   0        0        0    18409 2019-11-10 22:39:22.000000 iog-randomizer-4.4.9.1/randomizer/quintet_text.py
-drwxrwxrwx   0        0        0        0 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/randomizer/tests/
--rw-rw-rw-   0        0        0        0 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/tests/__init__.py
--rw-rw-rw-   0        0        0      407 2019-11-10 22:39:12.000000 iog-randomizer-4.4.9.1/randomizer/tests/test_generate_filename.py
--rw-rw-rw-   0        0        0       42 2023-04-09 04:47:14.359680 iog-randomizer-4.4.9.1/setup.cfg
--rw-rw-rw-   0        0        0      520 2023-04-09 04:45:36.000000 iog-randomizer-4.4.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:09:04.422208 iog-randomizer-4.7.2/
+-rw-rw-rw-   0        0        0     1233 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/LICENSE
+-rw-rw-rw-   0        0        0      233 2024-04-05 03:09:04.422208 iog-randomizer-4.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16459 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:09:04.422208 iog-randomizer-4.7.2/iog_randomizer.egg-info/
+-rw-rw-rw-   0        0        0      233 2024-04-05 03:09:04.000000 iog-randomizer-4.7.2/iog_randomizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2024-04-05 03:09:04.000000 iog-randomizer-4.7.2/iog_randomizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:09:04.000000 iog-randomizer-4.7.2/iog_randomizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 03:09:04.000000 iog-randomizer-4.7.2/iog_randomizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 03:09:04.000000 iog-randomizer-4.7.2/iog_randomizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 03:09:04.406598 iog-randomizer-4.7.2/randomizer/
+-rw-rw-rw-   0        0        0      834 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin
+-rw-rw-rw-   0        0        0      511 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/ATlMpMuSWWaterHighSub_Tilemap1_comp.bin
+-rw-rw-rw-   0        0        0     2341 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/ATlMpSpecInvBg_comp.bin
+-rw-rw-rw-   0        0        0     4437 2024-03-30 19:58:01.000000 iog-randomizer-4.7.2/randomizer/ConfigValueArray.asr
+-rw-rw-rw-   0        0        0     1257 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/Tilemap6D.bin
+-rw-rw-rw-   0        0        0      486 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/TilemapMuPassage.bin
+-rw-rw-rw-   0        0        0       25 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/__init__.py
+-rw-rw-rw-   0        0        0    72688 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/apocalypse_gaia_1.asr
+-rw-rw-rw-   0        0        0    20962 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/apocalypse_gaia_2.asr
+-rw-rw-rw-   0        0        0   489472 2024-04-01 04:14:16.000000 iog-randomizer-4.7.2/randomizer/asar-x64.dll
+-rw-rw-rw-   0        0        0   330280 2024-04-01 04:20:21.000000 iog-randomizer-4.7.2/randomizer/asar-x64.so
+-rw-rw-rw-   0        0        0   344576 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/asar-x86.dll
+-rw-rw-rw-   0        0        0    14569 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/asar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:09:04.406598 iog-randomizer-4.7.2/randomizer/bin/
+-rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/bin/__init__.py
+-rw-rw-rw-   0        0        0   422504 2024-04-04 00:57:03.000000 iog-randomizer-4.7.2/randomizer/classes.py
+-rw-rw-rw-   0        0        0      191 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/errors.py
+-rw-rw-rw-   0        0        0   247876 2024-03-30 20:09:45.000000 iog-randomizer-4.7.2/randomizer/iogr.asr
+-rw-rw-rw-   0        0        0    38030 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/iogr_81_exit_table.asr
+-rw-rw-rw-   0        0        0   218181 2024-03-30 18:04:55.000000 iog-randomizer-4.7.2/randomizer/iogr_8C_actor_table.asr
+-rw-rw-rw-   0        0        0    71930 2024-03-24 00:19:32.000000 iog-randomizer-4.7.2/randomizer/iogr_8D_asset_table.asr
+-rw-rw-rw-   0        0        0    12873 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/iogr_asset_ledger.asr
+-rw-rw-rw-   0        0        0    75385 2024-03-30 19:42:22.000000 iog-randomizer-4.7.2/randomizer/iogr_code_overflow.asr
+-rw-rw-rw-   0        0        0    29315 2024-03-20 04:46:27.000000 iog-randomizer-4.7.2/randomizer/iogr_dialogue_overflow.asr
+-rw-rw-rw-   0        0        0    52543 2024-03-14 01:52:07.000000 iog-randomizer-4.7.2/randomizer/iogr_exit_ledger.asr
+-rw-rw-rw-   0        0        0      112 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/iogr_fluteless_melody_anim.bin
+-rw-rw-rw-   0        0        0    12140 2024-03-30 19:35:02.000000 iog-randomizer-4.7.2/randomizer/iogr_misc_defines.asr
+-rw-rw-rw-   0        0        0   436119 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/iogr_monster_defaults.asr
+-rw-rw-rw-   0        0        0    56906 2024-04-04 01:18:16.000000 iog-randomizer-4.7.2/randomizer/iogr_rom.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:09:04.406598 iog-randomizer-4.7.2/randomizer/models/
+-rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/models/__init__.py
+-rw-rw-rw-   0        0        0     1452 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/models/enums.py
+-rw-rw-rw-   0        0        0     3164 2024-04-01 05:08:10.000000 iog-randomizer-4.7.2/randomizer/models/randomizer_data.py
+-rw-rw-rw-   0        0        0      818 2023-02-24 03:45:40.000000 iog-randomizer-4.7.2/randomizer/patch.py
+-rw-rw-rw-   0        0        0     4190 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/quintet_comp.py
+-rw-rw-rw-   0        0        0    18409 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/quintet_text.py
+-rw-rw-rw-   0        0        0      544 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/table_dialogue.txt
+-rw-rw-rw-   0        0        0      520 2024-03-11 03:06:01.000000 iog-randomizer-4.7.2/randomizer/table_invtext.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 03:09:04.406598 iog-randomizer-4.7.2/randomizer/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/tests/__init__.py
+-rw-rw-rw-   0        0        0      407 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2/randomizer/tests/test_generate_filename.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:09:04.422208 iog-randomizer-4.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      551 2024-04-02 00:18:14.000000 iog-randomizer-4.7.2/setup.py
```

### Comparing `iog-randomizer-4.4.9.1/LICENSE` & `iog-randomizer-4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9.1/README.md` & `iog-randomizer-4.7.2/README.md`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9.1/randomizer/bin/1a5a37_angelmap.bin` & `iog-randomizer-4.7.2/randomizer/Tilemap6D.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9.1/randomizer/models/randomizer_data.py` & `iog-randomizer-4.7.2/randomizer/models/randomizer_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,81 @@
 import random
 
-from .enums.difficulty import Difficulty
-from .enums.goal import Goal
-from .enums.statue_req import StatueReq
-from .enums.logic import Logic
-from .enums.entrance_shuffle import EntranceShuffle
-from .enums.enemizer import Enemizer
-from .enums.start_location import StartLocation
-from .enums.sprites import Sprite
-#from .enums.level import Level
-
+#from .enums.difficulty import Difficulty
+#from .enums.goal import Goal
+#from .enums.statue_req import StatueReq
+#from .enums.logic import Logic
+#from .enums.dungeon_shuffle import DungeonShuffle
+#from .enums.orb_rando import OrbRando
+#from .enums.darkrooms import DarkRooms
+#from .enums.enemizer import Enemizer
+#from .enums.start_location import StartLocation
+#from .enums.flute import FluteOpt
+#from .enums.sprites import Sprite
+from .enums import *
 
 class RandomizerData:
-    def __init__(self, seed: int = random.randint(0, 999999999),
-                 difficulty: Difficulty = Difficulty.NORMAL, goal: Goal = Goal.DARK_GAIA, logic: Logic = Logic.COMPLETABLE,
-                 statues: str = "4", statue_req: StatueReq = StatueReq.GAME_CHOICE, enemizer: Enemizer = Enemizer.NONE,
-                 start_location: StartLocation = StartLocation.SOUTH_CAPE, firebird: bool = False, ohko: bool = False,
-                 red_jewel_madness: bool = False, allow_glitches: bool = False, boss_shuffle: bool = False,
-                 open_mode: bool = False, z3: bool = False, overworld_shuffle: bool = False,
-                 entrance_shuffle: EntranceShuffle = EntranceShuffle.NONE, race_mode: bool = False, fluteless: bool = False,
-                 sprite: Sprite = Sprite.WILL, dungeon_shuffle: bool = False):
+    def __init__(self, 
+                 seed: int = random.randint(0, 999999999),
+                 difficulty: Difficulty = Difficulty.NORMAL, 
+                 goal: Goal = Goal.DARK_GAIA, 
+                 logic: Logic = Logic.COMPLETABLE,
+                 statues: str = "4", 
+                 statue_req: StatueReq = StatueReq.GAME_CHOICE, 
+                 start_location: StartLocation = StartLocation.SOUTH_CAPE, 
+                 enemizer: Enemizer = Enemizer.NONE,
+                 coupled_exits : bool = False,
+                 town_shuffle : bool = False,
+                 dungeon_shuffle: bool = False,
+                 overworld_shuffle: bool = False,
+                 orb_rando: bool = False,
+                 darkrooms: DarkRooms = DarkRooms.NONE,
+                 firebird: bool = False, 
+                 ohko: bool = False,
+                 red_jewel_madness: bool = False, 
+                 allow_glitches: bool = False, 
+                 boss_shuffle: bool = False,
+                 open_mode: bool = False, 
+                 z3: bool = False, 
+                 race_mode: bool = False, 
+                 flute: FluteOpt = FluteOpt.START,
+                 sprite: Sprite = Sprite.WILL,
+                 printlevel: PrintLevel = PrintLevel.SILENT,
+                 break_on_error: bool = False,
+                 break_on_init: bool = False,
+                 ingame_debug: bool = False,
+                 infinite_inventory: bool = False
+                 ):
         self.seed = seed
         self.difficulty = difficulty
-#        self.level = level
         self.start_location = start_location
         self.goal = goal
         self.statue_req = statue_req
         self.logic = logic
         self.statues = statues
         self.enemizer = enemizer
         self.firebird = firebird
         self.ohko = ohko
         self.red_jewel_madness = red_jewel_madness
         self.allow_glitches = allow_glitches
         self.boss_shuffle = boss_shuffle
+        self.coupled_exits = coupled_exits
+        self.town_shuffle = town_shuffle
         self.overworld_shuffle = overworld_shuffle
         self.dungeon_shuffle = dungeon_shuffle
+        self.orb_rando = orb_rando
+        self.darkrooms = darkrooms
         self.open_mode = open_mode
         self.z3 = z3
-        self.overworld_shuffle = overworld_shuffle
-        self.entrance_shuffle = entrance_shuffle
         self.race_mode = race_mode
-        self.fluteless = fluteless
+        self.flute = flute
         self.sprite = sprite
+        self.printlevel = printlevel
+        self.break_on_error = break_on_error
+        self.break_on_init = break_on_init
+        self.ingame_debug = ingame_debug
+        self.infinite_inventory = infinite_inventory
+        
+        
+        
+        
+
```

### Comparing `iog-randomizer-4.4.9.1/randomizer/patch.py` & `iog-randomizer-4.7.2/randomizer/patch.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9.1/randomizer/quintet_comp.py` & `iog-randomizer-4.7.2/randomizer/quintet_comp.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9.1/randomizer/quintet_text.py` & `iog-randomizer-4.7.2/randomizer/quintet_text.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.4.9.1/setup.py` & `iog-randomizer-4.7.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='iog-randomizer',
-    version='4.4.9.1',
+    version='4.7.2',
     description='The Illusion of Gaia Randomizer',
     author='dontbagume,bryon_w,raeven0',
     packages=setuptools.find_packages(),
     package_data={'': [
-        'bin/*.bin',
-        'bin/plugins/**/*.bin',
-        'bin/plugins/**/**/*.bin'
+        '*.bin',
+        '*.asr',
+        '*.txt',
+        'asar-x86.dll',
+        'asar-x64.dll',
+        'asar-x64.so'
     ]},
-    install_requires=['bitstring', 'graphviz'],
+    install_requires=['ips.py', 'bsdiff4'],
     python_requires='>=3.7'
 )
```

