# Comparing `tmp/cubestat-0.2.5.tar.gz` & `tmp/cubestat-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.2.5.tar", last modified: Tue Apr  2 16:21:30 2024, max compression
+gzip compressed data, was "cubestat-0.2.6.tar", last modified: Fri Apr  5 15:22:24 2024, max compression
```

## Comparing `cubestat-0.2.5.tar` & `cubestat-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.610425 cubestat-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-02 16:21:13.000000 cubestat-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-02 16:21:30.610425 cubestat-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-02 16:21:13.000000 cubestat-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.606425 cubestat-0.2.5/cubestat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14413 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.606425 cubestat-0.2.5/cubestat/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/free_swap_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/linux_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/macos_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/mem_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/nv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-02 16:21:13.000000 cubestat-0.2.5/cubestat/readers/swapusage_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:21:30.610425 cubestat-0.2.5/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 16:21:30.000000 cubestat-0.2.5/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:21:30.610425 cubestat-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 16:21:13.000000 cubestat-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.697566 cubestat-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 15:22:18.000000 cubestat-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 15:22:24.693566 cubestat-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-05 15:22:18.000000 cubestat-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.693566 cubestat-0.2.6/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15607 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.693566 cubestat-0.2.6/cubestat/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/free_swap_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/linux_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/macos_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/mem_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/nv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-05 15:22:18.000000 cubestat-0.2.6/cubestat/readers/swapusage_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:22:24.693566 cubestat-0.2.6/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:22:24.000000 cubestat-0.2.6/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:22:24.697566 cubestat-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 15:22:18.000000 cubestat-0.2.6/setup.py
```

### Comparing `cubestat-0.2.5/LICENSE` & `cubestat-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.5/README.md` & `cubestat-0.2.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,112 @@
 # system monitoring horizon charts for terminal
 
-cubestat is a command-line utility to monitor system metrics in horizon chart format. It was originally created for Apple M1/M2 devices, but now works on Linux with nVidia GPU as well, including Google Colab environment.
+cubestat is a command-line utility to monitor system metrics in horizon chart format. It was originally created for Apple M1/M2 devices, but supports Linux with NVIDIA GPU as well, including Google Colab environment.
+Numerous tools exist for tracking system metrics, yet horizon charts stand out due to their good information density which enables the display of many time-series data on a single screen.
 
 Let's start with an example:
 
-In the clip below we see Mixtral-8x7b inference on MacBook Air with FF layers offloaded to SSD. 
-We can notice somewhat low GPU util (not good), 2Gb/s+ of data read from disk (as we have to fetch the weights), but plenty of free RAM (And we are actually able to serve almost 100Gb model on 24Gb machine with fp16 precision).
-We can also see the disk writes before the inference started - that was model preprocessing which was writing the weights to disk individually.
-
-
 https://github.com/okuvshynov/cubestat/assets/661042/8e1e405e-ca61-4ffb-bedb-e04eb33f8bc2
 
+In the clip above we see Mixtral-8x7b inference on MacBook Air with FF layers offloaded to SSD. 
+We can notice somewhat low GPU util, 2Gb/s+ of data read from disk, as we have to fetch the weights, but plenty of free RAM (And we are actually able to serve almost 100Gb model on 24Gb machine with fp16 precision, even if very slow).
+
+We can also clearly see moment of change from model loading (cpu util, disk writes for model preprocessing) to model inference (disk reads, gpu util going up, cpu going down)
 
 Currently cubestat reports:
-1. CPU utilization - configurable per core ('expanded'), cluster of cores: Efficiency/Performance ('cluster') or both. Is shown as percentage.
-2. GPU utilization per card/chip. Is shown in percentage. Works for Apple's M1/M2 SoC and nVidia GPUs. For nVidia GPU shows memory usage as well.
-3. ANE (Apple's Neural Engine) power consumption. According to `man powermetrics` it is an estimate, but seems working good enough as a proxy to ANE utilization. Is shown as percentage.
+1. CPU utilization - configurable per core ('by_core'), cluster of cores on Apple M1+: Efficiency/Performance ('by_cluster') or all. Is shown as percentage.
+2. GPU utilization per card/chip. Is shown in percentage. Works for Apple's M1/M2 SoC and NVIDIA GPUs. For NVIDIA GPU can show VRAM usage as well. In case of multi-GPU can show individual GPUs or aggregated average.
+3. ANE (Neural Engine) power consumption. According to `man powermetrics` it is an estimate, but seems working good enough as a proxy to ANE utilization. Is shown as percentage.
 4. Disk and network IO; Is shown as rate (Kb/s, Mb/s, Gb/s).
 5. Memory usage in %
 6. Swap usage. Is shown as absolute value (Kb, Mb, Gb)
 
-Despite many monitoring tools available for monitoring system counters, horizon charts have nice information density properties which make it possible to show a history of N measurements for M metrics on a single screen for significantly large N and M. Thus, this tool was created.
+Known limitations:
+1. **On MacOS cubestat needs to run `powermetrics` with sudo**. You don't need to run cubestat itself with sudo, but you'll be asked sudo password when cubestat launches powermetrics. If you are comfortable doing that, you can add `powermetrics` to `/etc/sudoers` (`your_user_name ALL=(ALL) NOPASSWD: /usr/bin/powermetrics`) and avoid this.
+2. Neural engine utilization is an estimate based on power usage, more on that below.
+3. Needs 256 colors terminal
 
-## Installation and Usage:
+## Installation:
 
 ```
-pip install cubestat
+% pip install cubestat
+```
 
-usage: cubestat [-h] [--refresh_ms REFRESH_MS] [--buffer_size BUFFER_SIZE] [--cpu {all,by_cluster,by_core}] [--color {red,green,blue,mixed}] [--percentages {hidden,last}] [--disk] [--network] [--no-disk] [--no-network]
+or 
+
+```
+% pip install cubestat[cuda] # for instances with NVIDIA
+```
+
+## Usage
+
+```
+% cubestat [-h] [--refresh_ms REFRESH_MS] [--buffer_size BUFFER_SIZE] [--cpu {all,by_cluster,by_core}]
+                [--gpu {collapsed,load_only,load_and_vram}] [--color {red,green,blue,pink,mixed}]
+                [--percentages {hidden,last}] [--disk] [--swap] [--network] [--no-disk] [--no-swap] [--no-network]
 
 options:
   -h, --help            show this help message and exit
   --refresh_ms REFRESH_MS, -i REFRESH_MS
                         Update frequency, milliseconds
   --buffer_size BUFFER_SIZE
-                        How many datapoints to store. Having it larger than screen width is a good idea as terminal window can be resized
+                        How many datapoints to store. Having it larger than screen width is a good idea as terminal window
+                        can be resized
   --cpu {all,by_cluster,by_core}
                         CPU mode - showing all cores, only cumulative by cluster or both. Can be toggled by pressing c.
-  --color {red,green,blue,mixed}
+  --gpu {collapsed,load_only,load_and_vram}
+                        GPU mode - hidden, showing all GPUs load, or showing load and vram usage. Can be toggled by pressing
+                        g.
+  --color {red,green,blue,pink,mixed}
   --percentages {hidden,last}
                         Show/hide numeric utilization percentage. Can be toggled by pressing p.
   --disk                Show disk read/write. Can be toggled by pressing d.
+  --swap                Show swap . Can be toggled by pressing s.
   --network             Show network io. Can be toggled by pressing n.
   --no-disk             Hide disk read/write. Can be toggled by pressing d.
+  --no-swap             Hide swap. Can be toggled by pressing s.
   --no-network          Hide network io. Can be toggled by pressing n.
 ```
 
 Interactive commands:
 * q - quit
-* p - show/hide percentage for last data point
+* p - show/hide values for last data point
 * c - change cpu display mode (individual cores, aggregated or both)
+* g - change gpu display mode (individual gpus, aggregated and optionally VRAM usage)
 * d - show/hide disk reads/writes
 * n - show/hide network utilization
+* s - show/hide swap
 * UP/DOWN - scroll the lines in case there are more cores;
 * LEFT/RIGHT - scroll left/right. Autorefresh is paused when user scrolled to non-latest position. To resume autorefresh either scroll back to the right or press '0';
 * 0 - reset horizontal scroll, continue autorefresh.
 
-Running on Apple devices will require sudo access, as `powermetrics` has this limitation. If you are comfortable doing that, you can update /etc/sudoers to not require password to run powermetrics.
+## Notes and examples
+
+### Multi-gpu example 
 
-Running on Linux doesn't require sudo.
+https://github.com/okuvshynov/cubestat/assets/661042/c5e0750d-9bbd-4636-a1ea-71cc75ebbadb
 
-Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 GPU instance:
-![multigpu](static/multigpu.png)
+We see a workload with uneven distribution between 4 GPUs installed. By pressing 'g' we can toggle the view mode to either show aggregate load, per GPU load or per GPU load and VRAM usage.
 
-## Apple Neural Engine utilization
+### Apple Neural Engine utilization
 
-A few notes on 'what does this even represent?'. Utilization we report is essentially power consumption reported by powermetrics.
-To convert it to % we divide it by some 'maximum' value observed in experimentation. There are many drawbacks to this:
-* The concept of 'utilization' overall it pretty ambiguous, e.g. for a x86 CPU - when CPU is wasting cycles on a cache miss, is it 'utilized' or not? If CPU is doing scalar instructions on 1 execution port rather than vectorized instructions on several ports, is it 'utilized' or not?
+A few notes on 'what does this even represent?'. Utilization we show is essentially current power consumption reported by powermetrics. To convert it to % we divide it by some maximum value observed in experimentation. When reading this metric, be aware:
+* The concept of 'utilization' overall it pretty ambiguous, e.g. when CPU is wasting cycles on a cache miss, is it 'utilized' or not? If CPU is doing scalar instructions on 1 execution port rather than vectorized instructions on several ports, is it 'utilized' or not?
 * It is unclear if power consumption is a decent proxy for utilization;
-* The upper bound must be different for different models (M1, M1 Max, M2, etc.). Need to identify the model and do tests for them.
-* It is unclear if my tests are actually hitting upperbound. The highest I could achieve was multiple layers of convolutions with no non-linearities between them;
+* The upper bound must be different for different models (M1, M1 Max, M2, etc.). I tested it on M1, M2 and M1 Pro only;
+* It is unclear if my tests are actually hitting upperbound. The highest I could achieve was [multiple layers of convolutions with no non-linearities between them](scripts/apple_loadgen.py#L26-L31);
 
-## Running on Google Colab 
+### Running on Google Colab 
 
 We can run cubestat on Google Colab instances to monitor GPU/CPU/IO usage.
 
 First cell:
 ```
-!pip install cubestat
+!pip install cubestat[cuda]
 !pip install colab-xterm
-!pip install pynvml
 %load_ext colabxterm
 # export TERM=xterm-256color <---- RUN THIS IN TERMINAL
 # cubestat                   <---- RUN THIS IN TERMINAL
 ```
 
 Start xterm:
 ```
@@ -101,25 +123,17 @@
 
 ![colab cubestat](static/colab_cubestat.png)
 
 
 ## Dependencies
 * Python 3.?+
 * psutil 5.9.5+
-* [optional] pynvml for nVidia cards monitoring
+* [optional] pynvml for NVIDIA cards monitoring
 
 ## TODO
-* Apple Neural Engine correct scale.
-* GPU aggregation
-* CPU by socket/NUMA/SMT
-* status line (why though?)
-* better colors (especially for dark background)
+* better colors for dark background
 * multi-column layout for large instances (e.g. with 100+ cores)
-* try on Windows and BSD
-* Google TPU load?
-* AMD GPU load?
-* Filter by process?
 * joint scale for IO
-* logging 
-* showing time? 
-* storing history?
-* io by interface/disk 
+* showing time
+* show help
+* storing history
+* all of https://github.com/okuvshynov/cubestat/issues
```

### Comparing `cubestat-0.2.5/cubestat/cubestat.py` & `cubestat-0.2.6/cubestat/cubestat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
 import collections
 import curses
 import itertools
+import os
 import sys
 
 from enum import Enum
 from math import floor
 from threading import Thread, Lock
 
 from cubestat.readers.linux_reader import LinuxReader
@@ -26,26 +27,35 @@
     hidden = 'hidden'
     last = 'last'
     
 class CPUMode(EnumLoop, EnumStr):
     all = 'all'
     by_cluster = 'by_cluster'
     by_core = 'by_core'
+
+class GPUMode(EnumLoop, EnumStr):
+    collapsed = 'collapsed'
+    load_only = 'load_only'
+    load_and_vram = 'load_and_vram'
     
 class Color(EnumStr):
     red = 'red'
     green = 'green'
     blue = 'blue'
     pink = 'pink'
     mixed = 'mixed'
 
+def auto_cpu_mode():
+     return CPUMode.all if os.cpu_count() < 40 else CPUMode.by_cluster
+
 parser = argparse.ArgumentParser("cubestat")
 parser.add_argument('--refresh_ms', '-i', type=int, default=1000, help='Update frequency, milliseconds')
 parser.add_argument('--buffer_size', type=int, default=500, help='How many datapoints to store. Having it larger than screen width is a good idea as terminal window can be resized')
-parser.add_argument('--cpu', type=CPUMode, default=CPUMode.all, choices=list(CPUMode), help='CPU mode - showing all cores, only cumulative by cluster or both. Can be toggled by pressing c.')
+parser.add_argument('--cpu', type=CPUMode, default=auto_cpu_mode(), choices=list(CPUMode), help='CPU mode - showing all cores, only cumulative by cluster or both. Can be toggled by pressing c.')
+parser.add_argument('--gpu', type=GPUMode, default=GPUMode.load_only, choices=list(GPUMode), help='GPU mode - hidden, showing all GPUs load, or showing load and vram usage. Can be toggled by pressing g.')
 parser.add_argument('--color', type=Color, default=Color.mixed, choices=list(Color))
 parser.add_argument('--percentages', type=Percentages, default=Percentages.last, choices=list(Percentages), help='Show/hide numeric utilization percentage. Can be toggled by pressing p.')
 parser.add_argument('--disk', action="store_true", default=True, help="Show disk read/write. Can be toggled by pressing d.")
 parser.add_argument('--swap', action="store_true", default=True, help="Show swap . Can be toggled by pressing s.")
 parser.add_argument('--network', action="store_true", default=True, help="Show network io. Can be toggled by pressing n.")
 parser.add_argument('--no-disk', action="store_false", dest="disk", help="Hide disk read/write. Can be toggled by pressing d.")
 parser.add_argument('--no-swap', action="store_false", default=True, help="Hide swap. Can be toggled by pressing s.")
@@ -65,30 +75,32 @@
         self.filling = '.'
 
         self.cells = self.prepare_cells()
         self.stdscr = stdscr
 
         # all of the fields below are mutable and can be accessed from 2 threads
         self.lock = Lock()
-        self.data = {k: collections.defaultdict(lambda: collections.deque(maxlen=args.buffer_size)) for k in ['cpu', 'ram', 'swap', 'accelerators',  'disk', 'network']}
+        self.data = {k: collections.defaultdict(lambda: collections.deque(maxlen=args.buffer_size)) for k in ['cpu', 'ram', 'swap', 'gpu', 'ane', 'disk', 'network']}
         self.colormap = {
             'cpu': Color.green if args.color == Color.mixed else args.color,
             'ram': Color.pink if args.color == Color.mixed else args.color,
-            'accelerators': Color.red if args.color == Color.mixed else args.color,
+            'gpu': Color.red if args.color == Color.mixed else args.color,
+            'ane': Color.red if args.color == Color.mixed else args.color,
             'disk': Color.blue if args.color == Color.mixed else args.color,
             'network': Color.blue if args.color == Color.mixed else args.color,
             'swap': Color.pink if args.color == Color.mixed else args.color,
         }
         self.snapshots_observed = 0
         self.snapshots_rendered = 0
         self.percentage_mode = args.percentages
         self.cpumode = args.cpu
         self.show_disk = args.disk
         self.show_swap = args.swap
         self.show_network = args.network
+        self.gpumode = args.gpu
         self.settings_changed = False
         self.reader = reader
         self.vertical_shift = 0
         self.horizontal_shift = 0
 
     def prepare_cells(self):
         chrs = [' ', '▁', '▂', '▃', '▄', '▅', '▆', '▇', '█']
@@ -160,14 +172,15 @@
         # Each chart takes two lines, with format roughly
         # ╔ GPU util %........................................................................last:  4% ╗
         # ╚ ▁▁▁  ▁    ▁▆▅▄ ▁▁▁      ▂ ▇▃▃▂█▃▇▁▃▂▁▁▂▁▁▃▃▂▁▂▄▄▁▂▆▁▃▁▂▃▁▁▁▂▂▂▂▂▂▁▁▃▂▂▁▂▁▃▄▃ ▁▁▃▁▄▂▃▂▂▂▃▃▅▅ ╝
 
         with self.lock:
             i = 0
             skip = self.vertical_shift
+            is_multigpu = len(self.data['gpu']) > 1
             for group_name, group in self.data.items():
                 if group_name == 'disk' and not self.show_disk:
                     continue
                 if group_name == 'network' and not self.show_network:
                     continue
                 if group_name == 'swap' and not self.show_swap:
                     continue
@@ -180,14 +193,23 @@
                     if group_name == 'cpu':
                         if self.cpumode == CPUMode.by_cluster and title not in self.cpu_clusters:
                             continue
                         if self.cpumode == CPUMode.by_core and title in self.cpu_clusters:
                             continue
                         if self.cpumode == CPUMode.all and title not in self.cpu_clusters:
                             indent = '  '
+
+                    if group_name == 'gpu':
+                        if is_multigpu and self.gpumode == GPUMode.collapsed and "Total GPU" not in title:
+                            continue
+                        if self.gpumode == GPUMode.load_only and "vram" in title:
+                            continue
+                        if is_multigpu and "Total GPU" not in title:
+                            indent = '  '
+                    
                     if skip > 0:
                         skip -= 1
                         continue
 
                     # render title and left border, for example
                     #
                     # ╔ GPU util %
@@ -266,14 +288,18 @@
                 with self.lock:
                     self.percentage_mode = self.percentage_mode.next()
                     self.settings_changed = True
             if key == ord('c'):
                 with self.lock:
                     self.cpumode = self.cpumode.next()
                     self.settings_changed = True
+            if key == ord('g'):
+                with self.lock:
+                    self.gpumode = self.gpumode.next()
+                    self.settings_changed = True
             if key == ord('s'):
                 with self.lock:
                     self.show_swap = not self.show_swap
                     self.settings_changed = True
             if key == ord('d'):
                 with self.lock:
                     self.show_disk = not self.show_disk
```

### Comparing `cubestat-0.2.5/cubestat/readers/free_swap_reader.py` & `cubestat-0.2.6/cubestat/readers/free_swap_reader.py`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.5/cubestat/readers/linux_reader.py` & `cubestat-0.2.6/cubestat/readers/linux_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
         disk_load = psutil.disk_io_counters()
         nw_load = psutil.net_io_counters()
         d = self.interval_ms / 1000.0
 
         # TODO: numa nodes here?
         cpu_clusters = []
+        cpu_load = psutil.cpu_percent(percpu=True)
 
-        cluster_title = 'Total CPU Util, %'
+        cluster_title = f'[{len(cpu_load)}] Total CPU Util, %'
         cpu_clusters.append(cluster_title)
         total_load = 0.0
         res['cpu'][cluster_title] = 0.0
 
-        cpu_load = psutil.cpu_percent(percpu=True)
         for i, v in enumerate(cpu_load):
             title = f'CPU {i} util %'
             res['cpu'][title] = v
             total_load += v
         res['cpu'][cluster_title] = total_load / len(cpu_load)
 
-        res['accelerators'] = self.nv.read()
+        res['gpu'] = self.nv.read()
 
         if self.first:
             self.disk_read_last = disk_load.read_bytes
             self.disk_written_last = disk_load.write_bytes
             self.network_read_last = nw_load.bytes_recv
             self.network_written_last = nw_load.bytes_sent
             self.first = False
```

### Comparing `cubestat-0.2.5/cubestat/readers/swapusage_reader.py` & `cubestat-0.2.6/cubestat/readers/swapusage_reader.py`

 * *Files identical despite different names*

### Comparing `cubestat-0.2.5/setup.py` & `cubestat-0.2.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.2.5',
+    version='0.2.6',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
     description='Horizon chart in terminal for system monitoring',
     long_description='Horizon chart in terminal. Supports CPU/GPU/ANE/RAM/swap/IO monitoring for Apple M1/M2/M3, nVidia GPUs',
     packages=find_packages(),
     install_requires=[
         'psutil>=5.9.5',
```

