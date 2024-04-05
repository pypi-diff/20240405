# Comparing `tmp/turbx-0.3.8.tar.gz` & `tmp/turbx-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbx-0.3.8.tar", last modified: Tue Feb 13 17:18:16 2024, max compression
+gzip compressed data, was "turbx-0.3.9.tar", last modified: Fri Apr  5 11:43:38 2024, max compression
```

## Comparing `turbx-0.3.8.tar` & `turbx-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2024-02-13 17:18:16.331992 turbx-0.3.8/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.3.8/LICENSE
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2661 2024-02-13 17:18:16.331992 turbx-0.3.8/PKG-INFO
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.3.8/README.md
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)       38 2024-02-13 17:18:16.331992 turbx-0.3.8/setup.cfg
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2024-02-13 17:11:03.000000 turbx-0.3.8/setup.py
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2024-02-13 17:18:16.331992 turbx-0.3.8/turbx/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     3904 2024-02-13 17:10:40.000000 turbx-0.3.8/turbx/__init__.py
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1422302 2024-02-13 17:06:56.000000 turbx-0.3.8/turbx/turbx.py
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2024-02-13 17:18:16.331992 turbx-0.3.8/turbx.egg-info/
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2661 2024-02-13 17:18:16.000000 turbx-0.3.8/turbx.egg-info/PKG-INFO
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      203 2024-02-13 17:18:16.000000 turbx-0.3.8/turbx.egg-info/SOURCES.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        1 2024-02-13 17:18:16.000000 turbx-0.3.8/turbx.egg-info/dependency_links.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      143 2024-02-13 17:18:16.000000 turbx-0.3.8/turbx.egg-info/requires.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        6 2024-02-13 17:18:16.000000 turbx-0.3.8/turbx.egg-info/top_level.txt
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2024-04-05 11:43:38.476623 turbx-0.3.9/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.3.9/LICENSE
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2410 2024-04-05 11:43:38.476623 turbx-0.3.9/PKG-INFO
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)      918 2024-04-05 11:36:17.000000 turbx-0.3.9/README.md
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)       38 2024-04-05 11:43:38.476623 turbx-0.3.9/setup.cfg
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2200 2024-04-05 11:36:31.000000 turbx-0.3.9/setup.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2024-04-05 11:43:38.472623 turbx-0.3.9/turbx/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     4064 2024-04-05 11:33:21.000000 turbx-0.3.9/turbx/__init__.py
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1462080 2024-04-05 11:35:52.000000 turbx-0.3.9/turbx/turbx.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2024-04-05 11:43:38.476623 turbx-0.3.9/turbx.egg-info/
+-rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2410 2024-04-05 11:43:38.000000 turbx-0.3.9/turbx.egg-info/PKG-INFO
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      203 2024-04-05 11:43:38.000000 turbx-0.3.9/turbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        1 2024-04-05 11:43:38.000000 turbx-0.3.9/turbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      145 2024-04-05 11:43:38.000000 turbx-0.3.9/turbx.egg-info/requires.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        6 2024-04-05 11:43:38.000000 turbx-0.3.9/turbx.egg-info/top_level.txt
```

### Comparing `turbx-0.3.8/LICENSE` & `turbx-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `turbx-0.3.8/PKG-INFO` & `turbx-0.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
@@ -13,55 +13,49 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mpi4py>=3.1
-Requires-Dist: numpy>=1.22
-Requires-Dist: scipy>=1.8
-Requires-Dist: h5py>=3.6
-Requires-Dist: matplotlib>=3.6
-Requires-Dist: scikit-image>=0.19
+Requires-Dist: numpy>=1.25
+Requires-Dist: scipy>=1.11
+Requires-Dist: h5py>=3.10
+Requires-Dist: matplotlib>=3.8
+Requires-Dist: scikit-image>=0.22
 Requires-Dist: psutil>=5.9
-Requires-Dist: tqdm>=4.64
-Requires-Dist: cmocean>=2.0
+Requires-Dist: tqdm>=4.66
+Requires-Dist: cmocean>=3.0
 Requires-Dist: colorcet>=3.0
-Requires-Dist: cmasher>=1.6
+Requires-Dist: cmasher>=1.7
 
 # turbx
 [![PyPI version](https://badge.fury.io/py/turbx.svg)](https://badge.fury.io/py/turbx)
 [![Downloads](https://pepy.tech/badge/turbx)](https://pepy.tech/project/turbx)
 
 Extensible toolkit for analyzing turbulent flow datasets.
 
 Install with `pip`:
 
 ```
 pip install --upgrade --user turbx
 ```
 
-Documentation available at: https://iagappel.github.io/turbx
-
 `turbx` runs in `python3` and uses parallel `HDF5` (wrapped by `h5py`) for high-performance collective MPI-IO with `mpi4py`. This requires:
 
 - A `python3` installation (3.8+ recommended)
 - An MPI implementation such as `OpenMPI`
 - A parallel `HDF5` installation (must be compiled with `--enable-parallel`) 
 - `mpi4py` (optionally compiled from source)
 - `h5py` compiled with parallel configuration
 
-An environment configuration guide can be found here: https://iagappel.github.io/turbx/env
-
 Visualization of `HDF5` datasets is possible using `Paraview` with the use of `xdmf` data descriptor files, which are written automatically by calling `.make_xdmf()` on `turbx` data class (such as `rgd`) class instances.
```

### Comparing `turbx-0.3.8/README.md` & `turbx-0.3.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,16 @@
 
 Install with `pip`:
 
 ```
 pip install --upgrade --user turbx
 ```
 
-Documentation available at: https://iagappel.github.io/turbx
-
 `turbx` runs in `python3` and uses parallel `HDF5` (wrapped by `h5py`) for high-performance collective MPI-IO with `mpi4py`. This requires:
 
 - A `python3` installation (3.8+ recommended)
 - An MPI implementation such as `OpenMPI`
 - A parallel `HDF5` installation (must be compiled with `--enable-parallel`) 
 - `mpi4py` (optionally compiled from source)
 - `h5py` compiled with parallel configuration
 
-An environment configuration guide can be found here: https://iagappel.github.io/turbx/env
-
 Visualization of `HDF5` datasets is possible using `Paraview` with the use of `xdmf` data descriptor files, which are written automatically by calling `.make_xdmf()` on `turbx` data class (such as `rgd`) class instances.
```

### Comparing `turbx-0.3.8/setup.py` & `turbx-0.3.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,57 +7,55 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='turbx',
-    version='0.3.8',
+    version='0.3.9',
     description='Extensible toolkit for analyzing turbulent flow datasets',
     
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/iagappel/turbx',
     author='Jason A',
     maintainer='Jason A',
     #author_email='johndoe@gmail.com',
     license='MIT',
     packages=['turbx'],
     #packages=find_packages(exclude=('tests',)),
     install_requires=['mpi4py>=3.1',
-                      'numpy>=1.22',
-                      'scipy>=1.8',
-                      'h5py>=3.6',
-                      'matplotlib>=3.6',
-                      'scikit-image>=0.19',
+                      'numpy>=1.25',
+                      'scipy>=1.11',
+                      'h5py>=3.10',
+                      'matplotlib>=3.8',
+                      'scikit-image>=0.22',
                       'psutil>=5.9',
-                      'tqdm>=4.64',
-                      'cmocean>=2.0',
+                      'tqdm>=4.66',
+                      'cmocean>=3.0',
                       'colorcet>=3.0',
-                      'cmasher>=1.6',
+                      'cmasher>=1.7',
                       ],
     
     #setup_requires=['pytest-runner'],
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     #tests_require=['pytest'],
     platforms=['any'],
     
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
         'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Scientific/Engineering :: Visualization',
     ],
```

### Comparing `turbx-0.3.8/turbx/__init__.py` & `turbx-0.3.9/turbx/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 turbx
 
 Extensible toolkit for analyzing turbulent flow datasets
 '''
 
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 __author__ = 'Jason A'
 
 from .turbx import cgd
 from .turbx import rgd
 from .turbx import eas4
 from .turbx import ztmd
 from .turbx import lpd
@@ -35,14 +35,15 @@
 from .turbx import assemble_1d_fd_coeff_vector_custom
 from .turbx import gradient
 from .turbx import get_metric_tensor_3d
 from .turbx import get_metric_tensor_2d
 from .turbx import get_grid_quality_metrics_2d
 from .turbx import smoothstep
 from .turbx import stretch_1d_cluster_ends
+from .turbx import time_integrate_2d_seeder
 from .turbx import time_integrate_2d
 
 from .turbx import rect_to_cyl
 from .turbx import cyl_to_rect
 from .turbx import rotate_2d
 
 from .turbx import get_grad
@@ -56,14 +57,15 @@
 from .turbx import gulp
 
 from .turbx import format_time_string
 from .turbx import format_nbytes
 from .turbx import even_print
 
 from .turbx import set_mpl_env
+from .turbx import mpl_typeset_templates
 from .turbx import colors_table
 from .turbx import get_standard_colors
 from .turbx import cmap_Lch_edit
 from .turbx import colors_test_plot
 from .turbx import color_dict_to_tex
 from .turbx import get_Lch_colors
 from .turbx import hex2rgb
@@ -100,14 +102,15 @@
            'assemble_1d_fd_coeff_vector_custom',
            'gradient',
            'get_metric_tensor_3d',
            'get_metric_tensor_2d',
            'get_grid_quality_metrics_2d',
            'smoothstep',
            'stretch_1d_cluster_ends',
+           'time_integrate_2d_seeder',
            'time_integrate_2d',
            'rect_to_cyl',
            'cyl_to_rect',
            'rotate_2d',
            'get_grad',
            'get_curl',
            'get_overlapping_window_size',
@@ -115,14 +118,15 @@
            'ccor',
            'ccor_naive',
            'gulp',
            'format_time_string',
            'format_nbytes',
            'even_print',
            'set_mpl_env',
+           'mpl_typeset_templates',
            'colors_table',
            'get_standard_colors',
            'cmap_Lch_edit',
            'colors_test_plot',
            'color_dict_to_tex',
            'get_Lch_colors',
            'hex2rgb',
```

### Comparing `turbx-0.3.8/turbx/turbx.py` & `turbx-0.3.9/turbx/turbx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1409,27 +1409,27 @@
             float_bytes = dtype.itemsize
             data_gb = float_bytes*self.nt*self.nz*self.ny*self.nx / 1024**3
             shape  = (self.nt,self.nz,self.ny,self.nx)
             chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
             
             dsn = f'data/{scalar}'
             
-            self.usingmpi: self.comm.Barrier()
+            if self.usingmpi: self.comm.Barrier()
             t_start = timeit.default_timer()
             
             if verbose:
                 even_print(f'initializing data/{scalar}', f'{data_gb:0.2f} [GB]')
             
             dset = self.create_dataset(dsn, 
                                        shape=shape, 
                                        dtype=dtype,
                                        chunks=chunks,
                                        )
             
-            self.usingmpi: self.comm.Barrier()
+            if self.usingmpi: self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
             if verbose: even_print(f'initialize data/{scalar}', f'{data_gb:0.2f} [GB]  {t_delta:0.2f} [s]  {(data_gb/t_delta):0.3f} [GB/s]')
             
             chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
             if verbose:
                 even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                 even_print('chunk size', f'{int(round(chunk_kb_)):d} [KB]')
@@ -2750,15 +2750,15 @@
         
         self.scalars = ['u','v','w']
         #self.scalars = ['u']
         self.scalars_dtypes = [ np.float32 for s in self.scalars ]
         
         ## initialize datasets
         data_gb = 4*nx*ny*nz*nt / 1024.**3
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_start = timeit.default_timer()
         for scalar in self.scalars:
             if ('data/%s'%scalar in self):
                 del self['data/%s'%scalar]
             if verbose:
                 even_print('initializing data/%s'%(scalar,),'%0.2f [GB]'%(data_gb,))
             dset = self.create_dataset('data/%s'%scalar, 
@@ -2766,25 +2766,25 @@
                                         dtype=np.float32,
                                         chunks=chunks )
             
             chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
             if verbose:
                 even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                 even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_initialize = timeit.default_timer() - t_start
         
         if verbose: print(72*'-')
         
         # ===
         
         ## 5D [scalar][x,y,z,t] structured array --> data buffer
         data = np.zeros(shape=(nxr,nyr,nzr,ntr), dtype={'names':self.scalars, 'formats':self.scalars_dtypes})
         
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_start = timeit.default_timer()
         
         if False: ## ABC Flow
             
             A = np.sqrt(3)
             B = np.sqrt(2)
             C = 1.
@@ -2802,31 +2802,31 @@
         
         if True: ## random data
             
             rng = np.random.default_rng(seed=self.rank)
             for scalar in self.scalars:
                 data[scalar] = rng.uniform(-1, +1, size=(nxr,nyr,nzr,ntr)).astype(np.float32)
         
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_delta = timeit.default_timer() - t_start
         if verbose: even_print('gen data','%0.3f [s]'%(t_delta,))
         
         ## write data
         data_gb_write = 0.
         t_write = 0.
         for scalar in self.scalars:
             ds = self['data/%s'%scalar]
-            self.usingmpi: self.comm.Barrier()
+            if self.usingmpi: self.comm.Barrier()
             t_start = timeit.default_timer()
             if self.usingmpi:
                 with ds.collective:
                     ds[rt1:rt2,rz1:rz2,ry1:ry2,rx1:rx2] = data[scalar].T
             else:
                 ds[:,:,:,:] = data[scalar].T
-            self.usingmpi: self.comm.Barrier()
+            if self.usingmpi: self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
             data_gb = 4*nx*ny*nz*nt / 1024**3
             
             t_write       += t_delta
             data_gb_write += data_gb
             
             if verbose:
@@ -3850,15 +3850,15 @@
         tau_wall     = mu_wall * dds2_u1_wall
         q_wall       = self.cp * mu_wall / self.Pr * dds2_T ### wall heat flux
         
         ## friction velocity
         u_tau  = np.sqrt(tau_wall/rho_wall)
         #y_plus = np.copy( s2 * u_tau / nu_wall )
         
-        # === populate 1D & 2D arrays using calc_bl_edge_1d(), calc_d99_1d()
+        # === populate 1D & 2D arrays using calc_profile_edge_1d(), calc_d99_1d()
         
         psvel = np.zeros((nx,ny), dtype=np.float64)
         
         psvel_edge = np.zeros((nx,), dtype=np.float64)
         u1_edge    = np.zeros((nx,), dtype=np.float64)
         rho_edge   = np.zeros((nx,), dtype=np.float64)
         mu_edge    = np.zeros((nx,), dtype=np.float64)
@@ -3873,15 +3873,15 @@
         for i in range(nx):
             
             vort_z_ = np.copy( vort_z[i,:] )
             psvel_  = sp.integrate.cumulative_trapezoid(-1*vort_z_, s2, initial=0.)
             psvel[i,:] = psvel_
             
             ## get edge
-            s2_edge_ = calc_bl_edge_1d( y=s2, psvel=psvel_, ynorm=self.lchar, acc=acc, edge_stencil=edge_stencil, epsilon=epsilon )
+            s2_edge_ = calc_profile_edge_1d( y=s2, u=psvel_, lchar=self.lchar, acc=acc, edge_stencil=edge_stencil, epsilon=epsilon )
             #aa = ( s2_edge_ - s2.min() ) / ( s2.max() - s2.min() )
             #tqdm.write(f'{aa:0.9f}')
             s2_edge[i] = s2_edge_
             
             ## interpolate at edge
             psvel_edge_ = sp.interpolate.interp1d(s2, psvel_ , kind='cubic', bounds_error=True)(s2_edge_)
             psvel_edge_ = float(psvel_edge_)
@@ -3890,37 +3890,37 @@
             u1_edge[i]  = sp.interpolate.interp1d(s2, utang[i,:] , kind='cubic', bounds_error=True)(s2_edge_)
             rho_edge[i] = sp.interpolate.interp1d(s2, rho[i,:]   , kind='cubic', bounds_error=True)(s2_edge_)
             mu_edge[i]  = sp.interpolate.interp1d(s2, mu[i,:]    , kind='cubic', bounds_error=True)(s2_edge_)
             nu_edge[i]  = sp.interpolate.interp1d(s2, nu[i,:]    , kind='cubic', bounds_error=True)(s2_edge_)
             T_edge[i]   = sp.interpolate.interp1d(s2, T[i,:]     , kind='cubic', bounds_error=True)(s2_edge_)
             
             ## get d99
-            d99_ = calc_d99_1d( y=s2, y_edge=s2_edge_, psvel=psvel_, psvel_edge=psvel_edge_ )
+            d99_ = calc_d99_1d( y=s2, u=psvel_, y_edge=s2_edge_, u_edge=psvel_edge_ )
             d99_ = float(d99_)
             d99[i] = d99_
             
-            u1_99[i] = sp.interpolate.interp1d(s2, utang[i,:] , kind='cubic', bounds_error=True)(d99_)
+            u1_99[i] = sp.interpolate.interp1d(s2, utang[i,:], kind='cubic', bounds_error=True)(d99_)
         
         # === avg in [x]/[s1] --> leave [y]/[s2]
         
         psvel = np.mean( psvel , axis=0 )
         utang = np.mean( utang , axis=0 )
         rho   = np.mean( rho   , axis=0 )
         
-        psvel_edge  = np.mean( psvel_edge )
-        u1_edge     = np.mean( u1_edge    )
-        rho_edge    = np.mean( rho_edge   )
-        mu_edge     = np.mean( mu_edge    )
-        nu_edge     = np.mean( nu_edge    )
-        T_edge      = np.mean( T_edge     )
+        psvel_edge  = np.mean( psvel_edge , axis=0 )
+        u1_edge     = np.mean( u1_edge    , axis=0 )
+        rho_edge    = np.mean( rho_edge   , axis=0 )
+        mu_edge     = np.mean( mu_edge    , axis=0 )
+        nu_edge     = np.mean( nu_edge    , axis=0 )
+        T_edge      = np.mean( T_edge     , axis=0 )
         
-        s2_edge     = np.mean( s2_edge     )
-        d99         = np.mean( d99        )
+        s2_edge     = np.mean( s2_edge  , axis=0 )
+        d99         = np.mean( d99      , axis=0 )
         
-        u1_99       = np.mean( u1_99      )
+        u1_99       = np.mean( u1_99 , axis=0 )
         
         sc_l_out = d99
         sc_u_out = u1_99
         sc_t_out = d99/u1_99
         np.testing.assert_allclose(sc_t_out, sc_l_out/sc_u_out, rtol=1e-14, atol=1e-14)
         
         sc_u_in = u_tau
@@ -4009,15 +4009,15 @@
             even_print('δ99'                       , '%0.5e [m]'%d99                 )
             even_print('θ/δ99'                     , '%0.5f'%(dd['theta_cmp']/d99)   )
             even_print('δ*/δ99'                    , '%0.5f'%(dd['dstar_cmp']/d99)   )
             even_print('u_τ'                       , '%0.3f [m/s]'%u_tau             )
             even_print('ν_wall'                    , '%0.5e [m²/s]'%nu_wall          )
             even_print('τ_wall'                    , '%0.5e [Pa]'%tau_wall           )
             even_print('τ_wall/q_inf'              , '%0.5e'%(tau_wall/(self.rho_inf*self.U_inf**2)) )
-            even_print('cf = 2·τ_wall/q_edge'      , '%0.5e'%(2*tau_wall/(rho_edge*u_edge**2)) )
+            even_print('cf = 2·τ_wall/q_edge'      , '%0.5e'%(2*tau_wall/(rho_edge*u1_edge**2)) )
             even_print('t_meas'                    , '%0.5e [s]'%t_meas              )
             even_print('t_meas/tchar'              , '%0.1f'%(t_meas/self.tchar)     )
             even_print('t_eddy = t_meas/(δ99/u_τ)' , '%0.2f'%t_eddy                  )
             even_print('t_meas/(δ99/u1_99)'        , '%0.2f'%(t_meas/(d99/u1_99))    )
             even_print('t_meas/(20·δ99/u1_99)'     , '%0.2f'%(t_meas/(20*d99/u1_99)) )
             print(72*'-')
             even_print('sc_u_in = u_τ'               , '%0.5e [m/s]'%(sc_u_in,)  )
@@ -6838,15 +6838,15 @@
         nx = self.nx ; data['nx'] = nx
         ny = self.ny ; data['ny'] = ny
         nz = self.nz ; data['nz'] = nz
         nt = self.nt ; data['nt'] = nt
         
         t = np.copy( self['dims/t'][()] * self.tchar )
         
-        ## read in 1D coordinate arrays, then dimensinoalize [m]
+        ## read in 1D coordinate arrays, then dimensionalize [m]
         stang_ = np.copy(self['dims/stang'])
         stang  = np.copy( stang_ * self.lchar ) ## dimensional [m]
         data['stang'] = stang
         
         snorm_ = np.copy(self['dims/snorm'])
         snorm  = np.copy( snorm_ * self.lchar ) ## dimensional [m]
         data['snorm'] = snorm
@@ -7200,14 +7200,527 @@
         
         return
     
     def calc_turb_spectrum_time_xpln(self, **kwargs):
         raise NotImplementedError
         return
     
+    def calc_ccor_span(self, **kwargs):
+        '''
+        calculate cross-correlation in [z] and avg in [x,t] --> leave [y,Δz]
+        - designed for analyzing unsteady, thin planes in [x]
+        '''
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        if verbose: print('\n'+'cgd.calc_ccor_span()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        rx = kwargs.get('rx',1)
+        ry = kwargs.get('ry',1)
+        rz = kwargs.get('rz',1)
+        rt = kwargs.get('rt',1)
+        
+        fn_dat_ccor_span = kwargs.get('fn_dat_ccor_span',None)
+        #fn_dat_mean_dim  = kwargs.get('fn_dat_mean_dim',None)
+        
+        ## assert that a CGD with (fsubtype=='prime') was opened
+        if (self.fsubtype!='prime'):
+            raise ValueError("fsubtype!='prime'")
+        
+        ## for now only distribute data in [y]
+        if (rx!=1):
+            raise AssertionError('rx!=1')
+        if (rz!=1):
+            raise AssertionError('rz!=1')
+        if (rt!=1):
+            raise AssertionError('rt!=1')
+        
+        if (rx*ry*rz*rt != self.n_ranks):
+            raise AssertionError('rx*ry*rz*rt != self.n_ranks')
+        if (rx>self.nx):
+            raise AssertionError('rx>self.nx')
+        if (ry>self.ny):
+            raise AssertionError('ry>self.ny')
+        if (rz>self.nz):
+            raise AssertionError('rz>self.nz')
+        if (rt>self.nt):
+            raise AssertionError('rt>self.nt')
+        
+        # ===
+        
+        #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
+        #t4d = comm4d.Get_coords(self.rank)
+        
+        #rxl_ = np.array_split(np.array(range(self.nx),dtype=np.int64),min(rx,self.nx))
+        ryl_ = np.array_split(np.array(range(self.ny),dtype=np.int64),min(ry,self.ny))
+        #rzl_ = np.array_split(np.array(range(self.nz),dtype=np.int64),min(rz,self.nz))
+        #rtl_ = np.array_split(np.array(range(self.nt),dtype=np.int64),min(rt,self.nt))
+        
+        #rxl = [[b[0],b[-1]+1] for b in rxl_ ]
+        ryl = [[b[0],b[-1]+1] for b in ryl_ ]
+        #rzl = [[b[0],b[-1]+1] for b in rzl_ ]
+        #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
+        
+        #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
+        #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
+        #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
+        #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
+        
+        ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
+        
+        # # === mean dimensional file name (for reading) : .dat
+        # if (fn_dat_mean_dim is None):
+        #     fname_path = os.path.dirname(self.fname)
+        #     fname_base = os.path.basename(self.fname)
+        #     fname_root, fname_ext = os.path.splitext(fname_base)
+        #     fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+        #     fname_dat_mean_base = fname_root+'_mean_dim.dat'
+        #     fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
+        
+        # === cross-correlation file name (for writing) : dat
+        if (fn_dat_ccor_span is None):
+            fname_path = os.path.dirname(self.fname)
+            fname_base = os.path.basename(self.fname)
+            fname_root, fname_ext = os.path.splitext(fname_base)
+            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+            fname_ccor_span_dat_base = fname_root+'_ccor_span.dat'
+            fn_dat_ccor_span = str(PurePosixPath(fname_path, fname_ccor_span_dat_base))
+        
+        if verbose: even_print('fn_cgd_prime'     , self.fname       )
+        #if verbose: even_print('fn_dat_mean_dim'  , fn_dat_mean_dim  )
+        if verbose: even_print('fn_dat_ccor_span' , fn_dat_ccor_span )
+        if verbose: print(72*'-')
+        
+        # if not os.path.isfile(fn_dat_mean_dim):
+        #     raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
+        
+        # # === read in data (mean dim) --> every rank gets full [x,z]
+        # with open(fn_dat_mean_dim,'rb') as f:
+        #     data_mean_dim = pickle.load(f)
+        # fmd = type('foo', (object,), data_mean_dim)
+        
+        self.comm.Barrier()
+        
+        ## the data dictionary to be pickled later
+        data = {}
+        
+        if ('data_dim' not in self):
+            raise ValueError('group data_dim not present')
+        
+        ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+        for dsn in self['data_dim'].keys():
+            d_ = np.copy( self[f'data_dim/{dsn}'][()] )
+            if (d_.ndim == 0):
+                d_ = float(d_)
+            data[dsn] = d_
+        
+        ## 1D
+        rho_avg = np.copy( self['data_dim/rho'][()] )
+        #u_avg   = np.copy( self['data_dim/u'][()]   )
+        utang   = np.copy( self['data_dim/utang'][()] )
+        
+        ## 0D
+        u_tau    = float( self['data_dim/u_tau'][()]    )
+        nu_wall  = float( self['data_dim/nu_wall'][()]  )
+        rho_wall = float( self['data_dim/rho_wall'][()] )
+        d99      = float( self['data_dim/d99'][()]      )
+        #u_99     = float( self['data_dim/u_99'][()]     )
+        u1_99     = float( self['data_dim/u1_99'][()]     )
+        Re_tau   = float( self['data_dim/Re_tau'][()]   )
+        Re_theta = float( self['data_dim/Re_theta'][()] )
+        sc_u_in  = float( self['data_dim/sc_u_in'][()]  )
+        sc_l_in  = float( self['data_dim/sc_l_in'][()]  )
+        sc_t_in  = float( self['data_dim/sc_t_in'][()]  )
+        sc_u_out = float( self['data_dim/sc_u_out'][()] )
+        sc_l_out = float( self['data_dim/sc_l_out'][()] )
+        sc_t_out = float( self['data_dim/sc_t_out'][()] )
+        
+        ## these are recalculated and checked in next step
+        z1d_ = np.copy( self['data_dim/z1d'][()] )
+        dz0_ = np.copy( self['data_dim/dz0'][()] )
+        dt_  = np.copy( self['data_dim/dt'][()]  )
+        
+        # ===
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        ## 0D scalars
+        lchar   = self.lchar   ; data['lchar']   = lchar
+        U_inf   = self.U_inf   ; data['U_inf']   = U_inf
+        rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
+        T_inf   = self.T_inf   ; data['T_inf']   = T_inf
+        
+        #data['M_inf'] = self.M_inf
+        data['Ma'] = self.Ma
+        data['Pr'] = self.Pr
+        
+        ## read in 3D coordinate arrays, then dimensionalize [m]
+        ## every ranks gets full grid
+        x = np.copy( self['dims/x'][()].T * self.lchar )
+        y = np.copy( self['dims/y'][()].T * self.lchar )
+        z = np.copy( self['dims/z'][()].T * self.lchar )
+        
+        nx = self.nx ; data['nx'] = nx
+        ny = self.ny ; data['ny'] = ny
+        nz = self.nz ; data['nz'] = nz
+        nt = self.nt ; data['nt'] = nt
+        
+        t = np.copy( self['dims/t'][()] * self.tchar )
+        
+        ## read in 1D coordinate arrays, then dimensionalize [m]
+        stang_ = np.copy(self['dims/stang'])
+        stang  = np.copy( stang_ * self.lchar ) ## dimensional [m]
+        data['stang'] = stang
+        
+        snorm_ = np.copy(self['dims/snorm'])
+        snorm  = np.copy( snorm_ * self.lchar ) ## dimensional [m]
+        data['snorm'] = snorm
+        
+        ## assert [z] is same over all [x,y]
+        if (z.ndim!=3):
+            raise ValueError
+        z1d = np.copy(z[0,0,:])
+        for i in range(nx):
+            for j in range(ny):
+                np.testing.assert_allclose(z1d, z[i,j,:], rtol=1e-14, atol=1e-14)
+        
+        ## assert [x,y] is same over all [z]
+        x2d  = np.copy(x[:,:,0])
+        y2d  = np.copy(y[:,:,0])
+        xy2d = np.stack((x2d,y2d), axis=-1)
+        for k in range(nz):
+            x2d_  = np.copy(x[:,:,k])
+            y2d_  = np.copy(y[:,:,k])
+            xy2d_ = np.stack((x2d_,y2d_), axis=-1)
+            np.testing.assert_allclose(xy2d, xy2d_, rtol=1e-14, atol=1e-14)
+        
+        ## check if constant Δz (calculate Δz+ later)
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration * self.tchar
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+        
+        ## check against values in 'data_dim' (imported above)
+        np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
+        
+        zrange = z1d.max() - z1d.min()
+        
+        #data['x'] = x
+        #data['y'] = y
+        #data['z'] = z
+        data['z1d'] = z1d
+        
+        data['t'] = t
+        data['t_meas'] = t_meas
+        data['dt'] = dt
+        data['dz0'] = dz0
+        data['zrange'] = zrange
+        
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
+        
+        ## report
+        if verbose:
+            #even_print('nx'     , '%i'        %nx     )
+            #even_print('ny'     , '%i'        %ny     )
+            #even_print('nz'     , '%i'        %nz     )
+            #even_print('nt'     , '%i'        %nt     )
+            #even_print('dt'     , '%0.5e [s]' % dt      )
+            #even_print('t_meas' , '%0.5e [s]' % t_meas  )
+            even_print('dz0'    , '%0.5e [m]' % dz0     )
+            even_print('zrange' , '%0.5e [m]' % zrange  )
+            print(72*'-')
+        
+        ## report
+        if verbose:
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
+            ##
+            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99)  )
+            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in)  )
+            print(72*'-')
+        
+        t_eddy = t_meas / ( d99 / u_tau )
+        
+        if verbose:
+            even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
+            #even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99/u_99)))
+            even_print('t_meas/(δ99/u1_99)'          , '%0.2f'%(t_meas/(d99/u1_99)))
+            #even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99/u_99)))
+            even_print('t_meas/(20·δ99/u1_99)'       , '%0.2f'%(t_meas/(20*d99/u1_99)))
+        
+        ## get lags
+        lags,_  = ccor( np.ones(nz,dtype=np.float32) , np.ones(nz,dtype=np.float32), get_lags=True )
+        n_lags_ = nz*2-1
+        n_lags  = lags.shape[0]
+        if (n_lags!=n_lags_):
+            raise AssertionError('possible problem with lags calc --> check!')
+        
+        if verbose:
+            even_print('n lags (Δz)' , '%i'%(n_lags,))
+        
+        ## [var1, var2, density_scaling]
+        R_combis = [
+                   # [ 'uI'  , 'uI'  , False ],
+                   # [ 'vI'  , 'vI'  , False ],
+                   # [ 'wI'  , 'wI'  , False ],
+                   # [ 'uI'  , 'vI'  , False ],
+                   # [ 'uI'  , 'TI'  , False ],
+                   # [ 'vI'  , 'TI'  , False ],
+                   # [ 'TI'  , 'TI'  , False ],
+                   # [ 'uII' , 'uII' , True  ],
+                   # [ 'vII' , 'vII' , True  ],
+                   # [ 'wII' , 'wII' , True  ],
+                   # [ 'uII' , 'vII' , True  ],
+                   # [ 'uII' , 'TII' , True  ],
+                   # [ 'vII' , 'TII' , True  ],
+                   # [ 'TII' , 'TII' , True  ],
+                   ##
+                   [ 'utangI' , 'utangI' , False ],
+                   [ 'unormI' , 'unormI' , False ],
+                   [ 'wI'     , 'wI'     , False ],
+                   [ 'utangI' , 'unormI' , False ],
+                   [ 'utangI' , 'wI'     , False ],
+                   ]
+        
+        if verbose:
+            even_print('n ccor (Δz) scalar combinations' , '%i'%(len(R_combis),))
+            print(72*'-')
+        
+        ## decide if density will be needed
+        read_density = False
+        for cc in R_combis:
+            scalar_L, scalar_R, density_scaling = cc
+            if density_scaling:
+                read_density = True
+                break
+        
+        if verbose:
+            even_print('read ρ', str(read_density))
+        
+        ## confirm 'rho' is not in locals
+        if read_density and ('rho' in locals()):
+            raise ValueError('rho alread in locals... check')
+        
+        if read_density:
+            
+            ## buffer for rho (NOT rhoI) --> this is read from 'prime' file
+            rho = np.zeros(shape=(nx, nyr, nz, nt), dtype=np.float32)
+            
+            dset = self['data/rho']
+            self.comm.Barrier()
+            t_start = timeit.default_timer()
+            with dset.collective:
+                rho[:,:,:,:] = dset[:,:,ry1:ry2,:].T
+            self.comm.Barrier()
+            t_delta = timeit.default_timer() - t_start
+            data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
+            if verbose:
+                even_print( 'read: rho','%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+            
+            ## re-dimensionalize rho
+            rho *= rho_inf
+        
+        scalars_R        = [ '%s%s'%(cc[0],cc[1]) for cc in R_combis ]
+        scalars_dtypes_R = [ np.float32 for s in scalars_R ]
+        
+        ## averaged cross-correlation data buffer
+        ## 3D [scalar][y,Δz] structured array
+        data_R_avg = np.zeros(shape=(nyr, n_lags), dtype={'names':scalars_R, 'formats':scalars_dtypes_R})
+        
+        ## main loop --> cross-correlation in [Δz] at every [x,y,t]
+        if verbose:
+            progress_bar = tqdm(total=len(R_combis)*nx*nyr*nt, ncols=100, desc='ccor_span()', leave=False, file=sys.stdout)
+        
+        for cci,cc in enumerate(R_combis):
+            
+            scalar_L, scalar_R, density_scaling = cc
+            tag = '%s%s'%(scalar_L, scalar_R)
+            
+            ## check if autocorrelation
+            if (scalar_L==scalar_R):
+                scalars = [ scalar_L ]
+            else:
+                scalars = [ scalar_L, scalar_R ]
+            
+            scalars_dtypes = [self.scalars_dtypes_dict[s] for s in scalars]
+            
+            ## prime data buffer
+            ## 5D [scalar][x,y,z,t] structured array
+            data_prime = np.zeros(shape=(nx, nyr, nz, nt), dtype={'names':scalars, 'formats':scalars_dtypes})
+            
+            ## cross-correlation data buffer
+            ## 5D [scalar][x,y,z,t] structured array
+            #scalars_R        = [ tag ]
+            #scalars_dtypes_R = [ np.float32 for s in scalars_R ]
+            #data_R           = np.zeros(shape=(nx, nyr, n_lags, nt), dtype={'names':scalars_R, 'formats':scalars_dtypes_R})
+            
+            ## cross-correlation data buffer
+            ## 4D numpy array
+            data_R = np.zeros(shape=(nx, nyr, n_lags, nt), dtype=np.float32)
+            
+            ## read prime data
+            for scalar in scalars:
+                dset = self['data/%s'%scalar]
+                self.comm.Barrier()
+                t_start = timeit.default_timer()
+                with dset.collective:
+                    data_prime[scalar][:,:,:,:] = np.copy( dset[:,:,ry1:ry2,:].T )
+                self.comm.Barrier()
+                t_delta = timeit.default_timer() - t_start
+                data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
+                if verbose:
+                    tqdm.write(even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True))
+            
+            ## redimensionalize prime data
+            for var in data_prime.dtype.names:
+                if var in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII', 'utangI','unormI', 'utangII','unormII']:
+                    data_prime[var] *= U_inf
+                elif var in ['r_uII','r_vII','r_wII']:
+                    data_prime[var] *= (U_inf*rho_inf)
+                elif var in ['T','TI','TII']:
+                    data_prime[var] *= T_inf
+                elif var in ['r_TII']:
+                    data_prime[var] *= (T_inf*rho_inf)
+                elif var in ['rho','rhoI']:
+                    data_prime[var] *= rho_inf
+                elif var in ['p','pI','pII']:
+                    data_prime[var] *= (rho_inf * U_inf**2)
+                else:
+                    raise ValueError('condition needed for redimensionalizing \'%s\''%var)
+            
+            # ===
+            
+            ## print names of components being cross-correlated
+            if verbose:
+                if density_scaling:
+                    fancy_tag = '<ρ·%s,ρ·%s>'%(scalar_L,scalar_R)
+                else:
+                    fancy_tag = '<%s,%s>'%(scalar_L,scalar_R)
+                tqdm.write(even_print('running Δz cross-correlation calc', fancy_tag, s=True))
+            
+            for xi in range(nx):
+                for yi in range(nyr):
+                    for ti in range(nt):
+                        
+                        uL = np.copy( data_prime[scalar_L][xi,yi,:,ti]   )
+                        uR = np.copy( data_prime[scalar_R][xi,yi,:,ti]   )
+                        
+                        if density_scaling:
+                            rho1d = np.copy( rho[xi,yi,:,ti] )
+                        else:
+                            rho1d = None
+                        
+                        if density_scaling:
+                            data_R[xi,yi,:,ti] = ccor( rho1d*uL , rho1d*uR )
+                        else:
+                            data_R[xi,yi,:,ti] = ccor( uL , uR )
+                        
+                        if verbose: progress_bar.update()
+            
+            # ===
+            
+            ## average in [x,t] --> leave [y,lag] (where lag is Δz)
+            data_R_avg[tag] = np.mean(data_R, axis=(0,3), dtype=np.float64).astype(np.float32)
+            data_R = None; del data_R
+            
+            ## manually delete the prime data from memory
+            data_prime = None; del data_prime
+            self.comm.Barrier()
+        
+        if verbose:
+            progress_bar.close()
+            print(72*'-')
+        
+        # === gather all (pre-averaged) results
+        
+        self.comm.Barrier()
+        data_R_all = None
+        if (self.rank==0):
+            
+            j=0
+            data_R_all = np.zeros(shape=(ny,n_lags), dtype={'names':scalars_R, 'formats':scalars_dtypes_R})
+            
+            ## data this rank
+            for scalar_R in scalars_R:
+                data_R_all[scalar_R][ryl[j][0]:ryl[j][1],:] = data_R_avg[scalar_R]
+        
+        for scalar_R in scalars_R:
+            for ri in range(1,self.n_ranks):
+                j = ri
+                self.comm.Barrier()
+                if (self.rank==ri):
+                    sendbuf = np.copy(data_R_avg[scalar_R])
+                    self.comm.Send(sendbuf, dest=0, tag=ri)
+                    #print('rank %i sending %s'%(ri,scalar_R))
+                elif (self.rank==0):
+                    #print('rank %i receiving %s'%(self.rank,scalar_R))
+                    nyri = ryl[j][1] - ryl[j][0]
+                    
+                    recvbuf = np.zeros((nyri,n_lags), dtype=data_R_avg[scalar_R].dtype)
+                    
+                    #print('rank %i : recvbuf.shape=%s'%(rank,str(recvbuf.shape)))
+                    self.comm.Recv(recvbuf, source=ri, tag=ri)
+                    data_R_all[scalar_R][ryl[j][0]:ryl[j][1],:] = recvbuf
+                else:
+                    pass
+        
+        ## overwrite
+        if (self.rank==0):
+            R = np.copy(data_R_all)
+        
+        # === save results
+        
+        if (self.rank==0):
+            
+            data['R']    = R ## the main cross-correlation data array
+            data['lags'] = lags
+            
+            with open(fn_dat_ccor_span,'wb') as f:
+                pickle.dump(data, f, protocol=4)
+            print('--w-> %s : %0.2f [MB]'%(fn_dat_ccor_span,os.path.getsize(fn_dat_ccor_span)/1024**2))
+        
+        # ===
+        
+        self.comm.Barrier()
+        if verbose: print(72*'-')
+        if verbose: print('total time : cgd.calc_ccor_span() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
     # === polydata (turbx.spd() file)
     
     def export_polydata_wall(self, fn_spd=None, **kwargs):
         '''
         get 2D [x,z] wall quantities, export structured polydata (SPD) file
         '''
         
@@ -7407,32 +7920,44 @@
                     if verbose: even_print(dsn,'%s'%str(ds.shape))
                 else:
                     if verbose: even_print(dsn,'not found')
             
             if verbose: print(72*'-')
             
             ## initialize datasets
-            data_gb = (self.nx * self.nz) * 4 / 1024**3
-            shape  = (self.nx,self.nz,self.nt)
+            dtype    = np.dtype(np.float32)
+            itemsize = dtype.itemsize
+            shape    = (self.nx,self.nz,self.nt)
+            data_gb  = np.prod(shape) * itemsize / 1024**3
+            
             chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=4)
             
             scalars_spd = [ 'tau_u1_s2', 'tau_u3_s2', 'T','rho','mu','nu','u_tau','p' ]
             
             for scalar in scalars_spd:
                 
-                if verbose:
-                    even_print(f'initializing data/{scalar}','%0.1f [GB]'%(data_gb,))
                 if (f'data/{scalar}' in hfspd):
                     del hfspd[f'data/{scalar}']
+                
+                if self.usingmpi: self.comm.Barrier()
+                t_start = timeit.default_timer()
+                
+                if verbose:
+                    even_print(f'initializing data/{scalar}','%0.1f [GB]'%(data_gb,))
+                
                 dset = hfspd.create_dataset(f'data/{scalar}',
                                             shape=shape,
-                                            dtype=np.float32,
-                                            chunks=chunks )
+                                            dtype=dtype,
+                                            chunks=chunks)
                 
-                chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
+                if self.usingmpi: self.comm.Barrier()
+                t_delta = timeit.default_timer() - t_start
+                if verbose: even_print(f'initialize data/{scalar}', f'{data_gb:0.2f} [GB]  {t_delta:0.2f} [s]  {(data_gb/t_delta):0.3f} [GB/s]')
+                
+                chunk_kb_ = np.prod(dset.chunks)*itemsize / 1024. ## actual
                 if verbose:
                     #even_print('chunk shape (t,z,x)','%s'%str(dset.chunks))
                     even_print('chunk shape (x,z,t)','%s'%str(dset.chunks))
                     even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
         
         if verbose: print(72*'-')
         
@@ -10014,27 +10539,27 @@
                         if verbose: even_print(f'dset {dsn} dtype matches', str(False))
                     
                     if ( dset.shape == shape ) and ( dset.chunks == chunks ) and ( dset.dtype == dtype ):
                         do_dset_initialize = False
             
             if do_dset_initialize:
                 
-                self.usingmpi: self.comm.Barrier()
+                if self.usingmpi: self.comm.Barrier()
                 t_start = timeit.default_timer()
                 
                 if verbose:
                     even_print(f'initializing data/{scalar}', f'{data_gb:0.2f} [GB]')
                 
                 dset = self.create_dataset(dsn, 
                                            shape=shape, 
                                            dtype=dtype,
                                            chunks=chunks,
                                            )
                 
-                self.usingmpi: self.comm.Barrier()
+                if self.usingmpi: self.comm.Barrier()
                 t_delta = timeit.default_timer() - t_start
                 if verbose: even_print(f'initialize data/{scalar}', f'{data_gb:0.2f} [GB]  {t_delta:0.2f} [s]  {(data_gb/t_delta):0.3f} [GB/s]')
             
             chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
             if verbose:
                 even_print('chunk shape (t,z,y,x)', str(dset.chunks))
                 even_print('chunk size', f'{int(round(chunk_kb_)):d} [KB]')
@@ -10989,15 +11514,15 @@
         
         #self.scalars = ['u','v','w']
         self.scalars = ['u']
         self.scalars_dtypes = [np.float32 for s in self.scalars]
         
         ## initialize datasets
         data_gb = 4*nx*ny*nz*nt / 1024.**3
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_start = timeit.default_timer()
         for scalar in self.scalars:
             if ('data/%s'%scalar in self):
                 del self['data/%s'%scalar]
             if verbose:
                 even_print('initializing data/%s'%(scalar,),'%0.2f [GB]'%(data_gb,))
             dset = self.create_dataset('data/%s'%scalar, 
@@ -11005,46 +11530,46 @@
                                         dtype=np.float32,
                                         chunks=chunks )
             
             chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
             if verbose:
                 even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                 even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_initialize = timeit.default_timer() - t_start
         
         ## 5D [scalar][x,y,z,t] structured array --> data buffer
         data = np.zeros(shape=(nxr,nyr,nzr,ntr), dtype={'names':self.scalars, 'formats':self.scalars_dtypes})
         
         ## generate data
         if verbose: print(72*'-')
         
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_start = timeit.default_timer()
         rng = np.random.default_rng(seed=self.rank)
         for scalar in self.scalars:
             data[scalar] = rng.uniform(-1, +1, size=(nxr,nyr,nzr,ntr)).astype(np.float32)
-        self.usingmpi: self.comm.Barrier()
+        if self.usingmpi: self.comm.Barrier()
         t_delta = timeit.default_timer() - t_start
         if verbose: even_print('gen data','%0.3f [s]'%(t_delta,))
         if verbose: print(72*'-')
         
         ## write data
         data_gb_write = 0.
         t_write = 0.
         for scalar in self.scalars:
             ds = self['data/%s'%scalar]
-            self.usingmpi: self.comm.Barrier()
+            if self.usingmpi: self.comm.Barrier()
             t_start = timeit.default_timer()
             if self.usingmpi:
                 with ds.collective:
                     ds[rt1:rt2,rz1:rz2,ry1:ry2,rx1:rx2] = data[scalar].T
             else:
                 ds[:,:,:,:] = data[scalar].T
-            self.usingmpi: self.comm.Barrier()
+            if self.usingmpi: self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
             data_gb = 4*nx*ny*nz*nt / 1024**3
             
             t_write       += t_delta
             data_gb_write += data_gb
             
             if verbose:
@@ -12036,15 +12561,15 @@
         tau_wall    = mu_wall * ddy_u_wall
         q_wall      = self.cp * mu_wall / self.Pr * ddy_T_wall ## wall heat flux (?)
         
         ## friction velocity
         u_tau  = np.sqrt(tau_wall/rho_wall)
         #y_plus = np.copy( s2 * u_tau / nu_wall )
         
-        # === populate 1D & 2D arrays using calc_bl_edge_1d(), calc_d99_1d()
+        # === populate 1D & 2D arrays using calc_profile_edge_1d(), calc_d99_1d()
         
         psvel = np.zeros((nx,ny), dtype=np.float64)
         
         psvel_edge = np.zeros((nx,), dtype=np.float64)
         u_edge     = np.zeros((nx,), dtype=np.float64)
         rho_edge   = np.zeros((nx,), dtype=np.float64)
         mu_edge    = np.zeros((nx,), dtype=np.float64)
@@ -12059,15 +12584,15 @@
         for i in range(nx):
             
             vort_z_ = np.copy( vort_z[i,:] )
             psvel_  = sp.integrate.cumulative_trapezoid(-1*vort_z_, y, initial=0.)
             psvel[i,:] = psvel_
             
             ## get edge
-            y_edge_ = calc_bl_edge_1d( y=y, psvel=psvel_, ynorm=self.lchar, acc=acc, edge_stencil=edge_stencil, epsilon=epsilon )
+            y_edge_ = calc_profile_edge_1d( y=y, psvel=psvel_, ynorm=self.lchar, acc=acc, edge_stencil=edge_stencil, epsilon=epsilon )
             #aa = ( y_edge_ - y.min() ) / ( y.max() - y.min() )
             #tqdm.write(f'{aa:0.9f}')
             y_edge[i] = y_edge_
             
             ## interpolate at edge
             psvel_edge_ = sp.interpolate.interp1d(y, psvel_ , kind='cubic', bounds_error=True)(y_edge_)
             psvel_edge_ = float(psvel_edge_)
@@ -20154,14 +20679,15 @@
             udef_char = np.copy(self['header/udef_char'][:]) ## the unpacked numpy array of |S128 encoded fixed-length character objects
             udef_char = [s.decode('utf-8') for s in udef_char] ## convert it to a python list of utf-8 strings
             self.udef = dict(zip(udef_char, udef_real)) ## make dict where keys are udef_char and values are udef_real
             
             # === characteristic values
             
             self.Ma          = self.udef['Ma']
+            self.M_inf       = self.Ma
             self.Re          = self.udef['Re']
             self.Pr          = self.udef['Pr']
             self.kappa       = self.udef['kappa']
             self.R           = self.udef['R']
             self.p_inf       = self.udef['p_inf']
             self.T_inf       = self.udef['T_inf']
             self.mu_Suth_ref = self.udef['mu_Suth_ref']
@@ -20197,14 +20723,19 @@
             self.recov_fac = self.Pr**(1/3)
             self.Taw       = self.T_inf + self.recov_fac*self.U_inf**2/(2*self.cp)
             self.lchar     = self.Re*self.nu_inf/self.U_inf
             
             self.tchar = self.lchar / self.U_inf
             self.uchar = self.U_inf
             
+            #self.p_tot_inf = self.p_inf * (1 + (self.kappa-1)/2 * self.U_inf**2 / (self.kappa*self.R*self.T_inf))**(self.kappa/(self.kappa-1))
+            self.p_tot_inf   = self.p_inf   * (1 + (self.kappa-1)/2 * self.M_inf**2)**(self.kappa/(self.kappa-1))
+            self.T_tot_inf   = self.T_inf   * (1 + (self.kappa-1)/2 * self.M_inf**2)
+            self.rho_tot_inf = self.rho_inf * (1 + (self.kappa-1)/2 * self.M_inf**2)**(1/(self.kappa-1))
+            
             if verbose: print(72*'-')
             if verbose: even_print('rho_inf'         , '%0.3f [kg/m³]'    % self.rho_inf   )
             if verbose: even_print('mu_inf'          , '%0.6E [kg/(m·s)]' % self.mu_inf    )
             if verbose: even_print('nu_inf'          , '%0.6E [m²/s]'     % self.nu_inf    )
             if verbose: even_print('a_inf'           , '%0.6f [m/s]'      % self.a_inf     )
             if verbose: even_print('U_inf'           , '%0.6f [m/s]'      % self.U_inf     )
             if verbose: even_print('cp'              , '%0.3f [J/(kg·K)]' % self.cp        )
@@ -20242,14 +20773,17 @@
         
         if header_attr_based:
             
             ## set all attributes
             for attr_str in header_attr_str_list:
                 setattr( self, attr_str, self.attrs[attr_str] )
             
+            if hasattr(self,'Ma') and not hasattr(self,'M_inf'):
+                setattr(self,'M_inf',self.Ma)
+            
             self.C_Suth = self.mu_Suth_ref/(self.T_Suth_ref**(3/2))*(self.T_Suth_ref + self.S_Suth) ## [kg/(m·s·√K)]
             #self.udef['C_Suth'] = self.C_Suth
             
             if verbose: print(72*'-')
             if verbose: even_print('Ma'          , '%0.2f [-]'           % self.Ma          )
             if verbose: even_print('Re'          , '%0.1f [-]'           % self.Re          )
             if verbose: even_print('Pr'          , '%0.3f [-]'           % self.Pr          )
@@ -20278,14 +20812,19 @@
             self.recov_fac = self.Pr**(1/3)
             self.Taw       = self.T_inf + self.recov_fac*self.U_inf**2/(2*self.cp)
             self.lchar     = self.Re*self.nu_inf/self.U_inf
             
             self.tchar = self.lchar / self.U_inf
             self.uchar = self.U_inf
             
+            #self.p_tot_inf = self.p_inf * (1 + (self.kappa-1)/2 * self.U_inf**2 / (self.kappa*self.R*self.T_inf))**(self.kappa/(self.kappa-1))
+            self.p_tot_inf   = self.p_inf   * (1 + (self.kappa-1)/2 * self.M_inf**2)**(self.kappa/(self.kappa-1))
+            self.T_tot_inf   = self.T_inf   * (1 + (self.kappa-1)/2 * self.M_inf**2)
+            self.rho_tot_inf = self.rho_inf * (1 + (self.kappa-1)/2 * self.M_inf**2)**(1/(self.kappa-1))
+            
             if verbose: print(72*'-')
             if verbose: even_print('rho_inf'         , '%0.3f [kg/m³]'    % self.rho_inf   )
             if verbose: even_print('mu_inf'          , '%0.6E [kg/(m·s)]' % self.mu_inf    )
             if verbose: even_print('nu_inf'          , '%0.6E [m²/s]'     % self.nu_inf    )
             if verbose: even_print('a_inf'           , '%0.6f [m/s]'      % self.a_inf     )
             if verbose: even_print('U_inf'           , '%0.6f [m/s]'      % self.U_inf     )
             if verbose: even_print('cp'              , '%0.3f [J/(kg·K)]' % self.cp        )
@@ -20642,35 +21181,42 @@
                     mu_bak  = np.copy( mu )
                     mu_A    = np.copy( mu_Suth_ref*(T/T_Suth_ref)**(3/2) * ((T_Suth_ref+S_Suth)/(T+S_Suth)) )
                     mu_B    = np.copy( C_Suth * T**(3/2) / (T + S_Suth) )
                     np.testing.assert_allclose(mu_A, mu_B, rtol=1e-6, atol=1e-10) ## single precision
                     np.testing.assert_allclose(mu_bak, mu_A, rtol=0.002)
                 
                 ## derived values from base scalars
-                a     = np.sqrt( kappa * R * T )
-                nu    = mu / rho
-                umag  = np.sqrt( u**2 + v**2 + w**2 )
-                M     = umag / np.sqrt(kappa * R * T)
-                mflux = umag * rho
+                a     = np.copy( np.sqrt( kappa * R * T )      )
+                nu    = np.copy( mu / rho                      )
+                umag  = np.copy( np.sqrt( u**2 + v**2 + w**2 ) )
+                M     = np.copy( umag / np.sqrt(kappa * R * T) )
+                mflux = np.copy( umag * rho                    )
+                
+                T_tot   = np.copy( T   * (1 + (kappa-1)/2 * M**2)                    )
+                p_tot   = np.copy( p   * (1 + (kappa-1)/2 * M**2)**(kappa/(kappa-1)) )
+                rho_tot = np.copy( rho * (1 + (kappa-1)/2 * M**2)**(1/(kappa-1))     )
                 
                 ## base scalars [u,v,w,ρ,p,T]
-                dset = self.create_dataset('data/u'   , data=u.T   , chunks=None)
-                dset = self.create_dataset('data/v'   , data=v.T   , chunks=None)
-                dset = self.create_dataset('data/w'   , data=w.T   , chunks=None)
-                dset = self.create_dataset('data/rho' , data=rho.T , chunks=None)
-                dset = self.create_dataset('data/p'   , data=p.T   , chunks=None)
-                dset = self.create_dataset('data/T'   , data=T.T   , chunks=None)
+                self.create_dataset('data/u'   , data=u.T   , chunks=None)
+                self.create_dataset('data/v'   , data=v.T   , chunks=None)
+                self.create_dataset('data/w'   , data=w.T   , chunks=None)
+                self.create_dataset('data/rho' , data=rho.T , chunks=None)
+                self.create_dataset('data/p'   , data=p.T   , chunks=None)
+                self.create_dataset('data/T'   , data=T.T   , chunks=None)
                 
                 ## derived fields
-                dset = self.create_dataset('data/a'     , data=a.T     , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m/s]'
-                dset = self.create_dataset('data/mu'    , data=mu.T    , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[kg/(m·s)]'
-                dset = self.create_dataset('data/nu'    , data=nu.T    , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m²/s]'
-                dset = self.create_dataset('data/umag'  , data=umag.T  , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m/s]'
-                dset = self.create_dataset('data/M'     , data=M.T     , chunks=None) #; dset.attrs['dimensional'] = False
-                dset = self.create_dataset('data/mflux' , data=mflux.T , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[kg/(m²·s)]'
+                self.create_dataset('data/a'       , data=a.T       , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m/s]'
+                self.create_dataset('data/mu'      , data=mu.T      , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[kg/(m·s)]'
+                self.create_dataset('data/nu'      , data=nu.T      , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m²/s]'
+                self.create_dataset('data/umag'    , data=umag.T    , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[m/s]'
+                self.create_dataset('data/M'       , data=M.T       , chunks=None) #; dset.attrs['dimensional'] = False
+                self.create_dataset('data/mflux'   , data=mflux.T   , chunks=None) #; dset.attrs['dimensional'] = True  ; dset.attrs['unit'] = '[kg/(m²·s)]'
+                self.create_dataset('data/T_tot'   , data=T_tot.T   , chunks=None)
+                self.create_dataset('data/p_tot'   , data=p_tot.T   , chunks=None)
+                self.create_dataset('data/rho_tot' , data=rho_tot.T , chunks=None)
         
         if fn_Re_fluct.exists():
             even_print('eas4 Re fluct',str(fn_Re_fluct.relative_to(Path())))
             with eas4(str(fn_Re_fluct),'r',verbose=False) as f1:
                 
                 data_mean = f1.get_mean()
                 
@@ -21373,14 +21919,95 @@
         self.get_header(verbose=False)
         if verbose: print(72*'-')
         if verbose: print('total time : ztmd.calc_gradients() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    def calc_psvel(self,**kwargs):
+        '''
+        calculate pseudovelocity, wall-normal cumulative integration of (-) z-vorticity
+        '''
+        
+        verbose  = kwargs.get('verbose',True)
+        
+        if verbose: print('\n'+'ztmd.calc_psvel()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        if not ('data/vort_z' in self):
+            raise ValueError('data/vort_z not in ztmd')
+        
+        vort_z = np.copy( self['data/vort_z'][()].T )
+        
+        nx = self.nx
+        ny = self.ny
+        
+        if self.rectilinear:
+            
+            x = np.copy( self['dims/x'][()] )
+            y = np.copy( self['dims/y'][()] )
+        
+        elif self.curvilinear:
+            
+            ## copy dims into memory
+            x = np.copy( self['dims/x'][()].T ) ## 2D
+            y = np.copy( self['dims/y'][()].T ) ## 2D
+            
+            if ('dims/snorm' not in self):
+                raise AssertionError('dims/snorm not present')
+            if ('dims/stang' not in self):
+                raise AssertionError('dims/stang not present')
+            
+            snorm = np.copy( self['dims/snorm'][()] ) ## 1D
+            stang = np.copy( self['dims/stang'][()] ) ## 1D
+            
+            if ('data/utang' not in self):
+                raise AssertionError('data/utang not present')
+            
+            utang = np.copy( self['data/utang'][()].T )
+            unorm = np.copy( self['data/unorm'][()].T )
+            
+            ## copy csys datasets into memory
+            vtang = np.copy( self['csys/vtang'][()] )
+            vnorm = np.copy( self['csys/vnorm'][()] )
+            
+            if (x.shape != (self.nx,self.ny)):
+                raise ValueError('x.shape != (self.nx,self.ny)')
+            if (y.shape != (self.nx,self.ny)):
+                raise ValueError('y.shape != (self.nx,self.ny)')
+        
+        else:
+            raise ValueError
+        
+        ## the local 1D wall-normal coordinate
+        if self.rectilinear:
+            y_ = np.copy(y)
+        elif self.curvilinear:
+            y_ = np.copy(snorm)
+        else:
+            raise ValueError
+        
+        ## pseudo-velocity is a cumulative integration of (-) z-vorticity
+        psvel = np.zeros(shape=(nx,ny), dtype=np.float64)
+        for i in range(nx):
+            psvel_     = sp.integrate.cumulative_trapezoid(-1*vort_z[i,:], y_, initial=0.)
+            psvel[i,:] = psvel_
+        
+        if ('data/psvel' in self):
+            del self['data/psvel']
+        self.create_dataset('data/psvel', data=psvel.T, chunks=None)
+        if verbose: even_print('data/psvel','%s'%str(psvel.shape))
+        
+        self.get_header(verbose=False)
+        if verbose: print(72*'-')
+        if verbose: print('total time : ztmd.calc_psvel() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
     def calc_wall_quantities(self, acc=6, edge_stencil='full', **kwargs):
         '''
         get 1D wall quantities
         -----
         - [ ρ_wall, ν_wall, μ_wall, T_wall ]
         - τ_wall = μ_wall·ddn[utang] :: [kg/(m·s)]·[m/s]/[m] = [kg/(m·s²)] = [N/m²] = [Pa]
         - u_τ = (τ_wall/ρ_wall)^(1/2)
@@ -23575,15 +24202,15 @@
         y_edge : the wall-normal edge location
         j_edge : the nearest index to y_edge
         -----
         the 'edge' is where ∂<var>/∂y==ϵ
         '''
         
         verbose      = kwargs.get('verbose',True)
-        method       = kwargs.get('method','psvel') ## 'u','psvel'
+        method       = kwargs.get('method','psvel') ## 'u','psvel','p_tot'
         epsilon      = kwargs.get('epsilon',1e-5)
         acc          = kwargs.get('acc',6)
         edge_stencil = kwargs.get('edge_stencil','half')
         interp_kind  = kwargs.get('interp_kind','cubic') ## 'linear','cubic'
         
         if verbose: print('\n'+'ztmd.calc_bl_edge()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
@@ -23605,16 +24232,16 @@
                     raise AssertionError
         else:
             raise ValueError
         
         if self.requires_wall_norm_interp:
             raise NotImplementedError
         
-        if not any([(method=='u'),(method=='psvel')]):
-            raise ValueError(f"'method' should be one of: 'u','psvel'")
+        if not any([(method=='u'),(method=='psvel'),(method=='p_tot')]):
+            raise ValueError(f"'method' should be one of: 'u','psvel','p_tot'")
         if not any([(interp_kind=='linear'),(interp_kind=='cubic')]):
             raise ValueError(f"'interp_kind' should be one of: 'linear','cubic'")
         
         if verbose: even_print('method',method)
         if verbose: even_print('epsilon','%0.1e'%(epsilon,))
         if verbose: even_print('acc',f'{acc:d}')
         if verbose: even_print('edge_stencil',edge_stencil)
@@ -23622,28 +24249,30 @@
         
         # ===
         
         nx = self.nx
         ny = self.ny
         
         ## copy 2D datasets into memory
-        u   = np.copy( self['data/u'][()].T   )
-        T   = np.copy( self['data/T'][()].T   )
-        rho = np.copy( self['data/rho'][()].T )
+        u     = np.copy( self['data/u'][()].T     )
+        T     = np.copy( self['data/T'][()].T     )
+        rho   = np.copy( self['data/rho'][()].T   )
+        if (method=='p_tot'):
+            p_tot = np.copy( self['data/p_tot'][()].T )
         
         if self.rectilinear:
             
             x = np.copy( self['dims/x'][()] )
             y = np.copy( self['dims/y'][()] )
         
         elif self.curvilinear:
             
             ## copy dims into memory
-            x = np.copy( self['dims/x'][()].T )
-            y = np.copy( self['dims/y'][()].T )
+            x = np.copy( self['dims/x'][()].T ) ## 2D
+            y = np.copy( self['dims/y'][()].T ) ## 2D
             
             if ('dims/snorm' not in self):
                 raise AssertionError('dims/snorm not present')
             if ('dims/stang' not in self):
                 raise AssertionError('dims/stang not present')
             
             snorm = np.copy( self['dims/snorm'][()] ) ## 1D
@@ -23676,31 +24305,22 @@
             y_ = np.copy(snorm)
         else:
             raise ValueError
         
         # ===
         
         if (method=='psvel'):
-            
-            if ('data/psvel' in self):
-                psvel = np.copy( self['data/psvel'][()].T )
-            
-            else: ## if doesnt exist: calculate & save pseudovelocity
-                
-                vort_z = np.copy( self['data/vort_z'][()].T )
-                
-                ## pseudo-velocity is a cumulative integration of (-) z-vorticity
-                psvel = np.zeros(shape=(nx,ny), dtype=np.float64)
-                for i in range(nx):
-                    psvel_     = sp.integrate.cumulative_trapezoid(-1*vort_z[i,:], y_, initial=0.)
-                    psvel[i,:] = psvel_
-                
-                if ('data/psvel' in self): del self['data/psvel']
-                dset = self.create_dataset('data/psvel', data=psvel.T, chunks=None)
-                if verbose: even_print('data/psvel','%s'%str(psvel.shape))
+            if not ('data/psvel' in self):
+                if verbose: print('>>> psvel not found. calling ztmd.calc_psvel()')
+                self.calc_psvel(verbose=False)
+            psvel = np.copy( self['data/psvel'][()].T )
+        
+        if (method=='p_tot'):
+            if not ('data/p_tot' in self):
+                raise ValueError('data/p_tot not in ztmd')
         
         # ===
         
         y_edge    = np.zeros(shape=(nx,)  , dtype=np.float64 )
         j_edge    = np.zeros(shape=(nx,)  , dtype=np.int32   )
         y_edge_2d = np.zeros(shape=(nx,2) , dtype=np.float64 )
         y_edge_g  = np.zeros(shape=(nx,)  , dtype=np.float64 )
@@ -23739,37 +24359,66 @@
                                     acc=acc,
                                     edge_stencil=edge_stencil,
                                     )
             
             else:
                 raise ValueError
         
+        elif (method=='p_tot'):
+            
+            p_tot_dimless = np.copy( (p_tot-self.p_tot_inf)/(self.rho_inf*self.U_inf**2) )
+        
         else:
             raise ValueError
         
         if verbose: progress_bar = tqdm(total=nx, ncols=100, desc='y_edge', leave=False, file=sys.stdout)
         for i in range(nx):
             
             # if (i==1000):
             #     do_debug_plot = True
             # else:
             #     do_debug_plot = False
             
-            ddy_u_ = np.copy(ddy_var[i,:])
+            if (method=='u') or (method=='psvel'):
+                
+                ddy_u_ = np.copy(ddy_var[i,:]) ## wall-normal derivative of e.g. u,psvel
+                
+                y_edge_ = calc_profile_edge_1d(y=y_,
+                                               #u=u_,
+                                               ddy_u=ddy_u_,
+                                               epsilon=epsilon,
+                                               acc=acc,
+                                               lchar=1.,
+                                               edge_stencil=edge_stencil,
+                                               interp_kind=interp_kind,
+                                               #do_debug_plot=do_debug_plot,
+                                               deriv=True,
+                                               )
             
-            y_edge_ = calc_profile_edge_1d(y=y_,
-                                           #u=u_,
-                                           ddy_u=ddy_u_,
-                                           epsilon=epsilon,
-                                           acc=acc,
-                                           lchar=1.,
-                                           edge_stencil=edge_stencil,
-                                           interp_kind=interp_kind,
-                                           #do_debug_plot=do_debug_plot,
-                                           )
+            elif (method=='p_tot'):
+                
+                ## root func to input
+                u_ = np.copy(p_tot_dimless[i,:])
+                
+                ## subtract max p_tot this [x] position
+                u_ -= u_.max()
+                
+                y_edge_ = calc_profile_edge_1d(y=y_,
+                                               u=u_,
+                                               epsilon=epsilon,
+                                               acc=acc,
+                                               lchar=1.,
+                                               edge_stencil=edge_stencil,
+                                               interp_kind=interp_kind,
+                                               #do_debug_plot=do_debug_plot,
+                                               deriv=False,
+                                               )
+            
+            else:
+                raise ValueError
             
             # ===
             
             y_edge[i]   = y_edge_
             j_edge_     = np.abs( y_ - y_edge_ ).argmin()
             j_edge[i]   = j_edge_
             y_edge_g[i] = y_[j_edge_]
@@ -23816,15 +24465,16 @@
     
     def calc_bl_edge_quantities(self, **kwargs):
         '''
         calculate field quantity values at [y_edge]
         - skin friction coefficient: cf
         '''
         
-        verbose = kwargs.get('verbose',True)
+        verbose     = kwargs.get('verbose',True)
+        interp_kind = kwargs.get('interp_kind','cubic') ## 'linear','cubic'
         
         if verbose: print('\n'+'ztmd.calc_bl_edge_quantities()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
         # ===
         
         nx = self.nx
@@ -23874,17 +24524,23 @@
         elif self.curvilinear:
             y_ = np.copy(snorm)
         else:
             raise ValueError
         
         # === make a structured array
         
-        names  = [ 'rho', 'u', 'v', 'w', 'T', 'p', 'vort_z', 'mu', 'nu', 'M', 'psvel' ]
-        if self.curvilinear:
-            names += [ 'utang', 'unorm' ]
+        names  = [ 'rho', 'u', 'v', 'w', 'T', 'p', 'vort_z', 'mu', 'nu', 'M' ]
+        if ('data/psvel' in self):
+            names += [ 'psvel' ]
+        if ('data/utang' in self):
+            names += [ 'utang' ]
+        if ('data/unorm' in self):
+            names += [ 'unorm' ]
+        if ('data/umag' in self):
+            names += [ 'umag' ]
         
         dtypes=[]
         for n in names:
             ds = self[f'data/{n}']
             dtypes.append( ds.dtype )
         
         names_edge = [ n+'_edge' for n in names ]
@@ -23900,15 +24556,15 @@
         # === interpolate edge quantity for all vars
         
         if verbose: progress_bar = tqdm(total=nx*len(names), ncols=100, desc='edge quantities', leave=False, file=sys.stdout)
         for scalar in data.dtype.names:
             for i in range(nx):
                 
                 data_y_    = np.copy( data[scalar][i,:] )
-                intrp_func = sp.interpolate.interp1d(y_, data_y_, kind='cubic', bounds_error=True)
+                intrp_func = sp.interpolate.interp1d(y_, data_y_, kind=interp_kind, bounds_error=True)
                 
                 y_edge_    = y_edge[i]
                 data_edge_ = intrp_func(y_edge_)
                 
                 data_edge[scalar+'_edge'][i] = data_edge_
                 
                 if verbose: progress_bar.update()
@@ -24213,17 +24869,23 @@
         elif self.curvilinear:
             y_ = np.copy(snorm)
         else:
             raise ValueError
         
         # === make a structured array
         
-        names  = [ 'rho', 'u', 'v', 'w', 'T', 'p', 'vort_z', 'mu', 'nu', 'M', 'psvel' ]
-        if self.curvilinear:
-            names += [ 'utang', 'unorm' ]
+        names  = [ 'rho', 'u', 'v', 'w', 'T', 'p', 'vort_z', 'mu', 'nu', 'M' ]
+        if ('data/psvel' in self):
+            names += [ 'psvel' ]
+        if ('data/utang' in self):
+            names += [ 'utang' ]
+        if ('data/unorm' in self):
+            names += [ 'unorm' ]
+        if ('data/umag' in self):
+            names += [ 'umag' ]
         
         dtypes=[]
         for n in names:
             ds = self[f'data/{n}']
             dtypes.append( ds.dtype )
         
         #names_99 = [ n+'99' for n in names ]
@@ -28356,21 +29018,26 @@
         even_print('uchar'          , '%0.5f [m/s]'         % self.uchar      )
         even_print('lchar'          , '%0.5e [m]'           % self.lchar      )
         even_print('tchar'          , '%0.5e [s]'           % self.tchar      )
         print(72*'-')
         
         return
 
-def calc_profile_edge_1d(y, u=None, ddy_u=None, **kwargs):
+def calc_profile_edge_1d(y, u=None, ddy_u=None, deriv=True, **kwargs):
     '''
     determine the edge location of 1D BL profile
     - [y] is a 1D coordinate vector
-    - [u] is some profile variable (streamwise velocity, pseudovelocity, etc.)
-    - ddy_u is an externally calculated ∂u/∂y (passing it skips gradient calc in this func)
-    the 'edge' is determined by the point at which ∂u/∂y==ϵ
+    - [u] is some profile variable (streamwise velocity, pseudovelocity, p_tot, etc.)
+    -----
+    deriv=True:
+        - ddy_u is an externally calculated ∂u/∂y (passing it skips gradient calc in this func)
+        - the 'edge' is determined by the point at which ∂u/∂y==ϵ
+    deriv=False:
+        - u is a profile with a 0-crossing like [u-U_inf] or (p_tot-p_tot_inf)/(ρ·U_inf^2)
+        - the 'edge' is determined by the point at which |u(y)|==ϵ
     '''
     epsilon      = kwargs.get('epsilon',1e-5)
     acc          = kwargs.get('acc',6)
     edge_stencil = kwargs.get('edge_stencil','half')
     interp_kind  = kwargs.get('interp_kind','cubic')
     
     lchar = kwargs.get('lchar',1.) ## normalization factor for coord vector [y]
@@ -28383,14 +29050,17 @@
     
     ## make sure exactly one of u | ddy_u was passed
     if (u is None) and (ddy_u is None):
         raise ValueError('pass one of either u or ddy_u')
     if (u is not None) and (ddy_u is not None):
         raise ValueError('either pass u or ddy_u (not both)')
     
+    if not deriv and (ddy_u is not None):
+        raise ValueError('if deriv=False, then ddy_u should not be provided')
+    
     ## make sure dims of passed u | ddy_u are correct
     if (u is not None):
         if (u.ndim!=1):
             raise ValueError
         if (u.shape[0]!=y.shape[0]):
             raise ValueError
     if (ddy_u is not None):
@@ -28401,59 +29071,108 @@
     
     if not any([(interp_kind=='linear'),(interp_kind=='cubic')]):
         raise ValueError(f"'interp_kind' should be one of: 'linear','cubic'")
     
     ny = y.shape[0]
     
     ## ddy_u wasnt passed, need to calculate gradient in [y]
-    if (ddy_u is None):
+    if (ddy_u is None) and deriv:
         ddy_u = gradient( u/u.max(), y/lchar, axis=0, d=1, acc=acc, edge_stencil=edge_stencil )
     
     ## get [y] of first intersection
     jtop = ny-1
     for j in range(ny):
-        if ( ddy_u[j] < epsilon):
-            jtop = j
-            break
-    
-    intrp_func = sp.interpolate.interp1d(y/lchar, ddy_u, kind=interp_kind, bounds_error=True)
-    
-    def __f_opt_edge_locator(y_test, intrp_func, epsilon, lchar):
-        ddy_u_test = intrp_func(y_test/lchar)
-        root = np.abs( ddy_u_test - epsilon )
-        return root
+        if deriv:
+            if ( ddy_u[j] < epsilon):
+                jtop = j
+                break
+        else:
+            if (np.abs(u[j]) < epsilon):
+                jtop = j
+                break
     
-    sol = sp.optimize.least_squares(fun=__f_opt_edge_locator,
-                                    args=(intrp_func, epsilon, lchar),
-                                    x0=0.5*(y[jtop-2]+y[jtop]),
-                                    xtol=1e-15,
-                                    ftol=1e-15,
-                                    gtol=1e-15,
-                                    method='dogbox',
-                                    bounds=(y[jtop-2], y[jtop]))
-    if not sol.success:
-        raise ValueError
+    if (jtop<3):
+        raise ValueError('jtop<3')
     
-    y_edge = sol.x[0]
+    if deriv: ## use derivative-based method e.g. for u,pseudovel
+        
+        intrp_func = sp.interpolate.interp1d(y/lchar, ddy_u, kind=interp_kind, bounds_error=True)
+        
+        def __f_opt_edge_locator(y_test, intrp_func, epsilon, lchar):
+            ddy_u_test = intrp_func(y_test/lchar)
+            root = np.abs( ddy_u_test - epsilon )
+            return root
+        
+        sol = sp.optimize.least_squares(fun=__f_opt_edge_locator,
+                                        args=(intrp_func, epsilon, lchar),
+                                        x0=0.5*(y[jtop-2]+y[jtop]),
+                                        xtol=1e-15,
+                                        ftol=1e-15,
+                                        gtol=1e-15,
+                                        method='dogbox',
+                                        bounds=(y[jtop-2], y[jtop]))
+        if not sol.success:
+            raise ValueError
+        
+        y_edge = sol.x[0]
+        
+        if do_debug_plot:
+            plt.close('all')
+            fig1 = plt.figure(figsize=(2*(16/9),2), dpi=300)
+            ax1 = plt.gca()
+            ax1.set_xscale('log', base=10)
+            ax1.plot(ddy_u,
+                     y/lchar,
+                     lw=0.8,
+                     )
+            ax1.set_xlim(1e-30, 1e1)
+            ax1.axhline(y=y_edge/lchar, linestyle='dashed', c='gray', zorder=1, lw=0.5)
+            ax1.axvline(x=epsilon, linestyle='dashed', c='gray', zorder=1, lw=0.5)
+            fig1.tight_layout(pad=0.25)
+            fig1.tight_layout(pad=0.25)
+            plt.show()
     
-    if do_debug_plot:
-        plt.close('all')
-        fig1 = plt.figure(figsize=(2*(16/9),2), dpi=300)
-        ax1 = plt.gca()
-        ax1.set_xscale('log', base=10)
-        ax1.plot(ddy_u,
-                 y/lchar,
-                 lw=0.8,
-                 )
-        ax1.set_xlim(1e-30, 1e1)
-        ax1.axhline(y=y_edge/lchar, linestyle='dashed', c='gray', zorder=1, lw=0.5)
-        ax1.axvline(x=epsilon, linestyle='dashed', c='gray', zorder=1, lw=0.5)
-        fig1.tight_layout(pad=0.25)
-        fig1.tight_layout(pad=0.25)
-        plt.show()
+    else:
+        
+        intrp_func = sp.interpolate.interp1d(y/lchar, u, kind=interp_kind, bounds_error=True)
+        
+        def __f_opt_edge_locator(y_test, intrp_func, epsilon, lchar):
+            u_test = intrp_func(y_test/lchar)
+            root = np.abs( u_test - epsilon )
+            return root
+        
+        sol = sp.optimize.least_squares(fun=__f_opt_edge_locator,
+                                        args=(intrp_func, epsilon, lchar),
+                                        x0=0.5*(y[jtop-2]+y[jtop]),
+                                        xtol=1e-15,
+                                        ftol=1e-15,
+                                        gtol=1e-15,
+                                        method='dogbox',
+                                        bounds=(y[jtop-2], y[jtop]))
+        if not sol.success:
+            raise ValueError
+        
+        y_edge = sol.x[0]
+        
+        if do_debug_plot:
+            plt.close('all')
+            fig1 = plt.figure(figsize=(2*(16/9),2), dpi=300)
+            ax1 = plt.gca()
+            #ax1.set_xscale('log', base=10)
+            ax1.plot(u,
+                     y/lchar,
+                     lw=0.8,
+                     )
+            ax1.set_xlim(-1,+1)
+            ax1.axhline(y=y_edge/lchar, linestyle='dashed', c='gray', zorder=1, lw=0.5)
+            ax1.axvline(x=+epsilon, linestyle='dashed', c='gray', zorder=1, lw=0.5)
+            ax1.axvline(x=-epsilon, linestyle='dashed', c='gray', zorder=1, lw=0.5)
+            fig1.tight_layout(pad=0.25)
+            fig1.tight_layout(pad=0.25)
+            plt.show()
     
     return y_edge
 
 def calc_d99_1d(y, u, y_edge, u_edge=None, **kwargs):
     '''
     determine δ99 location of 1D profile
     - [y] is a 1D coordinate vector
@@ -29925,41 +30644,158 @@
         fig1.tight_layout(pad=0.25)
         dpi_out = 2160/plt.gcf().get_size_inches()[1]
         #fig1.savefig('dx.png', dpi=dpi_out)
         plt.show()
     
     return x
 
-def time_integrate_2d(u,v, x2d,y2d, xy_pts, dt,nt, uchar=1.,lchar=1., p=None, bounds_check=True):
+# time integration
+# ======================================================================
+
+class time_integrate_2d_seeder():
+    '''
+    for use with turbx.time_integrate_2d()
+    - yields (N,2) arrays of pts as func of timestep
+    - 'fixed position' : return original initialized points
+    '''
+    def __init__(self, xy_pts, dti=10, method='fixed position', **kwargs):
+        self.xy_pts = np.copy(xy_pts)
+        self.dti = dti
+        self.method = method
+    
+    def __call__(self,ti):
+        if (self.method=='fixed position'):
+            if (ti%self.dti==0):
+                return np.copy( self.xy_pts )
+            else:
+                return None
+        elif (self.method=='random in poly'):
+            raise NotImplementedError
+        else:
+            raise ValueError
+
+def time_integrate_2d(u,v, x2d,y2d, dt,nt, xy_pts=None, xy_pt_seeder=None, **kwargs):
     '''
     integrate [x,y] paths for a single [u,v] field
+    - xy_pts is a (N,2) numpy array describing the start locations of the particles
+    - xy_pt_seeder() callable provides particle coordinates as a function of time
     '''
     
-    ## check
-    ## ...
+    verbose      = kwargs.get('verbose',False)
+    method       = kwargs.get('method','cubic') ## interpolation method 'linear','cubic'
+    direction    = kwargs.get('direction','fwdbwd') ## 'fwd','bwd','fwdbwd'
+    bounds_check = kwargs.get('bounds_check',True)
     
-    xy_pts = np.copy(xy_pts)
+    method_integration = kwargs.get('method_integration','euler1D')
     
-    t = dt*np.arange(nt,dtype=np.float64)
+    if verbose: print('\n'+'turbx.time_integrate_2d()'+'\n'+72*'-')
+    t_start_func = timeit.default_timer()
+    
+    if verbose: even_print(f'bounds_check',str(bounds_check))
     
-    bwdfwd = True
-    if bwdfwd:
+    ## checks
+    if not any([(method=='linear'),(method=='cubic')]):
+        raise ValueError("'method' should be one of 'cubic' or 'linear'")
+    if not any([(direction=='fwd'),(direction=='bwd'),(direction=='fwdbwd')]):
+        raise ValueError("'direction' should be one of 'fwd','bwd','fwdbwd'")
+    if not isinstance(u, np.ndarray):
+        raise ValueError('u should be a numpy array')
+    if not isinstance(v, np.ndarray):
+        raise ValueError('v should be a numpy array')
+    if not isinstance(x2d, np.ndarray):
+        raise ValueError('x2d should be a numpy array')
+    if not isinstance(y2d, np.ndarray):
+        raise ValueError('y2d should be a numpy array')
+    
+    if (xy_pts is not None): ## there are initial points
+        if not isinstance(xy_pts, np.ndarray):
+            raise ValueError('xy_pts should be a numpy array')
+        if (xy_pts.ndim!=2):
+            raise ValueError('xy_pts.ndim!=2')
+        if (xy_pts.shape[1]!=2):
+            raise ValueError('xy_pts should have shape (N,2)')
+    else: ## there are no initial points
         
+        ## make sure that there is a callable 'xy_pt_seeder' to provide points
+        if (xy_pt_seeder is None):
+            raise ValueError
+        else:
+            if not callable(xy_pt_seeder):
+                raise ValueError
+    
+    if (x2d.ndim!=2):
+        raise ValueError('x2d.ndim!=2')
+    if (y2d.ndim!=2):
+        raise ValueError('y2d.ndim!=2')
+    if (u.shape!=v.shape):
+        raise ValueError('u.shape!=v.shape')
+    if (x2d.shape!=y2d.shape):
+        raise ValueError('x2d.shape!=y2d.shape')
+    if (u.shape!=x2d.shape):
+        raise ValueError('u.shape!=x2d.shape')
+    
+    ## are we using point seeding?
+    if (xy_pt_seeder is not None):
+        pt_seeding_active = True
+    else:
+        pt_seeding_active = False
+    
+    ## number of initial points
+    if (xy_pts is not None):
+        n_pts = xy_pts.shape[0]
+    else:
+        n_pts = 0
+    
+    ## if there are no initial points and none will be seeded
+    if (n_pts==0) and not pt_seeding_active:
+        raise ValueError
+    
+    if verbose: even_print(f'n pts (initial)',f'{n_pts:d}')
+    
+    ## naive time array, could be updated for 'fwdbwd'
+    t = dt*np.arange(nt,dtype=np.float64)
+    
+    if (direction=='fwd'):
+        ti_fwd = np.arange(nt)
+    elif (direction=='bwd'):
+        ti_bwd = np.flip(np.arange(nt))
+    elif (direction=='fwdbwd'):
         nt_nom = nt
         nt = 1 + 2*(nt-1)
         tL = np.copy( np.flip(-t[1:]) )
         tR = np.copy( t[1:] )
         t  = np.concatenate( [tL,np.array([0.],dtype=np.float64),tR] , casting='no' )
-        
         ti_fwd = np.arange(nt_nom-1,nt)
         ti_bwd = np.flip(np.arange(0,nt_nom))
+    else:
+        raise ValueError
     
-    ## construct polygon object using matplotlib
+    if verbose: even_print(f'nt',f'{nt:d}')
+    
+    ## do a 'test run' of the seeding function
+    ## get the total number of pts that will be seeded
+    n_pts_seeded=0
+    if pt_seeding_active:
+        for ti in range(nt):
+            xy_pts_seeded = xy_pt_seeder(ti=ti)
+            if (xy_pts_seeded is not None):
+                n_pts_seeded += xy_pts_seeded.shape[0]
+    if verbose: even_print(f'n pts (seeded)',f'{n_pts_seeded:d}')
+    
+    ## total points = initial points + seeded points
+    n_pts += n_pts_seeded
+    if verbose: even_print(f'n pts (total)',f'{n_pts:d}')
+    
+    ## shape of the [x,y] grid and the [u,v] fields for forming interpolant
     nx,ny = x2d.shape
+    if verbose: even_print(f'nx',f'{nx:d}')
+    if verbose: even_print(f'ny',f'{ny:d}')
     
+    ## if checking bounds, then
+    ## construct polygon object using matplotlib
     if bounds_check:
         n_edge_pts = 2*nx + 2*(ny-2)
         n_edge_faces = n_edge_pts
         poly = np.zeros((n_edge_faces,2),dtype=np.float64)
         ii=-1
         for j in range(ny): ## W
             ii+=1
@@ -29973,124 +30809,208 @@
             ii+=1
             poly[ii,0] = x2d[-1,-(j+1)]
             poly[ii,1] = y2d[-1,-(j+1)]
         for i in range(1,nx-1): ## S
             ii+=1
             poly[ii,0] = x2d[-(i+1),0]
             poly[ii,1] = y2d[-(i+1),0]
-    
-    ## a polygon/path object
-    if bounds_check:
+        
         poly_obj = mpl.path.Path(poly,closed=False)
     
-    ## interpolant callables
+    ## get interpolant callables
+    t_start = timeit.default_timer()
+    
+    if (method=='cubic'):
+        
+        f_u = sp.interpolate.CloughTocher2DInterpolator(points=(x2d.ravel(), y2d.ravel()),
+                                                                values=u.ravel(),
+                                                                fill_value=np.nan )
+        
+        f_v = sp.interpolate.CloughTocher2DInterpolator(points=(x2d.ravel(), y2d.ravel()),
+                                                                values=v.ravel(),
+                                                                fill_value=np.nan )
+    
+    elif (method=='linear'):
+        
+        f_u = sp.interpolate.LinearNDInterpolator(points=(x2d.ravel(), y2d.ravel()),
+                                                          values=u.ravel(),
+                                                          fill_value=np.nan )
+        
+        f_v = sp.interpolate.LinearNDInterpolator(points=(x2d.ravel(), y2d.ravel()),
+                                                          values=v.ravel(),
+                                                          fill_value=np.nan )
     
-    f_u = sp.interpolate.CloughTocher2DInterpolator(points=(x2d.ravel(), y2d.ravel()),
-                                                            values=u.ravel(),
-                                                            fill_value=np.nan )
-    
-    f_v = sp.interpolate.CloughTocher2DInterpolator(points=(x2d.ravel(), y2d.ravel()),
-                                                            values=v.ravel(),
-                                                            fill_value=np.nan )
-    
-    ## f_u = sp.interpolate.LinearNDInterpolator(points=(x2d.ravel(), y2d.ravel()),
-    ##                                                         values=u.ravel(),
-    ##                                                         fill_value=np.nan )
-    ## 
-    ## f_v = sp.interpolate.LinearNDInterpolator(points=(x2d.ravel(), y2d.ravel()),
-    ##                                                         values=v.ravel(),
-    ##                                                         fill_value=np.nan )
+    else:
+        raise NotImplementedError
     
-    n_particles = xy_pts.shape[0]
-    pnum = np.arange(n_particles, dtype=np.int64)
+    t_delta = timeit.default_timer() - t_start
+    if verbose: even_print(f'time construct interpolant',format_time_string(t_delta))
     
     scalars = [ 'x','y',
-                'u','v', #'p',
-                't','id',
+                'u','v',
+                't',
+                'id',
               ]
     
-    scalars_dtype = [ np.float64, np.float64, 
-                      np.float64, np.float64, #np.float64,
-                      np.float64, np.int64,
+    scalars_dtype = [ np.float64, np.float64,
+                      np.float64, np.float64,
+                      np.float64,
+                      np.int64,
                     ]
     
-    data = np.zeros(shape=(n_particles,nt), dtype={'names':scalars, 'formats':scalars_dtype})
+    data = np.zeros(shape=(n_pts,nt), dtype={'names':scalars, 'formats':scalars_dtype})
+    if verbose: even_print(f'size data','%0.1f %s'%format_nbytes(data.nbytes))
     
     ## fill in IDs
     for ti in range(nt):
-        data['id'][:,ti] = pnum
+        data['id'][:,ti] = np.arange(n_pts, dtype=np.int64)
     
-    xy_pts_orig = np.copy(xy_pts)
+    ## populate [x,y,u,v] in data storage array
+    data['x'][:,:] = np.nan
+    data['y'][:,:] = np.nan
+    data['u'][:,:] = np.nan
+    data['v'][:,:] = np.nan
+    
+    ## make copy of original locations
+    if (xy_pts is not None):
+        xy_pts_orig = np.copy(xy_pts)
+    else:
+        xy_pts_orig = None
     
-    ## convect (forwards)
-    for ti in ti_fwd:
-        tt = t[ti]
-        
-        ## store position
-        data['x'][:,ti] = np.copy( xy_pts[:,0] )
-        data['y'][:,ti] = np.copy( xy_pts[:,1] )
-        
-        ## store time
-        data['t'][:,ti] = tt
-        
-        ## interpolate velocity
-        u_pts = f_u( xy_pts[:,0], xy_pts[:,1] )
-        v_pts = f_v( xy_pts[:,0], xy_pts[:,1] )
-        
-        data['u'][:,ti] = np.copy( u_pts )
-        data['v'][:,ti] = np.copy( v_pts )
-        
-        ## convect (Euler 1D)
-        xy_pts[:,0] += u_pts*dt
-        xy_pts[:,1] += v_pts*dt
-        
-        ## test if contained after convect
-        if bounds_check:
-            contained = np.zeros((n_particles,), dtype=np.int32)
-            for pi in range(n_particles):
-                in_poly = poly_obj.contains_point(xy_pts[pi,:])
-                if in_poly:
-                    contained[pi] = 1
-            ii_nan = np.where(contained==0)
-            xy_pts[ii_nan,:] = np.nan
+    # ==================================================================
+    
+    t_start = timeit.default_timer()
     
-    ## reset position before bwd interpolation
-    xy_pts = np.copy(xy_pts_orig)
+    if verbose:
+        progress_bar = tqdm(total=nt, ncols=100, desc='convect', leave=False, file=sys.stdout)
+    
+    ## convect (forwards)
+    if any([(direction=='fwd'),(direction=='fwdbwd')]):
+        for ti in ti_fwd:
+            tt = t[ti]
+            
+            ## store time
+            data['t'][:,ti] = tt
+            
+            ## add pts
+            if pt_seeding_active:
+                xy_pts_seeded = xy_pt_seeder(ti=ti)
+                if (xy_pts_seeded is not None):
+                    try:
+                        xy_pts = np.concatenate((xy_pts,xy_pts_seeded),axis=0)
+                    except ValueError: ## e.g. is None
+                        xy_pts = np.copy(xy_pts_seeded)
+            
+            if (xy_pts is None):
+                raise ValueError(f'xy_pts is None at ti={ti:d}')
+            
+            n_pts = xy_pts.shape[0]
+            
+            ## store position
+            data['x'][:n_pts,ti] = np.copy( xy_pts[:,0] )
+            data['y'][:n_pts,ti] = np.copy( xy_pts[:,1] )
+            
+            ## get mask for NaN / non-NaN pts
+            ii_nan = np.where(  np.isnan(xy_pts[:,0]) |  np.isnan(xy_pts[:,1]) )
+            ii     = np.where( ~np.isnan(xy_pts[:,0]) & ~np.isnan(xy_pts[:,1]) )
+            if (len(ii[0])+len(ii_nan[0]) != n_pts):
+                raise ValueError
+            
+            ## interpolate velocity
+            u_pts = np.squeeze( f_u( xy_pts[ii,0], xy_pts[ii,1] ) )
+            v_pts = np.squeeze( f_v( xy_pts[ii,0], xy_pts[ii,1] ) )
+            
+            ## write to data array
+            data['u'][ii,ti]     = np.copy( u_pts )
+            data['v'][ii,ti]     = np.copy( v_pts )
+            data['u'][ii_nan,ti] = np.nan
+            data['v'][ii_nan,ti] = np.nan
+            
+            ## convect (forwards, Euler 1D)
+            xy_pts[ii,0] += u_pts*dt
+            xy_pts[ii,1] += v_pts*dt
+            
+            ## test if contained after convect
+            if bounds_check:
+                in_poly = poly_obj.contains_points(xy_pts)
+                ii_not_in_poly = np.invert(in_poly)
+                xy_pts[ii_not_in_poly,:] = np.nan
+            
+            if verbose: progress_bar.update()
     
     ## convect (backwards)
-    for ti in ti_bwd:
-        tt = t[ti]
+    if any([(direction=='bwd'),(direction=='fwdbwd')]):
+        
+        ## reset position before bwd interpolation
+        if (xy_pts_orig is None):
+            xy_pts = None
+        else:
+            xy_pts = np.copy(xy_pts_orig)
         
-        ## store position
-        data['x'][:,ti] = np.copy( xy_pts[:,0] )
-        data['y'][:,ti] = np.copy( xy_pts[:,1] )
-        
-        ## store time
-        data['t'][:,ti] = tt
-        
-        ## interpolate velocity
-        u_pts = f_u( xy_pts[:,0], xy_pts[:,1] )
-        v_pts = f_v( xy_pts[:,0], xy_pts[:,1] )
-        
-        data['u'][:,ti] = np.copy( u_pts )
-        data['v'][:,ti] = np.copy( v_pts )
-        
-        ## convect (backwards)
-        xy_pts[:,0] -= u_pts*dt
-        xy_pts[:,1] -= v_pts*dt
-        
-        ## test if contained after convect
-        if bounds_check:
-            contained = np.zeros((n_particles,), dtype=np.int32)
-            for pi in range(n_particles):
-                in_poly = poly_obj.contains_point(xy_pts[pi,:])
-                if in_poly:
-                    contained[pi] = 1
-            ii_nan = np.where(contained==0)
-            xy_pts[ii_nan,:] = np.nan
+        for ti in ti_bwd:
+            tt = t[ti]
+            
+            ## store time
+            data['t'][:,ti] = tt
+            
+            ## add pts
+            if pt_seeding_active:
+                #xy_pts_seeded = xy_pt_seeder(ti=ti)
+                xy_pts_seeded = xy_pt_seeder(ti=nt-ti-1) ## if seeding backwards
+                if (xy_pts_seeded is not None):
+                    try:
+                        xy_pts = np.concatenate((xy_pts,xy_pts_seeded),axis=0)
+                    except ValueError: ## e.g. is None
+                        xy_pts = np.copy(xy_pts_seeded)
+            
+            if (xy_pts is None):
+                raise ValueError(f'xy_pts is None at ti={ti:d}')
+            
+            n_pts = xy_pts.shape[0]
+            
+            ## store position
+            data['x'][:n_pts,ti] = np.copy( xy_pts[:,0] )
+            data['y'][:n_pts,ti] = np.copy( xy_pts[:,1] )
+            
+            ## get mask for NaN / non-NaN pts
+            ii_nan = np.where(  np.isnan(xy_pts[:,0]) |  np.isnan(xy_pts[:,1]) )
+            ii     = np.where( ~np.isnan(xy_pts[:,0]) & ~np.isnan(xy_pts[:,1]) )
+            if (len(ii[0])+len(ii_nan[0]) != n_pts):
+                raise ValueError
+            
+            ## interpolate velocity
+            u_pts = np.squeeze( f_u( xy_pts[ii,0], xy_pts[ii,1] ) )
+            v_pts = np.squeeze( f_v( xy_pts[ii,0], xy_pts[ii,1] ) )
+            
+            data['u'][ii,ti]     = np.copy( u_pts )
+            data['v'][ii,ti]     = np.copy( v_pts )
+            data['u'][ii_nan,ti] = np.nan
+            data['v'][ii_nan,ti] = np.nan
+            
+            ## convect (backwards, Euler 1D)
+            xy_pts[ii,0] -= u_pts*dt
+            xy_pts[ii,1] -= v_pts*dt
+            
+            ## test if contained after convect
+            if bounds_check:
+                in_poly = poly_obj.contains_points(xy_pts)
+                ii_not_in_poly = np.invert(in_poly)
+                xy_pts[ii_not_in_poly,:] = np.nan
+            
+            if verbose: progress_bar.update()
+    
+    if verbose: progress_bar.close()
+    
+    t_delta = timeit.default_timer() - t_start
+    if verbose: even_print(f'time convect',format_time_string(t_delta))
+    #if verbose: even_print(f'time total',format_time_string((timeit.default_timer() - t_start_func)))
+    
+    if verbose: print(72*'-')
+    if verbose: print('total time : turbx.time_integrate_2d() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+    if verbose: print(72*'-')
     
     return data
 
 # csys
 # ======================================================================
 
 def rect_to_cyl(xyz,**kwargs):
@@ -30718,14 +31638,15 @@
     --> download, install, then delete : C:/Users/%USERNAME%/.matplotlib/fontlist-v330.json
     --> this JSON file will get regenerated with newly installed fonts
     '''
     
     useTex   = kwargs.get('useTex',False) ## use LaTeX text rendering
     darkMode = kwargs.get('darkMode',True)
     font     = kwargs.get('font',None)
+    fontsize = kwargs.get('fontsize',10)
     
     ## mpl.rcParams.update(mpl.rcParamsDefault) ## reset rcparams to defaults
     
     if darkMode:
         mpl.style.use('dark_background') ## dark mode
     else:
         mpl.style.use('default')
@@ -30937,19 +31858,18 @@
             mpl.rcParams['mathtext.bf'] = fe.name+':bold'
     
     # ===
     
     ## ## list all options
     ## print(mpl.rcParams.keys())
     
-    fontsize = 10
     axesAndTickWidth = 0.5
     
-    mpl.rcParams['figure.figsize'] = 3*(16/9), 3
-    mpl.rcParams['figure.dpi']     = 300
+    mpl.rcParams['figure.figsize'] = 2*(16/9), 2
+    mpl.rcParams['figure.dpi']     = 400
     #mpl.rcParams['figure.facecolor'] = 'k'
     #mpl.rcParams['figure.autolayout'] = True ### tight_layout() --> just use instead : fig1.tight_layout(pad=0.20)
     
     #mpl.rcParams['figure.constrained_layout.use'] = True
     #mpl.rcParams['figure.constrained_layout.h_pad']  = 0.0 ## Padding around axes objects. Float representing
     #mpl.rcParams['figure.constrained_layout.w_pad']  = 0.0 ## inches. Default is 3/72 inches (3 points)
     #mpl.rcParams['figure.constrained_layout.hspace'] = 0.2 ## Space between subplot groups. Float representing
@@ -30963,15 +31883,15 @@
     #mpl.rcParams['figure.subplot.wspace'] = 0.2
     
     mpl.rcParams['pdf.compression'] = 2 ## 0-9
     #mpl.rcParams['pdf.fonttype'] = 42  # Output Type 3 (Type3) or Type 42 (TrueType)
     #mpl.rcParams['pdf.use14corefonts'] = False
     
     mpl.rcParams['savefig.pad_inches'] = 0.20
-    mpl.rcParams['savefig.dpi']        = 300
+    mpl.rcParams['savefig.dpi']        = 2160/2
     
     mpl.rcParams['xtick.major.size']  = 2.5
     mpl.rcParams['xtick.major.width'] = axesAndTickWidth
     mpl.rcParams['xtick.minor.size']  = 1.4
     mpl.rcParams['xtick.minor.width'] = axesAndTickWidth*1.0
     #mpl.rcParams['xtick.color'] = 'k' ## set with mpl.style.use()
     mpl.rcParams['xtick.direction']   = 'in'
@@ -30996,30 +31916,58 @@
     mpl.rcParams['lines.markeredgewidth'] = 0.
     
     #mpl.rcParams['axes.facecolor'] = 'k' ## set with mpl.style.use()
     mpl.rcParams['axes.linewidth'] = axesAndTickWidth
     mpl.rcParams['axes.labelpad']  = 3.0
     mpl.rcParams['axes.titlesize'] = fontsize
     mpl.rcParams['axes.labelsize'] = fontsize
-    mpl.rcParams['axes.formatter.use_mathtext'] = True
+    #mpl.rcParams['axes.formatter.use_mathtext'] = True
     mpl.rcParams['axes.axisbelow'] = False ## dont allow axes, ticks to be under lines --> doesn't work for artist objects with zorder >2.5
     
     mpl.rcParams['legend.fontsize'] = fontsize
     mpl.rcParams['legend.shadow']   = False
     mpl.rcParams['legend.borderpad'] = 0.3
     mpl.rcParams['legend.framealpha'] = 1.0
     mpl.rcParams['legend.edgecolor']  = 'inherit'
     mpl.rcParams['legend.handlelength'] = 1.0
-    mpl.rcParams['legend.handletextpad'] = 0.4
-    mpl.rcParams['legend.borderaxespad'] = 0.6
+    mpl.rcParams['legend.handletextpad'] = 0.3
+    mpl.rcParams['legend.borderaxespad'] = 0.7
     mpl.rcParams['legend.columnspacing'] = 0.5
     mpl.rcParams['legend.fancybox'] = False
     
     return
 
+class mpl_typeset_templates():
+    '''
+    figure & axis sizes for various typesetting templates
+    ---
+    - jfm : Journal of Fluid Mechanics
+        - \textwidth is 384 [pt] / ~5.3134 [in]
+        - figures have 9pt fontsize
+    '''
+    def __init__(self, template='jfm', aspect=1.6, nx=1):
+        if (template=='jfm'):
+            #self.textwidth = 5.31445 ## inches
+            #self.linewidth = 5.31445 ## inches
+            self.textwidth = 384/72.27 ## inches = [pt]/[pts per inch]
+            self.linewidth = 384/72.27 ## inches = [pt]/[pts per inch]
+            self.textwidth = round(self.textwidth,4)
+            self.linewidth = round(self.linewidth,4)
+            self.fontsize  = 9 ## fontsize in figure env
+        else:
+            raise ValueError
+        
+        self.nx = nx ## number of panels in [x]
+        self.aspect = aspect
+        
+        ## [in]
+        self.width   = self.textwidth / self.nx
+        self.height  = self.width / self.aspect
+        self.figsize = (self.width,self.height)
+
 def colors_table():
     '''
     a table of color hues
     -----
     clrs = colors_table()
     red = clrs['red'][9]
     -----
```

### Comparing `turbx-0.3.8/turbx.egg-info/PKG-INFO` & `turbx-0.3.9/turbx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
@@ -13,55 +13,49 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mpi4py>=3.1
-Requires-Dist: numpy>=1.22
-Requires-Dist: scipy>=1.8
-Requires-Dist: h5py>=3.6
-Requires-Dist: matplotlib>=3.6
-Requires-Dist: scikit-image>=0.19
+Requires-Dist: numpy>=1.25
+Requires-Dist: scipy>=1.11
+Requires-Dist: h5py>=3.10
+Requires-Dist: matplotlib>=3.8
+Requires-Dist: scikit-image>=0.22
 Requires-Dist: psutil>=5.9
-Requires-Dist: tqdm>=4.64
-Requires-Dist: cmocean>=2.0
+Requires-Dist: tqdm>=4.66
+Requires-Dist: cmocean>=3.0
 Requires-Dist: colorcet>=3.0
-Requires-Dist: cmasher>=1.6
+Requires-Dist: cmasher>=1.7
 
 # turbx
 [![PyPI version](https://badge.fury.io/py/turbx.svg)](https://badge.fury.io/py/turbx)
 [![Downloads](https://pepy.tech/badge/turbx)](https://pepy.tech/project/turbx)
 
 Extensible toolkit for analyzing turbulent flow datasets.
 
 Install with `pip`:
 
 ```
 pip install --upgrade --user turbx
 ```
 
-Documentation available at: https://iagappel.github.io/turbx
-
 `turbx` runs in `python3` and uses parallel `HDF5` (wrapped by `h5py`) for high-performance collective MPI-IO with `mpi4py`. This requires:
 
 - A `python3` installation (3.8+ recommended)
 - An MPI implementation such as `OpenMPI`
 - A parallel `HDF5` installation (must be compiled with `--enable-parallel`) 
 - `mpi4py` (optionally compiled from source)
 - `h5py` compiled with parallel configuration
 
-An environment configuration guide can be found here: https://iagappel.github.io/turbx/env
-
 Visualization of `HDF5` datasets is possible using `Paraview` with the use of `xdmf` data descriptor files, which are written automatically by calling `.make_xdmf()` on `turbx` data class (such as `rgd`) class instances.
```

