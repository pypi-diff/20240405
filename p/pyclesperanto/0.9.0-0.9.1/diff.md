# Comparing `tmp/pyclesperanto-0.9.0.tar.gz` & `tmp/pyclesperanto-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclesperanto-0.9.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyclesperanto-0.9.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyclesperanto-0.9.0.tar` & `pyclesperanto-0.9.1.tar`

### file list

```diff
@@ -1,241 +1,243 @@
--rw-r--r--   0        0        0     2774 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/CMakeLists.txt
--rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/LICENSE
--rw-r--r--   0        0        0     8370 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/README.md
--rw-r--r--   0        0        0     1211 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/README.md
--rw-r--r--   0        0        0    51553 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/images/cell_segmentation.png
--rw-r--r--   0        0        0     9139 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/images/explore_API.png
--rw-r--r--   0        0        0    34316 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/images/find_local_maxima.png
--rw-r--r--   0        0        0    44227 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/images/image_filtering.png
--rw-r--r--   0        0        0     9629 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/images/labeled_blobs.png
--rw-r--r--   0        0        0     7142 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/images/multi-gpu.png
--rw-r--r--   0        0        0    28625 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/demos/images/tribolium3d_segmentation.png
--rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/__init__.py
--rw-r--r--   0        0        0     9588 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_array.py
--rw-r--r--   0        0        0     5445 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_core.py
--rw-r--r--   0        0        0     3498 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_decorators.py
--rw-r--r--   0        0        0     8039 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_functionalities.py
--rw-r--r--   0        0        0     2641 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_interroperability.py
--rw-r--r--   0        0        0     3554 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_memory.py
--rw-r--r--   0        0        0    20658 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_operators.py
--rw-r--r--   0        0        0   120667 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier1.py
--rw-r--r--   0        0        0    38105 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier2.py
--rw-r--r--   0        0        0    13371 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier3.py
--rw-r--r--   0        0        0     4622 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier4.py
--rw-r--r--   0        0        0     3051 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier5.py
--rw-r--r--   0        0        0     5178 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier6.py
--rw-r--r--   0        0        0    14272 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier7.py
--rw-r--r--   0        0        0     2050 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_tier8.py
--rw-r--r--   0        0        0     2465 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_utils.py
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyclesperanto/_version.py
--rw-r--r--   0        0        0     2653 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1228 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/scripts/build-opencl-linux.sh
--rw-r--r--   0        0        0     1256 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/scripts/build-opencl-windows.sh
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/clic/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/array_.cpp
--rw-r--r--   0        0        0     3244 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/core_.cpp
--rw-r--r--   0        0        0      334 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/pycle_wrapper.cpp
--rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/pycle_wrapper.hpp
--rw-r--r--   0        0        0    28185 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier1_.cpp
--rw-r--r--   0        0        0     9329 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier2_.cpp
--rw-r--r--   0        0        0     3277 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier3_.cpp
--rw-r--r--   0        0        0     1340 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier4_.cpp
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier5_.cpp
--rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier6_.cpp
--rw-r--r--   0        0        0     3027 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier7_.cpp
--rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/tier8_.cpp
--rw-r--r--   0        0        0      865 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/src/wrapper/types_.cpp
--rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_absolute.py
--rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_absolute_difference.py
--rw-r--r--   0        0        0      588 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_add_image_and_scalar.py
--rwxr-xr-x   0        0        0     1253 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_add_images.py
--rw-r--r--   0        0        0     1836 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_add_images_weighted.py
--rw-r--r--   0        0        0      674 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_affine_transform.py
--rw-r--r--   0        0        0      385 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_array_equal.py
--rw-r--r--   0        0        0      654 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_array_operators.py
--rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_available_device_names.py
--rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_binary_and.py
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_binary_edge_detection.py
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_binary_not.py
--rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_binary_or.py
--rw-r--r--   0        0        0      403 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_binary_subtract.py
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_binary_xor.py
--rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_block_enumerate.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_bottom_hat_box.py
--rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_bottom_hat_sphere.py
--rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_bounding_box.py
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_cl_info.py
--rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_clip.py
--rw-r--r--   0        0        0     2445 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_closing_box.py
--rw-r--r--   0        0        0     2431 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_closing_labels.py
--rw-r--r--   0        0        0     2457 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_closing_sphere.py
--rw-r--r--   0        0        0     1353 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_connected_components_labeling_box.py
--rw-r--r--   0        0        0      500 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_connected_components_labeling_diamond.py
--rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_convolve.py
--rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_copy.py
--rw-r--r--   0        0        0     1343 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_count_touching_neighbors.py
--rw-r--r--   0        0        0     2956 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_create.py
--rw-r--r--   0        0        0     1106 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_crop.py
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_crop_border.py
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_cubic_root.py
--rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_dask_compatibility.py
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_degrees_to_radians.py
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_detect_label_edges.py
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_detect_maxima_box.py
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_detect_minima_box.py
--rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_difference_of_gaussian.py
--rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_dilate_box.py
--rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_dilate_sphere.py
--rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_divide_images.py
--rw-r--r--   0        0        0      520 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_divide_scalar_by_image.py
--rw-r--r--   0        0        0      705 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_ellipsis.py
--rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_equal.py
--rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_equal_constant.py
--rw-r--r--   0        0        0      770 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_erode_box.py
--rw-r--r--   0        0        0     4925 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_erode_labels.py
--rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_erode_sphere.py
--rw-r--r--   0        0        0      853 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_eroded_otsu_labeling.py
--rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_exclude_labels.py
--rw-r--r--   0        0        0     5281 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_exclude_labels_on_edges.py
--rw-r--r--   0        0        0      867 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_exponential.py
--rw-r--r--   0        0        0     1034 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_extend_labeling_via_voronoi.py
--rw-r--r--   0        0        0     1878 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_extended_getitem.py
--rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_extended_setitem.py
--rw-r--r--   0        0        0      449 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_flag_existing_labels.py
--rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_flip.py
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_gamma_correction.py
--rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_gauss_otsu_labeling.py
--rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_gaussian_blur.py
--rw-r--r--   0        0        0     1912 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_generate_binary_overlap_matrix.py
--rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_generate_distance_matrix.py
--rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_gpu_switch.py
--rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_gradient_x.py
--rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_gradient_y.py
--rw-r--r--   0        0        0     1776 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_gradient_z.py
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_greater.py
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_greater_constant.py
--rw-r--r--   0        0        0     1796 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_greater_or_equal.py
--rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_greater_or_equal_constant.py
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_hessian_eigenvalues.py
--rw-r--r--   0        0        0     1425 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_histogram.py
--rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_image.py
--rwxr-xr-x   0        0        0       51 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_import.py
--rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_indexing.py
--rw-r--r--   0        0        0      577 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_invert.py
--rw-r--r--   0        0        0     1177 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_iterator.py
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_jaccard_index.py
--rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_label_bounding_box.py
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_labelled_spots_to_pointlist.py
--rw-r--r--   0        0        0      781 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_laplace_box.py
--rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_laplace_diamond.py
--rw-r--r--   0        0        0      938 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_large_hessian_eigenvalue.py
--rw-r--r--   0        0        0      677 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_local_cross_correlation.py
--rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_logarithm.py
--rw-r--r--   0        0        0     1016 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mask.py
--rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mask_label.py
--rw-r--r--   0        0        0     1222 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_masked_voronoi_labeling.py
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_box.py
--rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_image_and_scalar.py
--rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_images.py
--rw-r--r--   0        0        0      746 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_of_all_pixels.py
--rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_sphere.py
--rw-r--r--   0        0        0     2117 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_x_projection.py
--rw-r--r--   0        0        0     2755 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_y_projection.py
--rw-r--r--   0        0        0     1944 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_maximum_z_projection.py
--rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mean_box.py
--rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mean_of_all_pixels.py
--rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mean_sphere.py
--rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mean_squared_error.py
--rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mean_x_projection.py
--rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mean_y_projection.py
--rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mean_z_projection.py
--rw-r--r--   0        0        0      798 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_median_box.py
--rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_median_sphere.py
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_box.py
--rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_image_and_scalar.py
--rw-r--r--   0        0        0     2017 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_images.py
--rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_of_all_pixels.py
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_of_masked_pixels.py
--rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_x_projection.py
--rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_y_projection.py
--rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_minimum_z_projection.py
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mode_box.py
--rw-r--r--   0        0        0     1395 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_mode_sphere.py
--rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_modulo_images.py
--rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_multiply_image_and_scalar.py
--rw-r--r--   0        0        0     1041 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_multiply_images.py
--rw-r--r--   0        0        0     1345 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_multiply_matrix.py
--rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_nan_to_num.py
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_nonzero_maximum_box.py
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_nonzero_maximum_diamond.py
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_nonzero_minimum_box.py
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_nonzero_minimum_diamond.py
--rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_not_equal.py
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_not_equal_constant.py
--rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_np_asarray.py
--rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_onlyzero_overwrite_maximum_box.py
--rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_onlyzero_overwrite_maximum_diamond.py
--rw-r--r--   0        0        0     2449 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_opening_box.py
--rw-r--r--   0        0        0     7044 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_opening_labels.py
--rw-r--r--   0        0        0     2461 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_opening_sphere.py
--rw-r--r--   0        0        0    14951 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_operators.py
--rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_paste.py
--rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_power.py
--rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_power_images.py
--rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_push.py
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_radians_to_degrees.py
--rw-r--r--   0        0        0     9500 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_range.py
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_reciprocal.py
--rw-r--r--   0        0        0      755 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_reduce_labels_to_label_edges.py
--rw-r--r--   0        0        0     3803 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_reduction.py
--rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_relabel_sequential.py
--rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_replace_intensities.py
--rw-r--r--   0        0        0      795 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_replace_intensity.py
--rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set.py
--rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_column.py
--rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_image_borders.py
--rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_nonzero_pixels_to_pixelindex.py
--rw-r--r--   0        0        0     1313 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_plane.py
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_ramp_x.py
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_ramp_y.py
--rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_ramp_z.py
--rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_row.py
--rw-r--r--   0        0        0      134 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_wait_for_kernel_finish.py
--rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_where_x_equals_y.py
--rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_where_x_greater_than_y.py
--rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_set_where_x_smaller_than_y.py
--rw-r--r--   0        0        0     1903 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_setitem.py
--rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_sign.py
--rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_small_hessian_eigenvalue.py
--rw-r--r--   0        0        0     1679 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_smaller.py
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_smaller_constant.py
--rw-r--r--   0        0        0     1690 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_smaller_or_equal.py
--rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_smaller_or_equal_constant.py
--rw-r--r--   0        0        0      973 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_smooth_labels.py
--rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_sobel.py
--rw-r--r--   0        0        0     1158 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_spots_to_pointlist.py
--rw-r--r--   0        0        0      351 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_square.py
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_square_root.py
--rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_squared_difference.py
--rw-r--r--   0        0        0      856 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_standard_deviation_box.py
--rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_standard_deviation_sphere.py
--rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_subtract_gaussian_background.py
--rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_subtract_image_from_scalar.py
--rw-r--r--   0        0        0      366 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_subtract_images.py
--rw-r--r--   0        0        0     1276 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_sum_of_all_pixels.py
--rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_sum_reduction.py
--rw-r--r--   0        0        0     1820 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_sum_x_projection.py
--rw-r--r--   0        0        0     1755 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_sum_y_projection.py
--rw-r--r--   0        0        0     2470 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_sum_z_projection.py
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_t.py
--rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_threshold_otsu.py
--rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_top_hat_box.py
--rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_top_hat_sphere.py
--rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_transpose_xy.py
--rw-r--r--   0        0        0     1188 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_transpose_xz.py
--rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_transpose_yz.py
--rw-r--r--   0        0        0     1173 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_undefined_to_zero.py
--rw-r--r--   0        0        0      845 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_variance_box.py
--rw-r--r--   0        0        0      821 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_variance_sphere.py
--rw-r--r--   0        0        0     1012 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_voronoi_labeling.py
--rw-r--r--   0        0        0     1005 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/tests/test_voronoi_otsu_labeling.py
--rw-r--r--   0        0        0     9618 2022-11-09 12:37:21.000000 pyclesperanto-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2774 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/LICENSE
+-rw-r--r--   0        0        0     8370 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/README.md
+-rw-r--r--   0        0        0     1211 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/README.md
+-rw-r--r--   0        0        0    51553 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/images/cell_segmentation.png
+-rw-r--r--   0        0        0     9139 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/images/explore_API.png
+-rw-r--r--   0        0        0    34316 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/images/find_local_maxima.png
+-rw-r--r--   0        0        0    44227 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/images/image_filtering.png
+-rw-r--r--   0        0        0     9629 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/images/labeled_blobs.png
+-rw-r--r--   0        0        0     7142 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/images/multi-gpu.png
+-rw-r--r--   0        0        0    28625 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/demos/images/tribolium3d_segmentation.png
+-rw-r--r--   0        0        0      777 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/__init__.py
+-rw-r--r--   0        0        0     9588 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_array.py
+-rw-r--r--   0        0        0     8087 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_core.py
+-rw-r--r--   0        0        0     3498 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_decorators.py
+-rw-r--r--   0        0        0     8039 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_functionalities.py
+-rw-r--r--   0        0        0     2641 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_interroperability.py
+-rw-r--r--   0        0        0     3554 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_memory.py
+-rw-r--r--   0        0        0    20658 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_operators.py
+-rw-r--r--   0        0        0   120667 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier1.py
+-rw-r--r--   0        0        0    38105 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier2.py
+-rw-r--r--   0        0        0    13371 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier3.py
+-rw-r--r--   0        0        0     4622 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier4.py
+-rw-r--r--   0        0        0     3051 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier5.py
+-rw-r--r--   0        0        0     5178 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier6.py
+-rw-r--r--   0        0        0    14272 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier7.py
+-rw-r--r--   0        0        0     2050 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_tier8.py
+-rw-r--r--   0        0        0     2465 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_utils.py
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyclesperanto/_version.py
+-rw-r--r--   0        0        0     2653 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1228 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/scripts/build-opencl-linux.sh
+-rw-r--r--   0        0        0     1256 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/scripts/build-opencl-windows.sh
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/clic/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/array_.cpp
+-rw-r--r--   0        0        0     3244 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/core_.cpp
+-rw-r--r--   0        0        0     2991 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/execute_.cpp
+-rw-r--r--   0        0        0      349 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/pycle_wrapper.cpp
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/pycle_wrapper.hpp
+-rw-r--r--   0        0        0    28185 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier1_.cpp
+-rw-r--r--   0        0        0     9329 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier2_.cpp
+-rw-r--r--   0        0        0     3277 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier3_.cpp
+-rw-r--r--   0        0        0     1340 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier4_.cpp
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier5_.cpp
+-rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier6_.cpp
+-rw-r--r--   0        0        0     3027 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier7_.cpp
+-rw-r--r--   0        0        0      737 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/tier8_.cpp
+-rw-r--r--   0        0        0      865 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/src/wrapper/types_.cpp
+-rw-r--r--   0        0        0      507 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_absolute.py
+-rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_absolute_difference.py
+-rw-r--r--   0        0        0      588 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_add_image_and_scalar.py
+-rwxr-xr-x   0        0        0     1253 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_add_images.py
+-rw-r--r--   0        0        0     1836 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_add_images_weighted.py
+-rw-r--r--   0        0        0      674 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_affine_transform.py
+-rw-r--r--   0        0        0      385 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_array_equal.py
+-rw-r--r--   0        0        0      654 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_array_operators.py
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_available_device_names.py
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_binary_and.py
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_binary_edge_detection.py
+-rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_binary_not.py
+-rw-r--r--   0        0        0      391 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_binary_or.py
+-rw-r--r--   0        0        0      403 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_binary_subtract.py
+-rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_binary_xor.py
+-rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_block_enumerate.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_bottom_hat_box.py
+-rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_bottom_hat_sphere.py
+-rw-r--r--   0        0        0      888 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_bounding_box.py
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_cl_info.py
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_clip.py
+-rw-r--r--   0        0        0     2445 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_closing_box.py
+-rw-r--r--   0        0        0     2431 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_closing_labels.py
+-rw-r--r--   0        0        0     2457 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_closing_sphere.py
+-rw-r--r--   0        0        0     1353 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_connected_components_labeling_box.py
+-rw-r--r--   0        0        0      500 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_connected_components_labeling_diamond.py
+-rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_convolve.py
+-rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_copy.py
+-rw-r--r--   0        0        0     1343 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_count_touching_neighbors.py
+-rw-r--r--   0        0        0     2956 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_create.py
+-rw-r--r--   0        0        0     1106 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_crop.py
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_crop_border.py
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_cubic_root.py
+-rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_dask_compatibility.py
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_degrees_to_radians.py
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_detect_label_edges.py
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_detect_maxima_box.py
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_detect_minima_box.py
+-rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_difference_of_gaussian.py
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_dilate_box.py
+-rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_dilate_sphere.py
+-rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_divide_images.py
+-rw-r--r--   0        0        0      520 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_divide_scalar_by_image.py
+-rw-r--r--   0        0        0      705 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_ellipsis.py
+-rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_equal.py
+-rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_equal_constant.py
+-rw-r--r--   0        0        0      770 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_erode_box.py
+-rw-r--r--   0        0        0     4925 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_erode_labels.py
+-rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_erode_sphere.py
+-rw-r--r--   0        0        0      853 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_eroded_otsu_labeling.py
+-rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_exclude_labels.py
+-rw-r--r--   0        0        0     5281 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_exclude_labels_on_edges.py
+-rw-r--r--   0        0        0      998 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_execute.py
+-rw-r--r--   0        0        0      867 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_exponential.py
+-rw-r--r--   0        0        0     1034 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_extend_labeling_via_voronoi.py
+-rw-r--r--   0        0        0     1878 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_extended_getitem.py
+-rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_extended_setitem.py
+-rw-r--r--   0        0        0      449 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_flag_existing_labels.py
+-rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_flip.py
+-rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_gamma_correction.py
+-rw-r--r--   0        0        0      829 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_gauss_otsu_labeling.py
+-rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_gaussian_blur.py
+-rw-r--r--   0        0        0     1912 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_generate_binary_overlap_matrix.py
+-rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_generate_distance_matrix.py
+-rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_gpu_switch.py
+-rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_gradient_x.py
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_gradient_y.py
+-rw-r--r--   0        0        0     1776 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_gradient_z.py
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_greater.py
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_greater_constant.py
+-rw-r--r--   0        0        0     1796 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_greater_or_equal.py
+-rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_greater_or_equal_constant.py
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_hessian_eigenvalues.py
+-rw-r--r--   0        0        0     1425 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_histogram.py
+-rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_image.py
+-rwxr-xr-x   0        0        0       51 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_import.py
+-rw-r--r--   0        0        0      263 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_indexing.py
+-rw-r--r--   0        0        0      577 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_invert.py
+-rw-r--r--   0        0        0     1177 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_iterator.py
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_jaccard_index.py
+-rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_label_bounding_box.py
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_labelled_spots_to_pointlist.py
+-rw-r--r--   0        0        0      781 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_laplace_box.py
+-rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_laplace_diamond.py
+-rw-r--r--   0        0        0      938 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_large_hessian_eigenvalue.py
+-rw-r--r--   0        0        0      677 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_local_cross_correlation.py
+-rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_logarithm.py
+-rw-r--r--   0        0        0     1016 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mask.py
+-rw-r--r--   0        0        0     1031 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mask_label.py
+-rw-r--r--   0        0        0     1222 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_masked_voronoi_labeling.py
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_box.py
+-rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_image_and_scalar.py
+-rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_images.py
+-rw-r--r--   0        0        0      746 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_of_all_pixels.py
+-rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_sphere.py
+-rw-r--r--   0        0        0     2117 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_x_projection.py
+-rw-r--r--   0        0        0     2755 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_y_projection.py
+-rw-r--r--   0        0        0     1944 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_maximum_z_projection.py
+-rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mean_box.py
+-rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mean_of_all_pixels.py
+-rw-r--r--   0        0        0      823 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mean_sphere.py
+-rw-r--r--   0        0        0      265 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mean_squared_error.py
+-rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mean_x_projection.py
+-rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mean_y_projection.py
+-rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mean_z_projection.py
+-rw-r--r--   0        0        0      798 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_median_box.py
+-rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_median_sphere.py
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_box.py
+-rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_image_and_scalar.py
+-rw-r--r--   0        0        0     2017 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_images.py
+-rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_of_all_pixels.py
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_of_masked_pixels.py
+-rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_x_projection.py
+-rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_y_projection.py
+-rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_minimum_z_projection.py
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mode_box.py
+-rw-r--r--   0        0        0     1395 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_mode_sphere.py
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_modulo_images.py
+-rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_multiply_image_and_scalar.py
+-rw-r--r--   0        0        0     1041 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_multiply_images.py
+-rw-r--r--   0        0        0     1345 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_multiply_matrix.py
+-rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_nan_to_num.py
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_nonzero_maximum_box.py
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_nonzero_maximum_diamond.py
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_nonzero_minimum_box.py
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_nonzero_minimum_diamond.py
+-rw-r--r--   0        0        0     1026 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_not_equal.py
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_not_equal_constant.py
+-rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_np_asarray.py
+-rw-r--r--   0        0        0      854 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_onlyzero_overwrite_maximum_box.py
+-rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_onlyzero_overwrite_maximum_diamond.py
+-rw-r--r--   0        0        0     2449 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_opening_box.py
+-rw-r--r--   0        0        0     7044 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_opening_labels.py
+-rw-r--r--   0        0        0     2461 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_opening_sphere.py
+-rw-r--r--   0        0        0    14951 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_operators.py
+-rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_paste.py
+-rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_power.py
+-rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_power_images.py
+-rw-r--r--   0        0        0      575 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_push.py
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_radians_to_degrees.py
+-rw-r--r--   0        0        0     9500 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_range.py
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_reciprocal.py
+-rw-r--r--   0        0        0      755 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_reduce_labels_to_label_edges.py
+-rw-r--r--   0        0        0     3803 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_reduction.py
+-rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_relabel_sequential.py
+-rw-r--r--   0        0        0      855 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_replace_intensities.py
+-rw-r--r--   0        0        0      795 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_replace_intensity.py
+-rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set.py
+-rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_column.py
+-rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_image_borders.py
+-rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_nonzero_pixels_to_pixelindex.py
+-rw-r--r--   0        0        0     1313 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_plane.py
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_ramp_x.py
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_ramp_y.py
+-rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_ramp_z.py
+-rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_row.py
+-rw-r--r--   0        0        0      134 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_wait_for_kernel_finish.py
+-rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_where_x_equals_y.py
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_where_x_greater_than_y.py
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_set_where_x_smaller_than_y.py
+-rw-r--r--   0        0        0     1903 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_setitem.py
+-rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_sign.py
+-rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_small_hessian_eigenvalue.py
+-rw-r--r--   0        0        0     1679 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_smaller.py
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_smaller_constant.py
+-rw-r--r--   0        0        0     1690 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_smaller_or_equal.py
+-rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_smaller_or_equal_constant.py
+-rw-r--r--   0        0        0      973 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_smooth_labels.py
+-rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_sobel.py
+-rw-r--r--   0        0        0     1158 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_spots_to_pointlist.py
+-rw-r--r--   0        0        0      351 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_square.py
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_square_root.py
+-rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_squared_difference.py
+-rw-r--r--   0        0        0      856 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_standard_deviation_box.py
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_standard_deviation_sphere.py
+-rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_subtract_gaussian_background.py
+-rw-r--r--   0        0        0      422 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_subtract_image_from_scalar.py
+-rw-r--r--   0        0        0      366 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_subtract_images.py
+-rw-r--r--   0        0        0     1276 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_sum_of_all_pixels.py
+-rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_sum_reduction.py
+-rw-r--r--   0        0        0     1820 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_sum_x_projection.py
+-rw-r--r--   0        0        0     1755 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_sum_y_projection.py
+-rw-r--r--   0        0        0     2470 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_sum_z_projection.py
+-rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_t.py
+-rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_threshold_otsu.py
+-rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_top_hat_box.py
+-rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_top_hat_sphere.py
+-rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_transpose_xy.py
+-rw-r--r--   0        0        0     1188 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_transpose_xz.py
+-rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_transpose_yz.py
+-rw-r--r--   0        0        0     1173 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_undefined_to_zero.py
+-rw-r--r--   0        0        0      845 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_variance_box.py
+-rw-r--r--   0        0        0      821 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_variance_sphere.py
+-rw-r--r--   0        0        0     1012 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_voronoi_labeling.py
+-rw-r--r--   0        0        0     1005 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/tests/test_voronoi_otsu_labeling.py
+-rw-r--r--   0        0        0     9618 2022-11-09 12:37:21.000000 pyclesperanto-0.9.1/PKG-INFO
```

### Comparing `pyclesperanto-0.9.0/CMakeLists.txt` & `pyclesperanto-0.9.1/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 set(CMAKE_SKIP_INSTALL_ALL_DEPENDENCY TRUE)
 option(BUILD_TESTING  OFF)
 option(BUILD_BENCHMARK  OFF)
 option(BUILD_SHARED_LIBS OFF)
 
 
 ## CLIc dependency
-set(CLIC_REPO_TAG 0.9.0) # branch name for dev
+set(CLIC_REPO_TAG 0.9.1) # branch name for dev
 set(CLIC_REPO_URL https://github.com/clEsperanto/CLIc.git)
 add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/src/clic EXCLUDE_FROM_ALL)
 
 
 ## look for python
 set(Python_FIND_VIRTUALENV "FIRST")
 find_package(Python COMPONENTS Interpreter Development.Module REQUIRED)
```

### Comparing `pyclesperanto-0.9.0/LICENSE` & `pyclesperanto-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/README.md` & `pyclesperanto-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/README.md` & `pyclesperanto-0.9.1/demos/README.md`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/images/cell_segmentation.png` & `pyclesperanto-0.9.1/demos/images/cell_segmentation.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/images/explore_API.png` & `pyclesperanto-0.9.1/demos/images/explore_API.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/images/find_local_maxima.png` & `pyclesperanto-0.9.1/demos/images/find_local_maxima.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/images/image_filtering.png` & `pyclesperanto-0.9.1/demos/images/image_filtering.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/images/labeled_blobs.png` & `pyclesperanto-0.9.1/demos/images/labeled_blobs.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/images/multi-gpu.png` & `pyclesperanto-0.9.1/demos/images/multi-gpu.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/demos/images/tribolium3d_segmentation.png` & `pyclesperanto-0.9.1/demos/images/tribolium3d_segmentation.png`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/__init__.py` & `pyclesperanto-0.9.1/pyclesperanto/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ._core import (
     gpu_info,
+    execute,
     select_backend,
     select_device,
     get_device,
     wait_for_kernel_to_finish,
     list_available_devices,
     list_available_backends,
     default_initialisation,
```

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_array.py` & `pyclesperanto-0.9.1/pyclesperanto/_array.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_decorators.py` & `pyclesperanto-0.9.1/pyclesperanto/_decorators.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_functionalities.py` & `pyclesperanto-0.9.1/pyclesperanto/_functionalities.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_interroperability.py` & `pyclesperanto-0.9.1/pyclesperanto/_interroperability.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_memory.py` & `pyclesperanto-0.9.1/pyclesperanto/_memory.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_operators.py` & `pyclesperanto-0.9.1/pyclesperanto/_operators.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier1.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier1.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier2.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier2.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier3.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier3.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier4.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier4.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier5.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier5.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier6.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier6.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier7.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier7.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_tier8.py` & `pyclesperanto-0.9.1/pyclesperanto/_tier8.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyclesperanto/_utils.py` & `pyclesperanto-0.9.1/pyclesperanto/_utils.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/pyproject.toml` & `pyclesperanto-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   "toolz; python_version >='3.7'",
   "matplotlib; python_version >='3.7'",
 ]
 description = "GPU-accelerated image processing in python using OpenCL"
 name = "pyclesperanto"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.9.0"
+version = "0.9.1"
 
 [project.urls]
 Documentation = "https://clesperanto.github.io/pyclesperanto/"
 Examples = "https://clesperanto.github.io/pyclesperanto/demos/"
 Issues = "https://github.com/clEsperanto/pyclesperanto/issues"
 Source = "https://github.com/clEsperanto/pyclesperanto/"
```

### Comparing `pyclesperanto-0.9.0/scripts/build-opencl-linux.sh` & `pyclesperanto-0.9.1/scripts/build-opencl-linux.sh`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/scripts/build-opencl-windows.sh` & `pyclesperanto-0.9.1/scripts/build-opencl-windows.sh`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/array_.cpp` & `pyclesperanto-0.9.1/src/wrapper/array_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/core_.cpp` & `pyclesperanto-0.9.1/src/wrapper/core_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/pycle_wrapper.hpp` & `pyclesperanto-0.9.1/src/wrapper/pycle_wrapper.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
 auto types_(pybind11::module_ &module) -> void;
 auto core_(pybind11::module_ &module) -> void;
 auto array_(pybind11::module_ &module) -> void;
+auto execute_(pybind11::module_ &module) -> void;
 
 auto tier1_(pybind11::module_ &module) -> void;
 auto tier2_(pybind11::module_ &module) -> void;
 auto tier3_(pybind11::module_ &module) -> void;
 auto tier4_(pybind11::module_ &module) -> void;
 auto tier5_(pybind11::module_ &module) -> void;
 auto tier6_(pybind11::module_ &module) -> void;
```

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier1_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier1_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier2_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier2_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier3_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier3_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier4_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier4_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier5_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier5_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier6_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier6_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier7_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier7_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/tier8_.cpp` & `pyclesperanto-0.9.1/src/wrapper/tier8_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/src/wrapper/types_.cpp` & `pyclesperanto-0.9.1/src/wrapper/types_.cpp`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_add_image_and_scalar.py` & `pyclesperanto-0.9.1/tests/test_add_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_add_images.py` & `pyclesperanto-0.9.1/tests/test_add_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_add_images_weighted.py` & `pyclesperanto-0.9.1/tests/test_add_images_weighted.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_affine_transform.py` & `pyclesperanto-0.9.1/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_array_operators.py` & `pyclesperanto-0.9.1/tests/test_array_operators.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_binary_and.py` & `pyclesperanto-0.9.1/tests/test_binary_and.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_binary_edge_detection.py` & `pyclesperanto-0.9.1/tests/test_binary_edge_detection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_block_enumerate.py` & `pyclesperanto-0.9.1/tests/test_block_enumerate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_bottom_hat_box.py` & `pyclesperanto-0.9.1/tests/test_bottom_hat_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_bottom_hat_sphere.py` & `pyclesperanto-0.9.1/tests/test_bottom_hat_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_bounding_box.py` & `pyclesperanto-0.9.1/tests/test_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_clip.py` & `pyclesperanto-0.9.1/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_closing_box.py` & `pyclesperanto-0.9.1/tests/test_closing_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_closing_labels.py` & `pyclesperanto-0.9.1/tests/test_closing_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_closing_sphere.py` & `pyclesperanto-0.9.1/tests/test_closing_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_connected_components_labeling_box.py` & `pyclesperanto-0.9.1/tests/test_connected_components_labeling_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_convolve.py` & `pyclesperanto-0.9.1/tests/test_convolve.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_count_touching_neighbors.py` & `pyclesperanto-0.9.1/tests/test_count_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_create.py` & `pyclesperanto-0.9.1/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_crop.py` & `pyclesperanto-0.9.1/tests/test_crop.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_crop_border.py` & `pyclesperanto-0.9.1/tests/test_crop_border.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_detect_label_edges.py` & `pyclesperanto-0.9.1/tests/test_detect_label_edges.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_detect_maxima_box.py` & `pyclesperanto-0.9.1/tests/test_detect_maxima_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_detect_minima_box.py` & `pyclesperanto-0.9.1/tests/test_detect_minima_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_difference_of_gaussian.py` & `pyclesperanto-0.9.1/tests/test_difference_of_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_dilate_box.py` & `pyclesperanto-0.9.1/tests/test_dilate_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_dilate_sphere.py` & `pyclesperanto-0.9.1/tests/test_dilate_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_divide_images.py` & `pyclesperanto-0.9.1/tests/test_divide_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_divide_scalar_by_image.py` & `pyclesperanto-0.9.1/tests/test_divide_scalar_by_image.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_ellipsis.py` & `pyclesperanto-0.9.1/tests/test_ellipsis.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_equal.py` & `pyclesperanto-0.9.1/tests/test_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_equal_constant.py` & `pyclesperanto-0.9.1/tests/test_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_erode_box.py` & `pyclesperanto-0.9.1/tests/test_erode_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_erode_labels.py` & `pyclesperanto-0.9.1/tests/test_erode_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_erode_sphere.py` & `pyclesperanto-0.9.1/tests/test_erode_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_eroded_otsu_labeling.py` & `pyclesperanto-0.9.1/tests/test_eroded_otsu_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_exclude_labels.py` & `pyclesperanto-0.9.1/tests/test_exclude_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_exclude_labels_on_edges.py` & `pyclesperanto-0.9.1/tests/test_exclude_labels_on_edges.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_exponential.py` & `pyclesperanto-0.9.1/tests/test_exponential.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_extend_labeling_via_voronoi.py` & `pyclesperanto-0.9.1/tests/test_extend_labeling_via_voronoi.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_extended_getitem.py` & `pyclesperanto-0.9.1/tests/test_extended_getitem.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_extended_setitem.py` & `pyclesperanto-0.9.1/tests/test_extended_setitem.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_flip.py` & `pyclesperanto-0.9.1/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_gamma_correction.py` & `pyclesperanto-0.9.1/tests/test_gamma_correction.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_gauss_otsu_labeling.py` & `pyclesperanto-0.9.1/tests/test_gauss_otsu_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_gaussian_blur.py` & `pyclesperanto-0.9.1/tests/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_generate_binary_overlap_matrix.py` & `pyclesperanto-0.9.1/tests/test_generate_binary_overlap_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_generate_distance_matrix.py` & `pyclesperanto-0.9.1/tests/test_generate_distance_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_gpu_switch.py` & `pyclesperanto-0.9.1/tests/test_gpu_switch.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_gradient_x.py` & `pyclesperanto-0.9.1/tests/test_gradient_x.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_gradient_y.py` & `pyclesperanto-0.9.1/tests/test_gradient_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_gradient_z.py` & `pyclesperanto-0.9.1/tests/test_gradient_z.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_greater.py` & `pyclesperanto-0.9.1/tests/test_greater.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_greater_constant.py` & `pyclesperanto-0.9.1/tests/test_greater_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_greater_or_equal.py` & `pyclesperanto-0.9.1/tests/test_greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_greater_or_equal_constant.py` & `pyclesperanto-0.9.1/tests/test_greater_or_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_hessian_eigenvalues.py` & `pyclesperanto-0.9.1/tests/test_hessian_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_histogram.py` & `pyclesperanto-0.9.1/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_image.py` & `pyclesperanto-0.9.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_invert.py` & `pyclesperanto-0.9.1/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_iterator.py` & `pyclesperanto-0.9.1/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_jaccard_index.py` & `pyclesperanto-0.9.1/tests/test_jaccard_index.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_labelled_spots_to_pointlist.py` & `pyclesperanto-0.9.1/tests/test_labelled_spots_to_pointlist.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_laplace_box.py` & `pyclesperanto-0.9.1/tests/test_laplace_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_laplace_diamond.py` & `pyclesperanto-0.9.1/tests/test_laplace_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_large_hessian_eigenvalue.py` & `pyclesperanto-0.9.1/tests/test_large_hessian_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_local_cross_correlation.py` & `pyclesperanto-0.9.1/tests/test_local_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mask.py` & `pyclesperanto-0.9.1/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mask_label.py` & `pyclesperanto-0.9.1/tests/test_mask_label.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_masked_voronoi_labeling.py` & `pyclesperanto-0.9.1/tests/test_masked_voronoi_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_maximum_box.py` & `pyclesperanto-0.9.1/tests/test_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_maximum_images.py` & `pyclesperanto-0.9.1/tests/test_maximum_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_maximum_of_all_pixels.py` & `pyclesperanto-0.9.1/tests/test_maximum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_maximum_sphere.py` & `pyclesperanto-0.9.1/tests/test_maximum_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_maximum_x_projection.py` & `pyclesperanto-0.9.1/tests/test_maximum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_maximum_y_projection.py` & `pyclesperanto-0.9.1/tests/test_maximum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_maximum_z_projection.py` & `pyclesperanto-0.9.1/tests/test_maximum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mean_box.py` & `pyclesperanto-0.9.1/tests/test_mean_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mean_of_all_pixels.py` & `pyclesperanto-0.9.1/tests/test_mean_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mean_sphere.py` & `pyclesperanto-0.9.1/tests/test_mean_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mean_x_projection.py` & `pyclesperanto-0.9.1/tests/test_mean_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mean_y_projection.py` & `pyclesperanto-0.9.1/tests/test_mean_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mean_z_projection.py` & `pyclesperanto-0.9.1/tests/test_mean_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_median_box.py` & `pyclesperanto-0.9.1/tests/test_median_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_median_sphere.py` & `pyclesperanto-0.9.1/tests/test_median_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_minimum_box.py` & `pyclesperanto-0.9.1/tests/test_minimum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_minimum_images.py` & `pyclesperanto-0.9.1/tests/test_minimum_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_minimum_of_all_pixels.py` & `pyclesperanto-0.9.1/tests/test_minimum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_minimum_of_masked_pixels.py` & `pyclesperanto-0.9.1/tests/test_minimum_of_masked_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_minimum_x_projection.py` & `pyclesperanto-0.9.1/tests/test_minimum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_minimum_y_projection.py` & `pyclesperanto-0.9.1/tests/test_minimum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_minimum_z_projection.py` & `pyclesperanto-0.9.1/tests/test_minimum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mode_box.py` & `pyclesperanto-0.9.1/tests/test_mode_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_mode_sphere.py` & `pyclesperanto-0.9.1/tests/test_mode_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_multiply_images.py` & `pyclesperanto-0.9.1/tests/test_multiply_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_multiply_matrix.py` & `pyclesperanto-0.9.1/tests/test_multiply_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_nan_to_num.py` & `pyclesperanto-0.9.1/tests/test_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_nonzero_maximum_box.py` & `pyclesperanto-0.9.1/tests/test_nonzero_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_nonzero_maximum_diamond.py` & `pyclesperanto-0.9.1/tests/test_nonzero_maximum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_nonzero_minimum_box.py` & `pyclesperanto-0.9.1/tests/test_nonzero_minimum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_nonzero_minimum_diamond.py` & `pyclesperanto-0.9.1/tests/test_nonzero_minimum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_not_equal.py` & `pyclesperanto-0.9.1/tests/test_not_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_not_equal_constant.py` & `pyclesperanto-0.9.1/tests/test_not_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_onlyzero_overwrite_maximum_box.py` & `pyclesperanto-0.9.1/tests/test_onlyzero_overwrite_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_onlyzero_overwrite_maximum_diamond.py` & `pyclesperanto-0.9.1/tests/test_onlyzero_overwrite_maximum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_opening_box.py` & `pyclesperanto-0.9.1/tests/test_opening_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_opening_labels.py` & `pyclesperanto-0.9.1/tests/test_opening_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_opening_sphere.py` & `pyclesperanto-0.9.1/tests/test_opening_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_operators.py` & `pyclesperanto-0.9.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_paste.py` & `pyclesperanto-0.9.1/tests/test_paste.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_power.py` & `pyclesperanto-0.9.1/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_power_images.py` & `pyclesperanto-0.9.1/tests/test_power_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_push.py` & `pyclesperanto-0.9.1/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_range.py` & `pyclesperanto-0.9.1/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_reduce_labels_to_label_edges.py` & `pyclesperanto-0.9.1/tests/test_reduce_labels_to_label_edges.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_reduction.py` & `pyclesperanto-0.9.1/tests/test_reduction.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_replace_intensities.py` & `pyclesperanto-0.9.1/tests/test_replace_intensities.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_replace_intensity.py` & `pyclesperanto-0.9.1/tests/test_replace_intensity.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_column.py` & `pyclesperanto-0.9.1/tests/test_set_column.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_image_borders.py` & `pyclesperanto-0.9.1/tests/test_set_image_borders.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_nonzero_pixels_to_pixelindex.py` & `pyclesperanto-0.9.1/tests/test_set_nonzero_pixels_to_pixelindex.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_plane.py` & `pyclesperanto-0.9.1/tests/test_set_plane.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_ramp_x.py` & `pyclesperanto-0.9.1/tests/test_set_ramp_x.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_ramp_y.py` & `pyclesperanto-0.9.1/tests/test_set_ramp_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_ramp_z.py` & `pyclesperanto-0.9.1/tests/test_set_ramp_z.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_set_row.py` & `pyclesperanto-0.9.1/tests/test_set_row.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_setitem.py` & `pyclesperanto-0.9.1/tests/test_setitem.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_small_hessian_eigenvalue.py` & `pyclesperanto-0.9.1/tests/test_small_hessian_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_smaller.py` & `pyclesperanto-0.9.1/tests/test_smaller.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_smaller_constant.py` & `pyclesperanto-0.9.1/tests/test_smaller_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_smaller_or_equal.py` & `pyclesperanto-0.9.1/tests/test_smaller_or_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_smaller_or_equal_constant.py` & `pyclesperanto-0.9.1/tests/test_smaller_or_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_smooth_labels.py` & `pyclesperanto-0.9.1/tests/test_smooth_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_sobel.py` & `pyclesperanto-0.9.1/tests/test_sobel.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_spots_to_pointlist.py` & `pyclesperanto-0.9.1/tests/test_spots_to_pointlist.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_standard_deviation_box.py` & `pyclesperanto-0.9.1/tests/test_standard_deviation_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_standard_deviation_sphere.py` & `pyclesperanto-0.9.1/tests/test_standard_deviation_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_subtract_gaussian_background.py` & `pyclesperanto-0.9.1/tests/test_subtract_gaussian_background.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_sum_of_all_pixels.py` & `pyclesperanto-0.9.1/tests/test_sum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_sum_reduction.py` & `pyclesperanto-0.9.1/tests/test_sum_reduction.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_sum_x_projection.py` & `pyclesperanto-0.9.1/tests/test_sum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_sum_y_projection.py` & `pyclesperanto-0.9.1/tests/test_sum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_sum_z_projection.py` & `pyclesperanto-0.9.1/tests/test_sum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_threshold_otsu.py` & `pyclesperanto-0.9.1/tests/test_threshold_otsu.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_top_hat_box.py` & `pyclesperanto-0.9.1/tests/test_top_hat_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_top_hat_sphere.py` & `pyclesperanto-0.9.1/tests/test_top_hat_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_transpose_xy.py` & `pyclesperanto-0.9.1/tests/test_transpose_xy.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_transpose_xz.py` & `pyclesperanto-0.9.1/tests/test_transpose_xz.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_transpose_yz.py` & `pyclesperanto-0.9.1/tests/test_transpose_yz.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_undefined_to_zero.py` & `pyclesperanto-0.9.1/tests/test_undefined_to_zero.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_variance_box.py` & `pyclesperanto-0.9.1/tests/test_variance_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_variance_sphere.py` & `pyclesperanto-0.9.1/tests/test_variance_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_voronoi_labeling.py` & `pyclesperanto-0.9.1/tests/test_voronoi_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/tests/test_voronoi_otsu_labeling.py` & `pyclesperanto-0.9.1/tests/test_voronoi_otsu_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto-0.9.0/PKG-INFO` & `pyclesperanto-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclesperanto
-Version: 0.9.0
+Version: 0.9.1
 Summary: GPU-accelerated image processing in python using OpenCL
 Author-Email: Stephane Rigaud <stephane.rigaud@pasteur.fr>, Robert Haase <robert.haase@uni-leipzig.de>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

