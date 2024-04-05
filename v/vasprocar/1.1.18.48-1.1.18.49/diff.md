# Comparing `tmp/vasprocar-1.1.18.48.tar.gz` & `tmp/vasprocar-1.1.18.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasprocar-1.1.18.48.tar", last modified: Thu Apr  4 11:18:53 2024, max compression
+gzip compressed data, was "vasprocar-1.1.18.49.tar", last modified: Fri Apr  5 15:48:32 2024, max compression
```

## Comparing `vasprocar-1.1.18.48.tar` & `vasprocar-1.1.18.49.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.822315 vasprocar-1.1.18.48/
--rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.18.48/LICENSE.txt
--rw-rw-rw-   0        0        0     2384 2024-04-04 11:18:53.822315 vasprocar-1.1.18.48/PKG-INFO
--rw-rw-rw-   0        0        0     1750 2024-02-22 09:27:02.000000 vasprocar-1.1.18.48/README.md
--rw-rw-rw-   0        0        0      167 2024-04-04 11:18:53.822315 vasprocar-1.1.18.48/setup.cfg
--rw-rw-rw-   0        0        0     1316 2024-04-04 11:18:05.000000 vasprocar-1.1.18.48/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:52.806692 vasprocar-1.1.18.48/vasprocar/
--rw-rw-rw-   0        0        0      354 2024-04-04 11:18:23.000000 vasprocar-1.1.18.48/vasprocar/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.18.48/vasprocar/DOI.png
--rw-rw-rw-   0        0        0     6780 2024-04-04 11:18:17.000000 vasprocar-1.1.18.48/vasprocar/VASProcar.py
--rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.18.48/vasprocar/__init__.py
--rw-rw-rw-   0        0        0     6770 2024-04-04 11:18:28.000000 vasprocar-1.1.18.48/vasprocar/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.056690 vasprocar-1.1.18.48/vasprocar/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.150442 vasprocar-1.1.18.48/vasprocar/src/_QE/
--rw-rw-rw-   0        0        0    12921 2024-03-16 13:46:55.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/_info.py
--rw-rw-rw-   0        0        0    16423 2024-03-16 13:47:11.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/_info_b.py
--rw-rw-rw-   0        0        0    12814 2023-09-21 16:58:26.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/_label.py
--rw-rw-rw-   0        0        0    44091 2023-12-03 17:37:36.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/_nscf.py
--rw-rw-rw-   0        0        0     2483 2023-09-21 16:59:54.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/_var_kpoints.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.181701 vasprocar-1.1.18.48/vasprocar/src/_QE/angular_momentum_plot/
--rw-rw-rw-   0        0        0    14015 2024-01-29 14:09:16.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum.py
--rw-rw-rw-   0        0        0     7508 2024-01-29 14:09:08.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum_grace.py
--rw-rw-rw-   0        0        0     6330 2023-09-22 16:45:30.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/contribuicao.py
--rw-rw-rw-   0        0        0    22403 2024-01-29 14:14:16.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_pdos_ldos.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.197323 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.228578 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/Grace/
--rw-rw-rw-   0        0        0     8336 2023-09-15 19:03:32.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    11554 2023-09-15 19:03:36.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0     9549 2023-09-15 19:03:38.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
--rw-rw-rw-   0        0        0     7562 2024-01-29 14:09:34.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    14126 2024-01-29 14:09:46.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    21098 2023-09-21 17:00:44.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/kpoints_2D_3D.py
--rw-rw-rw-   0        0        0    25817 2023-12-04 09:45:46.000000 vasprocar-1.1.18.48/vasprocar/src/_QE/projecao_angular_momentum.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.400524 vasprocar-1.1.18.48/vasprocar/src/_VASP/
--rw-rw-rw-   0        0        0    19222 2024-03-16 13:29:30.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/_info.py
--rw-rw-rw-   0        0        0    16150 2024-03-23 12:41:26.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/_info_b.py
--rw-rw-rw-   0        0        0    15757 2023-07-10 18:09:14.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/_label.py
--rw-rw-rw-   0        0        0    31582 2023-10-04 12:11:22.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/_nscf.py
--rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/_var_kpoints.py
--rw-rw-rw-   0        0        0    20778 2023-12-21 11:19:52.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/chgcar.py
--rw-rw-rw-   0        0        0     3973 2023-12-04 12:19:52.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/contcar_info.py
--rw-rw-rw-   0        0        0    32211 2023-11-27 23:28:10.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/contribuicao.py
--rw-rw-rw-   0        0        0    14157 2023-10-12 13:33:34.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/dielectric_function.py
--rw-rw-rw-   0        0        0    26844 2023-10-12 13:34:02.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    28798 2023-10-12 13:34:22.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    24750 2024-03-16 15:19:14.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/kpoints_2D_3D.py
--rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:48.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/parchg.py
--rw-rw-rw-   0        0        0    13024 2024-04-02 11:50:06.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/poscar_replace.py
--rw-rw-rw-   0        0        0     4159 2023-07-03 14:06:18.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/postar_combination.py
--rw-rw-rw-   0        0        0    14992 2024-03-23 12:24:01.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/potencial.py
--rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:32.000000 vasprocar-1.1.18.48/vasprocar/src/_VASP/wave_function.py
--rw-rw-rw-   0        0        0     2096 2023-09-21 18:37:20.000000 vasprocar-1.1.18.48/vasprocar/src/_dft.py
--rw-rw-rw-   0        0        0     2613 2023-08-16 17:17:52.000000 vasprocar-1.1.18.48/vasprocar/src/_dft2kp.py
--rw-rw-rw-   0        0        0      626 2023-02-07 16:00:06.000000 vasprocar-1.1.18.48/vasprocar/src/_loop.py
--rw-rw-rw-   0        0        0    22354 2024-03-16 15:20:46.000000 vasprocar-1.1.18.48/vasprocar/src/_settings.py
--rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:58.000000 vasprocar-1.1.18.48/vasprocar/src/_update.py
--rw-rw-rw-   0        0        0    17873 2024-01-29 14:10:10.000000 vasprocar-1.1.18.48/vasprocar/src/bandas_2D.py
--rw-rw-rw-   0        0        0    16726 2023-10-12 13:28:10.000000 vasprocar-1.1.18.48/vasprocar/src/bandas_3D.py
--rw-rw-rw-   0        0        0    15050 2023-10-12 13:29:40.000000 vasprocar-1.1.18.48/vasprocar/src/bandas_4D.py
--rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:58.000000 vasprocar-1.1.18.48/vasprocar/src/correction_file.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.416065 vasprocar-1.1.18.48/vasprocar/src/etc/
--rw-rw-rw-   0        0        0      354 2024-04-04 11:18:41.000000 vasprocar-1.1.18.48/vasprocar/src/etc/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.18.48/vasprocar/src/etc/DOI.png
--rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.18.48/vasprocar/src/etc/Greek_alphabet.jpg
--rw-rw-rw-   0        0        0    20207 2023-10-12 13:29:58.000000 vasprocar-1.1.18.48/vasprocar/src/fermi_surface.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.431697 vasprocar-1.1.18.48/vasprocar/src/inputs/
--rw-rw-rw-   0        0        0     1030 2024-03-23 11:43:33.000000 vasprocar-1.1.18.48/vasprocar/src/inputs/inputs.py
--rw-rw-rw-   0        0        0     4558 2024-03-23 11:42:30.000000 vasprocar-1.1.18.48/vasprocar/src/inputs/inputs_files.py
--rw-rw-rw-   0        0        0    17107 2023-10-12 13:30:18.000000 vasprocar-1.1.18.48/vasprocar/src/level_countour.py
--rw-rw-rw-   0        0        0    17750 2023-10-12 13:30:40.000000 vasprocar-1.1.18.48/vasprocar/src/orbital_texture.py
--rw-rw-rw-   0        0        0    23234 2023-10-12 13:31:08.000000 vasprocar-1.1.18.48/vasprocar/src/orbital_texture_vector.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.697355 vasprocar-1.1.18.48/vasprocar/src/plot/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:53.822315 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/
--rw-rw-rw-   0        0        0     5204 2023-04-28 13:13:46.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_chgcar.py
--rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:26.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:42.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:50.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
--rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:06.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_parchg.py
--rw-rw-rw-   0        0        0     4538 2024-03-23 13:43:36.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_potencial.py
--rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    11205 2024-02-20 15:02:00.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:00.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_psi.py
--rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:28.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_spin.py
--rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:34.000000 vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_wave_function.py
--rw-rw-rw-   0        0        0     6702 2023-10-11 15:26:00.000000 vasprocar-1.1.18.48/vasprocar/src/plot/_plot_settings.py
--rw-rw-rw-   0        0        0     5999 2024-01-29 13:57:08.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     5234 2024-03-14 17:09:52.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
--rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_3D_plotly.py
--rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:26.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_4D_plotly.py
--rw-rw-rw-   0        0        0     5162 2024-01-29 13:57:34.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_chgcar.py
--rw-rw-rw-   0        0        0     4451 2024-01-29 13:57:46.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    13077 2024-01-29 13:57:58.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    34343 2024-01-29 14:00:28.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0     8462 2024-03-02 21:35:54.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_fermi_surface.py
--rw-rw-rw-   0        0        0     6674 2024-01-29 14:01:36.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_level_countour.py
--rw-rw-rw-   0        0        0     5754 2024-02-19 12:35:00.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_orbital_texture.py
--rw-rw-rw-   0        0        0    15856 2024-01-29 14:02:28.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_orbital_texture_vector.py
--rw-rw-rw-   0        0        0     4841 2024-01-29 14:02:46.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_parchg.py
--rw-rw-rw-   0        0        0     5260 2024-03-23 13:44:41.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_potencial.py
--rw-rw-rw-   0        0        0    14457 2024-01-29 14:03:32.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    27211 2024-01-29 14:03:56.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0    14579 2024-01-29 14:04:20.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_psi.py
--rw-rw-rw-   0        0        0     7930 2024-01-29 14:04:36.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_spin.py
--rw-rw-rw-   0        0        0    11950 2024-01-29 14:05:04.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_2D.py
--rw-rw-rw-   0        0        0     9946 2023-08-19 20:48:50.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_3D.py
--rw-rw-rw-   0        0        0     6358 2023-08-19 20:51:30.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_4D.py
--rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:36.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
--rw-rw-rw-   0        0        0    17713 2024-02-28 18:33:30.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_contour.py
--rw-rw-rw-   0        0        0    17381 2024-03-02 21:35:34.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_contour_video.py
--rw-rw-rw-   0        0        0     4740 2024-01-29 14:06:52.000000 vasprocar-1.1.18.48/vasprocar/src/plot/plot_wave_function.py
--rw-rw-rw-   0        0        0    35093 2023-12-04 13:57:40.000000 vasprocar-1.1.18.48/vasprocar/src/projecao_localizacao.py
--rw-rw-rw-   0        0        0    34805 2023-12-01 18:31:14.000000 vasprocar-1.1.18.48/vasprocar/src/projecao_orbitais.py
--rw-rw-rw-   0        0        0    33341 2023-10-12 13:31:54.000000 vasprocar-1.1.18.48/vasprocar/src/projecao_psi.py
--rw-rw-rw-   0        0        0    35892 2023-12-05 12:53:10.000000 vasprocar-1.1.18.48/vasprocar/src/projecao_spin.py
--rw-rw-rw-   0        0        0    27113 2023-10-12 13:32:24.000000 vasprocar-1.1.18.48/vasprocar/src/spin_texture.py
--rw-rw-rw-   0        0        0    28679 2024-02-27 13:02:24.000000 vasprocar-1.1.18.48/vasprocar/src/spin_texture_contour.py
--rw-rw-rw-   0        0        0    28044 2023-10-12 13:33:00.000000 vasprocar-1.1.18.48/vasprocar/src/spin_texture_contour_video.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:18:52.837940 vasprocar-1.1.18.48/vasprocar.egg-info/
--rw-rw-rw-   0        0        0     2384 2024-04-04 11:18:52.000000 vasprocar-1.1.18.48/vasprocar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4251 2024-04-04 11:18:52.000000 vasprocar-1.1.18.48/vasprocar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:18:52.000000 vasprocar-1.1.18.48/vasprocar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-04 11:18:52.000000 vasprocar-1.1.18.48/vasprocar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      117 2024-04-04 11:18:52.000000 vasprocar-1.1.18.48/vasprocar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 11:18:52.000000 vasprocar-1.1.18.48/vasprocar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:32.589183 vasprocar-1.1.18.49/
+-rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.18.49/LICENSE.txt
+-rw-rw-rw-   0        0        0     2384 2024-04-05 15:48:32.589183 vasprocar-1.1.18.49/PKG-INFO
+-rw-rw-rw-   0        0        0     1750 2024-02-22 09:27:02.000000 vasprocar-1.1.18.49/README.md
+-rw-rw-rw-   0        0        0      167 2024-04-05 15:48:32.589183 vasprocar-1.1.18.49/setup.cfg
+-rw-rw-rw-   0        0        0     1316 2024-04-05 15:47:47.000000 vasprocar-1.1.18.49/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:31.542303 vasprocar-1.1.18.49/vasprocar/
+-rw-rw-rw-   0        0        0      354 2024-04-05 15:48:07.000000 vasprocar-1.1.18.49/vasprocar/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.18.49/vasprocar/DOI.png
+-rw-rw-rw-   0        0        0     6780 2024-04-05 15:48:01.000000 vasprocar-1.1.18.49/vasprocar/VASProcar.py
+-rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.18.49/vasprocar/__init__.py
+-rw-rw-rw-   0        0        0     6770 2024-04-05 15:47:56.000000 vasprocar-1.1.18.49/vasprocar/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:31.761047 vasprocar-1.1.18.49/vasprocar/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:31.870421 vasprocar-1.1.18.49/vasprocar/src/_QE/
+-rw-rw-rw-   0        0        0    12921 2024-03-16 13:46:54.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/_info.py
+-rw-rw-rw-   0        0        0    16423 2024-03-16 13:47:10.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/_info_b.py
+-rw-rw-rw-   0        0        0    12814 2023-09-21 16:58:26.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/_label.py
+-rw-rw-rw-   0        0        0    44091 2023-12-03 17:37:36.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/_nscf.py
+-rw-rw-rw-   0        0        0     2483 2023-09-21 16:59:54.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/_var_kpoints.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:31.886050 vasprocar-1.1.18.49/vasprocar/src/_QE/angular_momentum_plot/
+-rw-rw-rw-   0        0        0    14015 2024-01-29 14:09:16.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum.py
+-rw-rw-rw-   0        0        0     7508 2024-01-29 14:09:08.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum_grace.py
+-rw-rw-rw-   0        0        0     6330 2023-09-22 16:45:30.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/contribuicao.py
+-rw-rw-rw-   0        0        0    22403 2024-01-29 14:14:16.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_pdos_ldos.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:31.917298 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:31.948545 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/Grace/
+-rw-rw-rw-   0        0        0     8336 2023-09-15 19:03:32.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    11554 2023-09-15 19:03:36.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0     9549 2023-09-15 19:03:38.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
+-rw-rw-rw-   0        0        0     7562 2024-01-29 14:09:34.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    14126 2024-01-29 14:09:46.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    21098 2023-09-21 17:00:44.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/kpoints_2D_3D.py
+-rw-rw-rw-   0        0        0    25817 2023-12-04 09:45:46.000000 vasprocar-1.1.18.49/vasprocar/src/_QE/projecao_angular_momentum.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:32.104797 vasprocar-1.1.18.49/vasprocar/src/_VASP/
+-rw-rw-rw-   0        0        0    19222 2024-03-16 13:29:30.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/_info.py
+-rw-rw-rw-   0        0        0    16150 2024-03-23 12:41:26.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/_info_b.py
+-rw-rw-rw-   0        0        0    16979 2024-04-05 15:45:10.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/_label.py
+-rw-rw-rw-   0        0        0    31582 2023-10-04 12:11:22.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/_nscf.py
+-rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/_var_kpoints.py
+-rw-rw-rw-   0        0        0    20778 2023-12-21 11:19:52.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/chgcar.py
+-rw-rw-rw-   0        0        0     3973 2023-12-04 12:19:52.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/contcar_info.py
+-rw-rw-rw-   0        0        0    32211 2023-11-27 23:28:10.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/contribuicao.py
+-rw-rw-rw-   0        0        0    14157 2023-10-12 13:33:34.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/dielectric_function.py
+-rw-rw-rw-   0        0        0    26844 2023-10-12 13:34:02.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    28798 2023-10-12 13:34:22.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    24750 2024-03-16 15:19:14.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/kpoints_2D_3D.py
+-rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:48.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/parchg.py
+-rw-rw-rw-   0        0        0    13024 2024-04-02 11:50:06.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/poscar_replace.py
+-rw-rw-rw-   0        0        0     4159 2023-07-03 14:06:18.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/postar_combination.py
+-rw-rw-rw-   0        0        0    14992 2024-03-23 12:24:00.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/potencial.py
+-rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:32.000000 vasprocar-1.1.18.49/vasprocar/src/_VASP/wave_function.py
+-rw-rw-rw-   0        0        0     2096 2023-09-21 18:37:20.000000 vasprocar-1.1.18.49/vasprocar/src/_dft.py
+-rw-rw-rw-   0        0        0     2613 2023-08-16 17:17:52.000000 vasprocar-1.1.18.49/vasprocar/src/_dft2kp.py
+-rw-rw-rw-   0        0        0      626 2023-02-07 16:00:06.000000 vasprocar-1.1.18.49/vasprocar/src/_loop.py
+-rw-rw-rw-   0        0        0    22354 2024-03-16 15:20:46.000000 vasprocar-1.1.18.49/vasprocar/src/_settings.py
+-rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:58.000000 vasprocar-1.1.18.49/vasprocar/src/_update.py
+-rw-rw-rw-   0        0        0    17514 2024-04-05 15:46:20.000000 vasprocar-1.1.18.49/vasprocar/src/bandas_2D.py
+-rw-rw-rw-   0        0        0    16726 2023-10-12 13:28:10.000000 vasprocar-1.1.18.49/vasprocar/src/bandas_3D.py
+-rw-rw-rw-   0        0        0    15050 2023-10-12 13:29:40.000000 vasprocar-1.1.18.49/vasprocar/src/bandas_4D.py
+-rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:58.000000 vasprocar-1.1.18.49/vasprocar/src/correction_file.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:32.136046 vasprocar-1.1.18.49/vasprocar/src/etc/
+-rw-rw-rw-   0        0        0      354 2024-04-05 15:48:16.000000 vasprocar-1.1.18.49/vasprocar/src/etc/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.18.49/vasprocar/src/etc/DOI.png
+-rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.18.49/vasprocar/src/etc/Greek_alphabet.jpg
+-rw-rw-rw-   0        0        0    20207 2023-10-12 13:29:58.000000 vasprocar-1.1.18.49/vasprocar/src/fermi_surface.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:32.151672 vasprocar-1.1.18.49/vasprocar/src/inputs/
+-rw-rw-rw-   0        0        0     1030 2024-03-23 11:43:32.000000 vasprocar-1.1.18.49/vasprocar/src/inputs/inputs.py
+-rw-rw-rw-   0        0        0     4558 2024-03-23 11:42:30.000000 vasprocar-1.1.18.49/vasprocar/src/inputs/inputs_files.py
+-rw-rw-rw-   0        0        0    17107 2023-10-12 13:30:18.000000 vasprocar-1.1.18.49/vasprocar/src/level_countour.py
+-rw-rw-rw-   0        0        0    17750 2023-10-12 13:30:40.000000 vasprocar-1.1.18.49/vasprocar/src/orbital_texture.py
+-rw-rw-rw-   0        0        0    23234 2023-10-12 13:31:08.000000 vasprocar-1.1.18.49/vasprocar/src/orbital_texture_vector.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:32.464174 vasprocar-1.1.18.49/vasprocar/src/plot/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:32.573547 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/
+-rw-rw-rw-   0        0        0     5257 2024-04-05 15:06:09.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:26.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:42.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:50.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
+-rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:06.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_parchg.py
+-rw-rw-rw-   0        0        0     4538 2024-03-23 13:43:36.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_potencial.py
+-rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    11205 2024-02-20 15:02:00.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:00.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:28.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:34.000000 vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_wave_function.py
+-rw-rw-rw-   0        0        0     6702 2023-10-11 15:26:00.000000 vasprocar-1.1.18.49/vasprocar/src/plot/_plot_settings.py
+-rw-rw-rw-   0        0        0     5999 2024-01-29 13:57:08.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     5234 2024-03-14 17:09:52.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
+-rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_3D_plotly.py
+-rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:26.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_4D_plotly.py
+-rw-rw-rw-   0        0        0     5162 2024-01-29 13:57:34.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4451 2024-01-29 13:57:46.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    13077 2024-01-29 13:57:58.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    34343 2024-01-29 14:00:28.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0     8462 2024-03-02 21:35:54.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_fermi_surface.py
+-rw-rw-rw-   0        0        0     6674 2024-01-29 14:01:36.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_level_countour.py
+-rw-rw-rw-   0        0        0     5754 2024-02-19 12:35:00.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_orbital_texture.py
+-rw-rw-rw-   0        0        0    15856 2024-01-29 14:02:28.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_orbital_texture_vector.py
+-rw-rw-rw-   0        0        0     4841 2024-01-29 14:02:46.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_parchg.py
+-rw-rw-rw-   0        0        0     5260 2024-03-23 13:44:40.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_potencial.py
+-rw-rw-rw-   0        0        0    14457 2024-01-29 14:03:32.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    27211 2024-01-29 14:03:56.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0    14579 2024-01-29 14:04:20.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0     7930 2024-01-29 14:04:36.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0    11950 2024-01-29 14:05:04.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_2D.py
+-rw-rw-rw-   0        0        0     9946 2023-08-19 20:48:50.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_3D.py
+-rw-rw-rw-   0        0        0     6358 2023-08-19 20:51:30.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_4D.py
+-rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:36.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
+-rw-rw-rw-   0        0        0    17713 2024-02-28 18:33:30.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_contour.py
+-rw-rw-rw-   0        0        0    17381 2024-03-02 21:35:34.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_contour_video.py
+-rw-rw-rw-   0        0        0     4740 2024-01-29 14:06:52.000000 vasprocar-1.1.18.49/vasprocar/src/plot/plot_wave_function.py
+-rw-rw-rw-   0        0        0    34752 2024-04-05 15:46:45.000000 vasprocar-1.1.18.49/vasprocar/src/projecao_localizacao.py
+-rw-rw-rw-   0        0        0    34446 2024-04-05 15:47:02.000000 vasprocar-1.1.18.49/vasprocar/src/projecao_orbitais.py
+-rw-rw-rw-   0        0        0    33000 2024-04-05 15:47:16.000000 vasprocar-1.1.18.49/vasprocar/src/projecao_psi.py
+-rw-rw-rw-   0        0        0    35533 2024-04-05 15:47:35.000000 vasprocar-1.1.18.49/vasprocar/src/projecao_spin.py
+-rw-rw-rw-   0        0        0    27113 2023-10-12 13:32:24.000000 vasprocar-1.1.18.49/vasprocar/src/spin_texture.py
+-rw-rw-rw-   0        0        0    28679 2024-02-27 13:02:24.000000 vasprocar-1.1.18.49/vasprocar/src/spin_texture_contour.py
+-rw-rw-rw-   0        0        0    28044 2023-10-12 13:33:00.000000 vasprocar-1.1.18.49/vasprocar/src/spin_texture_contour_video.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:48:31.573579 vasprocar-1.1.18.49/vasprocar.egg-info/
+-rw-rw-rw-   0        0        0     2384 2024-04-05 15:48:31.000000 vasprocar-1.1.18.49/vasprocar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4251 2024-04-05 15:48:31.000000 vasprocar-1.1.18.49/vasprocar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:48:31.000000 vasprocar-1.1.18.49/vasprocar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-05 15:48:31.000000 vasprocar-1.1.18.49/vasprocar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2024-04-05 15:48:31.000000 vasprocar-1.1.18.49/vasprocar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 15:48:31.000000 vasprocar-1.1.18.49/vasprocar.egg-info/top_level.txt
```

### Comparing `vasprocar-1.1.18.48/LICENSE.txt` & `vasprocar-1.1.18.49/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/PKG-INFO` & `vasprocar-1.1.18.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.18.48
+Version: 1.1.18.49
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP/QE codes, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.18.48/README.md` & `vasprocar-1.1.18.49/README.md`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/setup.py` & `vasprocar-1.1.18.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "vasprocar",
-    version = "1.1.18.48",
+    version = "1.1.18.49",
     entry_points={'console_scripts': ['vasprocar = vasprocar:main']},
     description = "VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP/QE codes, through an interactive user interface.",
     author = "Augusto de Lelis Araujo and Renan da Paixao Maciel", 
     author_email = "augusto-lelis@outlook.com, renan.maciel@physics.uu.se",
     url = "https://doi.org/10.5281/zenodo.6343960",
     download_url = "https://doi.org/10.5281/zenodo.6343960",
     license = "GNU GPLv3",
```

### Comparing `vasprocar-1.1.18.48/vasprocar/DOI.png` & `vasprocar-1.1.18.49/vasprocar/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/VASProcar.py` & `vasprocar-1.1.18.49/vasprocar/VASProcar.py`

 * *Files identical despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import sys
 import shutil
 import pyfiglet
 import requests
 
-version = '1.1.18.48'
+version = '1.1.18.49'
 VASProcar_name = 'VASProcar version ' + version
 url_1 = 'https://pypi.org/project/vasprocar'
 url_2 = 'https://doi.org/10.5281/zenodo.6343960'
 url_3 = 'https://github.com/Augusto-de-Lelis-Araujo/VASProcar-Python-tools-VASP'
 
 texto = pyfiglet.figlet_format("VASPROCAR", font="slant", width=100, justify="left")
 print(texto)
```

### Comparing `vasprocar-1.1.18.48/vasprocar/__main__.py` & `vasprocar-1.1.18.49/vasprocar/__main__.py`

 * *Files identical despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import sys
 import shutil
 import pyfiglet
 import requests
 
-version = '1.1.18.48'
+version = '1.1.18.49'
 VASProcar_name = 'VASProcar version ' + version
 url_1 = 'https://pypi.org/project/vasprocar'
 url_2 = 'https://doi.org/10.5281/zenodo.6343960'
 url_3 = 'https://github.com/Augusto-de-Lelis-Araujo/VASProcar-Python-tools-VASP'
 
 texto = pyfiglet.figlet_format("VASPROCAR", font="slant", width=100, justify="left")
 print(texto)
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/_info.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/_info.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/_info_b.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/_info_b.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/_label.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/_label.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/_nscf.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/_nscf.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/_var_kpoints.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/_var_kpoints.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum_grace.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/angular_momentum_plot/plot_projecao_angular_momentum_grace.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/contribuicao.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/contribuicao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/dos_pdos_ldos.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/dos_plot/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/kpoints_2D_3D.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/kpoints_2D_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_QE/projecao_angular_momentum.py` & `vasprocar-1.1.18.49/vasprocar/src/_QE/projecao_angular_momentum.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/_info.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/_info.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/_info_b.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/_info_b.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/_label.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/_label.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,39 +44,22 @@
 
 #-------------
 inform.close()
 #-------------
 
 
 #======================================================================
-# Warning message for user to edit KPOINTS file =======================
+# Warning message for user to edit KPOINTS file (n_procar = 1) ========
 #======================================================================
 
 if (dest_k == 2 and n_procar == 1):
-
-   #-----------------------------------
-   n_kpoints = 0
-
-   try:
-       f = open(dir_files + '/KPOINTS')
-       f.close()
-       n_kpoints = 1
-   except:
-       print("")
-       print("... Missing KPOINTS file ...") 
-       print("")
-       print("--------------------------------------------------------------------------")
-       print("After inserting the KPOINTS file in the directory, press ENTER to continue")
-       print("--------------------------------------------------------------------------")
-       confirmacao = input (" "); confirmacao = str(confirmacao)       
-   #-----------------------------------   
-
-   #============================================================================
-   # Getting the number of k-points to be highlighted in the Bands structure ===
-   #============================================================================
+   #----------------------------
+   number = 0;     k_point = 0
+   dest_pk  = [];  label_pk = []
+   #----------------------------
 
    if (len(inputs) == 0):
       print("")
       print ("=============================================================================================")
       print ("Attention: Edit the KPOINTS file, inserting the desired label in the k-points of the file.   ")
       print ("               !!!! All k-points present in the KPOINTS file, must be labeled !!!!           ") 
       print ("=============================================================================================")
@@ -96,55 +79,156 @@
       print ("#18 = alfa        |  #19 = beta         |  #20 = pi        |  #21 = rho         |               ")
       print ("#22 = tau         |  #23 = upsilon      |  #24 = mu        |  #25 = nu          |               ")
       print ("#26 = epsilon     |  #27 = eta          |  #28 = kappa     |  #29 = xi          |  #30 = zeta   ")
       print ("#31 = left_arrow  |  #32 = right_arrow  |  #33 = up_arrow  |  #34 = down_arrow  |               ")
       print ("=============================================================================================")
       print ("After editing the KPOINTS file, press [ENTER] to continue                                    ")
       print ("=============================================================================================")
-      confirmacao = input (" "); confirmacao = str(confirmacao)       
+      confirmacao = input (" "); confirmacao = str(confirmacao) 
 
-   #------------------------------------------
-   kpoints = open(dir_files + '/KPOINTS', "r")
-   #------------------------------------------
 
-   VTemp = kpoints.readline()
-   VTemp = kpoints.readline()
+   #------------
+   n_kpoints = 0
+   #------------
+   try:
+       f = open(dir_files + '/KPOINTS')
+       f.close()
+       n_kpoints = 1
+   except:
+       print("")
+       print("... Missing KPOINTS file ...") 
+       print("")
+       print("--------------------------------------------------------------------------")
+       print("After inserting the KPOINTS file in the directory, press ENTER to continue")
+       print("--------------------------------------------------------------------------")
+       confirmacao = input (" "); confirmacao = str(confirmacao)       
 
-   points_path = int(VTemp)
 
-   number = 0
-   k_point = 0
+   #============================================================================
+   # Getting the number of k-points to be highlighted in the Bands structure ===
+   #============================================================================    
 
-   dest_pk  = []
-   label_pk = []
+   #------------------------------------------
+   kpoints = open(dir_files + '/KPOINTS', "r")
+   #------------------------------------------
+   VTemp = kpoints.readline()
+   VTemp = kpoints.readline();  points_path = int(VTemp)
 
    for i in range (100):
        VTemp = kpoints.readline().split()
        if (len(VTemp) >= 4):
-        
+          #----------
           number += 1 
           resto = (number % 2)
-     
-          if (resto == 1):
-             k_point = k_point + 1
-          if (resto == 0):
-             k_point = k_point + (points_path - 1)
-
+          #-------------------
+          if (resto == 1):  k_point = k_point + 1
+          if (resto == 0):  k_point = k_point + (points_path - 1)
+          #--------------------------------
           if (resto == 1 or k_point == nk):
              dest_pk.append(separacao[k_point])
              label_pk.append(str(VTemp[3]))
 
+   #------------------------
    contador2 = len(label_pk)
-
    #--------------
    kpoints.close()
    #--------------
 
 
 #======================================================================
+# Warning message for user to edit KPOINTS file (n_procar > 1) ========
+#======================================================================
+
+if (dest_k == 2 and n_procar > 1):
+   #------------------------------------------
+   k_point = 0;  dest_pk  = [];  label_pk = []
+   #------------------------------------------
+   for i in range (n_procar):
+
+
+       if (len(inputs) == 0 and i == 0):
+          print("")
+          print ("=============================================================================================")
+          print ("Attention: Edit the KPOINTS file, inserting the desired label in the k-points of the file.   ")
+          print ("               !!!! All k-points present in the KPOINTS file, must be labeled !!!!           ") 
+          print ("=============================================================================================")
+          print ("Example:                                                                                     ")
+          print ("         0.0 0.0 0.0 #1 (Gamma)                                                              ")
+          print ("         0.5 0.5 0.0 M                                                                       ")
+          print ("                                                                                             ")
+          print ("         0.5 0.5 0.0 M                                                                       ")
+          print ("         0.5 0.0 0.0 X                                                                       ")
+          print ("=============================================================================================")
+          print ("Use the following codes (#number) for using Greek symbols as labels:                         ") 
+          print ("                                                                                             ")
+          print ("#1  = Gamma       |  #2  = gamma        |  #3  = Delta     |  #4  = delta       |               ")
+          print ("#5  = Lambda      |  #6  = lambda       |  #7  = Sigma     |  #8  = sigma       |               ")
+          print ("#9  = Theta       |  #10 = tetha        |  #11 = Omega     |  #12 = omega       |               ")
+          print ("#13 = Psi         |  #14 = psi          |  #15 = Phi       |  #16 = phi         |  #17 = varphi ")
+          print ("#18 = alfa        |  #19 = beta         |  #20 = pi        |  #21 = rho         |               ")
+          print ("#22 = tau         |  #23 = upsilon      |  #24 = mu        |  #25 = nu          |               ")
+          print ("#26 = epsilon     |  #27 = eta          |  #28 = kappa     |  #29 = xi          |  #30 = zeta   ")
+          print ("#31 = left_arrow  |  #32 = right_arrow  |  #33 = up_arrow  |  #34 = down_arrow  |               ")
+          print ("=============================================================================================")
+          print ("After editing the KPOINTS file, press [ENTER] to continue                                    ")
+          print ("=============================================================================================")
+          confirmacao = input (" "); confirmacao = str(confirmacao) 
+
+
+       #------------
+       n_kpoints = 0
+       #------------
+       try:
+           f = open(dir_files + '/KPOINTS.' + str(i+1))
+           f.close()
+           n_kpoints = 1
+       except:
+           print("")
+           print(f'... Missing KPOINTS.{str(i+1)} file ...') 
+           print("")
+           print("----------------------------------------------------------------------------")
+           print(f'After inserting the KPOINTS.{str(i+1)} file in the directory, press ENTER to continue')
+           print("----------------------------------------------------------------------------")
+           confirmacao = input (" "); confirmacao = str(confirmacao)       
+
+
+       #============================================================================
+       # Getting the number of k-points to be highlighted in the Bands structure ===
+       #============================================================================
+
+       #------------------------------------------------------
+       kpoints = open(dir_files + '/KPOINTS.' + str(i+1), "r")
+       #------------------------------------------------------
+       VTemp = kpoints.readline()
+       VTemp = kpoints.readline();  points_path = int(VTemp)
+       for j in range (2): VTemp = kpoints.readline()
+       #---------------------------------------------
+       number = 0
+       for j in range(2):
+           VTemp = kpoints.readline().split()
+           if (len(VTemp) >= 4):
+              #----------
+              number += 1 
+              resto = (number % 2)
+              #-------------------
+              if (resto == 1):  k_point = k_point + 1
+              if (resto == 0):  k_point = k_point + (points_path - 1)
+              #--------------------------------
+              if (resto == 1 or k_point == nk):
+                 dest_pk.append(separacao[k_point])
+                 label_pk.append(str(VTemp[3]))     
+
+       #--------------
+       kpoints.close()
+   #------------------------
+   contador2 = len(label_pk)
+   #------------------------
+
+
+#======================================================================
 #======================================================================
 #======================================================================
 
 if (n_procar > 1 or (n_procar == 1 and dest_k < 2)):
 
    nk_total = nk*n_procar              # Total number of k-points for the band
    contador2 = 0
@@ -195,105 +279,14 @@
 
    #-------------
    inform.close()
    #-------------
 
 
 #======================================================================
-# Generating the label.txt file =======================================
-#======================================================================
-
-if (dest_k == 2):
-
-   #-------------------------------------------------
-   label = open(dir_files + '/output/label.txt', "w")
-   #-------------------------------------------------
-
-   if (n_procar > 1):
-      label.write(f'{contador2}                     ! Number of k-points to be labeled \n')
-
-# Criando uma lista com as letras de a-z ==============================
-
-   lab = []
-
-   for i in range(ord('a'), ord('z') + 1): # list the letters a-z
-       lab.append(chr(i))
-
-#======================================================================
-
-   if (n_procar > 1):
-      for i in range (contador2):
-          label.write(f'{dest_pk[i]:<18,.14f} {lab[i]}  ! k-point {n_pk[i]:<4}  ({k1_pk[i]}, {k2_pk[i]}, {k3_pk[i]}) \n')
-
-#======================================================================
-
-   if (n_procar > 1):
-      label.write(f' \n')
-      label.write(f'When editing this file, you can change the number of k-points to be labeled. \n')
-      label.write(f'The coordinate of each k-point can be found in the file output/informacoes.txt \n')
-      
-   label.write(f' \n')
-   label.write(f'===================================================================================================== \n')
-   label.write(f'To insert Greek symbols as a label for the que-points, use the codes (#number) below:                 \n')
-   label.write(f'===================================================================================================== \n')
-   label.write(f' \n')
-   label.write("#1  = Gamma       |  #2  = gamma        |  #3  = Delta     |  #4  = delta       |               \n") 
-   label.write("#5  = Lambda      |  #6  = lambda       |  #7  = Sigma     |  #8  = sigma       |               \n") 
-   label.write("#9  = Theta       |  #10 = tetha        |  #11 = Omega     |  #12 = omega       |               \n") 
-   label.write("#13 = Psi         |  #14 = psi          |  #15 = Phi       |  #16 = phi         |  #17 = varphi \n") 
-   label.write("#18 = alfa        |  #19 = beta         |  #20 = pi        |  #21 = rho         |               \n") 
-   label.write("#22 = tau         |  #23 = upsilon      |  #24 = mu        |  #25 = nu          |               \n") 
-   label.write("#26 = epsilon     |  #27 = eta          |  #28 = kappa     |  #29 = xi          |  #30 = zeta   \n")
-   label.write("#31 = left_arrow  |  #32 = right_arrow  |  #33 = up_arrow  |  #34 = down_arrow  |               \n") 
-   label.write(f' \n')
-
-   #------------
-   label.close()
-   #------------
-
-
-#======================================================================
-# Warning message for user to edit label.txt file =====================
-#======================================================================
-
-if (dest_k == 2 and n_procar > 1):
-   print (" ")
-   print ("##################################################################")
-   print ("Attention: Edit the label of the k-points in the label.txt file   ") 
-   print ("           After editing, confirm by pressing the [ENTER] button  ")
-   print ("==================================================================")
-   print ("Consult the coordinate of the k-points in the informacoes.txt file")
-   print ("##################################################################")
-   confirmacao = input (" "); confirmacao = str(confirmacao)
-
-   #======================================================================
-   # Reading the label.txt file to obtain k-point labels =================
-   #======================================================================
-
-   #-------------------------------------------------
-   label = open(dir_files + '/output/label.txt', "r")
-   #-------------------------------------------------
-
-   VTemp = label.readline().split()
-   contador2 = int(VTemp[0])
-
-   dest_pk = []
-   label_pk = []
-
-   for i in range(contador2):
-       VTemp = label.readline().split()
-       dest_pk.append(float(VTemp[0]))
-       label_pk.append(str(VTemp[1]))
-
-   #------------
-   label.close()
-   #------------
-
-
-#======================================================================
 # Defining the corresponding nomenclatures for GRACE and Matplotlib ===
 #======================================================================
 
 if (dest_k == 2):
 
    r_grace = []
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/_nscf.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/_nscf.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/_var_kpoints.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/_var_kpoints.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/chgcar.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/contcar_info.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/contcar_info.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/contribuicao.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/contribuicao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/dielectric_function.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/dos_pdos_ldos.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/kpoints_2D_3D.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/kpoints_2D_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/parchg.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/poscar_replace.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/poscar_replace.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/postar_combination.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/postar_combination.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/potencial.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_VASP/wave_function.py` & `vasprocar-1.1.18.49/vasprocar/src/_VASP/wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_dft.py` & `vasprocar-1.1.18.49/vasprocar/src/_dft.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_dft2kp.py` & `vasprocar-1.1.18.49/vasprocar/src/_dft2kp.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_loop.py` & `vasprocar-1.1.18.49/vasprocar/src/_loop.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_settings.py` & `vasprocar-1.1.18.49/vasprocar/src/_settings.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/_update.py` & `vasprocar-1.1.18.49/vasprocar/src/_update.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/bandas_2D.py` & `vasprocar-1.1.18.49/vasprocar/src/bandas_2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,22 +129,15 @@
       print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ")       
 
-   if (dest_k == 2):
-      print ("##############################################################")
-      print ("label.TXT file should be found inside the 'output' folder ====")
-      print ("after reading the PROCAR file ================================")
-      print ("##############################################################") 
-      print (" ")
-      #-----------
-      Dimensao = 1
+   if (dest_k == 2):  Dimensao = 1
 
    if (dest_k != 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/bandas_3D.py` & `vasprocar-1.1.18.49/vasprocar/src/bandas_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/bandas_4D.py` & `vasprocar-1.1.18.49/vasprocar/src/bandas_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/correction_file.py` & `vasprocar-1.1.18.49/vasprocar/src/correction_file.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/etc/DOI.png` & `vasprocar-1.1.18.49/vasprocar/src/etc/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/etc/Greek_alphabet.jpg` & `vasprocar-1.1.18.49/vasprocar/src/etc/Greek_alphabet.jpg`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/fermi_surface.py` & `vasprocar-1.1.18.49/vasprocar/src/fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/inputs/inputs.py` & `vasprocar-1.1.18.49/vasprocar/src/inputs/inputs.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/inputs/inputs_files.py` & `vasprocar-1.1.18.49/vasprocar/src/inputs/inputs_files.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/level_countour.py` & `vasprocar-1.1.18.49/vasprocar/src/level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/orbital_texture.py` & `vasprocar-1.1.18.49/vasprocar/src/orbital_texture.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/orbital_texture_vector.py` & `vasprocar-1.1.18.49/vasprocar/src/orbital_texture_vector.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_bandas_2D.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_bandas_2D.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 
 palavra = '"\\f{Symbol}2p/\\f{Times-Italic}a"'
 
 if (Dimensao == 1 and dest_k != 2): bandas.write(f'@    xaxis  label {palavra} \n') 
 if (Dimensao == 2 and dest_k != 2): bandas.write(f'@    xaxis  label "1/Angs." \n') 
 if (Dimensao == 3 and dest_k != 2): bandas.write(f'@    xaxis  label "1/nm" \n')
 
+print(contador2)
+print(label_pk)
+print(dest_pk)
+
 if (dest_k == 2):
    bandas.write(f'@    xaxis  tick spec type both \n')
    bandas.write(f'@    xaxis  tick spec {contador2} \n')
    for i in range (contador2):   
        bandas.write(f'@    xaxis  tick major {i}, {dest_pk[i]} \n')
        temp_r = label_pk[i]
        for j in range(34):
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_chgcar.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dielectric_function.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_parchg.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_potencial.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_localizacao.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_orbitais.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_psi.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_projecao_spin.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/Grace/plot_wave_function.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/Grace/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/_plot_settings.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/_plot_settings.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_2D.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_3D_matplotlib.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_3D_matplotlib.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_3D_plotly.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_3D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_bandas_4D_plotly.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_bandas_4D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_chgcar.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_dielectric_function.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_dos_pdos_ldos.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_fermi_surface.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_level_countour.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_orbital_texture.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_orbital_texture.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_orbital_texture_vector.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_orbital_texture_vector.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_parchg.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_potencial.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_localizacao.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_orbitais.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_psi.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_projecao_spin.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_2D.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_3D.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_4D.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_4D_[iso].py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_4D_[iso].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_contour.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_spin_texture_contour_video.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/plot/plot_wave_function.py` & `vasprocar-1.1.18.49/vasprocar/src/plot/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/projecao_localizacao.py` & `vasprocar-1.1.18.49/vasprocar/src/projecao_localizacao.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,22 +384,15 @@
       print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ") 
 
-   if (dest_k == 2):
-      print ("##############################################################")
-      print ("label.TXT file should be found inside the 'output' folder ====")
-      print ("after reading the PROCAR file ================================")
-      print ("##############################################################") 
-      print (" ")
-
-      Dimensao = 1
+   if (dest_k == 2):  Dimensao = 1
 
    if (dest_k != 2 and len(inputs) == 0):   
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/projecao_orbitais.py` & `vasprocar-1.1.18.49/vasprocar/src/projecao_orbitais.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,22 +355,15 @@
       print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ") 
 
-   if (dest_k == 2):
-      print ("##############################################################")
-      print ("label.TXT file should be found inside the 'output' folder ====")
-      print ("after reading the PROCAR file ================================")
-      print ("##############################################################") 
-      print (" ")
-      #-----------
-      Dimensao = 1
+   if (dest_k == 2):  Dimensao = 1
 
    if (dest_k != 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/projecao_psi.py` & `vasprocar-1.1.18.49/vasprocar/src/projecao_psi.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,22 +361,15 @@
       print ("Do you want to insert the symmetries as label of the k-points?")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ") 
 
-   if (dest_k == 2):
-      print ("##############################################################")
-      print ("label.TXT file should be found inside the 'output' folder ====")
-      print ("after reading the PROCAR file ================================")
-      print ("##############################################################") 
-      print (" ")
-
-      Dimensao = 1
+   if (dest_k == 2):  Dimensao = 1
 
    if (dest_k != 2):   
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/projecao_spin.py` & `vasprocar-1.1.18.49/vasprocar/src/projecao_spin.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,22 +351,15 @@
       print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ") 
 
-   if (dest_k == 2):
-      print ("##############################################################")
-      print ("label.TXT file should be found inside the 'output' folder ====")
-      print ("after reading the PROCAR file ================================")
-      print ("##############################################################") 
-      print (" ")
-      #-----------
-      Dimensao = 1
+   if (dest_k == 2):  Dimensao = 1
 
    if (dest_k != 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
```

### Comparing `vasprocar-1.1.18.48/vasprocar/src/spin_texture.py` & `vasprocar-1.1.18.49/vasprocar/src/spin_texture.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/spin_texture_contour.py` & `vasprocar-1.1.18.49/vasprocar/src/spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar/src/spin_texture_contour_video.py` & `vasprocar-1.1.18.49/vasprocar/src/spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.18.48/vasprocar.egg-info/PKG-INFO` & `vasprocar-1.1.18.49/vasprocar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.18.48
+Version: 1.1.18.49
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP/QE codes, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.18.48/vasprocar.egg-info/SOURCES.txt` & `vasprocar-1.1.18.49/vasprocar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

