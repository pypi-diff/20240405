# Comparing `tmp/asdf-astropy-0.6.0.tar.gz` & `tmp/asdf-astropy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asdf-astropy-0.6.0.tar", last modified: Wed Mar 13 18:52:06 2024, max compression
+gzip compressed data, was "asdf-astropy-0.6.1.tar", last modified: Fri Apr  5 19:55:02 2024, max compression
```

## Comparing `asdf-astropy-0.6.0.tar` & `asdf-astropy-0.6.1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.162539 asdf-astropy-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.134539 asdf-astropy-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.142539 asdf-astropy-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/.github/workflows/downstream.yml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-03-13 18:52:06.162539 asdf-astropy-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.142539 asdf-astropy-0.6.0/asdf_astropy/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-13 18:52:06.000000 asdf-astropy-0.6.0/asdf_astropy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.142539 asdf-astropy-0.6.0/asdf_astropy/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/earth_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/sky_coord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/spectral_coord.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_earth_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_sky_coord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_spectral_coord.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/fits/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/fits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/fits/fits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/fits/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/fits/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/fits/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/table/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/table/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/table/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/table/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/table/tests/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/time/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.146539 asdf-astropy-0.6.0/asdf_astropy/converters/time/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/time/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/time/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/time/tests/test_time_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/time/time.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/time/time_delta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.150539 asdf-astropy-0.6.0/asdf_astropy/converters/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/functional_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/math_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/projections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/rotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.150539 asdf-astropy-0.6.0/asdf_astropy/converters/transform/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37200 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/transform/tests/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.150539 asdf-astropy-0.6.0/asdf_astropy/converters/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/equivalency.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/magunit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/quantity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.150539 asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_equivalency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_magunit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/unit/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/converters/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/io/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/io/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/manifests/astropy-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/manifests/astropy-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/manifests/astropy-1.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/manifests/units-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/manifests/units-1.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.138539 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/fits/
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/fits/fits-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/fits/fits-1.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/ndarraymixin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/table-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/table-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/table-1.2.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/time/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/time/timedelta-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/time/timedelta-1.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/transform/units_mapping-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/transform/units_mapping-1.1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/units/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/units/equivalency-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/units/equivalency-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/resources/schemas/units/magunit-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.154539 asdf-astropy-0.6.0/asdf_astropy/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/testing/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.158539 asdf-astropy-0.6.0/asdf_astropy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/asdf_astropy/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.158539 asdf-astropy-0.6.0/asdf_astropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-03-13 18:52:06.000000 asdf-astropy-0.6.0/asdf_astropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-03-13 18:52:06.000000 asdf-astropy-0.6.0/asdf_astropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 18:52:06.000000 asdf-astropy-0.6.0/asdf_astropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-13 18:52:06.000000 asdf-astropy-0.6.0/asdf_astropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-13 18:52:06.000000 asdf-astropy-0.6.0/asdf_astropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 18:52:06.000000 asdf-astropy-0.6.0/asdf_astropy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.158539 asdf-astropy-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.158539 asdf-astropy-0.6.0/docs/asdf-astropy/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/details.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/example.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/manifest.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/migrating.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/asdf-astropy/table.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.158539 asdf-astropy-0.6.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:52:06.158539 asdf-astropy-0.6.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/scripts/generate_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 18:52:06.162539 asdf-astropy-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-03-13 18:51:55.000000 asdf-astropy-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.820216 asdf-astropy-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.792216 asdf-astropy-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.800216 asdf-astropy-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/.github/workflows/downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-05 19:55:02.820216 asdf-astropy-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.800216 asdf-astropy-0.6.1/asdf_astropy/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 19:55:02.000000 asdf-astropy-0.6.1/asdf_astropy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.800216 asdf-astropy-0.6.1/asdf_astropy/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.804216 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/earth_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/sky_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/spectral_coord.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.804216 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_earth_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_sky_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_spectral_coord.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.804216 asdf-astropy-0.6.1/asdf_astropy/converters/fits/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/fits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/fits/fits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.804216 asdf-astropy-0.6.1/asdf_astropy/converters/fits/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/fits/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/fits/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.804216 asdf-astropy-0.6.1/asdf_astropy/converters/table/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/table/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.804216 asdf-astropy-0.6.1/asdf_astropy/converters/table/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/table/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/table/tests/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.804216 asdf-astropy-0.6.1/asdf_astropy/converters/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.808216 asdf-astropy-0.6.1/asdf_astropy/converters/time/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/time/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/time/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/time/tests/test_time_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/time/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/time/time_delta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.808216 asdf-astropy-0.6.1/asdf_astropy/converters/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/functional_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/math_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.808216 asdf-astropy-0.6.1/asdf_astropy/converters/transform/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37200 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/transform/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.808216 asdf-astropy-0.6.1/asdf_astropy/converters/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/equivalency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/magunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/quantity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_equivalency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_magunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/unit/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/converters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/io/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/io/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/manifests/astropy-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/manifests/astropy-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/manifests/astropy-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/manifests/units-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/manifests/units-1.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.796216 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/fits/
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/fits/fits-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/fits/fits-1.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/ndarraymixin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/table-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/table-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/table-1.2.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/time/timedelta-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/time/timedelta-1.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.812216 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/transform/units_mapping-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/transform/units_mapping-1.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.816216 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/units/equivalency-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/units/equivalency-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/resources/schemas/units/magunit-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.816216 asdf-astropy-0.6.1/asdf_astropy/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/testing/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.816216 asdf-astropy-0.6.1/asdf_astropy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/asdf_astropy/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.820216 asdf-astropy-0.6.1/asdf_astropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-05 19:55:02.000000 asdf-astropy-0.6.1/asdf_astropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-05 19:55:02.000000 asdf-astropy-0.6.1/asdf_astropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:55:02.000000 asdf-astropy-0.6.1/asdf_astropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 19:55:02.000000 asdf-astropy-0.6.1/asdf_astropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 19:55:02.000000 asdf-astropy-0.6.1/asdf_astropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 19:55:02.000000 asdf-astropy-0.6.1/asdf_astropy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.816216 asdf-astropy-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.816216 asdf-astropy-0.6.1/docs/asdf-astropy/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/manifest.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/migrating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/asdf-astropy/table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.816216 asdf-astropy-0.6.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:55:02.816216 asdf-astropy-0.6.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/scripts/generate_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:55:02.820216 asdf-astropy-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 19:54:52.000000 asdf-astropy-0.6.1/tox.ini
```

### Comparing `asdf-astropy-0.6.0/.github/workflows/changelog.yml` & `asdf-astropy-0.6.1/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/.github/workflows/ci.yml` & `asdf-astropy-0.6.1/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,15 @@
       cache-restore-keys: |
         pip-
       # Any env name which does not start with `pyXY` will use this Python version.
       default_python: '3.9'
       envs: |
         - linux: py39-parallel-cov
         - linux: py311-test-devdeps-parallel-cov
-        - linux: py39-astropylts-parallel-cov
-        - linux: py39-transformlts-parallel-cov
+        - linux: py312-test-predeps-parallel-cov
       coverage: codecov
 
   asdf-schemas:
     needs: [setup]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       cache-path: ~/.cache/pip
```

### Comparing `asdf-astropy-0.6.0/.github/workflows/downstream.yml` & `asdf-astropy-0.6.1/.github/workflows/downstream.yml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/CHANGES.rst` & `asdf-astropy-0.6.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.6.1 (2024-04-05)
+------------------
+
+- update ``copy`` usage in ``Quantity`` converter to
+  deal with astropy 6.1 changes. [#224]
+
 0.6.0 (2024-03-13)
 ------------------
 
 - Add python 3.12 support. [#219]
 - Update ASDF standard 1.6.0 support. [#219]
 - Increase minimum versions for ``asdf-coordinates-schemas``
   ``asdf-transform-schemas`` and list ``asdf-standard`` as
```

### Comparing `asdf-astropy-0.6.0/CITATION` & `asdf-astropy-0.6.1/CITATION`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/LICENSE.rst` & `asdf-astropy-0.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/PKG-INFO` & `asdf-astropy-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdf-astropy
-Version: 0.6.0
+Version: 0.6.1
 Summary: ASDF serialization support for astropy
 Author-email: The Astropy Developers <astropy.team@gmail.com>
 License: Copyright (c) 2011-2022, Astropy Developers
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `asdf-astropy-0.6.0/README.rst` & `asdf-astropy-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/__init__.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/__init__.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/angle.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/angle.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/frame.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/frame.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/representation.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/representation.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/spectral_coord.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/spectral_coord.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_angle.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_angle.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_earth_location.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_earth_location.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_frame.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_representation.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_representation.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_sky_coord.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_sky_coord.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/coordinates/tests/test_spectral_coord.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/coordinates/tests/test_spectral_coord.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/fits/fits.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/fits/fits.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/fits/tests/test_fits.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/fits/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/helpers.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/table/table.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/table/table.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/table/tests/test_table.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/table/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/time/tests/test_time.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/time/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/time/tests/test_time_delta.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/time/tests/test_time_delta.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/time/time.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/time/time.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/__init__.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/compound.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/compound.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/core.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/core.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/functional_models.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/functional_models.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/mappings.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/mappings.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/math_functions.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/math_functions.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/polynomial.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/polynomial.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/projections.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/projections.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/properties.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/properties.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/rotations.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/rotations.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/spline.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/spline.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/tabular.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/tabular.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/transform/tests/test_transform.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/transform/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/unit/equivalency.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/unit/equivalency.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_equivalency.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_equivalency.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_magunit.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_magunit.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_quantity.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/unit/tests/test_unit.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/unit/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/converters/unit/unit.py` & `asdf-astropy-0.6.1/asdf_astropy/converters/unit/unit.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/extensions.py` & `asdf-astropy-0.6.1/asdf_astropy/extensions.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/integration.py` & `asdf-astropy-0.6.1/asdf_astropy/integration.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/io/connect.py` & `asdf-astropy-0.6.1/asdf_astropy/io/connect.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/io/tests/test_io.py` & `asdf-astropy-0.6.1/asdf_astropy/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/manifests/astropy-1.0.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/manifests/astropy-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/manifests/astropy-1.1.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/manifests/astropy-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/manifests/astropy-1.2.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/manifests/astropy-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/manifests/units-1.0.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/manifests/units-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/manifests/units-1.1.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/manifests/units-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/fits/fits-1.0.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/fits/fits-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/fits/fits-1.1.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/fits/fits-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/table-1.0.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/table-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/table-1.1.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/table-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/table/table-1.2.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/table/table-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/time/timedelta-1.0.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/time/timedelta-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/time/timedelta-1.1.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/time/timedelta-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/transform/units_mapping-1.0.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/transform/units_mapping-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/transform/units_mapping-1.1.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/transform/units_mapping-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/units/equivalency-1.0.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/units/equivalency-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/resources/schemas/units/equivalency-1.1.0.yaml` & `asdf-astropy-0.6.1/asdf_astropy/resources/schemas/units/equivalency-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/testing/helpers.py` & `asdf-astropy-0.6.1/asdf_astropy/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy/tests/test_integration.py` & `asdf-astropy-0.6.1/asdf_astropy/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/asdf_astropy.egg-info/PKG-INFO` & `asdf-astropy-0.6.1/asdf_astropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdf-astropy
-Version: 0.6.0
+Version: 0.6.1
 Summary: ASDF serialization support for astropy
 Author-email: The Astropy Developers <astropy.team@gmail.com>
 License: Copyright (c) 2011-2022, Astropy Developers
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `asdf-astropy-0.6.0/asdf_astropy.egg-info/SOURCES.txt` & `asdf-astropy-0.6.1/asdf_astropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/Makefile` & `asdf-astropy-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/asdf-astropy/details.rst` & `asdf-astropy-0.6.1/docs/asdf-astropy/details.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/asdf-astropy/example.rst` & `asdf-astropy-0.6.1/docs/asdf-astropy/example.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/asdf-astropy/install.rst` & `asdf-astropy-0.6.1/docs/asdf-astropy/install.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/asdf-astropy/migrating.rst` & `asdf-astropy-0.6.1/docs/asdf-astropy/migrating.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/asdf-astropy/quickstart.rst` & `asdf-astropy-0.6.1/docs/asdf-astropy/quickstart.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/asdf-astropy/schemas.rst` & `asdf-astropy-0.6.1/docs/asdf-astropy/schemas.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/asdf-astropy/table.rst` & `asdf-astropy-0.6.1/docs/asdf-astropy/table.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/conf.py` & `asdf-astropy-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/index.rst` & `asdf-astropy-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/docs/make.bat` & `asdf-astropy-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/pyproject.toml` & `asdf-astropy-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/scripts/generate_manifest.py` & `asdf-astropy-0.6.1/scripts/generate_manifest.py`

 * *Files identical despite different names*

### Comparing `asdf-astropy-0.6.0/tox.ini` & `asdf-astropy-0.6.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tox]
 envlist =
     py{39,310}-test{,-alldeps}
     py38-test-devdeps{,-numpydev}
     py38-cov
-    py38-astropylts
     py39-test-oldestdep-parallels-cov
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
 isolated_build = true
 
+
 [testenv]
 description =
     run tests
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
     cov: and test coverage
-    astropylts: with astropy LTS
 
 setenv =
     devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
 
+pip_pre =
+    predeps: true
+    !predeps: false
+
 # The following provides some specific pinnings for key packages
 deps =
     cov: coverage
-    astropylts: astropy==5.0.*
-    transformlts: asdf-transform-schemas==0.2.*
 
     devdeps: -rrequirements-dev.txt
     oldestdeps: minimum_dependencies
 
     parallel: pytest-xdist
 extras =
     test
```

