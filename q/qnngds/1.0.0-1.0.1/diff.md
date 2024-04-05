# Comparing `tmp/qnngds-1.0.0.tar.gz` & `tmp/qnngds-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-1.0.0.tar", last modified: Thu Apr  4 21:08:58 2024, max compression
+gzip compressed data, was "qnngds-1.0.1.tar", last modified: Thu Apr  4 21:36:38 2024, max compression
```

## Comparing `qnngds-1.0.0.tar` & `qnngds-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-04-04 20:17:36.246389 qnngds-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1229 2024-04-04 20:17:36.255378 qnngds-1.0.0/README.md
--rw-r--r--   0        0        0     1108 2024-04-04 21:08:58.459673 qnngds-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      114 2024-04-04 20:17:36.381837 qnngds-1.0.0/src/qnngds/__init__.py
--rw-r--r--   0        0        0    10894 2024-04-04 20:17:36.386818 qnngds-1.0.0/src/qnngds/circuits.py
--rw-r--r--   0        0        0    52650 2024-04-04 20:17:36.404847 qnngds-1.0.0/src/qnngds/design.py
--rw-r--r--   0        0        0     8294 2024-04-04 20:17:36.419863 qnngds-1.0.0/src/qnngds/devices.py
--rw-r--r--   0        0        0     8508 2024-04-04 20:17:36.440380 qnngds-1.0.0/src/qnngds/geometries.py
--rw-r--r--   0        0        0    21961 2024-04-04 20:17:36.464166 qnngds-1.0.0/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 qnngds-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-04 21:36:36.131832 qnngds-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1199 2024-04-04 21:36:36.131832 qnngds-1.0.1/README.md
+-rw-r--r--   0        0        0     1108 2024-04-04 21:36:38.987835 qnngds-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-04-04 21:36:36.135832 qnngds-1.0.1/src/qnngds/__init__.py
+-rw-r--r--   0        0        0    10600 2024-04-04 21:36:36.135832 qnngds-1.0.1/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    51283 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/design.py
+-rw-r--r--   0        0        0     8019 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/devices.py
+-rw-r--r--   0        0        0     8244 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/geometries.py
+-rw-r--r--   0        0        0    21375 2024-04-04 21:36:36.139832 qnngds-1.0.1/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 qnngds-1.0.1/PKG-INFO
```

### Comparing `qnngds-1.0.0/LICENSE.txt` & `qnngds-1.0.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2016 The Python Packaging Authority (PyPA)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2016 The Python Packaging Authority (PyPA)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `qnngds-1.0.0/README.md` & `qnngds-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# QNNGDS
-
-## Description
-QNNGDS is a toolbox built on top of phidl for device design in the QNN group.
-It is made for helping in the design of gds files. The package is composed of 5 main modules:
-- design (contains pre-built cells, ready to be added to a design)
-- utilities (contains useful functions for building a new cell)
-- geometries (contains test structures and geometry tools)
-- circuits (contains circuits made of devices)
-- devices (contains devices like ntron, htron, snspd)
-
-## Getting Started
-### Installing
-- Make sure [gdspy](https://pypi.org/project/gdspy/) is installed
-- Install qnngds package with 'pip install qnngds'
-
-### Dependencies
-- [phidl](https://pypi.org/project/phidl/)
-- [scipy](https://pypi.org/project/scipy/)
-
-## License
-This project is licensed under the MIT License - see the LICENSE.txt file for details
-
-## [Documentation](https://qnngds.readthedocs.io/en/latest/)
-- [API](https://qnngds.readthedocs.io/en/latest/api.html)
-- [Libraries](https://qnngds.readthedocs.io/en/latest/libraries.html)
-- [Tutorials](https://qnngds.readthedocs.io/en/latest/tutorials.html)
-
-## How to contribute
-- [Developer's documentation](https://qnngds-dev.readthedocs.io/en/latest)
+# QNNGDS
+
+## Description
+QNNGDS is a toolbox built on top of phidl for device design in the QNN group.
+It is made for helping in the design of gds files. The package is composed of 5 main modules:
+- design (contains pre-built cells, ready to be added to a design)
+- utilities (contains useful functions for building a new cell)
+- geometries (contains test structures and geometry tools)
+- circuits (contains circuits made of devices)
+- devices (contains devices like ntron, htron, snspd)
+
+## Getting Started
+### Installing
+- Make sure [gdspy](https://pypi.org/project/gdspy/) is installed
+- Install qnngds package with 'pip install qnngds'
+
+### Dependencies
+- [phidl](https://pypi.org/project/phidl/)
+- [scipy](https://pypi.org/project/scipy/)
+
+## License
+This project is licensed under the MIT License - see the LICENSE.txt file for details
+
+## [Documentation](https://qnngds.readthedocs.io/en/latest/)
+- [API](https://qnngds.readthedocs.io/en/latest/api.html)
+- [Libraries](https://qnngds.readthedocs.io/en/latest/libraries.html)
+- [Tutorials](https://qnngds.readthedocs.io/en/latest/tutorials.html)
+
+## How to contribute
+- [Developer's documentation](https://qnngds-dev.readthedocs.io/en/latest)
```

### Comparing `qnngds-1.0.0/pyproject.toml` & `qnngds-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
 ]
```

### Comparing `qnngds-1.0.0/src/qnngds/circuits.py` & `qnngds-1.0.1/src/qnngds/circuits.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-"""Circuits module contains a library of QNN's circuits (e.g. snspd coupled to
-ntron, logic gates etc.)"""
-
-from phidl import Device
-from phidl import quickplot as qp
-from phidl import set_quickplot_options
-import phidl.geometry as pg
-from typing import Tuple, Union
-import math
-
-import qnngds.devices as qd
-
-set_quickplot_options(blocking=True)
-
-
-def snspd_ntron(
-    w_snspd: float = 0.1,
-    pitch_snspd: float = 0.3,
-    size_snspd: Tuple[Union[int, float]] = (3, 3),
-    w_inductor: float = 0.3,
-    pitch_inductor: float = 0.6,
-    k_inductor13: Union[int, float] = 10,
-    k_inductor2: Union[int, float] = 4,
-    w_choke: float = 0.02,
-    w_channel: float = 0.12,
-    w_pad: Union[int, float] = 1,
-    layer: int = 0,
-) -> Device:
-    """Creates a SNSPD coupled to an NTRON, with 3 inductors in the circuit as:
-
-    >>> |        |
-    >>> L1       L3
-    >>> |        |
-    >>> |__L2__NTRON
-    >>> |        |
-    >>> SNSPD
-    >>> |
-
-    The length of L1, L2, and L3 (long nanowires) where scaled against the SNSPD:
-    L1 = L3 = k13 * L and L2 = k2 * L where L is the SNSPD kinetic inductance.
-
-    Parameters:
-        w_snspd (float): Width of the SNSPD.
-        pitch_snspd (float): Pitch of the SNSPD.
-        size_snspd (Tuple[Union[int, float]]): Size of the SNSPD.
-        w_inductor (float): Width of the inductors.
-        pitch_inductor (float): Pitch of the inductors.
-        k_inductor13 (Union[int, float]): The factor for scaling L1 and L3 relative to the SNSPD kinetic inductance.
-        k_inductor2 (Union[int, float]): The factor for scaling L2 relative to the SNSPD kinetic inductance.
-        w_choke (float): Width of the choke in the NTRON.
-        w_channel (float): Width of the channel in the NTRON.
-        w_pad (Union[int, float]): Width of the external connections to the cell.
-        layer (int): Layer of the device.
-
-    Returns:
-        Device: The created device.
-    """
-
-    def scale_inductors_to_snspd():
-
-        l_snspd = size_snspd[0] * size_snspd[1] / pitch_snspd
-        l_inductor13 = k_inductor13 * w_inductor / w_snspd * l_snspd
-        l_inductor2 = k_inductor2 * w_inductor / w_snspd * l_snspd
-
-        n_inductor13 = math.sqrt(l_inductor13 * pitch_inductor)
-        n_inductor2 = math.sqrt(l_inductor2 * pitch_inductor)
-
-        size_inductor13 = (n_inductor13, n_inductor13)
-        size_inductor2 = (n_inductor2, n_inductor2)
-
-        return size_inductor13, size_inductor2
-
-    def crossA():
-
-        D = Device()
-        tee = pg.tee(
-            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
-        )
-        first_tee = D << tee.movey(-w_inductor / 2)
-        second_tee = D << tee
-        second_tee.rotate(180)
-
-        D = pg.union(D)
-        D.add_port(port=first_tee.ports[1], name="E")
-        D.add_port(port=first_tee.ports[2], name="W")
-        D.add_port(port=first_tee.ports[3], name="S")
-        D.add_port(port=second_tee.ports[3], name="N")
-
-        D.flatten()
-        return D
-
-    def crossB():
-
-        D = Device()
-        tee = pg.tee(
-            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
-        )
-        first_tee = D << tee.movey(-w_inductor / 2)
-        first_tee.rotate(180)
-
-        D.add_port(port=first_tee.ports[1], name="W")
-        D.add_port(port=first_tee.ports[2], name="E")
-        D.add_port(port=first_tee.ports[3], name="N")
-
-        D.flatten()
-        return D
-
-    def crossC():
-
-        D = Device()
-        tee = pg.tee(
-            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
-        )
-        first_tee = D << tee.movey(-w_inductor / 2)
-        first_tee.rotate(90)
-
-        D.add_port(port=first_tee.ports[1], name="N")
-        D.add_port(port=first_tee.ports[2], name="S")
-        D.add_port(port=first_tee.ports[3], name="E")
-
-        D.flatten()
-        return D
-
-    def create_snspd():
-        ## SNSPD
-        SNSPD = SNSPD_NTRON << pg.snspd(
-            wire_width=w_snspd,
-            wire_pitch=pitch_snspd,
-            size=size_snspd,
-            num_squares=None,
-            turn_ratio=4,
-            terminals_same_side=False,
-            layer=layer,
-        )
-        SNSPD.rotate(90)
-        # port 1 connected to gnd
-        route = SNSPD_NTRON << pg.optimal_step(
-            SNSPD.ports[1].width, w_pad, symmetric=True
-        )
-        route.connect(route.ports[1], SNSPD.ports[1])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="S1")
-        # port 2 connected to crossA south
-        route_step = SNSPD_NTRON << pg.optimal_step(
-            SNSPD.ports[2].width, CROSSA.ports["S"].width, symmetric=True
-        )
-        route_step.connect(route_step.ports[1], SNSPD.ports[2])
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], route_step.ports[2])
-        CROSSA.connect(CROSSA.ports["S"], route.ports["N"])
-
-    def create_inductor1():
-        ## INDUCTOR1
-        INDUCTOR1 = SNSPD_NTRON << pg.snspd(
-            wire_width=w_inductor,
-            wire_pitch=pitch_inductor,
-            size=size_inductor13,
-            num_squares=None,
-            terminals_same_side=False,
-            layer=layer,
-        )
-        INDUCTOR1.rotate(90).mirror()
-        # port 1 connected to crossA north
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], CROSSA.ports["N"])
-        INDUCTOR1.connect(INDUCTOR1.ports[1], route.ports["N"])
-        # port 2 connected to pad
-        route = SNSPD_NTRON << pg.optimal_step(
-            INDUCTOR1.ports[2].width, w_pad, symmetric=True
-        )
-        route.connect(route.ports[1], INDUCTOR1.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="N1")
-
-    def create_inductor2():
-        ## INDUCTOR2
-        INDUCTOR2 = Device()
-        inductor2 = INDUCTOR2 << pg.snspd(
-            wire_width=w_inductor,
-            wire_pitch=pitch_inductor,
-            size=size_inductor2,
-            num_squares=None,
-            terminals_same_side=True,
-            layer=layer,
-        )
-        arcleft = INDUCTOR2 << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
-        arcright = INDUCTOR2 << pg.arc(
-            radius=2 * w_inductor, width=w_inductor, theta=90
-        )
-        arcleft.connect(arcleft.ports[2], inductor2.ports[1])
-        arcright.connect(arcright.ports[1], inductor2.ports[2])
-        INDUCTOR2.add_port(port=arcleft.ports[1])
-        INDUCTOR2.add_port(port=arcright.ports[2])
-        INDUCTOR2 = SNSPD_NTRON << INDUCTOR2
-        # port 1 connected to crossA east
-        INDUCTOR2.connect(INDUCTOR2.ports[1], CROSSA.ports["E"])
-        # port 2 connected to crossB west
-        route = SNSPD_NTRON << pg.compass((w_pad / 2, w_inductor))
-        route.connect(route.ports["W"], INDUCTOR2.ports[2])
-        CROSSB.connect(CROSSB.ports["W"], route.ports["E"])
-
-    def create_ntron():
-        ## NTRON
-        NTRON = SNSPD_NTRON << qd.ntron(
-            choke_w=w_choke,
-            gate_w=w_inductor,
-            channel_w=w_channel,
-            source_w=w_inductor,
-            drain_w=w_inductor,
-            choke_shift=-3 * w_channel,
-            layer=layer,
-        )
-        # port 3 connected to crossB east
-        route = SNSPD_NTRON << pg.compass((w_pad / 2, w_inductor))
-        route.connect(route.ports["W"], CROSSB.ports["E"])
-        NTRON.connect(NTRON.ports[3], route.ports["E"])
-        # port 1 connected to crossC south
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], NTRON.ports[1])
-        CROSSC.connect(CROSSC.ports["S"], route.ports["N"])
-        # port 2 connected to gnd
-        route = SNSPD_NTRON << pg.optimal_step(
-            NTRON.ports[2].width, w_pad, symmetric=True
-        )
-        route.connect(route.ports[1], NTRON.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="S2")
-
-    def create_inductor3():
-        ## INDUCTOR3
-        INDUCTOR3 = SNSPD_NTRON << pg.snspd(
-            wire_width=w_inductor,
-            wire_pitch=pitch_inductor,
-            size=size_inductor13,
-            num_squares=None,
-            terminals_same_side=False,
-            layer=layer,
-        )
-        INDUCTOR3.rotate(90)
-        # port 1 connected to crossC north
-        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
-        route.connect(route.ports["S"], CROSSC.ports["N"])
-        INDUCTOR3.connect(INDUCTOR3.ports[1], route.ports["N"])
-        # port 2 connected to pad
-        route = SNSPD_NTRON << pg.optimal_step(
-            INDUCTOR3.ports[2].width, w_pad, symmetric=True
-        )
-        route.connect(route.ports[1], INDUCTOR3.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports[2], name="N3")
-
-    def create_probing_routes():
-        ## SNSPD PROBING PAD
-        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
-        step.connect(step.ports[1], CROSSA.ports["W"])
-        route = SNSPD_NTRON << pg.compass((abs(SNSPD_NTRON.xmin - step.xmin), w_pad))
-        route.connect(route.ports["E"], step.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports["W"], name="W1")
-
-        ## NTRON IN PROBING PAD
-        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
-        step.connect(step.ports[1], CROSSB.ports["N"])
-        route = SNSPD_NTRON << pg.compass((w_pad, abs(SNSPD_NTRON.ymax - step.ymax)))
-        route.connect(route.ports["S"], step.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports["N"], name="N2")
-
-        ## NTRON OUT PROBING PAD
-        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
-        step.connect(step.ports[1], CROSSC.ports["E"])
-        route = SNSPD_NTRON << pg.compass((abs(SNSPD_NTRON.xmax - step.xmax), w_pad))
-        route.connect(route.ports["W"], step.ports[2])
-        SNSPD_NTRON.add_port(port=route.ports["E"], name="E1")
-
-    SNSPD_NTRON = Device(f"SNSPD NTRON {w_snspd} {w_choke} ")
-
-    size_inductor13, size_inductor2 = scale_inductors_to_snspd()
-
-    CROSSA = SNSPD_NTRON << crossA()
-    CROSSB = SNSPD_NTRON << crossB()
-    CROSSC = SNSPD_NTRON << crossC()
-
-    create_snspd()
-    create_inductor1()
-    create_inductor2()
-    create_ntron()
-    create_inductor3()
-    create_probing_routes()
-
-    SNSPD_NTRON.flatten()
-
-    ports = SNSPD_NTRON.get_ports()
-    SNSPD_NTRON = pg.union(SNSPD_NTRON, layer=layer)
-    for port in ports:
-        SNSPD_NTRON.add_port(port)
-
-    SNSPD_NTRON.move(SNSPD_NTRON.center, (0, 0))
-    SNSPD_NTRON.name = f"SNSPD NTRON {w_snspd} {w_choke} "
-    return SNSPD_NTRON
+"""Circuits module contains a library of QNN's circuits (e.g. snspd coupled to
+ntron, logic gates etc.)"""
+
+from phidl import Device
+from phidl import quickplot as qp
+from phidl import set_quickplot_options
+import phidl.geometry as pg
+from typing import Tuple, Union
+import math
+
+import qnngds.devices as qd
+
+set_quickplot_options(blocking=True)
+
+
+def snspd_ntron(
+    w_snspd: float = 0.1,
+    pitch_snspd: float = 0.3,
+    size_snspd: Tuple[Union[int, float]] = (3, 3),
+    w_inductor: float = 0.3,
+    pitch_inductor: float = 0.6,
+    k_inductor13: Union[int, float] = 10,
+    k_inductor2: Union[int, float] = 4,
+    w_choke: float = 0.02,
+    w_channel: float = 0.12,
+    w_pad: Union[int, float] = 1,
+    layer: int = 0,
+) -> Device:
+    """Creates a SNSPD coupled to an NTRON, with 3 inductors in the circuit as:
+
+    >>> |        |
+    >>> L1       L3
+    >>> |        |
+    >>> |__L2__NTRON
+    >>> |        |
+    >>> SNSPD
+    >>> |
+
+    The length of L1, L2, and L3 (long nanowires) where scaled against the SNSPD:
+    L1 = L3 = k13 * L and L2 = k2 * L where L is the SNSPD kinetic inductance.
+
+    Parameters:
+        w_snspd (float): Width of the SNSPD.
+        pitch_snspd (float): Pitch of the SNSPD.
+        size_snspd (Tuple[Union[int, float]]): Size of the SNSPD.
+        w_inductor (float): Width of the inductors.
+        pitch_inductor (float): Pitch of the inductors.
+        k_inductor13 (Union[int, float]): The factor for scaling L1 and L3 relative to the SNSPD kinetic inductance.
+        k_inductor2 (Union[int, float]): The factor for scaling L2 relative to the SNSPD kinetic inductance.
+        w_choke (float): Width of the choke in the NTRON.
+        w_channel (float): Width of the channel in the NTRON.
+        w_pad (Union[int, float]): Width of the external connections to the cell.
+        layer (int): Layer of the device.
+
+    Returns:
+        Device: The created device.
+    """
+
+    def scale_inductors_to_snspd():
+
+        l_snspd = size_snspd[0] * size_snspd[1] / pitch_snspd
+        l_inductor13 = k_inductor13 * w_inductor / w_snspd * l_snspd
+        l_inductor2 = k_inductor2 * w_inductor / w_snspd * l_snspd
+
+        n_inductor13 = math.sqrt(l_inductor13 * pitch_inductor)
+        n_inductor2 = math.sqrt(l_inductor2 * pitch_inductor)
+
+        size_inductor13 = (n_inductor13, n_inductor13)
+        size_inductor2 = (n_inductor2, n_inductor2)
+
+        return size_inductor13, size_inductor2
+
+    def crossA():
+
+        D = Device()
+        tee = pg.tee(
+            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
+        )
+        first_tee = D << tee.movey(-w_inductor / 2)
+        second_tee = D << tee
+        second_tee.rotate(180)
+
+        D = pg.union(D)
+        D.add_port(port=first_tee.ports[1], name="E")
+        D.add_port(port=first_tee.ports[2], name="W")
+        D.add_port(port=first_tee.ports[3], name="S")
+        D.add_port(port=second_tee.ports[3], name="N")
+
+        D.flatten()
+        return D
+
+    def crossB():
+
+        D = Device()
+        tee = pg.tee(
+            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
+        )
+        first_tee = D << tee.movey(-w_inductor / 2)
+        first_tee.rotate(180)
+
+        D.add_port(port=first_tee.ports[1], name="W")
+        D.add_port(port=first_tee.ports[2], name="E")
+        D.add_port(port=first_tee.ports[3], name="N")
+
+        D.flatten()
+        return D
+
+    def crossC():
+
+        D = Device()
+        tee = pg.tee(
+            (3 * w_inductor, w_inductor), (w_inductor, w_inductor), taper_type="fillet"
+        )
+        first_tee = D << tee.movey(-w_inductor / 2)
+        first_tee.rotate(90)
+
+        D.add_port(port=first_tee.ports[1], name="N")
+        D.add_port(port=first_tee.ports[2], name="S")
+        D.add_port(port=first_tee.ports[3], name="E")
+
+        D.flatten()
+        return D
+
+    def create_snspd():
+        ## SNSPD
+        SNSPD = SNSPD_NTRON << pg.snspd(
+            wire_width=w_snspd,
+            wire_pitch=pitch_snspd,
+            size=size_snspd,
+            num_squares=None,
+            turn_ratio=4,
+            terminals_same_side=False,
+            layer=layer,
+        )
+        SNSPD.rotate(90)
+        # port 1 connected to gnd
+        route = SNSPD_NTRON << pg.optimal_step(
+            SNSPD.ports[1].width, w_pad, symmetric=True
+        )
+        route.connect(route.ports[1], SNSPD.ports[1])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="S1")
+        # port 2 connected to crossA south
+        route_step = SNSPD_NTRON << pg.optimal_step(
+            SNSPD.ports[2].width, CROSSA.ports["S"].width, symmetric=True
+        )
+        route_step.connect(route_step.ports[1], SNSPD.ports[2])
+        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], route_step.ports[2])
+        CROSSA.connect(CROSSA.ports["S"], route.ports["N"])
+
+    def create_inductor1():
+        ## INDUCTOR1
+        INDUCTOR1 = SNSPD_NTRON << pg.snspd(
+            wire_width=w_inductor,
+            wire_pitch=pitch_inductor,
+            size=size_inductor13,
+            num_squares=None,
+            terminals_same_side=False,
+            layer=layer,
+        )
+        INDUCTOR1.rotate(90).mirror()
+        # port 1 connected to crossA north
+        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], CROSSA.ports["N"])
+        INDUCTOR1.connect(INDUCTOR1.ports[1], route.ports["N"])
+        # port 2 connected to pad
+        route = SNSPD_NTRON << pg.optimal_step(
+            INDUCTOR1.ports[2].width, w_pad, symmetric=True
+        )
+        route.connect(route.ports[1], INDUCTOR1.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="N1")
+
+    def create_inductor2():
+        ## INDUCTOR2
+        INDUCTOR2 = Device()
+        inductor2 = INDUCTOR2 << pg.snspd(
+            wire_width=w_inductor,
+            wire_pitch=pitch_inductor,
+            size=size_inductor2,
+            num_squares=None,
+            terminals_same_side=True,
+            layer=layer,
+        )
+        arcleft = INDUCTOR2 << pg.arc(radius=2 * w_inductor, width=w_inductor, theta=90)
+        arcright = INDUCTOR2 << pg.arc(
+            radius=2 * w_inductor, width=w_inductor, theta=90
+        )
+        arcleft.connect(arcleft.ports[2], inductor2.ports[1])
+        arcright.connect(arcright.ports[1], inductor2.ports[2])
+        INDUCTOR2.add_port(port=arcleft.ports[1])
+        INDUCTOR2.add_port(port=arcright.ports[2])
+        INDUCTOR2 = SNSPD_NTRON << INDUCTOR2
+        # port 1 connected to crossA east
+        INDUCTOR2.connect(INDUCTOR2.ports[1], CROSSA.ports["E"])
+        # port 2 connected to crossB west
+        route = SNSPD_NTRON << pg.compass((w_pad / 2, w_inductor))
+        route.connect(route.ports["W"], INDUCTOR2.ports[2])
+        CROSSB.connect(CROSSB.ports["W"], route.ports["E"])
+
+    def create_ntron():
+        ## NTRON
+        NTRON = SNSPD_NTRON << qd.ntron(
+            choke_w=w_choke,
+            gate_w=w_inductor,
+            channel_w=w_channel,
+            source_w=w_inductor,
+            drain_w=w_inductor,
+            choke_shift=-3 * w_channel,
+            layer=layer,
+        )
+        # port 3 connected to crossB east
+        route = SNSPD_NTRON << pg.compass((w_pad / 2, w_inductor))
+        route.connect(route.ports["W"], CROSSB.ports["E"])
+        NTRON.connect(NTRON.ports[3], route.ports["E"])
+        # port 1 connected to crossC south
+        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], NTRON.ports[1])
+        CROSSC.connect(CROSSC.ports["S"], route.ports["N"])
+        # port 2 connected to gnd
+        route = SNSPD_NTRON << pg.optimal_step(
+            NTRON.ports[2].width, w_pad, symmetric=True
+        )
+        route.connect(route.ports[1], NTRON.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="S2")
+
+    def create_inductor3():
+        ## INDUCTOR3
+        INDUCTOR3 = SNSPD_NTRON << pg.snspd(
+            wire_width=w_inductor,
+            wire_pitch=pitch_inductor,
+            size=size_inductor13,
+            num_squares=None,
+            terminals_same_side=False,
+            layer=layer,
+        )
+        INDUCTOR3.rotate(90)
+        # port 1 connected to crossC north
+        route = SNSPD_NTRON << pg.compass((w_inductor, w_pad / 2))
+        route.connect(route.ports["S"], CROSSC.ports["N"])
+        INDUCTOR3.connect(INDUCTOR3.ports[1], route.ports["N"])
+        # port 2 connected to pad
+        route = SNSPD_NTRON << pg.optimal_step(
+            INDUCTOR3.ports[2].width, w_pad, symmetric=True
+        )
+        route.connect(route.ports[1], INDUCTOR3.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports[2], name="N3")
+
+    def create_probing_routes():
+        ## SNSPD PROBING PAD
+        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step.connect(step.ports[1], CROSSA.ports["W"])
+        route = SNSPD_NTRON << pg.compass((abs(SNSPD_NTRON.xmin - step.xmin), w_pad))
+        route.connect(route.ports["E"], step.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports["W"], name="W1")
+
+        ## NTRON IN PROBING PAD
+        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step.connect(step.ports[1], CROSSB.ports["N"])
+        route = SNSPD_NTRON << pg.compass((w_pad, abs(SNSPD_NTRON.ymax - step.ymax)))
+        route.connect(route.ports["S"], step.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports["N"], name="N2")
+
+        ## NTRON OUT PROBING PAD
+        step = SNSPD_NTRON << pg.optimal_step(w_inductor, w_pad, symmetric=True)
+        step.connect(step.ports[1], CROSSC.ports["E"])
+        route = SNSPD_NTRON << pg.compass((abs(SNSPD_NTRON.xmax - step.xmax), w_pad))
+        route.connect(route.ports["W"], step.ports[2])
+        SNSPD_NTRON.add_port(port=route.ports["E"], name="E1")
+
+    SNSPD_NTRON = Device(f"SNSPD NTRON {w_snspd} {w_choke} ")
+
+    size_inductor13, size_inductor2 = scale_inductors_to_snspd()
+
+    CROSSA = SNSPD_NTRON << crossA()
+    CROSSB = SNSPD_NTRON << crossB()
+    CROSSC = SNSPD_NTRON << crossC()
+
+    create_snspd()
+    create_inductor1()
+    create_inductor2()
+    create_ntron()
+    create_inductor3()
+    create_probing_routes()
+
+    SNSPD_NTRON.flatten()
+
+    ports = SNSPD_NTRON.get_ports()
+    SNSPD_NTRON = pg.union(SNSPD_NTRON, layer=layer)
+    for port in ports:
+        SNSPD_NTRON.add_port(port)
+
+    SNSPD_NTRON.move(SNSPD_NTRON.center, (0, 0))
+    SNSPD_NTRON.name = f"SNSPD NTRON {w_snspd} {w_choke} "
+    return SNSPD_NTRON
```

### Comparing `qnngds-1.0.0/src/qnngds/design.py` & `qnngds-1.0.1/src/qnngds/design.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,1367 +1,1367 @@
-"""Design's module is though for users to be able to access pre-built cells
-that are made of circuits, devices or test structures already integrated in a
-die cell.
-
-It is a module that is sufficient in itself to build an entire new
-design.
-"""
-
-from phidl import Device
-
-# from phidl import quickplot as qp
-# from phidl import set_quickplot_options
-import phidl.geometry as pg
-import phidl.routing as pr
-from typing import Tuple, List, Union, Optional
-import math
-import os
-import qnngds.geometries as qg
-import qnngds.devices as qd
-import qnngds.circuits as qc
-import qnngds.utilities as qu
-
-Free = True
-Occupied = False
-
-auto_param = None
-die_cell_border = 80
-
-# default parameters
-dflt_chip_w = 10000
-dflt_chip_margin = 100
-dflt_N_dies = 11
-dflt_die_w = 980
-dflt_pad_size = (150, 250)
-dflt_device_outline = 0.5
-dflt_die_outline = 10
-dflt_ebeam_overlap = 10
-dflt_layers = {"annotation": 0, "device": 1, "die": 2, "pad": 3}
-dflt_text = auto_param
-
-## to build a design
-
-
-def create_chip(
-    chip_w: Union[int, float] = dflt_chip_w,
-    margin: Union[int, float] = dflt_chip_margin,
-    N_dies: int = dflt_N_dies,
-    die_w: Union[None, int, float] = auto_param,
-    annotations_layer: int = dflt_layers["annotation"],
-    unpack_chip_map: bool = True,
-    create_devices_map_txt: Union[bool, str] = False,
-) -> Union[
-    Tuple[Device, Union[int, float], List[List[bool]], str],
-    Tuple[Device, Union[int, float], str],
-    Tuple[Device, Union[int, float], List[List[bool]]],
-    Tuple[Device, Union[int, float]],
-]:
-    """Creates a chip map in the annotations layer.
-
-    If unpack_chip_map is set to True, creates a map (2D array) to monitor the
-    states of each cell of the chip. The user should input N_dies xor die_w.
-
-    Parameters:
-        chip_w (int or float): The overall width (in um) of the chip.
-        margin (int or float): The width (in um) of the outline of the chip where no device should be placed.
-        N_dies (int): Number of dies/units to be placed by row and column.
-        die_w (None, int, or float): If specified, the width of each die/unit to be placed by row and column.
-        annotations_layer (int or array-like[2]): The layer where to put the device.
-        unpack_chip_map (bool): If True, the function returns a map (2D array) of states to be filled later (e.g., with place_on_chip()).
-        create_devices_map_txt (bool or string): If True or string, the function creates a txt file that will map the devices.
-
-    Returns:
-        Tuple[Device, float, List[List[bool]], str]: A tuple containing from 2 to 4 elements, depending on what needs to be extracted (parameters dependent):
-
-        - **CHIP** (*Device*): The chip map.
-        - **die_w** (*float*): The width of each die. (returned if die_w was None)
-        - **N_dies** (*float*): The number of dies/units on each row and column. (returned if die_w was not None)
-        - **chip_map** (*array-like[N_dies][N_dies] of bool*): A 2D array filled with "Free" (=True) states. (returned if unpack_chip_map is True)
-        - **file_name** (*str*): The name of the created devices map text file. (returned if create_devices_map_txt is not False)
-    """
-
-    CHIP = Device("CHIP ")
-    CHIP.add_polygon(
-        [(0, 0), (chip_w, 0), (chip_w, chip_w), (0, chip_w)], layer=annotations_layer
-    )
-
-    useful_w = chip_w - margin * 2
-    useful_area = CHIP.add_polygon(
-        [(0, 0), (useful_w, 0), (useful_w, useful_w), (0, useful_w)],
-        layer=annotations_layer,
-    )
-    useful_area.move((margin, margin))
-
-    if die_w is not None:
-        N_dies = useful_w / die_w
-        return_N_or_w = N_dies
-    else:
-        die_w = useful_w / N_dies
-        return_N_or_w = die_w
-    CELL = pg.rectangle([die_w, die_w], layer=annotations_layer)
-    array = CHIP.add_array(CELL, columns=N_dies, rows=N_dies, spacing=(die_w, die_w))
-    array.move((0, 0), (margin, margin))
-
-    CHIP.flatten()
-    CHIP.move((margin, margin), (0, 0))
-
-    if create_devices_map_txt:
-        ## create a devices map ...
-        if create_devices_map_txt == True:
-            file_name = "devices map"
-        else:
-            file_name = f"{create_devices_map_txt}"
-
-        # check that file does not already exist, in which case it will add a int to its name:
-        i = 0
-        file_to_find = file_name
-        while True:
-            if i != 0:
-                file_to_find = file_name + f"({i})"
-            file_already_exists = os.path.exists(f"{file_to_find}.txt")
-            i += 1
-            if not file_already_exists:
-                file_name = file_to_find
-                break
-        with open(f"{file_name}.txt", "a") as file:
-            file.write("Devices placed on the chip: \n\n")
-            file.write("(row, col) : device.name\n\n")
-
-        ## ... and return the devices map filename in the outputs
-        if unpack_chip_map:
-            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
-            return CHIP, return_N_or_w, chip_map, file_name
-        else:
-            return CHIP, return_N_or_w, file_name
-    else:
-        if unpack_chip_map:
-            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
-            return CHIP, return_N_or_w, chip_map
-        else:
-            return CHIP, return_N_or_w
-
-
-def place_on_chip(
-    cell: Device,
-    coordinates: Tuple[int, int],
-    chip_map: List[List[bool]],
-    die_w: Union[int, float],
-    devices_map_txt: Union[None, str] = None,
-) -> bool:
-    """Moves the chip to the coordinates specified.
-
-    Update the chip map with Occupied states where the device has been placed.
-
-    NB: The cell is aligned from its bottom left corner to the coordinates.
-
-    Parameters:
-        cell (Device): Device to be moved.
-        coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
-            Note that the indices start at 0.
-        chip_map (2D array): The 2D array mapping the free cells in the chip map.
-        die_w (int or float): The width of a die/unit in the chip map.
-        devices_map_txt (str or None): Name of the devices map text file to write placement information.
-            If None, no file will be written.
-
-    Returns:
-        bool: False, if the Device falls out of the chip map, prints an error
-        message and does not place the device. True, otherwise.
-
-    Raises:
-        Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
-    """
-
-    # update the chip's availabilities
-    n_cell = round(cell.xsize / die_w)
-    m_cell = round(cell.ysize / die_w)
-    for n in range(n_cell):
-        for m in range(m_cell):
-            try:
-                if chip_map[coordinates[1] + m][coordinates[0] + n] == Occupied:
-                    print(
-                        f"Warning, placing Device {cell.name} "
-                        + f"in an occupied state ({coordinates[1]+m}, {coordinates[0]+n})"
-                    )
-                else:
-                    chip_map[coordinates[1] + m][coordinates[0] + n] = Occupied
-            except IndexError:
-                print(
-                    f"Error, Device {cell.name} "
-                    + f"falls out of the chip map ({coordinates[1]+m}, {coordinates[0]+n})"
-                )
-                return False
-
-    # move the cell
-    cell_bottom_left = cell.get_bounding_box()[0]
-    cell.move(cell_bottom_left, (coordinates[0] * die_w, coordinates[1] * die_w))
-
-    # write the cell's place on the devices map text file
-    if devices_map_txt is not None:
-        with open(f"{devices_map_txt}.txt", "a") as file:
-            try:
-                name = cell.name.replace("\n", "")
-            except AttributeError:
-                name = "unnamed"
-            file.write(f"({coordinates[0]}, {coordinates[1]}) : {name}\n")
-
-    return True
-
-
-def place_remaining_devices(
-    devices_to_place: List[Device],
-    chip_map: List[List[bool]],
-    die_w: Union[int, float],
-    write_devices_map_txt: Union[bool, str] = False,
-) -> Optional[None]:
-    """Go through the chip map and place the devices given, where the chip map
-    is Free.
-
-    Parameters:
-        devices_to_place (list of Device objects): The devices to be placed.
-        chip_map (2D array): The 2D array mapping the free cells in the chip map.
-        die_w (int or float): The width of a die/unit in the chip map.
-        write_devices_map_txt (bool or str): If True, write a .txt file mapping the devices that were placed.
-            If str, specifies the filename of the .txt file.
-
-    Note:
-        The list of devices is not re-ordered to fit as many of them as possible.
-        Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
-    """
-
-    # name and create the file if no file was given
-    if write_devices_map_txt == True:
-
-        file_name = "remaining_cells_map"
-        with open(f"{file_name}.txt", "a") as file:
-            file.write("Remaining devices placed on the chip:\n\n")
-            file.write("(row, col) : device.name\n\n")
-    # use the file's name is a file was given
-    elif write_devices_map_txt:
-        file_name = write_devices_map_txt
-    # pass false if no txt file should be created
-    else:
-        file_name = None
-
-    for row_i, row in enumerate(chip_map):
-        for col_i, status in enumerate(row):
-            if status == Free and devices_to_place:
-                if place_on_chip(
-                    devices_to_place[0], (col_i, row_i), chip_map, die_w, file_name
-                ):
-                    devices_to_place.pop(0)
-
-    if devices_to_place:
-        print(
-            "Some devices are still to be placed, " + "no place remaining on the chip."
-        )
-
-
-## basics:
-
-
-def create_alignment_cell(
-    die_w: Union[int, float] = dflt_die_w,
-    layers_to_align: List[int] = [dflt_layers["die"], dflt_layers["pad"]],
-    outline_die: Union[int, float] = dflt_die_outline,
-    die_layer: int = dflt_layers["die"],
-    text: Union[None, str] = dflt_text,
-) -> Device:
-    """Creates alignment marks in an integer number of unit cells.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        layers_to_align (list of int): Layers to align.
-        outline_die (int or float): The width of the die's outline.
-        die_layer (int): The layer where the die is placed.
-        text (str): Text to be displayed.
-
-    Returns:
-        DIE_ALIGN (Device): A device that centers the alignment marks in an n*m unit cell.
-    """
-
-    if text is None:
-        text = ""
-    DIE = Device(f"DIE ALIGN {text} ")
-
-    ALIGN = qg.alignment_mark(layers_to_align)
-
-    n = math.ceil((ALIGN.xsize) / die_w)
-    m = math.ceil((ALIGN.ysize) / die_w)
-
-    BORDER = qu.die_cell(
-        die_size=(n * die_w, m * die_w),
-        device_max_size=(ALIGN.xsize + 20, ALIGN.ysize + 20),
-        ports={},
-        ports_gnd={},
-        isolation=outline_die,
-        text=f"ALIGN {text}",
-        layer=die_layer,
-        invert=True,
-    )
-
-    DIE << BORDER.flatten()
-    DIE << ALIGN
-
-    return DIE
-
-
-def create_vdp_cell(
-    die_w: Union[int, float] = dflt_die_w,
-    pad_size: Tuple[float] = dflt_pad_size,
-    layers_to_probe: List[int] = [dflt_layers["pad"]],
-    layers_to_outline: Union[None, List[int]] = auto_param,
-    outline: Union[int, float] = dflt_die_outline,
-    die_layer: Union[int, float] = dflt_layers["die"],
-    pad_layer: int = dflt_layers["pad"],
-    text: Union[None, str] = dflt_text,
-) -> Device:
-    r"""Creates a cell containing a Van Der Pauw structure between 4 contact
-    pads.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        layers_to_probe (list of int): The layers on which to place the VDP structure.
-        layers_to_outline (list of int): Among the VDP layers, the ones for which structure must not be filled but outlined.
-        outline (int or float): The width of the VDP and die's outline.
-        die_layer (int or tuple of int): The layer where the die is placed.
-        pad_layer (int or tuple of int): The layer where the pads are placed.
-        text (str, optional): If None, the text is f"VDP \n{layers_to_probe}".
-
-    Returns:
-        DIE_VANDP (Device): The created device.
-    """
-
-    if text is None:
-        text = layers_to_probe
-    DIE_VANDP = Device(f"DIE VAN DER PAUW {text} ")
-
-    ## Create the die
-    w = die_w - 2 * (pad_size[1] + 2 * outline)  # width of max device size
-    BORDER = qu.die_cell(
-        die_size=(die_w, die_w),
-        device_max_size=(w, w),
-        pad_size=pad_size,
-        contact_w=pad_size[0],
-        contact_l=0,
-        ports={"N": 1, "E": 1, "W": 1, "S": 1},
-        ports_gnd=["N", "E", "W", "S"],
-        text=f"VDP \n{text} ",
-        isolation=outline,
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-    )
-    PADS = pg.deepcopy(BORDER)
-    PADS = PADS.remove_layers([pad_layer], invert_selection=True)
-
-    DIE_VANDP << BORDER.flatten()
-
-    ## Create the test structure
-    DEVICE = Device()
-
-    # the test structure is an hexagonal shape between the die's ports
-    TEST = Device()
-    TEST << PADS
-    rect = TEST << pg.straight((PADS.ports["E1"].x - PADS.ports["W1"].x, pad_size[0]))
-    rect.move(rect.center, (0, 0))
-    TEST << pr.route_quad(PADS.ports["N1"], rect.ports[1])
-    TEST << pr.route_quad(PADS.ports["S1"], rect.ports[2])
-    TEST = pg.union(TEST)
-
-    # outline the test structure for layers that need to be outlined
-
-    if layers_to_outline is None:
-        layers_to_outline = [die_layer]
-    for layer in layers_to_probe:
-        TEST_LAY = pg.deepcopy(TEST)
-        if layer in layers_to_outline:
-            TEST_LAY = pg.outline(TEST_LAY, outline)
-        DEVICE << TEST_LAY.flatten(single_layer=layer)
-
-    DIE_VANDP << DEVICE
-
-    DIE_VANDP = pg.union(DIE_VANDP, by_layer=True)
-    DIE_VANDP.name = f"DIE VAN DER PAUW {text} "
-    return DIE_VANDP
-
-
-def create_etch_test_cell(
-    die_w: Union[int, float] = dflt_die_w,
-    layers_to_etch: List[List[int]] = [[dflt_layers["pad"]]],
-    outline_die: Union[int, float] = dflt_die_outline,
-    die_layer: int = dflt_layers["die"],
-    text: Union[None, str] = dflt_text,
-) -> Device:
-    """Creates etch test structures in an integer number of unit cells.
-
-    These test structures are thought to be used by probing on pads (with a
-    simple multimeter) that should be isolated one from another if the etching
-    is complete.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        layers_to_etch (list of list of int): Each element of the list corresponds to one test point, to put on the list of layers specified.
-                                               Example: [[1, 2], [1], [2]]
-        outline_die (int or float): The width of the die's outline.
-        die_layer (int): The layer where the die is placed.
-        text (str): Text to be displayed.
-
-    Returns:
-        DIE_ETCH_TEST (Device): A device (with size n*m of unit cells) with etch tests in its center.
-    """
-
-    if text is None:
-        text = f"{layers_to_etch}"
-    DIE_ETCH_TEST = Device(f"DIE ETCH TEST {text} ")
-
-    TEST = Device()
-
-    ## Create the probing areas
-
-    margin = 0.12 * die_w
-    rect = pg.rectangle((die_w - 2 * margin, die_w - 2 * margin))
-    for i, layer_to_etch in enumerate(layers_to_etch):
-        probe = Device()
-        probe.add_array(rect, 2, 1, (die_w, die_w))
-        for layer in layer_to_etch:
-            TEST << pg.outline(probe, -outline_die, layer=layer).movey(i * die_w)
-
-    ## Create the die
-
-    n = math.ceil((TEST.xsize + 2 * die_cell_border) / die_w)
-    m = math.ceil((TEST.ysize + 2 * die_cell_border) / die_w)
-    BORDER = qu.die_cell(
-        die_size=(n * die_w, m * die_w),
-        ports={},
-        ports_gnd={},
-        text=f"ETCH TEST {text}",
-        isolation=10,
-        layer=die_layer,
-        invert=True,
-    )
-
-    BORDER.move(TEST.center)
-    DIE_ETCH_TEST << BORDER.flatten()
-    DIE_ETCH_TEST << TEST
-    DIE_ETCH_TEST.move(DIE_ETCH_TEST.center, (0, 0))
-
-    return DIE_ETCH_TEST
-
-
-def create_resolution_test_cell(
-    die_w: Union[int, float] = dflt_die_w,
-    layer_to_resolve: int = dflt_layers["device"],
-    resolutions_to_test: List[float] = [
-        0.025,
-        0.05,
-        0.075,
-        0.1,
-        0.25,
-        0.5,
-        1,
-        1.5,
-        2.0,
-    ],
-    outline: Union[int, float] = dflt_die_outline,
-    die_layer: int = dflt_layers["die"],
-    text: Union[None, str] = dflt_text,
-) -> Device:
-    r"""Creates a cell containing a resolution test.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        layer_to_resolve (int): The layer to put the resolution test on.
-        resolutions_to_test (list of float): The resolutions to test in µm.
-        outline (int or float): The width of the VDP and die's outline.
-        die_layer (int or tuple of int): The layer where the die is placed.
-        text (str, optional): If None, the text is f"RES TEST \n{layer_to_resolve}".
-
-    Returns:
-        DIE_RES_TEST (Device): The created device.
-    """
-
-    if text is None:
-        text = layer_to_resolve
-    DIE_RES_TEST = Device(f"DIE RESOLUTION TEST {text} ")
-
-    ## Create the test structure
-    TEST_RES = Device(f"RESOLUTION TEST {text} ")
-    test_res = TEST_RES << qg.resolution_test(
-        resolutions=resolutions_to_test, inverted=False, layer=layer_to_resolve
-    )
-    test_res_invert = TEST_RES << qg.resolution_test(
-        resolutions=resolutions_to_test,
-        inverted=resolutions_to_test[-1],
-        layer=layer_to_resolve,
-    )
-    test_res_invert.movey(
-        test_res_invert.ymin, test_res.ymax + 5 * resolutions_to_test[-1]
-    )
-
-    DIE_RES_TEST << TEST_RES.move(TEST_RES.center, (0, 0))
-
-    ## Create the die
-    n = math.ceil((TEST_RES.xsize) / die_w)
-    m = math.ceil((TEST_RES.ysize) / die_w)
-    BORDER = qu.die_cell(
-        die_size=(n * die_w, m * die_w),
-        ports={},
-        ports_gnd=[],
-        text=f"RES TEST \n{text} ",
-        isolation=outline,
-        layer=die_layer,
-        invert=True,
-    )
-
-    DIE_RES_TEST << BORDER.flatten()
-
-    return DIE_RES_TEST
-
-
-## devices:
-
-
-def create_nanowires_cell(
-    die_w: Union[int, float] = dflt_die_w,
-    pad_size: Tuple[float] = dflt_pad_size,
-    channels_sources_w: List[Tuple[float, float]] = [(0.1, 1), (0.5, 3), (1, 10)],
-    overlap_w: Union[int, float] = dflt_ebeam_overlap,
-    outline_die: Union[int, float] = dflt_die_outline,
-    outline_dev: Union[int, float] = dflt_device_outline,
-    device_layer: int = dflt_layers["device"],
-    die_layer: int = dflt_layers["die"],
-    pad_layer: int = dflt_layers["pad"],
-    text: Union[None, str] = dflt_text,
-) -> Device:
-    """Creates a cell that contains several nanowires of given channel and
-    source.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        channels_sources_w (list of tuple of float): The list of (channel_w, source_w) of the nanowires to create.
-        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
-                                   (useful for ebeam lithography).
-        outline_die (int or float): The width of the pads outline.
-        outline_dev (int or float): The width of the device's outline.
-        device_layer (int or tuple of int): The layer where the device is placed.
-        die_layer (int or tuple of int): The layer where the die is placed.
-        pad_layer (int or tuple of int): The layer where the pads are placed.
-        text (str, optional): If None, the text is "NWIRES".
-
-    Returns:
-        Device: A device (of size n*m unit cells) containing the nanowires, the
-        border of the die (created with die_cell function), and the connections
-        between the nanowires and pads.
-    """
-
-    if text is None:
-        text = ""
-
-    NANOWIRES_DIE = Device(f"DIE NWIRES {text} ")
-
-    DEVICE = Device(f"NWIRES {text} ")
-
-    ## Create the NANOWIRES
-
-    NANOWIRES = Device()
-    nanowires_ref = []
-    for i, channel_source_w in enumerate(channels_sources_w):
-        nanowire_ref = NANOWIRES << qd.nanowire(
-            channel_source_w[0], channel_source_w[1]
-        )
-        nanowires_ref.append(nanowire_ref)
-    DEVICE << NANOWIRES
-
-    ## Create the DIE
-
-    # die parameters, checkup conditions
-    n = len(channels_sources_w)
-    die_size = (math.ceil((2 * (n + 1) * pad_size[0]) / die_w) * die_w, die_w)
-    die_contact_w = NANOWIRES.xsize + overlap_w
-    dev_contact_w = NANOWIRES.xsize
-    routes_margin = 4 * die_contact_w
-    dev_max_size = (2 * n * pad_size[0], NANOWIRES.ysize + routes_margin)
-
-    # die, with calculated parameters
-    BORDER = qu.die_cell(
-        die_size=die_size,
-        device_max_size=dev_max_size,
-        pad_size=pad_size,
-        contact_w=die_contact_w,
-        contact_l=overlap_w,
-        ports={"N": n, "S": n},
-        ports_gnd=["S"],
-        isolation=outline_die,
-        text=f"NWIRES {text}",
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-    )
-
-    ## Place the nanowires
-
-    for i, nanowire_ref in enumerate(nanowires_ref):
-        nanowire_ref.movex(BORDER.ports[f"N{i+1}"].x)
-        NANOWIRES.add_port(port=nanowire_ref.ports[1], name=f"N{i+1}")
-        NANOWIRES.add_port(port=nanowire_ref.ports[2], name=f"S{i+1}")
-
-    ## Route the nanowires and the die
-
-    # hyper tapers
-    HT, dev_ports = qu.add_hyptap_to_cell(BORDER.get_ports(), overlap_w, dev_contact_w)
-    DEVICE.ports = dev_ports.ports
-    DEVICE << HT
-
-    # routes from nanowires to hyper tapers
-    ROUTES = qu.route_to_dev(HT.get_ports(), NANOWIRES.ports)
-    DEVICE << ROUTES
-
-    DEVICE.ports = dev_ports.ports
-    DEVICE = pg.outline(DEVICE, outline_dev, open_ports=2 * outline_dev)
-    DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"NWIRES {text} "
-
-    NANOWIRES_DIE << DEVICE
-    NANOWIRES_DIE << BORDER
-
-    NANOWIRES_DIE = pg.union(NANOWIRES_DIE, by_layer=True)
-    NANOWIRES_DIE.name = f"DIE NWIRES {text} "
-    return NANOWIRES_DIE
-
-
-def create_ntron_cell(
-    die_w: Union[int, float] = dflt_die_w,
-    pad_size: Tuple[float, float] = dflt_pad_size,
-    choke_w: Union[int, float] = 0.1,
-    channel_w: Union[int, float] = 0.5,
-    gate_w: Union[None, int, float] = auto_param,
-    source_w: Union[None, int, float] = auto_param,
-    drain_w: Union[None, int, float] = auto_param,
-    choke_shift: Union[None, int, float] = auto_param,
-    overlap_w: Union[None, int, float] = dflt_ebeam_overlap,
-    outline_die: Union[None, int, float] = dflt_die_outline,
-    outline_dev: Union[None, int, float] = dflt_device_outline,
-    device_layer: int = dflt_layers["device"],
-    die_layer: int = dflt_layers["die"],
-    pad_layer: int = dflt_layers["pad"],
-    text: Union[None, str] = dflt_text,
-) -> Device:
-    """Creates a standardized cell specifically for a single ntron.
-
-    Unless specified, scales the ntron parameters as:
-    gate_w = drain_w = source_w = 3 * channel_w
-    choke_shift = -3 * channel_w
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        choke_w (int or float): The width of the ntron's choke in µm.
-        channel_w (int or float): The width of the ntron's channel in µm.
-        gate_w (int or float, optional): If None, gate width is 3 times the channel width.
-        source_w (int or float, optional): If None, source width is 3 times the channel width.
-        drain_w (int or float, optional): If None, drain width is 3 times the channel width.
-        choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
-        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
-                                             (useful for ebeam lithography).
-        outline_die (int or float): The width of the pads outline.
-        outline_dev (int or float): The width of the device's outline.
-        device_layer (int or array-like[2]): The layer where the device is placed.
-        die_layer (int or array-like[2]): The layer where the die is placed.
-        pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, the text is the ntron's choke and channel widths.
-
-    Returns:
-        Device: A device containing the ntron, the border of the die (created with die_cell function),
-        and the connections between the ports.
-    """
-
-    ## Create the NTRON
-
-    # sizes the ntron parameters that were not given
-    if source_w is None and drain_w is None:
-        drain_w = source_w = 3 * channel_w
-    elif source_w is None:
-        source_w = drain_w
-    else:
-        drain_w = source_w
-    if gate_w is None:
-        gate_w = source_w
-    if choke_shift is None:
-        choke_shift = -3 * channel_w
-
-    NTRON = qd.ntron_compassPorts(
-        choke_w, gate_w, channel_w, source_w, drain_w, choke_shift, device_layer
-    )
-
-    if text is None:
-        text = f"chk: {choke_w} \nchnl: {channel_w}"
-    DIE_NTRON = Device(f"DIE NTRON {text} ")
-
-    DEVICE = Device(f"NTRON {text} ")
-    DEVICE << NTRON
-
-    ## Create the DIE
-
-    # die parameters, checkup conditions
-    die_contact_w = NTRON.ports["N1"].width + overlap_w
-    routes_margin = 2 * die_contact_w
-    dev_min_w = (
-        die_contact_w + 3 * outline_die
-    )  # condition imposed by the die parameters (contacts width)
-    device_max_w = max(2 * routes_margin + max(NTRON.size), dev_min_w)
-
-    # the die with calculated parameters
-    BORDER = qu.die_cell(
-        die_size=(die_w, die_w),
-        device_max_size=(device_max_w, device_max_w),
-        pad_size=pad_size,
-        contact_w=die_contact_w,
-        contact_l=overlap_w,
-        ports={"N": 1, "W": 1, "S": 1},
-        ports_gnd=["S"],
-        text=text,
-        isolation=10,
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-    )
-
-    # place the ntron
-    NTRON.movex(NTRON.ports["N1"].midpoint[0], BORDER.ports["N1"].midpoint[0])
-
-    # Route DIE and NTRON
-
-    # hyper tapers
-    dev_contact_w = NTRON.ports["N1"].width
-    HT, device_ports = qu.add_hyptap_to_cell(
-        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
-    )
-    DEVICE << HT
-    DEVICE.ports = device_ports.ports
-    # routes
-    ROUTES = qu.route_to_dev(HT.get_ports(), NTRON.ports, device_layer)
-    DEVICE << ROUTES
-
-    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
-    DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"NTRON {text} "
-
-    DIE_NTRON << DEVICE
-    DIE_NTRON << BORDER
-
-    DIE_NTRON = pg.union(DIE_NTRON, by_layer=True)
-    DIE_NTRON.name = f"DIE NTRON {text} "
-    return DIE_NTRON
-
-
-def create_snspd_ntron_cell(
-    die_w: Union[int, float] = dflt_die_w,
-    pad_size: Tuple[float, float] = dflt_pad_size,
-    w_choke: Union[int, float] = 0.1,
-    w_snspd: Union[int, float] = auto_param,
-    overlap_w: Union[int, float] = dflt_ebeam_overlap,
-    outline_die: Union[int, float] = dflt_die_outline,
-    outline_dev: Union[int, float] = dflt_device_outline,
-    device_layer: int = dflt_layers["device"],
-    die_layer: int = dflt_layers["die"],
-    pad_layer: int = dflt_layers["pad"],
-    text: Union[None, str] = dflt_text,
-) -> Device:
-    """Creates a cell that contains an SNSPD coupled to an NTRON. The device's
-    parameters are sized according to the SNSPD's width and the NTRON's choke.
-
-    Parameters:
-        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        w_choke (int or float): The width of the NTRON choke in µm.
-        w_snspd (int or float, optional): The width of the SNSPD nanowire in µm (if None, scaled to 5 * w_choke).
-        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
-                                             (useful for ebeam lithography).
-        outline_die (int or float): The width of the pads outline.
-        outline_dev (int or float): The width of the device's outline.
-        device_layer (int or array-like[2]): The layer where the device is placed.
-        die_layer (int or array-like[2]): The layer where the die is placed.
-        pad_layer (int or array-like[2]): The layer where the pads are placed.
-        text (string, optional): If None, text = f'SNSPD {w_choke}'.
-
-    Returns:
-        Device: A cell containing a die in die_layer, pads in pad layer,
-        and an SNSPD-NTRON properly routed in the device layer.
-    """
-
-    # Create SNSPD-NTRON
-    if w_snspd is None:
-        w_snspd = 5 * w_choke
-
-    if text is None:
-        text = f"SNSPD \n{w_snspd} {w_choke} "
-    DIE_SNSPD_NTRON = Device(f"DIE {text} ")
-    DEVICE = Device(f"{text} ")
-
-    SNSPD_NTRON = qc.snspd_ntron(
-        w_snspd=w_snspd,
-        pitch_snspd=3 * w_snspd,
-        size_snspd=(30 * w_snspd, 30 * w_snspd),
-        w_inductor=3 * w_snspd,
-        pitch_inductor=6 * w_snspd,
-        k_inductor13=20 * w_snspd,
-        k_inductor2=8 * w_snspd,
-        w_choke=w_choke,
-        w_channel=6 * w_choke,
-        w_pad=10 * w_snspd,
-        layer=device_layer,
-    )
-    DEVICE << SNSPD_NTRON
-
-    # Create DIE
-
-    die_contact_w = min(
-        10 * SNSPD_NTRON.ports["N1"].width + overlap_w, 0.5 * pad_size[0]
-    )
-
-    routes_margin = 2 * die_contact_w
-    margin = 2 * (pad_size[1] + outline_die + routes_margin)
-    n = max(2, math.ceil((SNSPD_NTRON.xsize + margin) / die_w))
-    m = max(1, math.ceil((SNSPD_NTRON.ysize + margin) / die_w))
-
-    dev_min_size = [
-        (die_contact_w + 3 * outline_die) * x for x in (5, 3)
-    ]  # condition imposed by the die parameters (contacts width)
-    device_max_size = (
-        max(
-            min(n * die_w - margin, 8 * routes_margin + SNSPD_NTRON.size[0]),
-            dev_min_size[0],
-        ),
-        max(
-            min(m * die_w - margin, 2 * routes_margin + SNSPD_NTRON.size[1]),
-            dev_min_size[1],
-        ),
-    )
-
-    BORDER = qu.die_cell(
-        die_size=(n * die_w, m * die_w),
-        device_max_size=device_max_size,
-        pad_size=pad_size,
-        contact_w=die_contact_w,
-        contact_l=overlap_w,
-        ports={"N": 3, "E": 1, "W": 1, "S": 2},
-        ports_gnd=["S"],
-        text=text,
-        isolation=outline_die,
-        layer=die_layer,
-        pad_layer=pad_layer,
-        invert=True,
-    )
-
-    # Route DIE and SNSPD-NTRON
-
-    # hyper tapers
-    dev_contact_w = min(4 * SNSPD_NTRON.ports["N1"].width, 0.8 * die_contact_w)
-    HT, device_ports = qu.add_hyptap_to_cell(
-        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
-    )
-    DEVICE << HT
-    DEVICE.ports = device_ports.ports
-
-    # routes
-    ROUTES = qu.route_to_dev(HT.get_ports(), SNSPD_NTRON.ports, device_layer)
-    DEVICE << ROUTES
-
-    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
-    DEVICE = pg.union(DEVICE, layer=device_layer)
-    DEVICE.name = f"DIE {text} "
-
-    DIE_SNSPD_NTRON << DEVICE
-    DIE_SNSPD_NTRON << BORDER
-
-    DIE_SNSPD_NTRON = pg.union(DIE_SNSPD_NTRON, by_layer=True)
-    DIE_SNSPD_NTRON.name = f"SNSPD \n{w_snspd} {w_choke} "
-
-    return DIE_SNSPD_NTRON
-
-
-class Design:
-    """A class for a design on a single layer of superconducting material, and
-    additional contact pads.
-
-    It is though for a process like:
-
-    - exposing the superconductiong material using e-beam lithography. Two
-      exposures at low and high currents are possible by distinguishing two
-      layers: device layer and die layer. Equivalently, the shapes outlines
-      (though for positive tone resist) have two different widths for the device
-      and die layers.
-    - exposing the pads layer using photolithography.
-
-    Args:
-        name (str): The name of the design.
-        chip_w (int or float): The overall width of the chip.
-        chip_margin (int or float): The width of the outline of the chip where
-            no device should be placed.
-        N_dies (int): Number of dies/units to be placed by row and column.
-        die_w (int or float, optional): Width of a unit die/cell in the design
-            (the output device will be an integer number of unit cells).
-        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-        device_outline (int or float): The width of the device's outline.
-        die_outline (int or float): The width of the pads outline.
-        ebeam_overlap (int or float): Extra length of the routes above the die's
-            ports to assure alignment with the device (useful for ebeam
-            lithography).
-        annotation_layer (int): The layer where to put the annotations.
-        device_layer (int or array-like[2]): The layer where the device is placed.
-        die_layer (int or array-like[2]): The layer where the die is placed.
-        pad_layer (int or array-like[2]): The layer where the pads are placed.
-
-    Example:
-        Here is an example of how to create the class.
-
-        >>> # Choose some design parameters, let the others to default
-        >>> chip_w = 10000
-        >>> N_dies = 11
-        >>> device_outline = 0.3
-        >>> die_outline = 10
-
-        >>> # Create the design and initialize the chip
-        >>> demo_project = Design(name="demo design",
-        >>>                       chip_w=chip_w,
-        >>>                       N_dies=N_dies,
-        >>>                       device_outline=device_outline,
-        >>>                       die_outline=die_outline)
-        >>> demo_project.create_chip()
-
-        >>> # Quickplot the chip skeletton!
-        >>> qp(demo_project.CHIP)
-    """
-
-    def __init__(
-        self,
-        name="new_design",
-        chip_w=dflt_chip_w,
-        chip_margin=dflt_chip_margin,
-        N_dies=dflt_N_dies,
-        die_w=auto_param,
-        pad_size=dflt_pad_size,
-        device_outline=dflt_device_outline,
-        die_outline=dflt_die_outline,
-        ebeam_overlap=dflt_ebeam_overlap,
-        annotation_layer=dflt_layers["annotation"],
-        device_layer=dflt_layers["device"],
-        die_layer=dflt_layers["die"],
-        pad_layer=dflt_layers["pad"],
-    ):
-        """
-        Args:
-            name (str): The name of the design.
-            chip_w (int or float): The overall width of the chip.
-            chip_margin (int or float): The width of the outline of the chip where no device should be placed.
-            N_dies (int): Number of dies/units to be placed by row and column.
-            die_w (int or float, optional): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
-            pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
-            device_outline (int or float): The width of the device's outline.
-            die_outline (int or float): The width of the pads outline.
-            ebeam_overlap (int or float): Extra length of the routes above the die's ports to assure alignment with the device (useful for ebeam lithography).
-            annotation_layer (int): The layer where to put the annotations.
-            device_layer (int or array-like[2]): The layer where the device is placed.
-            die_layer (int or array-like[2]): The layer where the die is placed.
-            pad_layer (int or array-like[2]): The layer where the pads are placed.
-        """
-
-        self.name = name
-
-        self.chip_w = chip_w
-        self.chip_margin = chip_margin
-        self.N_dies = N_dies
-        self.die_w = die_w
-
-        self.pad_size = pad_size
-        self.device_outline = device_outline
-        self.die_outline = die_outline
-        self.ebeam_overlap = ebeam_overlap
-
-        self.layers = {
-            "annotation": annotation_layer,
-            "device": device_layer,
-            "die": die_layer,
-            "pad": pad_layer,
-        }
-
-    # help building a design
-
-    def create_chip(self, create_devices_map_txt: Union[bool, str] = True) -> Device:
-        """Creates the chip, with unit cells.
-
-        The CHIP created will be the foundation of the design, the Device to add
-        all references to. The function creates a chip_map (2D array) to help placing
-        the cells on the chip (aligned with the unit cells). The function also generates
-        a txt file if create_devices_map_txt is True to follow the devices placements
-        on the chip.
-
-        Parameters:
-            create_devices_map_txt (bool or str): If True, generates a text file
-                to follow the devices placements on the chip. If string, the text file
-                is named after the string.
-
-        Returns:
-            CHIP (Device): The chip map, in the annotations layer
-        """
-        if create_devices_map_txt:
-            if create_devices_map_txt == True:
-                create_devices_map_txt = f"{self.name} devices map"
-            else:
-                create_devices_map_txt = f"{create_devices_map_txt}"
-            self.CHIP, N_or_w, self.chip_map, self.devices_map_txt = create_chip(
-                chip_w=self.chip_w,
-                margin=self.chip_margin,
-                N_dies=self.N_dies,
-                die_w=self.die_w,
-                annotations_layer=self.layers["annotation"],
-                unpack_chip_map=True,
-                create_devices_map_txt=create_devices_map_txt,
-            )
-        else:
-            self.devices_map_txt = None
-            create_devices_map_txt = False
-            self.CHIP, N_or_w, self.chip_map = create_chip(
-                chip_w=self.chip_w,
-                margin=self.chip_margin,
-                N_dies=self.N_dies,
-                die_w=self.die_w,
-                annotations_layer=self.layers["annotation"],
-                unpack_chip_map=True,
-                create_devices_map_txt=create_devices_map_txt,
-            )
-
-        if self.die_w is not None:
-            self.N_dies = N_or_w
-        else:
-            self.die_w = N_or_w
-
-        return self.CHIP
-
-    def place_on_chip(
-        self, cell: Device, coordinates: Tuple[int, int], add_to_chip: bool = True
-    ) -> bool:
-        """Moves the chip to the coordinates specified. Update the chip map
-        with Occupied states where the device has been placed.
-
-        NB: the cell is aligned from its bottom left corner to the coordinates.
-
-        Parameters:
-            cell (Device): Device to be moved.
-            coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
-                Note that the indices start at 0.
-
-        Returns:
-            bool: False, if the Device falls out of the chip map, prints an error message and does not place the device. True, otherwise.
-
-        Raises:
-            Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
-
-        Examples:
-            Here is an example of placing alignment cells on two given positions of the chip.
-
-            >>> align_left  = demo_project.create_alignment_cell(layers_to_align=[2, 3])
-            >>> align_right = demo_project.create_alignment_cell(layers_to_align=[2, 3])
-            >>> demo_project.place_on_chip(cell=align_left,  coordinates=(0, 5))
-            >>> demo_project.place_on_chip(cell=align_right, coordinates=(10, 5))
-        """
-
-        if add_to_chip:
-            self.CHIP << cell
-        return place_on_chip(
-            cell=cell,
-            coordinates=coordinates,
-            chip_map=self.chip_map,
-            die_w=self.die_w,
-            devices_map_txt=self.devices_map_txt,
-        )
-
-    def place_remaining_devices(
-        self,
-        devices_to_place: List[Device],
-        add_to_chip: bool = True,
-        write_remaining_devices_map_txt: Union[bool, str] = False,
-    ) -> Optional[None]:
-        """Go through the chip map and place the devices given, where the chip
-        map is Free.
-
-        Parameters:
-            devices_to_place (list of Device objects): The devices to be placed.
-            add_to_chip (bool): Add the devices provided to the Design's CHIP.
-            write_remaining_devices_map_txt (bool or string): If True, write a .txt
-                file mapping the devices that were placed. If string, the filename is
-                the given string, except if a file has already been created.
-
-        Note:
-            The list of devices is not re-ordered to fit as many of them as possible.
-            Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
-
-        Examples:
-            Here is a typical example of why this function is useful and how to
-            use it. If design is a Design class initalized, and the
-            create_chip() function has previously been executed.
-
-            >>> channels_w = [0.5, 0.75, 1, 1.25, 1.5]
-            >>> ntrons_to_place = []
-            >>> for channel_w in channels_w:
-            >>>     ntron = design.create_ntron_cell(choke_w=0.05, channel_w=channel_w)
-            >>>     ntrons_to_place.append(ntron)
-            >>> design.place_remaining_cells(ntrons_to_place)
-        """
-        if self.devices_map_txt is not None:
-            # the decision taken when creating the chip overwrites this one
-            write_devices_map_txt = self.devices_map_txt
-        else:
-            # a devices map can still be created, as decided when calling this function
-            write_devices_map_txt = write_remaining_devices_map_txt
-
-        if add_to_chip:
-            self.CHIP << devices_to_place
-        place_remaining_devices(
-            devices_to_place=devices_to_place,
-            chip_map=self.chip_map,
-            die_w=self.die_w,
-            write_devices_map_txt=write_devices_map_txt,
-        )
-
-    def write_gds(self, text: Union[None, str] = dflt_text) -> Union[None, str]:
-        """Write a GDS file.
-
-        Args:
-            text (str or None): The filename for the GDS file.
-                If None, the name of the Design will be used.
-
-        Returns:
-            str or None: The filename of the written GDS file, or None if no file was written.
-        """
-        if text is None:
-            text = self.name
-        return self.CHIP.write_gds(filename=f"{text}.gds")
-
-    # basics:
-
-    def create_alignment_cell(
-        self, layers_to_align: List[int], text: Union[None, str] = dflt_text
-    ) -> Device:
-        """Creates alignment marks in an integer number of unit cells.
-
-        Parameters:
-            layers_to_align (List[int]): Layers to align.
-            text (str): The text of the cell is f"ALIGN {text}".
-
-        Returns:
-            Device: A device that centers the alignment marks in an n*m unit cell.
-        """
-        return create_alignment_cell(
-            die_w=self.die_w,
-            layers_to_align=layers_to_align,
-            outline_die=self.die_outline,
-            die_layer=self.layers["die"],
-            text=text,
-        )
-
-    def create_vdp_cell(
-        self,
-        layers_to_probe: List[int],
-        layers_to_outline: Union[List[int], None] = auto_param,
-        text: Union[None, str] = dflt_text,
-    ) -> Device:
-        r"""Creates a cell containing a Van Der Pauw structure between 4 contact
-        pads.
-
-        Parameters:
-            layers_to_probe (List[int]): The layers on which to place the VDP structure.
-            layers_to_outline (List[int]): Among the VDP layers, the ones for which structure must not be filled but outlined.
-            text (str, optional): If None, the text is f"VDP \n{layers_to_probe}". Otherwise, f"VDP \n{text}".
-
-        Returns:
-            Device: The created device.
-        """
-
-        return create_vdp_cell(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            layers_to_probe=layers_to_probe,
-            layers_to_outline=layers_to_outline,
-            outline=self.die_outline,
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-        )
-
-    def create_etch_test_cell(
-        self, layers_to_etch: List[List[int]], text: Union[None, str] = dflt_text
-    ) -> Device:
-        """Creates etch test structures in an integer number of unit cells.
-
-        These test structures are thought to be used by probing on pads (with a simple multimeter)
-        that should be isolated one from another if the etching is complete.
-
-        Parameters:
-            layers_to_etch (List[List[int]]): Each element of the list corresponds to one test point,
-                to put on the list of layers specified. Example: [[1, 2], [1], [2]].
-            text (str, optional): If None, the cell text is f"ETCH TEST {layers_to_etch}".
-
-        Returns:
-            Device: A device (with size n*m of unit cells) with etch tests in its center.
-        """
-
-        return create_etch_test_cell(
-            die_w=self.die_w,
-            layers_to_etch=layers_to_etch,
-            outline_die=self.die_outline,
-            die_layer=self.layers["die"],
-            text=text,
-        )
-
-    def create_resolution_test_cell(
-        self,
-        layer_to_resolve: int,
-        resolutions_to_test: List[float] = [
-            0.025,
-            0.05,
-            0.075,
-            0.1,
-            0.25,
-            0.5,
-            1,
-            1.5,
-            2,
-        ],
-        text: Union[None, str] = dflt_text,
-    ) -> Device:
-        r"""Creates a cell containing a resolution test.
-
-        Parameters:
-            layer_to_resolve (int): The layer to put the resolution test on.
-            resolutions_to_test (List[float]): The resolutions to test in µm.
-            text (str, optional): If None, the text is f"RES TEST \n{layer_to_resolve}".
-
-        Returns:
-            Device: The created device.
-        """
-
-        return create_resolution_test_cell(
-            die_w=self.die_w,
-            layer_to_resolve=layer_to_resolve,
-            resolutions_to_test=resolutions_to_test,
-            outline=self.die_outline,
-            die_layer=self.layers["die"],
-            text=text,
-        )
-
-    # devices:
-
-    def create_nanowires_cell(
-        self,
-        channels_sources_w: List[Tuple[float, float]],
-        text: Union[None, str] = dflt_text,
-    ) -> Device:
-        """Creates a cell containing several nanowires of given channel and
-        source.
-
-        Parameters:
-            channels_sources_w (List[Tuple[float, float]]): The list of
-                (channel_w, source_w) of the nanowires to create.
-            text (str, optional): If None, the text is "NWIRES".
-
-        Returns:
-            Device: A device containing the nanowires, the border of the die
-            (created with die_cell function), and the connections between the
-            nanowires and pads.
-        """
-
-        return create_nanowires_cell(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            channels_sources_w=channels_sources_w,
-            overlap_w=self.ebeam_overlap,
-            outline_die=self.die_outline,
-            outline_dev=self.device_outline,
-            device_layer=self.layers["device"],
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-        )
-
-    def create_ntron_cell(
-        self,
-        choke_w: float,
-        channel_w: float,
-        gate_w: Union[float, None] = auto_param,
-        source_w: Union[float, None] = auto_param,
-        drain_w: Union[float, None] = auto_param,
-        choke_shift: Union[float, None] = auto_param,
-        text: Union[str, None] = dflt_text,
-    ) -> Device:
-        r"""Creates a standardized cell specifically for a single ntron.
-
-        Unless specified, scales the ntron parameters as:
-        gate_w = drain_w = source_w = 3*channel_w
-        choke_shift = -3*channel_w
-
-        Parameters:
-            choke_w (int or float): The width of the ntron's choke in µm.
-            channel_w (int or float): The width of the ntron's channel in µm.
-            gate_w (int or float, optional): If None, gate width is 3 times the channel width.
-            source_w (int or float, optional): If None, source width is 3 times the channel width.
-            drain_w (int or float, optional): If None, drain width is 3 times the channel width.
-            choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
-            text (str, optional): If None, the text is f"chk: {choke_w} /n chnl: {channel_w}".
-
-        Returns:
-            Device: A device containing the ntron, the border of the die (created with die_cell function),
-            and the connections between the ports.
-        """
-
-        return create_ntron_cell(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            choke_w=choke_w,
-            channel_w=channel_w,
-            gate_w=gate_w,
-            source_w=source_w,
-            drain_w=drain_w,
-            choke_shift=choke_shift,
-            overlap_w=self.ebeam_overlap,
-            outline_die=self.die_outline,
-            outline_dev=self.device_outline,
-            device_layer=self.layers["device"],
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-        )
-
-    def create_snspd_ntron_cell(
-        self,
-        w_choke: float,
-        w_snspd: Union[float, None] = auto_param,
-        text: Union[str, None] = dflt_text,
-    ) -> Device:
-        """Creates a cell that contains an SNSPD coupled to an NTRON. The
-        device's parameters are sized according to the SNSPD's width and the
-        NTRON's choke.
-
-        Parameters:
-            w_choke (int or float): The width of the NTRON choke in µm.
-            w_snspd (int or float, optional): The width of the SNSPD nanowire in µm. If None, scaled to 5*w_choke.
-            text (str, optional): If None, text = f'SNSPD {w_choke}'.
-
-        Returns:
-            Device: A cell containing a die in die_layer, pads in pad layer, and an SNSPD-NTRON properly routed in the device layer.
-        """
-
-        return create_snspd_ntron_cell(
-            die_w=self.die_w,
-            pad_size=self.pad_size,
-            w_choke=w_choke,
-            w_snspd=w_snspd,
-            overlap_w=self.ebeam_overlap,
-            outline_die=self.die_outline,
-            outline_dev=self.device_outline,
-            device_layer=self.layers["device"],
-            die_layer=self.layers["die"],
-            pad_layer=self.layers["pad"],
-            text=text,
-        )
+"""Design's module is though for users to be able to access pre-built cells
+that are made of circuits, devices or test structures already integrated in a
+die cell.
+
+It is a module that is sufficient in itself to build an entire new
+design.
+"""
+
+from phidl import Device
+
+# from phidl import quickplot as qp
+# from phidl import set_quickplot_options
+import phidl.geometry as pg
+import phidl.routing as pr
+from typing import Tuple, List, Union, Optional
+import math
+import os
+import qnngds.geometries as qg
+import qnngds.devices as qd
+import qnngds.circuits as qc
+import qnngds.utilities as qu
+
+Free = True
+Occupied = False
+
+auto_param = None
+die_cell_border = 80
+
+# default parameters
+dflt_chip_w = 10000
+dflt_chip_margin = 100
+dflt_N_dies = 11
+dflt_die_w = 980
+dflt_pad_size = (150, 250)
+dflt_device_outline = 0.5
+dflt_die_outline = 10
+dflt_ebeam_overlap = 10
+dflt_layers = {"annotation": 0, "device": 1, "die": 2, "pad": 3}
+dflt_text = auto_param
+
+## to build a design
+
+
+def create_chip(
+    chip_w: Union[int, float] = dflt_chip_w,
+    margin: Union[int, float] = dflt_chip_margin,
+    N_dies: int = dflt_N_dies,
+    die_w: Union[None, int, float] = auto_param,
+    annotations_layer: int = dflt_layers["annotation"],
+    unpack_chip_map: bool = True,
+    create_devices_map_txt: Union[bool, str] = False,
+) -> Union[
+    Tuple[Device, Union[int, float], List[List[bool]], str],
+    Tuple[Device, Union[int, float], str],
+    Tuple[Device, Union[int, float], List[List[bool]]],
+    Tuple[Device, Union[int, float]],
+]:
+    """Creates a chip map in the annotations layer.
+
+    If unpack_chip_map is set to True, creates a map (2D array) to monitor the
+    states of each cell of the chip. The user should input N_dies xor die_w.
+
+    Parameters:
+        chip_w (int or float): The overall width (in um) of the chip.
+        margin (int or float): The width (in um) of the outline of the chip where no device should be placed.
+        N_dies (int): Number of dies/units to be placed by row and column.
+        die_w (None, int, or float): If specified, the width of each die/unit to be placed by row and column.
+        annotations_layer (int or array-like[2]): The layer where to put the device.
+        unpack_chip_map (bool): If True, the function returns a map (2D array) of states to be filled later (e.g., with place_on_chip()).
+        create_devices_map_txt (bool or string): If True or string, the function creates a txt file that will map the devices.
+
+    Returns:
+        Tuple[Device, float, List[List[bool]], str]: A tuple containing from 2 to 4 elements, depending on what needs to be extracted (parameters dependent):
+
+        - **CHIP** (*Device*): The chip map.
+        - **die_w** (*float*): The width of each die. (returned if die_w was None)
+        - **N_dies** (*float*): The number of dies/units on each row and column. (returned if die_w was not None)
+        - **chip_map** (*array-like[N_dies][N_dies] of bool*): A 2D array filled with "Free" (=True) states. (returned if unpack_chip_map is True)
+        - **file_name** (*str*): The name of the created devices map text file. (returned if create_devices_map_txt is not False)
+    """
+
+    CHIP = Device("CHIP ")
+    CHIP.add_polygon(
+        [(0, 0), (chip_w, 0), (chip_w, chip_w), (0, chip_w)], layer=annotations_layer
+    )
+
+    useful_w = chip_w - margin * 2
+    useful_area = CHIP.add_polygon(
+        [(0, 0), (useful_w, 0), (useful_w, useful_w), (0, useful_w)],
+        layer=annotations_layer,
+    )
+    useful_area.move((margin, margin))
+
+    if die_w is not None:
+        N_dies = useful_w / die_w
+        return_N_or_w = N_dies
+    else:
+        die_w = useful_w / N_dies
+        return_N_or_w = die_w
+    CELL = pg.rectangle([die_w, die_w], layer=annotations_layer)
+    array = CHIP.add_array(CELL, columns=N_dies, rows=N_dies, spacing=(die_w, die_w))
+    array.move((0, 0), (margin, margin))
+
+    CHIP.flatten()
+    CHIP.move((margin, margin), (0, 0))
+
+    if create_devices_map_txt:
+        ## create a devices map ...
+        if create_devices_map_txt == True:
+            file_name = "devices map"
+        else:
+            file_name = f"{create_devices_map_txt}"
+
+        # check that file does not already exist, in which case it will add a int to its name:
+        i = 0
+        file_to_find = file_name
+        while True:
+            if i != 0:
+                file_to_find = file_name + f"({i})"
+            file_already_exists = os.path.exists(f"{file_to_find}.txt")
+            i += 1
+            if not file_already_exists:
+                file_name = file_to_find
+                break
+        with open(f"{file_name}.txt", "a") as file:
+            file.write("Devices placed on the chip: \n\n")
+            file.write("(row, col) : device.name\n\n")
+
+        ## ... and return the devices map filename in the outputs
+        if unpack_chip_map:
+            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
+            return CHIP, return_N_or_w, chip_map, file_name
+        else:
+            return CHIP, return_N_or_w, file_name
+    else:
+        if unpack_chip_map:
+            chip_map = [[Free for _ in range(N_dies)] for _ in range(N_dies)]
+            return CHIP, return_N_or_w, chip_map
+        else:
+            return CHIP, return_N_or_w
+
+
+def place_on_chip(
+    cell: Device,
+    coordinates: Tuple[int, int],
+    chip_map: List[List[bool]],
+    die_w: Union[int, float],
+    devices_map_txt: Union[None, str] = None,
+) -> bool:
+    """Moves the chip to the coordinates specified.
+
+    Update the chip map with Occupied states where the device has been placed.
+
+    NB: The cell is aligned from its bottom left corner to the coordinates.
+
+    Parameters:
+        cell (Device): Device to be moved.
+        coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
+            Note that the indices start at 0.
+        chip_map (2D array): The 2D array mapping the free cells in the chip map.
+        die_w (int or float): The width of a die/unit in the chip map.
+        devices_map_txt (str or None): Name of the devices map text file to write placement information.
+            If None, no file will be written.
+
+    Returns:
+        bool: False, if the Device falls out of the chip map, prints an error
+        message and does not place the device. True, otherwise.
+
+    Raises:
+        Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
+    """
+
+    # update the chip's availabilities
+    n_cell = round(cell.xsize / die_w)
+    m_cell = round(cell.ysize / die_w)
+    for n in range(n_cell):
+        for m in range(m_cell):
+            try:
+                if chip_map[coordinates[1] + m][coordinates[0] + n] == Occupied:
+                    print(
+                        f"Warning, placing Device {cell.name} "
+                        + f"in an occupied state ({coordinates[1]+m}, {coordinates[0]+n})"
+                    )
+                else:
+                    chip_map[coordinates[1] + m][coordinates[0] + n] = Occupied
+            except IndexError:
+                print(
+                    f"Error, Device {cell.name} "
+                    + f"falls out of the chip map ({coordinates[1]+m}, {coordinates[0]+n})"
+                )
+                return False
+
+    # move the cell
+    cell_bottom_left = cell.get_bounding_box()[0]
+    cell.move(cell_bottom_left, (coordinates[0] * die_w, coordinates[1] * die_w))
+
+    # write the cell's place on the devices map text file
+    if devices_map_txt is not None:
+        with open(f"{devices_map_txt}.txt", "a") as file:
+            try:
+                name = cell.name.replace("\n", "")
+            except AttributeError:
+                name = "unnamed"
+            file.write(f"({coordinates[0]}, {coordinates[1]}) : {name}\n")
+
+    return True
+
+
+def place_remaining_devices(
+    devices_to_place: List[Device],
+    chip_map: List[List[bool]],
+    die_w: Union[int, float],
+    write_devices_map_txt: Union[bool, str] = False,
+) -> Optional[None]:
+    """Go through the chip map and place the devices given, where the chip map
+    is Free.
+
+    Parameters:
+        devices_to_place (list of Device objects): The devices to be placed.
+        chip_map (2D array): The 2D array mapping the free cells in the chip map.
+        die_w (int or float): The width of a die/unit in the chip map.
+        write_devices_map_txt (bool or str): If True, write a .txt file mapping the devices that were placed.
+            If str, specifies the filename of the .txt file.
+
+    Note:
+        The list of devices is not re-ordered to fit as many of them as possible.
+        Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
+    """
+
+    # name and create the file if no file was given
+    if write_devices_map_txt == True:
+
+        file_name = "remaining_cells_map"
+        with open(f"{file_name}.txt", "a") as file:
+            file.write("Remaining devices placed on the chip:\n\n")
+            file.write("(row, col) : device.name\n\n")
+    # use the file's name is a file was given
+    elif write_devices_map_txt:
+        file_name = write_devices_map_txt
+    # pass false if no txt file should be created
+    else:
+        file_name = None
+
+    for row_i, row in enumerate(chip_map):
+        for col_i, status in enumerate(row):
+            if status == Free and devices_to_place:
+                if place_on_chip(
+                    devices_to_place[0], (col_i, row_i), chip_map, die_w, file_name
+                ):
+                    devices_to_place.pop(0)
+
+    if devices_to_place:
+        print(
+            "Some devices are still to be placed, " + "no place remaining on the chip."
+        )
+
+
+## basics:
+
+
+def create_alignment_cell(
+    die_w: Union[int, float] = dflt_die_w,
+    layers_to_align: List[int] = [dflt_layers["die"], dflt_layers["pad"]],
+    outline_die: Union[int, float] = dflt_die_outline,
+    die_layer: int = dflt_layers["die"],
+    text: Union[None, str] = dflt_text,
+) -> Device:
+    """Creates alignment marks in an integer number of unit cells.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        layers_to_align (list of int): Layers to align.
+        outline_die (int or float): The width of the die's outline.
+        die_layer (int): The layer where the die is placed.
+        text (str): Text to be displayed.
+
+    Returns:
+        DIE_ALIGN (Device): A device that centers the alignment marks in an n*m unit cell.
+    """
+
+    if text is None:
+        text = ""
+    DIE = Device(f"DIE ALIGN {text} ")
+
+    ALIGN = qg.alignment_mark(layers_to_align)
+
+    n = math.ceil((ALIGN.xsize) / die_w)
+    m = math.ceil((ALIGN.ysize) / die_w)
+
+    BORDER = qu.die_cell(
+        die_size=(n * die_w, m * die_w),
+        device_max_size=(ALIGN.xsize + 20, ALIGN.ysize + 20),
+        ports={},
+        ports_gnd={},
+        isolation=outline_die,
+        text=f"ALIGN {text}",
+        layer=die_layer,
+        invert=True,
+    )
+
+    DIE << BORDER.flatten()
+    DIE << ALIGN
+
+    return DIE
+
+
+def create_vdp_cell(
+    die_w: Union[int, float] = dflt_die_w,
+    pad_size: Tuple[float] = dflt_pad_size,
+    layers_to_probe: List[int] = [dflt_layers["pad"]],
+    layers_to_outline: Union[None, List[int]] = auto_param,
+    outline: Union[int, float] = dflt_die_outline,
+    die_layer: Union[int, float] = dflt_layers["die"],
+    pad_layer: int = dflt_layers["pad"],
+    text: Union[None, str] = dflt_text,
+) -> Device:
+    r"""Creates a cell containing a Van Der Pauw structure between 4 contact
+    pads.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        layers_to_probe (list of int): The layers on which to place the VDP structure.
+        layers_to_outline (list of int): Among the VDP layers, the ones for which structure must not be filled but outlined.
+        outline (int or float): The width of the VDP and die's outline.
+        die_layer (int or tuple of int): The layer where the die is placed.
+        pad_layer (int or tuple of int): The layer where the pads are placed.
+        text (str, optional): If None, the text is f"VDP \n{layers_to_probe}".
+
+    Returns:
+        DIE_VANDP (Device): The created device.
+    """
+
+    if text is None:
+        text = layers_to_probe
+    DIE_VANDP = Device(f"DIE VAN DER PAUW {text} ")
+
+    ## Create the die
+    w = die_w - 2 * (pad_size[1] + 2 * outline)  # width of max device size
+    BORDER = qu.die_cell(
+        die_size=(die_w, die_w),
+        device_max_size=(w, w),
+        pad_size=pad_size,
+        contact_w=pad_size[0],
+        contact_l=0,
+        ports={"N": 1, "E": 1, "W": 1, "S": 1},
+        ports_gnd=["N", "E", "W", "S"],
+        text=f"VDP \n{text} ",
+        isolation=outline,
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+    )
+    PADS = pg.deepcopy(BORDER)
+    PADS = PADS.remove_layers([pad_layer], invert_selection=True)
+
+    DIE_VANDP << BORDER.flatten()
+
+    ## Create the test structure
+    DEVICE = Device()
+
+    # the test structure is an hexagonal shape between the die's ports
+    TEST = Device()
+    TEST << PADS
+    rect = TEST << pg.straight((PADS.ports["E1"].x - PADS.ports["W1"].x, pad_size[0]))
+    rect.move(rect.center, (0, 0))
+    TEST << pr.route_quad(PADS.ports["N1"], rect.ports[1])
+    TEST << pr.route_quad(PADS.ports["S1"], rect.ports[2])
+    TEST = pg.union(TEST)
+
+    # outline the test structure for layers that need to be outlined
+
+    if layers_to_outline is None:
+        layers_to_outline = [die_layer]
+    for layer in layers_to_probe:
+        TEST_LAY = pg.deepcopy(TEST)
+        if layer in layers_to_outline:
+            TEST_LAY = pg.outline(TEST_LAY, outline)
+        DEVICE << TEST_LAY.flatten(single_layer=layer)
+
+    DIE_VANDP << DEVICE
+
+    DIE_VANDP = pg.union(DIE_VANDP, by_layer=True)
+    DIE_VANDP.name = f"DIE VAN DER PAUW {text} "
+    return DIE_VANDP
+
+
+def create_etch_test_cell(
+    die_w: Union[int, float] = dflt_die_w,
+    layers_to_etch: List[List[int]] = [[dflt_layers["pad"]]],
+    outline_die: Union[int, float] = dflt_die_outline,
+    die_layer: int = dflt_layers["die"],
+    text: Union[None, str] = dflt_text,
+) -> Device:
+    """Creates etch test structures in an integer number of unit cells.
+
+    These test structures are thought to be used by probing on pads (with a
+    simple multimeter) that should be isolated one from another if the etching
+    is complete.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        layers_to_etch (list of list of int): Each element of the list corresponds to one test point, to put on the list of layers specified.
+                                               Example: [[1, 2], [1], [2]]
+        outline_die (int or float): The width of the die's outline.
+        die_layer (int): The layer where the die is placed.
+        text (str): Text to be displayed.
+
+    Returns:
+        DIE_ETCH_TEST (Device): A device (with size n*m of unit cells) with etch tests in its center.
+    """
+
+    if text is None:
+        text = f"{layers_to_etch}"
+    DIE_ETCH_TEST = Device(f"DIE ETCH TEST {text} ")
+
+    TEST = Device()
+
+    ## Create the probing areas
+
+    margin = 0.12 * die_w
+    rect = pg.rectangle((die_w - 2 * margin, die_w - 2 * margin))
+    for i, layer_to_etch in enumerate(layers_to_etch):
+        probe = Device()
+        probe.add_array(rect, 2, 1, (die_w, die_w))
+        for layer in layer_to_etch:
+            TEST << pg.outline(probe, -outline_die, layer=layer).movey(i * die_w)
+
+    ## Create the die
+
+    n = math.ceil((TEST.xsize + 2 * die_cell_border) / die_w)
+    m = math.ceil((TEST.ysize + 2 * die_cell_border) / die_w)
+    BORDER = qu.die_cell(
+        die_size=(n * die_w, m * die_w),
+        ports={},
+        ports_gnd={},
+        text=f"ETCH TEST {text}",
+        isolation=10,
+        layer=die_layer,
+        invert=True,
+    )
+
+    BORDER.move(TEST.center)
+    DIE_ETCH_TEST << BORDER.flatten()
+    DIE_ETCH_TEST << TEST
+    DIE_ETCH_TEST.move(DIE_ETCH_TEST.center, (0, 0))
+
+    return DIE_ETCH_TEST
+
+
+def create_resolution_test_cell(
+    die_w: Union[int, float] = dflt_die_w,
+    layer_to_resolve: int = dflt_layers["device"],
+    resolutions_to_test: List[float] = [
+        0.025,
+        0.05,
+        0.075,
+        0.1,
+        0.25,
+        0.5,
+        1,
+        1.5,
+        2.0,
+    ],
+    outline: Union[int, float] = dflt_die_outline,
+    die_layer: int = dflt_layers["die"],
+    text: Union[None, str] = dflt_text,
+) -> Device:
+    r"""Creates a cell containing a resolution test.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        layer_to_resolve (int): The layer to put the resolution test on.
+        resolutions_to_test (list of float): The resolutions to test in µm.
+        outline (int or float): The width of the VDP and die's outline.
+        die_layer (int or tuple of int): The layer where the die is placed.
+        text (str, optional): If None, the text is f"RES TEST \n{layer_to_resolve}".
+
+    Returns:
+        DIE_RES_TEST (Device): The created device.
+    """
+
+    if text is None:
+        text = layer_to_resolve
+    DIE_RES_TEST = Device(f"DIE RESOLUTION TEST {text} ")
+
+    ## Create the test structure
+    TEST_RES = Device(f"RESOLUTION TEST {text} ")
+    test_res = TEST_RES << qg.resolution_test(
+        resolutions=resolutions_to_test, inverted=False, layer=layer_to_resolve
+    )
+    test_res_invert = TEST_RES << qg.resolution_test(
+        resolutions=resolutions_to_test,
+        inverted=resolutions_to_test[-1],
+        layer=layer_to_resolve,
+    )
+    test_res_invert.movey(
+        test_res_invert.ymin, test_res.ymax + 5 * resolutions_to_test[-1]
+    )
+
+    DIE_RES_TEST << TEST_RES.move(TEST_RES.center, (0, 0))
+
+    ## Create the die
+    n = math.ceil((TEST_RES.xsize) / die_w)
+    m = math.ceil((TEST_RES.ysize) / die_w)
+    BORDER = qu.die_cell(
+        die_size=(n * die_w, m * die_w),
+        ports={},
+        ports_gnd=[],
+        text=f"RES TEST \n{text} ",
+        isolation=outline,
+        layer=die_layer,
+        invert=True,
+    )
+
+    DIE_RES_TEST << BORDER.flatten()
+
+    return DIE_RES_TEST
+
+
+## devices:
+
+
+def create_nanowires_cell(
+    die_w: Union[int, float] = dflt_die_w,
+    pad_size: Tuple[float] = dflt_pad_size,
+    channels_sources_w: List[Tuple[float, float]] = [(0.1, 1), (0.5, 3), (1, 10)],
+    overlap_w: Union[int, float] = dflt_ebeam_overlap,
+    outline_die: Union[int, float] = dflt_die_outline,
+    outline_dev: Union[int, float] = dflt_device_outline,
+    device_layer: int = dflt_layers["device"],
+    die_layer: int = dflt_layers["die"],
+    pad_layer: int = dflt_layers["pad"],
+    text: Union[None, str] = dflt_text,
+) -> Device:
+    """Creates a cell that contains several nanowires of given channel and
+    source.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        channels_sources_w (list of tuple of float): The list of (channel_w, source_w) of the nanowires to create.
+        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
+                                   (useful for ebeam lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or tuple of int): The layer where the device is placed.
+        die_layer (int or tuple of int): The layer where the die is placed.
+        pad_layer (int or tuple of int): The layer where the pads are placed.
+        text (str, optional): If None, the text is "NWIRES".
+
+    Returns:
+        Device: A device (of size n*m unit cells) containing the nanowires, the
+        border of the die (created with die_cell function), and the connections
+        between the nanowires and pads.
+    """
+
+    if text is None:
+        text = ""
+
+    NANOWIRES_DIE = Device(f"DIE NWIRES {text} ")
+
+    DEVICE = Device(f"NWIRES {text} ")
+
+    ## Create the NANOWIRES
+
+    NANOWIRES = Device()
+    nanowires_ref = []
+    for i, channel_source_w in enumerate(channels_sources_w):
+        nanowire_ref = NANOWIRES << qd.nanowire(
+            channel_source_w[0], channel_source_w[1]
+        )
+        nanowires_ref.append(nanowire_ref)
+    DEVICE << NANOWIRES
+
+    ## Create the DIE
+
+    # die parameters, checkup conditions
+    n = len(channels_sources_w)
+    die_size = (math.ceil((2 * (n + 1) * pad_size[0]) / die_w) * die_w, die_w)
+    die_contact_w = NANOWIRES.xsize + overlap_w
+    dev_contact_w = NANOWIRES.xsize
+    routes_margin = 4 * die_contact_w
+    dev_max_size = (2 * n * pad_size[0], NANOWIRES.ysize + routes_margin)
+
+    # die, with calculated parameters
+    BORDER = qu.die_cell(
+        die_size=die_size,
+        device_max_size=dev_max_size,
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": n, "S": n},
+        ports_gnd=["S"],
+        isolation=outline_die,
+        text=f"NWIRES {text}",
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+    )
+
+    ## Place the nanowires
+
+    for i, nanowire_ref in enumerate(nanowires_ref):
+        nanowire_ref.movex(BORDER.ports[f"N{i+1}"].x)
+        NANOWIRES.add_port(port=nanowire_ref.ports[1], name=f"N{i+1}")
+        NANOWIRES.add_port(port=nanowire_ref.ports[2], name=f"S{i+1}")
+
+    ## Route the nanowires and the die
+
+    # hyper tapers
+    HT, dev_ports = qu.add_hyptap_to_cell(BORDER.get_ports(), overlap_w, dev_contact_w)
+    DEVICE.ports = dev_ports.ports
+    DEVICE << HT
+
+    # routes from nanowires to hyper tapers
+    ROUTES = qu.route_to_dev(HT.get_ports(), NANOWIRES.ports)
+    DEVICE << ROUTES
+
+    DEVICE.ports = dev_ports.ports
+    DEVICE = pg.outline(DEVICE, outline_dev, open_ports=2 * outline_dev)
+    DEVICE = pg.union(DEVICE, layer=device_layer)
+    DEVICE.name = f"NWIRES {text} "
+
+    NANOWIRES_DIE << DEVICE
+    NANOWIRES_DIE << BORDER
+
+    NANOWIRES_DIE = pg.union(NANOWIRES_DIE, by_layer=True)
+    NANOWIRES_DIE.name = f"DIE NWIRES {text} "
+    return NANOWIRES_DIE
+
+
+def create_ntron_cell(
+    die_w: Union[int, float] = dflt_die_w,
+    pad_size: Tuple[float, float] = dflt_pad_size,
+    choke_w: Union[int, float] = 0.1,
+    channel_w: Union[int, float] = 0.5,
+    gate_w: Union[None, int, float] = auto_param,
+    source_w: Union[None, int, float] = auto_param,
+    drain_w: Union[None, int, float] = auto_param,
+    choke_shift: Union[None, int, float] = auto_param,
+    overlap_w: Union[None, int, float] = dflt_ebeam_overlap,
+    outline_die: Union[None, int, float] = dflt_die_outline,
+    outline_dev: Union[None, int, float] = dflt_device_outline,
+    device_layer: int = dflt_layers["device"],
+    die_layer: int = dflt_layers["die"],
+    pad_layer: int = dflt_layers["pad"],
+    text: Union[None, str] = dflt_text,
+) -> Device:
+    """Creates a standardized cell specifically for a single ntron.
+
+    Unless specified, scales the ntron parameters as:
+    gate_w = drain_w = source_w = 3 * channel_w
+    choke_shift = -3 * channel_w
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        choke_w (int or float): The width of the ntron's choke in µm.
+        channel_w (int or float): The width of the ntron's channel in µm.
+        gate_w (int or float, optional): If None, gate width is 3 times the channel width.
+        source_w (int or float, optional): If None, source width is 3 times the channel width.
+        drain_w (int or float, optional): If None, drain width is 3 times the channel width.
+        choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
+        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
+                                             (useful for ebeam lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+        text (string, optional): If None, the text is the ntron's choke and channel widths.
+
+    Returns:
+        Device: A device containing the ntron, the border of the die (created with die_cell function),
+        and the connections between the ports.
+    """
+
+    ## Create the NTRON
+
+    # sizes the ntron parameters that were not given
+    if source_w is None and drain_w is None:
+        drain_w = source_w = 3 * channel_w
+    elif source_w is None:
+        source_w = drain_w
+    else:
+        drain_w = source_w
+    if gate_w is None:
+        gate_w = source_w
+    if choke_shift is None:
+        choke_shift = -3 * channel_w
+
+    NTRON = qd.ntron_compassPorts(
+        choke_w, gate_w, channel_w, source_w, drain_w, choke_shift, device_layer
+    )
+
+    if text is None:
+        text = f"chk: {choke_w} \nchnl: {channel_w}"
+    DIE_NTRON = Device(f"DIE NTRON {text} ")
+
+    DEVICE = Device(f"NTRON {text} ")
+    DEVICE << NTRON
+
+    ## Create the DIE
+
+    # die parameters, checkup conditions
+    die_contact_w = NTRON.ports["N1"].width + overlap_w
+    routes_margin = 2 * die_contact_w
+    dev_min_w = (
+        die_contact_w + 3 * outline_die
+    )  # condition imposed by the die parameters (contacts width)
+    device_max_w = max(2 * routes_margin + max(NTRON.size), dev_min_w)
+
+    # the die with calculated parameters
+    BORDER = qu.die_cell(
+        die_size=(die_w, die_w),
+        device_max_size=(device_max_w, device_max_w),
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": 1, "W": 1, "S": 1},
+        ports_gnd=["S"],
+        text=text,
+        isolation=10,
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+    )
+
+    # place the ntron
+    NTRON.movex(NTRON.ports["N1"].midpoint[0], BORDER.ports["N1"].midpoint[0])
+
+    # Route DIE and NTRON
+
+    # hyper tapers
+    dev_contact_w = NTRON.ports["N1"].width
+    HT, device_ports = qu.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
+    )
+    DEVICE << HT
+    DEVICE.ports = device_ports.ports
+    # routes
+    ROUTES = qu.route_to_dev(HT.get_ports(), NTRON.ports, device_layer)
+    DEVICE << ROUTES
+
+    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
+    DEVICE = pg.union(DEVICE, layer=device_layer)
+    DEVICE.name = f"NTRON {text} "
+
+    DIE_NTRON << DEVICE
+    DIE_NTRON << BORDER
+
+    DIE_NTRON = pg.union(DIE_NTRON, by_layer=True)
+    DIE_NTRON.name = f"DIE NTRON {text} "
+    return DIE_NTRON
+
+
+def create_snspd_ntron_cell(
+    die_w: Union[int, float] = dflt_die_w,
+    pad_size: Tuple[float, float] = dflt_pad_size,
+    w_choke: Union[int, float] = 0.1,
+    w_snspd: Union[int, float] = auto_param,
+    overlap_w: Union[int, float] = dflt_ebeam_overlap,
+    outline_die: Union[int, float] = dflt_die_outline,
+    outline_dev: Union[int, float] = dflt_device_outline,
+    device_layer: int = dflt_layers["device"],
+    die_layer: int = dflt_layers["die"],
+    pad_layer: int = dflt_layers["pad"],
+    text: Union[None, str] = dflt_text,
+) -> Device:
+    """Creates a cell that contains an SNSPD coupled to an NTRON. The device's
+    parameters are sized according to the SNSPD's width and the NTRON's choke.
+
+    Parameters:
+        die_w (int or float): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        w_choke (int or float): The width of the NTRON choke in µm.
+        w_snspd (int or float, optional): The width of the SNSPD nanowire in µm (if None, scaled to 5 * w_choke).
+        overlap_w (int or float): Extra length of the routes above the die's ports to assure alignment with the device
+                                             (useful for ebeam lithography).
+        outline_die (int or float): The width of the pads outline.
+        outline_dev (int or float): The width of the device's outline.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+        text (string, optional): If None, text = f'SNSPD {w_choke}'.
+
+    Returns:
+        Device: A cell containing a die in die_layer, pads in pad layer,
+        and an SNSPD-NTRON properly routed in the device layer.
+    """
+
+    # Create SNSPD-NTRON
+    if w_snspd is None:
+        w_snspd = 5 * w_choke
+
+    if text is None:
+        text = f"SNSPD \n{w_snspd} {w_choke} "
+    DIE_SNSPD_NTRON = Device(f"DIE {text} ")
+    DEVICE = Device(f"{text} ")
+
+    SNSPD_NTRON = qc.snspd_ntron(
+        w_snspd=w_snspd,
+        pitch_snspd=3 * w_snspd,
+        size_snspd=(30 * w_snspd, 30 * w_snspd),
+        w_inductor=3 * w_snspd,
+        pitch_inductor=6 * w_snspd,
+        k_inductor13=20 * w_snspd,
+        k_inductor2=8 * w_snspd,
+        w_choke=w_choke,
+        w_channel=6 * w_choke,
+        w_pad=10 * w_snspd,
+        layer=device_layer,
+    )
+    DEVICE << SNSPD_NTRON
+
+    # Create DIE
+
+    die_contact_w = min(
+        10 * SNSPD_NTRON.ports["N1"].width + overlap_w, 0.5 * pad_size[0]
+    )
+
+    routes_margin = 2 * die_contact_w
+    margin = 2 * (pad_size[1] + outline_die + routes_margin)
+    n = max(2, math.ceil((SNSPD_NTRON.xsize + margin) / die_w))
+    m = max(1, math.ceil((SNSPD_NTRON.ysize + margin) / die_w))
+
+    dev_min_size = [
+        (die_contact_w + 3 * outline_die) * x for x in (5, 3)
+    ]  # condition imposed by the die parameters (contacts width)
+    device_max_size = (
+        max(
+            min(n * die_w - margin, 8 * routes_margin + SNSPD_NTRON.size[0]),
+            dev_min_size[0],
+        ),
+        max(
+            min(m * die_w - margin, 2 * routes_margin + SNSPD_NTRON.size[1]),
+            dev_min_size[1],
+        ),
+    )
+
+    BORDER = qu.die_cell(
+        die_size=(n * die_w, m * die_w),
+        device_max_size=device_max_size,
+        pad_size=pad_size,
+        contact_w=die_contact_w,
+        contact_l=overlap_w,
+        ports={"N": 3, "E": 1, "W": 1, "S": 2},
+        ports_gnd=["S"],
+        text=text,
+        isolation=outline_die,
+        layer=die_layer,
+        pad_layer=pad_layer,
+        invert=True,
+    )
+
+    # Route DIE and SNSPD-NTRON
+
+    # hyper tapers
+    dev_contact_w = min(4 * SNSPD_NTRON.ports["N1"].width, 0.8 * die_contact_w)
+    HT, device_ports = qu.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w, device_layer
+    )
+    DEVICE << HT
+    DEVICE.ports = device_ports.ports
+
+    # routes
+    ROUTES = qu.route_to_dev(HT.get_ports(), SNSPD_NTRON.ports, device_layer)
+    DEVICE << ROUTES
+
+    DEVICE = pg.outline(DEVICE, outline_dev, precision=0.000001, open_ports=outline_dev)
+    DEVICE = pg.union(DEVICE, layer=device_layer)
+    DEVICE.name = f"DIE {text} "
+
+    DIE_SNSPD_NTRON << DEVICE
+    DIE_SNSPD_NTRON << BORDER
+
+    DIE_SNSPD_NTRON = pg.union(DIE_SNSPD_NTRON, by_layer=True)
+    DIE_SNSPD_NTRON.name = f"SNSPD \n{w_snspd} {w_choke} "
+
+    return DIE_SNSPD_NTRON
+
+
+class Design:
+    """A class for a design on a single layer of superconducting material, and
+    additional contact pads.
+
+    It is though for a process like:
+
+    - exposing the superconductiong material using e-beam lithography. Two
+      exposures at low and high currents are possible by distinguishing two
+      layers: device layer and die layer. Equivalently, the shapes outlines
+      (though for positive tone resist) have two different widths for the device
+      and die layers.
+    - exposing the pads layer using photolithography.
+
+    Args:
+        name (str): The name of the design.
+        chip_w (int or float): The overall width of the chip.
+        chip_margin (int or float): The width of the outline of the chip where
+            no device should be placed.
+        N_dies (int): Number of dies/units to be placed by row and column.
+        die_w (int or float, optional): Width of a unit die/cell in the design
+            (the output device will be an integer number of unit cells).
+        pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+        device_outline (int or float): The width of the device's outline.
+        die_outline (int or float): The width of the pads outline.
+        ebeam_overlap (int or float): Extra length of the routes above the die's
+            ports to assure alignment with the device (useful for ebeam
+            lithography).
+        annotation_layer (int): The layer where to put the annotations.
+        device_layer (int or array-like[2]): The layer where the device is placed.
+        die_layer (int or array-like[2]): The layer where the die is placed.
+        pad_layer (int or array-like[2]): The layer where the pads are placed.
+
+    Example:
+        Here is an example of how to create the class.
+
+        >>> # Choose some design parameters, let the others to default
+        >>> chip_w = 10000
+        >>> N_dies = 11
+        >>> device_outline = 0.3
+        >>> die_outline = 10
+
+        >>> # Create the design and initialize the chip
+        >>> demo_project = Design(name="demo design",
+        >>>                       chip_w=chip_w,
+        >>>                       N_dies=N_dies,
+        >>>                       device_outline=device_outline,
+        >>>                       die_outline=die_outline)
+        >>> demo_project.create_chip()
+
+        >>> # Quickplot the chip skeletton!
+        >>> qp(demo_project.CHIP)
+    """
+
+    def __init__(
+        self,
+        name="new_design",
+        chip_w=dflt_chip_w,
+        chip_margin=dflt_chip_margin,
+        N_dies=dflt_N_dies,
+        die_w=auto_param,
+        pad_size=dflt_pad_size,
+        device_outline=dflt_device_outline,
+        die_outline=dflt_die_outline,
+        ebeam_overlap=dflt_ebeam_overlap,
+        annotation_layer=dflt_layers["annotation"],
+        device_layer=dflt_layers["device"],
+        die_layer=dflt_layers["die"],
+        pad_layer=dflt_layers["pad"],
+    ):
+        """
+        Args:
+            name (str): The name of the design.
+            chip_w (int or float): The overall width of the chip.
+            chip_margin (int or float): The width of the outline of the chip where no device should be placed.
+            N_dies (int): Number of dies/units to be placed by row and column.
+            die_w (int or float, optional): Width of a unit die/cell in the design (the output device will be an integer number of unit cells).
+            pad_size (tuple of int or float): Dimensions of the die's pads (width, height).
+            device_outline (int or float): The width of the device's outline.
+            die_outline (int or float): The width of the pads outline.
+            ebeam_overlap (int or float): Extra length of the routes above the die's ports to assure alignment with the device (useful for ebeam lithography).
+            annotation_layer (int): The layer where to put the annotations.
+            device_layer (int or array-like[2]): The layer where the device is placed.
+            die_layer (int or array-like[2]): The layer where the die is placed.
+            pad_layer (int or array-like[2]): The layer where the pads are placed.
+        """
+
+        self.name = name
+
+        self.chip_w = chip_w
+        self.chip_margin = chip_margin
+        self.N_dies = N_dies
+        self.die_w = die_w
+
+        self.pad_size = pad_size
+        self.device_outline = device_outline
+        self.die_outline = die_outline
+        self.ebeam_overlap = ebeam_overlap
+
+        self.layers = {
+            "annotation": annotation_layer,
+            "device": device_layer,
+            "die": die_layer,
+            "pad": pad_layer,
+        }
+
+    # help building a design
+
+    def create_chip(self, create_devices_map_txt: Union[bool, str] = True) -> Device:
+        """Creates the chip, with unit cells.
+
+        The CHIP created will be the foundation of the design, the Device to add
+        all references to. The function creates a chip_map (2D array) to help placing
+        the cells on the chip (aligned with the unit cells). The function also generates
+        a txt file if create_devices_map_txt is True to follow the devices placements
+        on the chip.
+
+        Parameters:
+            create_devices_map_txt (bool or str): If True, generates a text file
+                to follow the devices placements on the chip. If string, the text file
+                is named after the string.
+
+        Returns:
+            CHIP (Device): The chip map, in the annotations layer
+        """
+        if create_devices_map_txt:
+            if create_devices_map_txt == True:
+                create_devices_map_txt = f"{self.name} devices map"
+            else:
+                create_devices_map_txt = f"{create_devices_map_txt}"
+            self.CHIP, N_or_w, self.chip_map, self.devices_map_txt = create_chip(
+                chip_w=self.chip_w,
+                margin=self.chip_margin,
+                N_dies=self.N_dies,
+                die_w=self.die_w,
+                annotations_layer=self.layers["annotation"],
+                unpack_chip_map=True,
+                create_devices_map_txt=create_devices_map_txt,
+            )
+        else:
+            self.devices_map_txt = None
+            create_devices_map_txt = False
+            self.CHIP, N_or_w, self.chip_map = create_chip(
+                chip_w=self.chip_w,
+                margin=self.chip_margin,
+                N_dies=self.N_dies,
+                die_w=self.die_w,
+                annotations_layer=self.layers["annotation"],
+                unpack_chip_map=True,
+                create_devices_map_txt=create_devices_map_txt,
+            )
+
+        if self.die_w is not None:
+            self.N_dies = N_or_w
+        else:
+            self.die_w = N_or_w
+
+        return self.CHIP
+
+    def place_on_chip(
+        self, cell: Device, coordinates: Tuple[int, int], add_to_chip: bool = True
+    ) -> bool:
+        """Moves the chip to the coordinates specified. Update the chip map
+        with Occupied states where the device has been placed.
+
+        NB: the cell is aligned from its bottom left corner to the coordinates.
+
+        Parameters:
+            cell (Device): Device to be moved.
+            coordinates (tuple of int): (i, j) indices of the chip grid, where to place the cell.
+                Note that the indices start at 0.
+
+        Returns:
+            bool: False, if the Device falls out of the chip map, prints an error message and does not place the device. True, otherwise.
+
+        Raises:
+            Warning: Prints a warning if the Device is overlapping with already occupied coordinates.
+
+        Examples:
+            Here is an example of placing alignment cells on two given positions of the chip.
+
+            >>> align_left  = demo_project.create_alignment_cell(layers_to_align=[2, 3])
+            >>> align_right = demo_project.create_alignment_cell(layers_to_align=[2, 3])
+            >>> demo_project.place_on_chip(cell=align_left,  coordinates=(0, 5))
+            >>> demo_project.place_on_chip(cell=align_right, coordinates=(10, 5))
+        """
+
+        if add_to_chip:
+            self.CHIP << cell
+        return place_on_chip(
+            cell=cell,
+            coordinates=coordinates,
+            chip_map=self.chip_map,
+            die_w=self.die_w,
+            devices_map_txt=self.devices_map_txt,
+        )
+
+    def place_remaining_devices(
+        self,
+        devices_to_place: List[Device],
+        add_to_chip: bool = True,
+        write_remaining_devices_map_txt: Union[bool, str] = False,
+    ) -> Optional[None]:
+        """Go through the chip map and place the devices given, where the chip
+        map is Free.
+
+        Parameters:
+            devices_to_place (list of Device objects): The devices to be placed.
+            add_to_chip (bool): Add the devices provided to the Design's CHIP.
+            write_remaining_devices_map_txt (bool or string): If True, write a .txt
+                file mapping the devices that were placed. If string, the filename is
+                the given string, except if a file has already been created.
+
+        Note:
+            The list of devices is not re-ordered to fit as many of them as possible.
+            Some edges of the chip may remain empty because the list contained 2-units long devices (for e.g.).
+
+        Examples:
+            Here is a typical example of why this function is useful and how to
+            use it. If design is a Design class initalized, and the
+            create_chip() function has previously been executed.
+
+            >>> channels_w = [0.5, 0.75, 1, 1.25, 1.5]
+            >>> ntrons_to_place = []
+            >>> for channel_w in channels_w:
+            >>>     ntron = design.create_ntron_cell(choke_w=0.05, channel_w=channel_w)
+            >>>     ntrons_to_place.append(ntron)
+            >>> design.place_remaining_cells(ntrons_to_place)
+        """
+        if self.devices_map_txt is not None:
+            # the decision taken when creating the chip overwrites this one
+            write_devices_map_txt = self.devices_map_txt
+        else:
+            # a devices map can still be created, as decided when calling this function
+            write_devices_map_txt = write_remaining_devices_map_txt
+
+        if add_to_chip:
+            self.CHIP << devices_to_place
+        place_remaining_devices(
+            devices_to_place=devices_to_place,
+            chip_map=self.chip_map,
+            die_w=self.die_w,
+            write_devices_map_txt=write_devices_map_txt,
+        )
+
+    def write_gds(self, text: Union[None, str] = dflt_text) -> Union[None, str]:
+        """Write a GDS file.
+
+        Args:
+            text (str or None): The filename for the GDS file.
+                If None, the name of the Design will be used.
+
+        Returns:
+            str or None: The filename of the written GDS file, or None if no file was written.
+        """
+        if text is None:
+            text = self.name
+        return self.CHIP.write_gds(filename=f"{text}.gds")
+
+    # basics:
+
+    def create_alignment_cell(
+        self, layers_to_align: List[int], text: Union[None, str] = dflt_text
+    ) -> Device:
+        """Creates alignment marks in an integer number of unit cells.
+
+        Parameters:
+            layers_to_align (List[int]): Layers to align.
+            text (str): The text of the cell is f"ALIGN {text}".
+
+        Returns:
+            Device: A device that centers the alignment marks in an n*m unit cell.
+        """
+        return create_alignment_cell(
+            die_w=self.die_w,
+            layers_to_align=layers_to_align,
+            outline_die=self.die_outline,
+            die_layer=self.layers["die"],
+            text=text,
+        )
+
+    def create_vdp_cell(
+        self,
+        layers_to_probe: List[int],
+        layers_to_outline: Union[List[int], None] = auto_param,
+        text: Union[None, str] = dflt_text,
+    ) -> Device:
+        r"""Creates a cell containing a Van Der Pauw structure between 4 contact
+        pads.
+
+        Parameters:
+            layers_to_probe (List[int]): The layers on which to place the VDP structure.
+            layers_to_outline (List[int]): Among the VDP layers, the ones for which structure must not be filled but outlined.
+            text (str, optional): If None, the text is f"VDP \n{layers_to_probe}". Otherwise, f"VDP \n{text}".
+
+        Returns:
+            Device: The created device.
+        """
+
+        return create_vdp_cell(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            layers_to_probe=layers_to_probe,
+            layers_to_outline=layers_to_outline,
+            outline=self.die_outline,
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+        )
+
+    def create_etch_test_cell(
+        self, layers_to_etch: List[List[int]], text: Union[None, str] = dflt_text
+    ) -> Device:
+        """Creates etch test structures in an integer number of unit cells.
+
+        These test structures are thought to be used by probing on pads (with a simple multimeter)
+        that should be isolated one from another if the etching is complete.
+
+        Parameters:
+            layers_to_etch (List[List[int]]): Each element of the list corresponds to one test point,
+                to put on the list of layers specified. Example: [[1, 2], [1], [2]].
+            text (str, optional): If None, the cell text is f"ETCH TEST {layers_to_etch}".
+
+        Returns:
+            Device: A device (with size n*m of unit cells) with etch tests in its center.
+        """
+
+        return create_etch_test_cell(
+            die_w=self.die_w,
+            layers_to_etch=layers_to_etch,
+            outline_die=self.die_outline,
+            die_layer=self.layers["die"],
+            text=text,
+        )
+
+    def create_resolution_test_cell(
+        self,
+        layer_to_resolve: int,
+        resolutions_to_test: List[float] = [
+            0.025,
+            0.05,
+            0.075,
+            0.1,
+            0.25,
+            0.5,
+            1,
+            1.5,
+            2,
+        ],
+        text: Union[None, str] = dflt_text,
+    ) -> Device:
+        r"""Creates a cell containing a resolution test.
+
+        Parameters:
+            layer_to_resolve (int): The layer to put the resolution test on.
+            resolutions_to_test (List[float]): The resolutions to test in µm.
+            text (str, optional): If None, the text is f"RES TEST \n{layer_to_resolve}".
+
+        Returns:
+            Device: The created device.
+        """
+
+        return create_resolution_test_cell(
+            die_w=self.die_w,
+            layer_to_resolve=layer_to_resolve,
+            resolutions_to_test=resolutions_to_test,
+            outline=self.die_outline,
+            die_layer=self.layers["die"],
+            text=text,
+        )
+
+    # devices:
+
+    def create_nanowires_cell(
+        self,
+        channels_sources_w: List[Tuple[float, float]],
+        text: Union[None, str] = dflt_text,
+    ) -> Device:
+        """Creates a cell containing several nanowires of given channel and
+        source.
+
+        Parameters:
+            channels_sources_w (List[Tuple[float, float]]): The list of
+                (channel_w, source_w) of the nanowires to create.
+            text (str, optional): If None, the text is "NWIRES".
+
+        Returns:
+            Device: A device containing the nanowires, the border of the die
+            (created with die_cell function), and the connections between the
+            nanowires and pads.
+        """
+
+        return create_nanowires_cell(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            channels_sources_w=channels_sources_w,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+        )
+
+    def create_ntron_cell(
+        self,
+        choke_w: float,
+        channel_w: float,
+        gate_w: Union[float, None] = auto_param,
+        source_w: Union[float, None] = auto_param,
+        drain_w: Union[float, None] = auto_param,
+        choke_shift: Union[float, None] = auto_param,
+        text: Union[str, None] = dflt_text,
+    ) -> Device:
+        r"""Creates a standardized cell specifically for a single ntron.
+
+        Unless specified, scales the ntron parameters as:
+        gate_w = drain_w = source_w = 3*channel_w
+        choke_shift = -3*channel_w
+
+        Parameters:
+            choke_w (int or float): The width of the ntron's choke in µm.
+            channel_w (int or float): The width of the ntron's channel in µm.
+            gate_w (int or float, optional): If None, gate width is 3 times the channel width.
+            source_w (int or float, optional): If None, source width is 3 times the channel width.
+            drain_w (int or float, optional): If None, drain width is 3 times the channel width.
+            choke_shift (int or float, optional): If None, choke shift is -3 times the channel width.
+            text (str, optional): If None, the text is f"chk: {choke_w} /n chnl: {channel_w}".
+
+        Returns:
+            Device: A device containing the ntron, the border of the die (created with die_cell function),
+            and the connections between the ports.
+        """
+
+        return create_ntron_cell(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            choke_w=choke_w,
+            channel_w=channel_w,
+            gate_w=gate_w,
+            source_w=source_w,
+            drain_w=drain_w,
+            choke_shift=choke_shift,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+        )
+
+    def create_snspd_ntron_cell(
+        self,
+        w_choke: float,
+        w_snspd: Union[float, None] = auto_param,
+        text: Union[str, None] = dflt_text,
+    ) -> Device:
+        """Creates a cell that contains an SNSPD coupled to an NTRON. The
+        device's parameters are sized according to the SNSPD's width and the
+        NTRON's choke.
+
+        Parameters:
+            w_choke (int or float): The width of the NTRON choke in µm.
+            w_snspd (int or float, optional): The width of the SNSPD nanowire in µm. If None, scaled to 5*w_choke.
+            text (str, optional): If None, text = f'SNSPD {w_choke}'.
+
+        Returns:
+            Device: A cell containing a die in die_layer, pads in pad layer, and an SNSPD-NTRON properly routed in the device layer.
+        """
+
+        return create_snspd_ntron_cell(
+            die_w=self.die_w,
+            pad_size=self.pad_size,
+            w_choke=w_choke,
+            w_snspd=w_snspd,
+            overlap_w=self.ebeam_overlap,
+            outline_die=self.die_outline,
+            outline_dev=self.device_outline,
+            device_layer=self.layers["device"],
+            die_layer=self.layers["die"],
+            pad_layer=self.layers["pad"],
+            text=text,
+        )
```

### Comparing `qnngds-1.0.0/src/qnngds/devices.py` & `qnngds-1.0.1/src/qnngds/devices.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-"""Devices module contain the basic devices that QNN uses in its circuits (e.g.
-ntron, htron etc)."""
-
-from phidl import Device
-
-# from phidl import quickplot as qp
-# from phidl import set_quickplot_options
-import phidl.geometry as pg
-from typing import Tuple, Optional
-
-
-def ntron(
-    choke_w: float = 0.03,
-    gate_w: float = 0.2,
-    channel_w: float = 0.1,
-    source_w: float = 0.3,
-    drain_w: float = 0.3,
-    choke_shift: float = -0.3,
-    layer: int = 0,
-) -> Device:
-    """Creates a ntron device.
-
-    Args:
-        choke_w (float): Width of the choke region.
-        gate_w (float): Width of the gate region.
-        channel_w (float): Width of the channel region.
-        source_w (float): Width of the source region.
-        drain_w (float): Width of the drain region.
-        choke_shift (float): Shift of the choke region.
-        layer (int): Layer for the device to be created on.
-
-    Returns:
-        Device: The ntron device.
-    """
-
-    D = Device()
-
-    choke = pg.optimal_step(gate_w, choke_w, symmetric=True, num_pts=100)
-    k = D << choke
-
-    channel = pg.compass(size=(channel_w, choke_w))
-    c = D << channel
-    c.connect(channel.ports["W"], choke.ports[2])
-
-    drain = pg.optimal_step(drain_w, channel_w)
-    d = D << drain
-    d.connect(drain.ports[2], c.ports["N"])
-
-    source = pg.optimal_step(channel_w, source_w)
-    s = D << source
-    s.connect(source.ports[1], c.ports["S"])
-
-    k.movey(choke_shift)
-
-    D = pg.union(D)
-    D.flatten(single_layer=layer)
-    D.add_port(name=3, port=k.ports[1])
-    D.add_port(name=1, port=d.ports[1])
-    D.add_port(name=2, port=s.ports[2])
-    D.name = f"NTRON {choke_w} {channel_w} "
-    D.info = locals()
-
-    return D
-
-
-def ntron_compassPorts(
-    choke_w: float = 0.03,
-    gate_w: float = 0.2,
-    channel_w: float = 0.1,
-    source_w: float = 0.3,
-    drain_w: float = 0.3,
-    choke_shift: float = -0.3,
-    layer: int = 0,
-) -> Device:
-    """Creates a ntron device with compass ports (i.e. N1, W1, S1 for drain,
-    gate, source respectively).
-
-    Args:
-        choke_w (float): Width of the choke region.
-        gate_w (float): Width of the gate region.
-        channel_w (float): Width of the channel region.
-        source_w (float): Width of the source region.
-        drain_w (float): Width of the drain region.
-        choke_shift (float): Shift of the choke region.
-        layer (int): Layer for the device to be created on.
-
-    Returns:
-        Device: The ntron device.
-    """
-
-    D = Device()
-
-    choke = pg.optimal_step(gate_w, choke_w, symmetric=True, num_pts=100)
-    k = D << choke
-
-    channel = pg.compass(size=(channel_w, choke_w))
-    c = D << channel
-    c.connect(channel.ports["W"], choke.ports[2])
-
-    drain = pg.optimal_step(drain_w, channel_w)
-    d = D << drain
-    d.connect(drain.ports[2], c.ports["N"])
-
-    source = pg.optimal_step(channel_w, source_w)
-    s = D << source
-    s.connect(source.ports[1], c.ports["S"])
-
-    k.movey(choke_shift)
-
-    D = pg.union(D)
-    D.flatten(single_layer=layer)
-    D.add_port(name="N1", port=d.ports[1])
-    D.add_port(name="S1", port=s.ports[2])
-    D.add_port(name="W1", port=k.ports[1])
-    D.name = f"NTRON {choke_w} {channel_w} "
-    D.info = locals()
-
-    return D
-
-
-def ntron_sharp(
-    choke_w: float = 0.03,
-    choke_l: float = 0.5,
-    gate_w: float = 0.2,
-    channel_w: float = 0.1,
-    source_w: float = 0.3,
-    drain_w: float = 0.3,
-    layer: int = 0,
-) -> Device:
-    """Creates a sharp ntron device.
-
-    Args:
-        choke_w (float): Width of the choke region.
-        choke_l (float): Length of the choke region.
-        gate_w (float): Width of the gate region.
-        channel_w (float): Width of the channel region.
-        source_w (float): Width of the source region.
-        drain_w (float): Width of the drain region.
-        layer (int): Layer for the device to be created on.
-
-    Returns:
-        Device: The sharp ntron device.
-    """
-
-    D = Device("nTron")
-
-    choke = pg.taper(choke_l, gate_w, choke_w)
-    k = D << choke
-
-    channel = pg.compass(size=(channel_w, choke_w / 10))
-    c = D << channel
-    c.connect(channel.ports["W"], choke.ports[2])
-
-    drain = pg.taper(channel_w * 6, drain_w, channel_w)
-    d = D << drain
-    d.connect(drain.ports[2], c.ports["N"])
-
-    source = pg.taper(channel_w * 6, channel_w, source_w)
-    s = D << source
-    s.connect(source.ports[1], c.ports["S"])
-
-    D = pg.union(D)
-    D.flatten(single_layer=layer)
-    D.add_port(name="g", port=k.ports[1])
-    D.add_port(name="d", port=d.ports[1])
-    D.add_port(name="s", port=s.ports[2])
-    D.name = "nTron"
-    D.info = locals()
-    return D
-
-
-def nanowire(
-    channel_w: float = 0.1, source_w: float = 0.3, layer: int = 0, num_pts: int = 100
-) -> Device:
-    """Creates a single wire, with the same appearance as an NTRON but without
-    the gate.
-
-    Args:
-        channel_w (int or float): The width of the channel (at the hot-spot location).
-        source_w (int or float): The width of the nanowire's "source".
-        layer (int): The layer where to put the device.
-        num_pts (int): The number of points comprising the optimal_steps geometries.
-
-    Returns:
-        Device: A device containing 2 optimal steps joined at their channel_w end.
-    """
-
-    NANOWIRE = Device(f"NANOWIRE {channel_w} ")
-    wire = pg.optimal_step(channel_w, source_w, symmetric=True, num_pts=num_pts)
-    source = NANOWIRE << wire
-    gnd = NANOWIRE << wire
-    source.connect(source.ports[1], gnd.ports[1])
-
-    NANOWIRE.flatten(single_layer=layer)
-    NANOWIRE.add_port(name=1, port=source.ports[2])
-    NANOWIRE.add_port(name=2, port=gnd.ports[2])
-    NANOWIRE.rotate(-90)
-    NANOWIRE.move(NANOWIRE.center, (0, 0))
-
-    return NANOWIRE
-
-
-def snspd_vert(
-    wire_width: float = 0.2,
-    wire_pitch: float = 0.6,
-    size: Tuple[int, int] = (6, 10),
-    num_squares: Optional[int] = None,
-    terminals_same_side: bool = False,
-    extend: Optional[float] = None,
-    layer: int = 0,
-) -> Device:
-    """Creates a vertical superconducting nanowire single-photon detector
-    (SNSPD).
-
-    Args:
-        wire_width (float): Width of the nanowire.
-        wire_pitch (float): Pitch of the nanowire.
-        size (Tuple[int, int]): Size of the detector in squares (width, height).
-        num_squares (Optional[int]): Number of squares in the detector.
-        terminals_same_side (bool): Whether the terminals are on the same side of the detector.
-        extend (Optional[bool]): Whether or not to extend the ports.
-        layer (int): Layer for the device to be created on.
-
-    Returns:
-        Device: The vertical SNSPD device.
-    """
-    D = Device("snspd_vert")
-    S = pg.snspd(
-        wire_width=wire_width,
-        wire_pitch=wire_pitch,
-        size=size,
-        num_squares=num_squares,
-        terminals_same_side=terminals_same_side,
-        layer=layer,
-    )
-    s1 = D << S
-
-    HP = pg.optimal_hairpin(
-        width=wire_width, pitch=wire_pitch, length=size[0] / 2, layer=layer
-    )
-    h1 = D << HP
-    h1.connect(h1.ports[1], S.references[0].ports["E"])
-    h1.rotate(180, h1.ports[1])
-
-    h2 = D << HP
-    h2.connect(h2.ports[1], S.references[-1].ports["E"])
-    h2.rotate(180, h2.ports[1])
-
-    T = pg.optimal_90deg(width=wire_width, layer=layer)
-    t1 = D << T
-    T_width = t1.ports[2].midpoint[0]
-    t1.connect(t1.ports[1], h1.ports[2])
-    t1.movex(-T_width + wire_width / 2)
-
-    t2 = D << T
-    t2.connect(t2.ports[1], h2.ports[2])
-    t2.movex(T_width - wire_width / 2)
-
-    D = pg.union(D, layer=layer)
-    D.flatten()
-    if extend:
-        E = pg.straight(size=(wire_width, extend), layer=layer)
-        e1 = D << E
-        e1.connect(e1.ports[1], t1.ports[2])
-        e2 = D << E
-        e2.connect(e2.ports[1], t2.ports[2])
-        D = pg.union(D, layer=layer)
-        D.add_port(name=1, port=e1.ports[2])
-        D.add_port(name=2, port=e2.ports[2])
-    else:
-        D.add_port(name=1, port=t1.ports[2])
-        D.add_port(name=2, port=t2.ports[2])
-
-    D.info = S.info
-    return D
+"""Devices module contain the basic devices that QNN uses in its circuits (e.g.
+ntron, htron etc)."""
+
+from phidl import Device
+
+# from phidl import quickplot as qp
+# from phidl import set_quickplot_options
+import phidl.geometry as pg
+from typing import Tuple, Optional
+
+
+def ntron(
+    choke_w: float = 0.03,
+    gate_w: float = 0.2,
+    channel_w: float = 0.1,
+    source_w: float = 0.3,
+    drain_w: float = 0.3,
+    choke_shift: float = -0.3,
+    layer: int = 0,
+) -> Device:
+    """Creates a ntron device.
+
+    Args:
+        choke_w (float): Width of the choke region.
+        gate_w (float): Width of the gate region.
+        channel_w (float): Width of the channel region.
+        source_w (float): Width of the source region.
+        drain_w (float): Width of the drain region.
+        choke_shift (float): Shift of the choke region.
+        layer (int): Layer for the device to be created on.
+
+    Returns:
+        Device: The ntron device.
+    """
+
+    D = Device()
+
+    choke = pg.optimal_step(gate_w, choke_w, symmetric=True, num_pts=100)
+    k = D << choke
+
+    channel = pg.compass(size=(channel_w, choke_w))
+    c = D << channel
+    c.connect(channel.ports["W"], choke.ports[2])
+
+    drain = pg.optimal_step(drain_w, channel_w)
+    d = D << drain
+    d.connect(drain.ports[2], c.ports["N"])
+
+    source = pg.optimal_step(channel_w, source_w)
+    s = D << source
+    s.connect(source.ports[1], c.ports["S"])
+
+    k.movey(choke_shift)
+
+    D = pg.union(D)
+    D.flatten(single_layer=layer)
+    D.add_port(name=3, port=k.ports[1])
+    D.add_port(name=1, port=d.ports[1])
+    D.add_port(name=2, port=s.ports[2])
+    D.name = f"NTRON {choke_w} {channel_w} "
+    D.info = locals()
+
+    return D
+
+
+def ntron_compassPorts(
+    choke_w: float = 0.03,
+    gate_w: float = 0.2,
+    channel_w: float = 0.1,
+    source_w: float = 0.3,
+    drain_w: float = 0.3,
+    choke_shift: float = -0.3,
+    layer: int = 0,
+) -> Device:
+    """Creates a ntron device with compass ports (i.e. N1, W1, S1 for drain,
+    gate, source respectively).
+
+    Args:
+        choke_w (float): Width of the choke region.
+        gate_w (float): Width of the gate region.
+        channel_w (float): Width of the channel region.
+        source_w (float): Width of the source region.
+        drain_w (float): Width of the drain region.
+        choke_shift (float): Shift of the choke region.
+        layer (int): Layer for the device to be created on.
+
+    Returns:
+        Device: The ntron device.
+    """
+
+    D = Device()
+
+    choke = pg.optimal_step(gate_w, choke_w, symmetric=True, num_pts=100)
+    k = D << choke
+
+    channel = pg.compass(size=(channel_w, choke_w))
+    c = D << channel
+    c.connect(channel.ports["W"], choke.ports[2])
+
+    drain = pg.optimal_step(drain_w, channel_w)
+    d = D << drain
+    d.connect(drain.ports[2], c.ports["N"])
+
+    source = pg.optimal_step(channel_w, source_w)
+    s = D << source
+    s.connect(source.ports[1], c.ports["S"])
+
+    k.movey(choke_shift)
+
+    D = pg.union(D)
+    D.flatten(single_layer=layer)
+    D.add_port(name="N1", port=d.ports[1])
+    D.add_port(name="S1", port=s.ports[2])
+    D.add_port(name="W1", port=k.ports[1])
+    D.name = f"NTRON {choke_w} {channel_w} "
+    D.info = locals()
+
+    return D
+
+
+def ntron_sharp(
+    choke_w: float = 0.03,
+    choke_l: float = 0.5,
+    gate_w: float = 0.2,
+    channel_w: float = 0.1,
+    source_w: float = 0.3,
+    drain_w: float = 0.3,
+    layer: int = 0,
+) -> Device:
+    """Creates a sharp ntron device.
+
+    Args:
+        choke_w (float): Width of the choke region.
+        choke_l (float): Length of the choke region.
+        gate_w (float): Width of the gate region.
+        channel_w (float): Width of the channel region.
+        source_w (float): Width of the source region.
+        drain_w (float): Width of the drain region.
+        layer (int): Layer for the device to be created on.
+
+    Returns:
+        Device: The sharp ntron device.
+    """
+
+    D = Device("nTron")
+
+    choke = pg.taper(choke_l, gate_w, choke_w)
+    k = D << choke
+
+    channel = pg.compass(size=(channel_w, choke_w / 10))
+    c = D << channel
+    c.connect(channel.ports["W"], choke.ports[2])
+
+    drain = pg.taper(channel_w * 6, drain_w, channel_w)
+    d = D << drain
+    d.connect(drain.ports[2], c.ports["N"])
+
+    source = pg.taper(channel_w * 6, channel_w, source_w)
+    s = D << source
+    s.connect(source.ports[1], c.ports["S"])
+
+    D = pg.union(D)
+    D.flatten(single_layer=layer)
+    D.add_port(name="g", port=k.ports[1])
+    D.add_port(name="d", port=d.ports[1])
+    D.add_port(name="s", port=s.ports[2])
+    D.name = "nTron"
+    D.info = locals()
+    return D
+
+
+def nanowire(
+    channel_w: float = 0.1, source_w: float = 0.3, layer: int = 0, num_pts: int = 100
+) -> Device:
+    """Creates a single wire, with the same appearance as an NTRON but without
+    the gate.
+
+    Args:
+        channel_w (int or float): The width of the channel (at the hot-spot location).
+        source_w (int or float): The width of the nanowire's "source".
+        layer (int): The layer where to put the device.
+        num_pts (int): The number of points comprising the optimal_steps geometries.
+
+    Returns:
+        Device: A device containing 2 optimal steps joined at their channel_w end.
+    """
+
+    NANOWIRE = Device(f"NANOWIRE {channel_w} ")
+    wire = pg.optimal_step(channel_w, source_w, symmetric=True, num_pts=num_pts)
+    source = NANOWIRE << wire
+    gnd = NANOWIRE << wire
+    source.connect(source.ports[1], gnd.ports[1])
+
+    NANOWIRE.flatten(single_layer=layer)
+    NANOWIRE.add_port(name=1, port=source.ports[2])
+    NANOWIRE.add_port(name=2, port=gnd.ports[2])
+    NANOWIRE.rotate(-90)
+    NANOWIRE.move(NANOWIRE.center, (0, 0))
+
+    return NANOWIRE
+
+
+def snspd_vert(
+    wire_width: float = 0.2,
+    wire_pitch: float = 0.6,
+    size: Tuple[int, int] = (6, 10),
+    num_squares: Optional[int] = None,
+    terminals_same_side: bool = False,
+    extend: Optional[float] = None,
+    layer: int = 0,
+) -> Device:
+    """Creates a vertical superconducting nanowire single-photon detector
+    (SNSPD).
+
+    Args:
+        wire_width (float): Width of the nanowire.
+        wire_pitch (float): Pitch of the nanowire.
+        size (Tuple[int, int]): Size of the detector in squares (width, height).
+        num_squares (Optional[int]): Number of squares in the detector.
+        terminals_same_side (bool): Whether the terminals are on the same side of the detector.
+        extend (Optional[bool]): Whether or not to extend the ports.
+        layer (int): Layer for the device to be created on.
+
+    Returns:
+        Device: The vertical SNSPD device.
+    """
+    D = Device("snspd_vert")
+    S = pg.snspd(
+        wire_width=wire_width,
+        wire_pitch=wire_pitch,
+        size=size,
+        num_squares=num_squares,
+        terminals_same_side=terminals_same_side,
+        layer=layer,
+    )
+    s1 = D << S
+
+    HP = pg.optimal_hairpin(
+        width=wire_width, pitch=wire_pitch, length=size[0] / 2, layer=layer
+    )
+    h1 = D << HP
+    h1.connect(h1.ports[1], S.references[0].ports["E"])
+    h1.rotate(180, h1.ports[1])
+
+    h2 = D << HP
+    h2.connect(h2.ports[1], S.references[-1].ports["E"])
+    h2.rotate(180, h2.ports[1])
+
+    T = pg.optimal_90deg(width=wire_width, layer=layer)
+    t1 = D << T
+    T_width = t1.ports[2].midpoint[0]
+    t1.connect(t1.ports[1], h1.ports[2])
+    t1.movex(-T_width + wire_width / 2)
+
+    t2 = D << T
+    t2.connect(t2.ports[1], h2.ports[2])
+    t2.movex(T_width - wire_width / 2)
+
+    D = pg.union(D, layer=layer)
+    D.flatten()
+    if extend:
+        E = pg.straight(size=(wire_width, extend), layer=layer)
+        e1 = D << E
+        e1.connect(e1.ports[1], t1.ports[2])
+        e2 = D << E
+        e2.connect(e2.ports[1], t2.ports[2])
+        D = pg.union(D, layer=layer)
+        D.add_port(name=1, port=e1.ports[2])
+        D.add_port(name=2, port=e2.ports[2])
+    else:
+        D.add_port(name=1, port=t1.ports[2])
+        D.add_port(name=2, port=t2.ports[2])
+
+    D.info = S.info
+    return D
```

### Comparing `qnngds-1.0.0/src/qnngds/utilities.py` & `qnngds-1.0.1/src/qnngds/utilities.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,586 +1,586 @@
-"""Utilies is used for building cells in design.
-
-Cells are made of devices
-(found in utilities) and a die_cell border, wich contains pads, text etc... The
-device and its die are linked thanks to functions present in this module.
-"""
-
-from phidl import Device, Port
-
-# from phidl import quickplot as qp
-# from phidl import set_quickplot_options
-import phidl.geometry as pg
-import phidl.routing as pr
-from typing import Tuple, List, Union, Dict, Set
-from phidl.device_layout import (
-    Device,
-    Port,
-)
-import qnngds.geometries as qg
-
-auto_param = None
-die_cell_border = 80
-
-# default parameters
-dflt_chip_w = 10000
-dflt_chip_margin = 100
-dflt_N_dies = 11
-dflt_die_w = 980
-dflt_pad_size = (150, 250)
-dflt_device_outline = 0.5
-dflt_die_outline = 10
-dflt_ebeam_overlap = 10
-dflt_layers = {"annotation": 0, "device": 1, "die": 2, "pad": 3}
-dflt_text = auto_param
-
-
-def die_cell(
-    die_size: Tuple[int, int] = (dflt_die_w, dflt_die_w),
-    device_max_size: Tuple[int, int] = (100, 100),
-    pad_size: Tuple[int, int] = dflt_pad_size,
-    contact_w: Union[int, float] = 50,
-    contact_l: Union[int, float] = dflt_ebeam_overlap,
-    ports: Dict[str, int] = {"N": 1, "E": 1, "W": 1, "S": 1},
-    ports_gnd: List[str] = ["E", "S"],
-    isolation: Union[int, float] = dflt_die_outline,
-    text: str = "",
-    text_size: Union[int, float] = die_cell_border / 2,
-    layer: int = dflt_layers["die"],
-    pad_layer: int = dflt_layers["pad"],
-    invert: bool = False,
-) -> Device:
-    """Creates a die cell with dicing marks, text, and pads to connect to a
-    device.
-
-    Parameters:
-        die_size (tuple of int): Overall size of the cell (width, height).
-        device_max_size (tuple of int): Max dimensions of the device inside the cell (width, height).
-        pad_size (tuple of int): Dimensions of the cell's pads (width, height).
-        contact_w (int or float): Width of the ports and route to be connected to a device.
-        contact_l (int or float): Extra length of the routes above the ports to assure alignment with the device
-                                   (useful for ebeam lithography).
-        ports (dict): The ports of the device, format must be {'N':m, 'E':n, 'W':p, 'S':q}.
-        ports_gnd (list of string): The ports connected to ground.
-        isolation (int or float): The width of the pads outline.
-        text (string): The text to be displayed on the cell.
-        text_size (int or float): Size of text, corresponds to phidl geometry std.
-        layer (int or array-like[2]): The layer where to put the cell.
-        pad_layer (int or array-like[2]): The layer where to put the contact pads.
-        invert (bool): If True, the cell is inverted (useful for positive tone resists exposure).
-
-    Returns:
-        DIE (Device): The cell, with ports of width contact_w positioned around a device_max_size area.
-    """
-
-    def offset(overlap_port):
-        port_name = overlap_port.name[0]
-        if port_name == "N":
-            overlap_port.midpoint[1] += -contact_l
-        elif port_name == "S":
-            overlap_port.midpoint[1] += contact_l
-        elif port_name == "W":
-            overlap_port.midpoint[0] += contact_l
-        elif port_name == "E":
-            overlap_port.midpoint[0] += -contact_l
-
-    DIE = Device(f"DIE {text} ")
-
-    border = pg.rectangle(die_size)
-    border.move(border.center, (0, 0))
-    borderOut = Device()
-
-    ## Make the routes and pads
-    padOut = Device()
-
-    pad_block_size = (
-        die_size[0] - 2 * pad_size[1] - 4 * isolation,
-        die_size[1] - 2 * pad_size[1] - 4 * isolation,
-    )
-    inner_block = pg.compass_multi(device_max_size, ports)
-    outer_block = pg.compass_multi(pad_block_size, ports)
-    inner_ports = list(inner_block.ports.values())
-
-    for i, port in enumerate(list(outer_block.ports.values())):
-
-        CONNECT = Device()
-        port.rotate(180)
-
-        # create the pad
-        pad = pg.rectangle(pad_size, layer={layer, pad_layer})
-        pad.add_port(
-            "1", midpoint=(pad_size[0] / 2, 0), width=pad_size[0], orientation=90
-        )
-        pad_ref = CONNECT << pad
-        pad_ref.connect(pad.ports["1"], port)
-
-        # create the route from pad to contact
-        port.width = pad_size[0]
-        inner_ports[i].width = contact_w
-        CONNECT << pr.route_quad(port, inner_ports[i], layer=layer)
-
-        # create the route from contact to overlap
-        overlap_port = CONNECT.add_port(port=inner_ports[i])
-        offset(overlap_port)
-        overlap_port.rotate(180)
-        CONNECT << pr.route_quad(inner_ports[i], overlap_port, layer=layer)
-
-        # isolate the pads that are not grounded
-        port_grounded = any(port.name[0] == P for P in ports_gnd)
-        if not port_grounded:
-            padOut << pg.outline(
-                CONNECT, distance=isolation, join="round", open_ports=2 * isolation
-            )
-
-        # add the port to the die
-        DIE.add_port(port=inner_ports[i].rotate(180))
-        DIE << CONNECT
-
-    borderOut << padOut
-
-    ## Add the die markers
-
-    # mark the corners
-    cornersOut = Device()
-
-    corners_coord = [
-        (
-            -die_size[0] / 2 + die_cell_border / 2,
-            -die_size[1] / 2 + die_cell_border / 2,
-        ),
-        (die_size[0] / 2 - die_cell_border / 2, -die_size[1] / 2 + die_cell_border / 2),
-        (die_size[0] / 2 - die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
-        (-die_size[0] / 2 + die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
-    ]
-    for corner_coord in corners_coord:
-        corner = pg.rectangle(
-            (die_cell_border - isolation, die_cell_border - isolation)
-        )
-        corner = pg.outline(corner, -1 * isolation)
-        corner.move(corner.center, corner_coord)
-        cornersOut << corner
-
-    borderOut << cornersOut
-
-    # label the cell
-    label = pg.text(text, size=text_size, layer=layer)
-    label.move((label.xmin, label.ymin), (0, 0))
-    pos = [x + 2 * isolation + 10 for x in (-die_size[0] / 2, -die_size[1] / 2)]
-    label.move(pos)
-    DIE << label
-    labelOut = pg.outline(label, isolation)
-
-    borderOut << labelOut
-
-    border = pg.boolean(border, borderOut, "A-B", layer=layer)
-    DIE << border
-
-    DIE.flatten()
-    ports = DIE.get_ports()
-    DIE = pg.union(DIE, by_layer=True)
-    if invert:
-        PADS = pg.deepcopy(DIE)
-        PADS.remove_layers([layer])
-        DIE = pg.invert(DIE, border=0, layer=layer)
-        DIE << PADS
-    for port in ports:
-        DIE.add_port(port)
-    DIE.name = f"DIE {text}"
-    return DIE
-
-
-def add_hyptap_to_cell(
-    die_ports: List[Port],
-    overlap_w: Union[int, float] = dflt_ebeam_overlap,
-    contact_w: Union[int, float] = 5,
-    layer: int = dflt_layers["device"],
-) -> Tuple[Device, Device]:
-    """Takes the cell and adds hyper taper at its ports.
-
-    Parameters:
-        die_ports (list of Port): The ports of the die cell (use .get_ports()).
-        overlap_w (int or float): The overlap width in µm (accounts for
-            misalignment between 1st and 2nd ebeam exposures).
-        contact_w (int or float): The width of the contact with the device's
-            route in µm (width of hyper taper's end).
-        layer (int or array-like[2]): The layer on which to place the device.
-
-    Returns:
-        Tuple[Device, Device]: a tuple containing:
-
-        - **HT** (*Device*): The hyper tapers, positioned at the die's ports.
-          Ports of the same name as the die's ports are added to the output of
-          the tapers.
-        - **device_ports** (*Device*): A device containing only the input ports
-          of the tapers, named as the die's ports.
-    """
-
-    HT = Device("HYPER TAPERS ")
-    device_ports = Device()
-
-    for port in die_ports:
-        ht_w = port.width + 2 * overlap_w
-        ht = HT << qg.hyper_taper(overlap_w, ht_w, contact_w)
-        ht.connect(ht.ports[2], port)
-        HT.add_port(port=ht.ports[1], name=port.name)
-        device_ports.add_port(port=ht.ports[2], name=port.name)
-
-    HT.flatten(single_layer=layer)
-    return HT, device_ports
-
-
-def route_to_dev(
-    ext_ports: List[Port], dev_ports: Set[Port], layer: int = dflt_layers["device"]
-) -> Device:
-    """Creates smooth routes from external ports to the device's ports.
-
-    Parameters:
-        ext_ports (list of Port): The external ports, e.g., of the die or hyper tapers (use .get_ports()).
-        dev_ports (set of Port): The device's ports, should be named as the external ports (use .ports).
-        layer (int or array-like[2]): The layer to put the routes on.
-
-    Returns:
-        ROUTES (Device): The routes from ports to ports, on the specified layer.
-    """
-
-    ROUTES = Device("ROUTES ")
-
-    for port in ext_ports:
-        dev_port = dev_ports[port.name]
-        try:
-            radius = port.width
-            length1 = 2 * radius
-            length2 = 2 * radius
-            ROUTES << pr.route_smooth(
-                port, dev_port, radius, path_type="Z", length1=length1, length2=length2
-            )
-        except ValueError:
-            try:
-                radius = dev_port.width
-                length1 = radius
-                length2 = radius
-                ROUTES << pr.route_smooth(
-                    port,
-                    dev_port,
-                    radius,
-                    path_type="Z",
-                    length1=length1,
-                    length2=length2,
-                )
-            except ValueError:
-                print("Error: Could not route to device.")
-                return ROUTES
-    ROUTES.flatten(single_layer=layer)
-    return ROUTES
-
-
-# from previous qnngds: to be tested...
-
-# def outline(elements, distance = 1, precision = 1e-4, num_divisions = [1, 1],
-#             join = 'miter', tolerance = 2, join_first = True,
-#             max_points = 4000, layer = 0, open_ports=-1, rotate_ports=False):
-#     """ Creates an outline around all the polygons passed in the `elements`
-#     argument. `elements` may be a Device, Polygon, or list of Devices.
-#     Parameters
-#     ----------
-#     elements : Device(/Reference), list of Device(/Reference), or Polygon
-#         Polygons to outline or Device containing polygons to outline.
-#     distance : int or float
-#         Distance to offset polygons. Positive values expand, negative shrink.
-#     precision : float
-#         Desired precision for rounding vertex coordinates.
-#     num_divisions : array-like[2] of int
-#         The number of divisions with which the geometry is divided into
-#         multiple rectangular regions. This allows for each region to be
-#         processed sequentially, which is more computationally efficient.
-#     join : {'miter', 'bevel', 'round'}
-#         Type of join used to create the offset polygon.
-#     tolerance : int or float
-#         For miter joints, this number must be at least 2 and it represents the
-#         maximal distance in multiples of offset between new vertices and their
-#         original position before beveling to avoid spikes at acute joints. For
-#         round joints, it indicates the curvature resolution in number of
-#         points per full circle.
-#     join_first : bool
-#         Join all paths before offsetting to avoid unnecessary joins in
-#         adjacent polygon sides.
-#     max_points : int
-#         The maximum number of vertices within the resulting polygon.
-#     layer : int, array-like[2], or set
-#         Specific layer(s) to put polygon geometry on.
-#   open_ports : int or float
-#       Trims the outline at each port of the element. The value of open_port
-#       scales the length of the trim gemoetry (must be positive).
-#       Useful for positive tone layouts.
-#     Returns
-#     -------
-#     D : Device
-#         A Device containing the outlined polygon(s).
-#     """
-#     D = Device('outline')
-#     if type(elements) is not list: elements = [elements]
-#     for e in elements:
-#         if isinstance(e, Device): D.add_ref(e)
-#         else: D.add(e)
-#     gds_layer, gds_datatype = _parse_layer(layer)
-#     D_bloated = pg.offset(D, distance = distance, join_first = join_first,
-#                        num_divisions = num_divisions, precision = precision,
-#                        max_points = max_points, join = join,
-#                        tolerance = tolerance, layer = layer)
-#     Outline = pg.boolean(A = D_bloated, B = D, operation = 'A-B',
-#                       num_divisions = num_divisions, max_points = max_points,
-#                       precision = precision, layer = layer)
-#     if open_ports>=0:
-#       for i in e.ports:
-#           trim = pg.rectangle(size=(distance, e.ports[i].width+open_ports*distance))
-
-#           trim.rotate(e.ports[i].orientation)
-#           trim.move(trim.center, destination=e.ports[i].midpoint)
-#           if rotate_ports:
-#               trim.movex(-np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
-#               trim.movey(-np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
-#           else:
-#               trim.movex(np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
-#               trim.movey(np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
-
-#           Outline = pg.boolean(A = Outline, B = trim, operation = 'A-B',
-#                      num_divisions = num_divisions, max_points = max_points,
-#                      precision = precision, layer = layer)
-#       for i in e.ports: Outline.add_port(port=e.ports[i])
-#     return Outline
-
-# def assign_ids(device_list, ids):
-#     """
-#     Attach device ID to device list.
-
-#     Parameters
-#     ----------
-#     device_list : LIST
-#         List of phidl device objects.
-#     ids : LIST
-#         list of identification strings.
-#         typically generated from packer_rect/text_labels.
-
-#     Returns
-#     -------
-#     None.
-
-#     """
-#     device_list = list(filter(None,device_list))
-#     for i in range(len(device_list)):
-#         device_list[i].name = ids[i]
-
-# def packer(D_list,
-#            text_letter,
-#            text_pos=(0,-70),
-#            text_layer=1,
-#            text_height=50,
-#            spacing = 100,
-#            aspect_ratio = (1,1),
-#            max_size = (None,750),
-#            sort_by_area = False,
-#            density = 1.1,
-#            precision = 1e-2,
-#            verbose = False):
-#     """
-#     Returns Device "p" with references from D_list. Names, or index, of each device is assigned and can be called from p.references[i].parent.name
-
-
-#     Parameters
-#     ----------
-#     D_list : TYPE
-#         DESCRIPTION.
-#     text_letter : TYPE
-#         DESCRIPTION.
-#     text_pos : TYPE, optional
-#         DESCRIPTION. The default is None.
-#     text_layer : TYPE, optional
-#         DESCRIPTION. The default is 1.
-#     text_height : TYPE, optional
-#         DESCRIPTION. The default is 50.
-#     spacing : TYPE, optional
-#         DESCRIPTION. The default is 10.
-#     aspect_ratio : TYPE, optional
-#         DESCRIPTION. The default is (1,1).
-#     max_size : TYPE, optional
-#         DESCRIPTION. The default is (None,None).
-#     sort_by_area : TYPE, optional
-#         DESCRIPTION. The default is True.
-#     density : TYPE, optional
-#         DESCRIPTION. The default is 1.1.
-#     precision : TYPE, optional
-#         DESCRIPTION. The default is 1e-2.
-#     verbose : TYPE, optional
-#         DESCRIPTION. The default is False.
-#      : TYPE
-#         DESCRIPTION.
-
-#     Returns
-#     -------
-#     TYPE
-#         DESCRIPTION.
-
-#     """
-
-#     p = pg.packer(D_list,
-#         spacing = spacing,
-#         aspect_ratio = aspect_ratio,
-#         max_size = max_size,
-#         sort_by_area = sort_by_area,
-#         density = density,
-#         precision = precision,
-#         verbose = verbose,
-#         )
-
-
-#     for i in range(len(p[0].references)):
-#         device_text = text_letter+str(i)
-#         text_object = pg.text(text=device_text, size = text_height, justify='left', layer=text_layer)
-#         t = p[0].references[i].parent.add_ref(text_object)
-#         t.move(origin=text_object.bbox[0], destination= (text_pos[0], text_pos[1]))
-
-#         p[0].references[i].parent.name = device_text
-
-#     p = p[0]
-#     p.name = text_letter
-#     p._internal_name = text_letter
-#     # p.flatten() # do not flatten.
-
-#     return p
-
-# def packer_rect(device_list, dimensions, spacing, text_pos=None, text_size = 50, text_layer = 1):
-#     """
-#     This function distributes devices from a list onto a rectangular grid. The aspect ratio (dimensions) and spacing must be specified.
-#     If specified, text can be added automatically in a A1, B2, C3, style. The text will start with A0 in the NW corner.
-
-#     Parameters
-#     ----------
-#     device_list : LIST
-#         LIST OF PHIDL DEVICE OBJECTS
-#     dimensions : TUPLE
-#         (X,Y) X BY Y GRID POINTS
-#     spacing : TUPLE
-#         (dX,dY) SPACING BETWEEN GRID POINTS
-#     text_pos : TUPLE, optional
-#         IF SPECIFIED THE GENERATED TEXT IS LOCATED AT (dX,dY) FROM SW CORNER. The default is None.
-#     text_size : INT, optional
-#         SIZE OF TEXT LABEL. The default is 50.
-#     text_layer : INT, optional
-#         LAYER TO ADD TEXT LABEL TO The default is 1.
-
-#     Returns
-#     -------
-#     D : DEVICE
-#         PHIDL device object. List is entered and a single device is returned with labels.
-#     text_list : LIST
-#         LIST of strings of device labels.
-
-#     """
-
-#     letters = list(string.ascii_uppercase)
-
-#     while len(device_list) < np.product(dimensions):
-#         device_list.append(None)
-
-#     new_shape = np.reshape(device_list,dimensions)
-#     text_list=[]
-#     D = Device('return')
-#     for i in range(dimensions[0]):
-#         for j in range(dimensions[1]):
-#             if not new_shape[i][j] == None:
-#                 moved_device = new_shape[i][j].move(origin=new_shape[i][j].bbox[0], destination=(i*spacing[0], -j*spacing[1]))
-#                 D.add_ref(moved_device)
-#                 if text_pos:
-#                     device_text = letters[i]+str(j)
-#                     text_list.append(device_text)
-#                     text_object = pg.text(text=device_text, size = text_size, justify='left', layer=text_layer)
-#                     text_object.move(destination= (i*spacing[0]+text_pos[0], -j*spacing[1]+text_pos[1]))
-#                     D.add_ref(text_object)
-
-#     return D, text_list
-
-# def packer_doc(D_pack_list):
-#     """
-#     This function creates a text document to be referenced during meansurement.
-#     Its primary purpose is to serve as a reference for device specifications on chip.
-#     For instance, "A2 is a 3um device."
-
-#     Currently. This function really only works with D_pack_list from packer().
-#     It looks at each reference and grabs the device parameters (which are hard coded).
-#     'line.append(str(D_pack_list[i].references[j].parent.width))'
-#     It would be great to have this as a dynamical property that can be expounded for every kind of device/parameter.
-
-#     'create_device_doc' predated this function and took every np.array parameter in the parameter-dict and wrote it to a .txt file.
-#     The main problem with this function is that the device name is not associated in the parameter-dict.
-
-#     Inputs
-#     ----------
-#     sample: STRING
-#         enter a sample name "SPX000". The file path will be generated on the NAS and the .txt file will be saved there.
-
-#     Parameters
-#     ----------
-#     D_pack_list : LIST
-#         List containing PHIDL Device objects.
-
-#     Returns
-#     -------
-#     None.
-
-#     """
-
-#     """ Safety net for writing to the correct location"""
-
-#     sample = input('enter a sample name: ')
-#     if sample == '':
-#         print('Doc not created')
-#         return
-#     else:
-#         path = os.path.join('S:\SC\Measurements',sample)
-#         os.makedirs(path, exist_ok=True)
-
-#         path = os.path.join('S:\SC\Measurements',sample, sample+'_device_doc.txt')
-
-#         file = open(path, "w")
-
-#         tab = ',\t'
-#         string_list=[]
-#         headers = ['ID', 'WIDTH', 'AREA', 'SQUARES']
-#         headers.append('\n----------------------------------\n')
-
-#         for i in range(len(D_pack_list)):
-#             for j in range(len(D_pack_list[i].references)):
-#                 line = []
-#                 line.append(str(D_pack_list[i].references[j].parent.name))
-#                 line.append(str(D_pack_list[i].references[j].parent.width))
-#                 line.append(str(D_pack_list[i].references[j].parent.area))
-#                 line.append(str(D_pack_list[i].references[j].parent.squares))
-
-#                 line.append('\n')
-#                 string_list.append(tab.join(line))
-#                 string_list.append('. . . . . . . . . . . . . . . . \n')
-#             string_list.append('\\-----------------------------------\\ \n')
-
-#         file.write(tab.join(headers))
-#         file.writelines(string_list)
-#         file.close()
-
-# def assign_ids(device_list, ids):
-#     """
-#     Attach device ID to device list.
-
-#     Parameters
-#     ----------
-#     device_list : LIST
-#         List of phidl device objects.
-#     ids : LIST
-#         list of identification strings.
-#         typically generated from packer_rect/text_labels.
-
-#     Returns
-#     -------
-#     None.
-
-#     """
-#     device_list = list(filter(None,device_list))
-#     for i in range(len(device_list)):
-#         device_list[i].name = ids[i]
+"""Utilies is used for building cells in design.
+
+Cells are made of devices
+(found in utilities) and a die_cell border, wich contains pads, text etc... The
+device and its die are linked thanks to functions present in this module.
+"""
+
+from phidl import Device, Port
+
+# from phidl import quickplot as qp
+# from phidl import set_quickplot_options
+import phidl.geometry as pg
+import phidl.routing as pr
+from typing import Tuple, List, Union, Dict, Set
+from phidl.device_layout import (
+    Device,
+    Port,
+)
+import qnngds.geometries as qg
+
+auto_param = None
+die_cell_border = 80
+
+# default parameters
+dflt_chip_w = 10000
+dflt_chip_margin = 100
+dflt_N_dies = 11
+dflt_die_w = 980
+dflt_pad_size = (150, 250)
+dflt_device_outline = 0.5
+dflt_die_outline = 10
+dflt_ebeam_overlap = 10
+dflt_layers = {"annotation": 0, "device": 1, "die": 2, "pad": 3}
+dflt_text = auto_param
+
+
+def die_cell(
+    die_size: Tuple[int, int] = (dflt_die_w, dflt_die_w),
+    device_max_size: Tuple[int, int] = (100, 100),
+    pad_size: Tuple[int, int] = dflt_pad_size,
+    contact_w: Union[int, float] = 50,
+    contact_l: Union[int, float] = dflt_ebeam_overlap,
+    ports: Dict[str, int] = {"N": 1, "E": 1, "W": 1, "S": 1},
+    ports_gnd: List[str] = ["E", "S"],
+    isolation: Union[int, float] = dflt_die_outline,
+    text: str = "",
+    text_size: Union[int, float] = die_cell_border / 2,
+    layer: int = dflt_layers["die"],
+    pad_layer: int = dflt_layers["pad"],
+    invert: bool = False,
+) -> Device:
+    """Creates a die cell with dicing marks, text, and pads to connect to a
+    device.
+
+    Parameters:
+        die_size (tuple of int): Overall size of the cell (width, height).
+        device_max_size (tuple of int): Max dimensions of the device inside the cell (width, height).
+        pad_size (tuple of int): Dimensions of the cell's pads (width, height).
+        contact_w (int or float): Width of the ports and route to be connected to a device.
+        contact_l (int or float): Extra length of the routes above the ports to assure alignment with the device
+                                   (useful for ebeam lithography).
+        ports (dict): The ports of the device, format must be {'N':m, 'E':n, 'W':p, 'S':q}.
+        ports_gnd (list of string): The ports connected to ground.
+        isolation (int or float): The width of the pads outline.
+        text (string): The text to be displayed on the cell.
+        text_size (int or float): Size of text, corresponds to phidl geometry std.
+        layer (int or array-like[2]): The layer where to put the cell.
+        pad_layer (int or array-like[2]): The layer where to put the contact pads.
+        invert (bool): If True, the cell is inverted (useful for positive tone resists exposure).
+
+    Returns:
+        DIE (Device): The cell, with ports of width contact_w positioned around a device_max_size area.
+    """
+
+    def offset(overlap_port):
+        port_name = overlap_port.name[0]
+        if port_name == "N":
+            overlap_port.midpoint[1] += -contact_l
+        elif port_name == "S":
+            overlap_port.midpoint[1] += contact_l
+        elif port_name == "W":
+            overlap_port.midpoint[0] += contact_l
+        elif port_name == "E":
+            overlap_port.midpoint[0] += -contact_l
+
+    DIE = Device(f"DIE {text} ")
+
+    border = pg.rectangle(die_size)
+    border.move(border.center, (0, 0))
+    borderOut = Device()
+
+    ## Make the routes and pads
+    padOut = Device()
+
+    pad_block_size = (
+        die_size[0] - 2 * pad_size[1] - 4 * isolation,
+        die_size[1] - 2 * pad_size[1] - 4 * isolation,
+    )
+    inner_block = pg.compass_multi(device_max_size, ports)
+    outer_block = pg.compass_multi(pad_block_size, ports)
+    inner_ports = list(inner_block.ports.values())
+
+    for i, port in enumerate(list(outer_block.ports.values())):
+
+        CONNECT = Device()
+        port.rotate(180)
+
+        # create the pad
+        pad = pg.rectangle(pad_size, layer={layer, pad_layer})
+        pad.add_port(
+            "1", midpoint=(pad_size[0] / 2, 0), width=pad_size[0], orientation=90
+        )
+        pad_ref = CONNECT << pad
+        pad_ref.connect(pad.ports["1"], port)
+
+        # create the route from pad to contact
+        port.width = pad_size[0]
+        inner_ports[i].width = contact_w
+        CONNECT << pr.route_quad(port, inner_ports[i], layer=layer)
+
+        # create the route from contact to overlap
+        overlap_port = CONNECT.add_port(port=inner_ports[i])
+        offset(overlap_port)
+        overlap_port.rotate(180)
+        CONNECT << pr.route_quad(inner_ports[i], overlap_port, layer=layer)
+
+        # isolate the pads that are not grounded
+        port_grounded = any(port.name[0] == P for P in ports_gnd)
+        if not port_grounded:
+            padOut << pg.outline(
+                CONNECT, distance=isolation, join="round", open_ports=2 * isolation
+            )
+
+        # add the port to the die
+        DIE.add_port(port=inner_ports[i].rotate(180))
+        DIE << CONNECT
+
+    borderOut << padOut
+
+    ## Add the die markers
+
+    # mark the corners
+    cornersOut = Device()
+
+    corners_coord = [
+        (
+            -die_size[0] / 2 + die_cell_border / 2,
+            -die_size[1] / 2 + die_cell_border / 2,
+        ),
+        (die_size[0] / 2 - die_cell_border / 2, -die_size[1] / 2 + die_cell_border / 2),
+        (die_size[0] / 2 - die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
+        (-die_size[0] / 2 + die_cell_border / 2, die_size[1] / 2 - die_cell_border / 2),
+    ]
+    for corner_coord in corners_coord:
+        corner = pg.rectangle(
+            (die_cell_border - isolation, die_cell_border - isolation)
+        )
+        corner = pg.outline(corner, -1 * isolation)
+        corner.move(corner.center, corner_coord)
+        cornersOut << corner
+
+    borderOut << cornersOut
+
+    # label the cell
+    label = pg.text(text, size=text_size, layer=layer)
+    label.move((label.xmin, label.ymin), (0, 0))
+    pos = [x + 2 * isolation + 10 for x in (-die_size[0] / 2, -die_size[1] / 2)]
+    label.move(pos)
+    DIE << label
+    labelOut = pg.outline(label, isolation)
+
+    borderOut << labelOut
+
+    border = pg.boolean(border, borderOut, "A-B", layer=layer)
+    DIE << border
+
+    DIE.flatten()
+    ports = DIE.get_ports()
+    DIE = pg.union(DIE, by_layer=True)
+    if invert:
+        PADS = pg.deepcopy(DIE)
+        PADS.remove_layers([layer])
+        DIE = pg.invert(DIE, border=0, layer=layer)
+        DIE << PADS
+    for port in ports:
+        DIE.add_port(port)
+    DIE.name = f"DIE {text}"
+    return DIE
+
+
+def add_hyptap_to_cell(
+    die_ports: List[Port],
+    overlap_w: Union[int, float] = dflt_ebeam_overlap,
+    contact_w: Union[int, float] = 5,
+    layer: int = dflt_layers["device"],
+) -> Tuple[Device, Device]:
+    """Takes the cell and adds hyper taper at its ports.
+
+    Parameters:
+        die_ports (list of Port): The ports of the die cell (use .get_ports()).
+        overlap_w (int or float): The overlap width in µm (accounts for
+            misalignment between 1st and 2nd ebeam exposures).
+        contact_w (int or float): The width of the contact with the device's
+            route in µm (width of hyper taper's end).
+        layer (int or array-like[2]): The layer on which to place the device.
+
+    Returns:
+        Tuple[Device, Device]: a tuple containing:
+
+        - **HT** (*Device*): The hyper tapers, positioned at the die's ports.
+          Ports of the same name as the die's ports are added to the output of
+          the tapers.
+        - **device_ports** (*Device*): A device containing only the input ports
+          of the tapers, named as the die's ports.
+    """
+
+    HT = Device("HYPER TAPERS ")
+    device_ports = Device()
+
+    for port in die_ports:
+        ht_w = port.width + 2 * overlap_w
+        ht = HT << qg.hyper_taper(overlap_w, ht_w, contact_w)
+        ht.connect(ht.ports[2], port)
+        HT.add_port(port=ht.ports[1], name=port.name)
+        device_ports.add_port(port=ht.ports[2], name=port.name)
+
+    HT.flatten(single_layer=layer)
+    return HT, device_ports
+
+
+def route_to_dev(
+    ext_ports: List[Port], dev_ports: Set[Port], layer: int = dflt_layers["device"]
+) -> Device:
+    """Creates smooth routes from external ports to the device's ports.
+
+    Parameters:
+        ext_ports (list of Port): The external ports, e.g., of the die or hyper tapers (use .get_ports()).
+        dev_ports (set of Port): The device's ports, should be named as the external ports (use .ports).
+        layer (int or array-like[2]): The layer to put the routes on.
+
+    Returns:
+        ROUTES (Device): The routes from ports to ports, on the specified layer.
+    """
+
+    ROUTES = Device("ROUTES ")
+
+    for port in ext_ports:
+        dev_port = dev_ports[port.name]
+        try:
+            radius = port.width
+            length1 = 2 * radius
+            length2 = 2 * radius
+            ROUTES << pr.route_smooth(
+                port, dev_port, radius, path_type="Z", length1=length1, length2=length2
+            )
+        except ValueError:
+            try:
+                radius = dev_port.width
+                length1 = radius
+                length2 = radius
+                ROUTES << pr.route_smooth(
+                    port,
+                    dev_port,
+                    radius,
+                    path_type="Z",
+                    length1=length1,
+                    length2=length2,
+                )
+            except ValueError:
+                print("Error: Could not route to device.")
+                return ROUTES
+    ROUTES.flatten(single_layer=layer)
+    return ROUTES
+
+
+# from previous qnngds: to be tested...
+
+# def outline(elements, distance = 1, precision = 1e-4, num_divisions = [1, 1],
+#             join = 'miter', tolerance = 2, join_first = True,
+#             max_points = 4000, layer = 0, open_ports=-1, rotate_ports=False):
+#     """ Creates an outline around all the polygons passed in the `elements`
+#     argument. `elements` may be a Device, Polygon, or list of Devices.
+#     Parameters
+#     ----------
+#     elements : Device(/Reference), list of Device(/Reference), or Polygon
+#         Polygons to outline or Device containing polygons to outline.
+#     distance : int or float
+#         Distance to offset polygons. Positive values expand, negative shrink.
+#     precision : float
+#         Desired precision for rounding vertex coordinates.
+#     num_divisions : array-like[2] of int
+#         The number of divisions with which the geometry is divided into
+#         multiple rectangular regions. This allows for each region to be
+#         processed sequentially, which is more computationally efficient.
+#     join : {'miter', 'bevel', 'round'}
+#         Type of join used to create the offset polygon.
+#     tolerance : int or float
+#         For miter joints, this number must be at least 2 and it represents the
+#         maximal distance in multiples of offset between new vertices and their
+#         original position before beveling to avoid spikes at acute joints. For
+#         round joints, it indicates the curvature resolution in number of
+#         points per full circle.
+#     join_first : bool
+#         Join all paths before offsetting to avoid unnecessary joins in
+#         adjacent polygon sides.
+#     max_points : int
+#         The maximum number of vertices within the resulting polygon.
+#     layer : int, array-like[2], or set
+#         Specific layer(s) to put polygon geometry on.
+#   open_ports : int or float
+#       Trims the outline at each port of the element. The value of open_port
+#       scales the length of the trim gemoetry (must be positive).
+#       Useful for positive tone layouts.
+#     Returns
+#     -------
+#     D : Device
+#         A Device containing the outlined polygon(s).
+#     """
+#     D = Device('outline')
+#     if type(elements) is not list: elements = [elements]
+#     for e in elements:
+#         if isinstance(e, Device): D.add_ref(e)
+#         else: D.add(e)
+#     gds_layer, gds_datatype = _parse_layer(layer)
+#     D_bloated = pg.offset(D, distance = distance, join_first = join_first,
+#                        num_divisions = num_divisions, precision = precision,
+#                        max_points = max_points, join = join,
+#                        tolerance = tolerance, layer = layer)
+#     Outline = pg.boolean(A = D_bloated, B = D, operation = 'A-B',
+#                       num_divisions = num_divisions, max_points = max_points,
+#                       precision = precision, layer = layer)
+#     if open_ports>=0:
+#       for i in e.ports:
+#           trim = pg.rectangle(size=(distance, e.ports[i].width+open_ports*distance))
+
+#           trim.rotate(e.ports[i].orientation)
+#           trim.move(trim.center, destination=e.ports[i].midpoint)
+#           if rotate_ports:
+#               trim.movex(-np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
+#               trim.movey(-np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
+#           else:
+#               trim.movex(np.cos(e.ports[i].orientation/180*np.pi)*distance/2)
+#               trim.movey(np.sin(e.ports[i].orientation/180*np.pi)*distance/2)
+
+#           Outline = pg.boolean(A = Outline, B = trim, operation = 'A-B',
+#                      num_divisions = num_divisions, max_points = max_points,
+#                      precision = precision, layer = layer)
+#       for i in e.ports: Outline.add_port(port=e.ports[i])
+#     return Outline
+
+# def assign_ids(device_list, ids):
+#     """
+#     Attach device ID to device list.
+
+#     Parameters
+#     ----------
+#     device_list : LIST
+#         List of phidl device objects.
+#     ids : LIST
+#         list of identification strings.
+#         typically generated from packer_rect/text_labels.
+
+#     Returns
+#     -------
+#     None.
+
+#     """
+#     device_list = list(filter(None,device_list))
+#     for i in range(len(device_list)):
+#         device_list[i].name = ids[i]
+
+# def packer(D_list,
+#            text_letter,
+#            text_pos=(0,-70),
+#            text_layer=1,
+#            text_height=50,
+#            spacing = 100,
+#            aspect_ratio = (1,1),
+#            max_size = (None,750),
+#            sort_by_area = False,
+#            density = 1.1,
+#            precision = 1e-2,
+#            verbose = False):
+#     """
+#     Returns Device "p" with references from D_list. Names, or index, of each device is assigned and can be called from p.references[i].parent.name
+
+
+#     Parameters
+#     ----------
+#     D_list : TYPE
+#         DESCRIPTION.
+#     text_letter : TYPE
+#         DESCRIPTION.
+#     text_pos : TYPE, optional
+#         DESCRIPTION. The default is None.
+#     text_layer : TYPE, optional
+#         DESCRIPTION. The default is 1.
+#     text_height : TYPE, optional
+#         DESCRIPTION. The default is 50.
+#     spacing : TYPE, optional
+#         DESCRIPTION. The default is 10.
+#     aspect_ratio : TYPE, optional
+#         DESCRIPTION. The default is (1,1).
+#     max_size : TYPE, optional
+#         DESCRIPTION. The default is (None,None).
+#     sort_by_area : TYPE, optional
+#         DESCRIPTION. The default is True.
+#     density : TYPE, optional
+#         DESCRIPTION. The default is 1.1.
+#     precision : TYPE, optional
+#         DESCRIPTION. The default is 1e-2.
+#     verbose : TYPE, optional
+#         DESCRIPTION. The default is False.
+#      : TYPE
+#         DESCRIPTION.
+
+#     Returns
+#     -------
+#     TYPE
+#         DESCRIPTION.
+
+#     """
+
+#     p = pg.packer(D_list,
+#         spacing = spacing,
+#         aspect_ratio = aspect_ratio,
+#         max_size = max_size,
+#         sort_by_area = sort_by_area,
+#         density = density,
+#         precision = precision,
+#         verbose = verbose,
+#         )
+
+
+#     for i in range(len(p[0].references)):
+#         device_text = text_letter+str(i)
+#         text_object = pg.text(text=device_text, size = text_height, justify='left', layer=text_layer)
+#         t = p[0].references[i].parent.add_ref(text_object)
+#         t.move(origin=text_object.bbox[0], destination= (text_pos[0], text_pos[1]))
+
+#         p[0].references[i].parent.name = device_text
+
+#     p = p[0]
+#     p.name = text_letter
+#     p._internal_name = text_letter
+#     # p.flatten() # do not flatten.
+
+#     return p
+
+# def packer_rect(device_list, dimensions, spacing, text_pos=None, text_size = 50, text_layer = 1):
+#     """
+#     This function distributes devices from a list onto a rectangular grid. The aspect ratio (dimensions) and spacing must be specified.
+#     If specified, text can be added automatically in a A1, B2, C3, style. The text will start with A0 in the NW corner.
+
+#     Parameters
+#     ----------
+#     device_list : LIST
+#         LIST OF PHIDL DEVICE OBJECTS
+#     dimensions : TUPLE
+#         (X,Y) X BY Y GRID POINTS
+#     spacing : TUPLE
+#         (dX,dY) SPACING BETWEEN GRID POINTS
+#     text_pos : TUPLE, optional
+#         IF SPECIFIED THE GENERATED TEXT IS LOCATED AT (dX,dY) FROM SW CORNER. The default is None.
+#     text_size : INT, optional
+#         SIZE OF TEXT LABEL. The default is 50.
+#     text_layer : INT, optional
+#         LAYER TO ADD TEXT LABEL TO The default is 1.
+
+#     Returns
+#     -------
+#     D : DEVICE
+#         PHIDL device object. List is entered and a single device is returned with labels.
+#     text_list : LIST
+#         LIST of strings of device labels.
+
+#     """
+
+#     letters = list(string.ascii_uppercase)
+
+#     while len(device_list) < np.product(dimensions):
+#         device_list.append(None)
+
+#     new_shape = np.reshape(device_list,dimensions)
+#     text_list=[]
+#     D = Device('return')
+#     for i in range(dimensions[0]):
+#         for j in range(dimensions[1]):
+#             if not new_shape[i][j] == None:
+#                 moved_device = new_shape[i][j].move(origin=new_shape[i][j].bbox[0], destination=(i*spacing[0], -j*spacing[1]))
+#                 D.add_ref(moved_device)
+#                 if text_pos:
+#                     device_text = letters[i]+str(j)
+#                     text_list.append(device_text)
+#                     text_object = pg.text(text=device_text, size = text_size, justify='left', layer=text_layer)
+#                     text_object.move(destination= (i*spacing[0]+text_pos[0], -j*spacing[1]+text_pos[1]))
+#                     D.add_ref(text_object)
+
+#     return D, text_list
+
+# def packer_doc(D_pack_list):
+#     """
+#     This function creates a text document to be referenced during meansurement.
+#     Its primary purpose is to serve as a reference for device specifications on chip.
+#     For instance, "A2 is a 3um device."
+
+#     Currently. This function really only works with D_pack_list from packer().
+#     It looks at each reference and grabs the device parameters (which are hard coded).
+#     'line.append(str(D_pack_list[i].references[j].parent.width))'
+#     It would be great to have this as a dynamical property that can be expounded for every kind of device/parameter.
+
+#     'create_device_doc' predated this function and took every np.array parameter in the parameter-dict and wrote it to a .txt file.
+#     The main problem with this function is that the device name is not associated in the parameter-dict.
+
+#     Inputs
+#     ----------
+#     sample: STRING
+#         enter a sample name "SPX000". The file path will be generated on the NAS and the .txt file will be saved there.
+
+#     Parameters
+#     ----------
+#     D_pack_list : LIST
+#         List containing PHIDL Device objects.
+
+#     Returns
+#     -------
+#     None.
+
+#     """
+
+#     """ Safety net for writing to the correct location"""
+
+#     sample = input('enter a sample name: ')
+#     if sample == '':
+#         print('Doc not created')
+#         return
+#     else:
+#         path = os.path.join('S:\SC\Measurements',sample)
+#         os.makedirs(path, exist_ok=True)
+
+#         path = os.path.join('S:\SC\Measurements',sample, sample+'_device_doc.txt')
+
+#         file = open(path, "w")
+
+#         tab = ',\t'
+#         string_list=[]
+#         headers = ['ID', 'WIDTH', 'AREA', 'SQUARES']
+#         headers.append('\n----------------------------------\n')
+
+#         for i in range(len(D_pack_list)):
+#             for j in range(len(D_pack_list[i].references)):
+#                 line = []
+#                 line.append(str(D_pack_list[i].references[j].parent.name))
+#                 line.append(str(D_pack_list[i].references[j].parent.width))
+#                 line.append(str(D_pack_list[i].references[j].parent.area))
+#                 line.append(str(D_pack_list[i].references[j].parent.squares))
+
+#                 line.append('\n')
+#                 string_list.append(tab.join(line))
+#                 string_list.append('. . . . . . . . . . . . . . . . \n')
+#             string_list.append('\\-----------------------------------\\ \n')
+
+#         file.write(tab.join(headers))
+#         file.writelines(string_list)
+#         file.close()
+
+# def assign_ids(device_list, ids):
+#     """
+#     Attach device ID to device list.
+
+#     Parameters
+#     ----------
+#     device_list : LIST
+#         List of phidl device objects.
+#     ids : LIST
+#         list of identification strings.
+#         typically generated from packer_rect/text_labels.
+
+#     Returns
+#     -------
+#     None.
+
+#     """
+#     device_list = list(filter(None,device_list))
+#     for i in range(len(device_list)):
+#         device_list[i].name = ids[i]
```

### Comparing `qnngds-1.0.0/PKG-INFO` & `qnngds-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 1.0.0
+Version: 1.0.1
 Summary: The QNN library for creating gds files
 Keywords: phidl nanowire_electronics nanofabrication gds
 Author-Email: A. Jacquillat <audrey01@mit.edu>, A. Jacquillat <audrey.jacquillat@gmail.com>
 Maintainer-Email: A. Jacquillat <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

