# Comparing `tmp/ipyparallel-8.6.1.tar.gz` & `tmp/ipyparallel-8.7.0.tar.gz`

## Comparing `ipyparallel-8.6.1.tar` & `ipyparallel-8.7.0.tar`

### file list

```diff
@@ -1,295 +1,297 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.coveragerc
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.eslintignore
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.eslintrc.js
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.flake8
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.mailmap
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.prettierignore
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/asv.conf.json
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/install.json
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/package.json
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/readthedocs.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/tsconfig.json
--rw-r--r--   0        0        0   202459 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/yarn.lock
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.binder/jupyter_config.json
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.binder/postBuild
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.binder/requirements.txt
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv.conf.json
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv_normal.sh
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv_quick.sh
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/asv_runner.py
--rw-r--r--   0        0        0   182323 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/async_benchmark.ipynb
--rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmark_result.py
--rw-r--r--   0        0        0   669564 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmark_results.ipynb
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/cluster_start.py
--rw-r--r--   0        0        0    79070 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/depth_benchmark.ipynb
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/engines_test.py
--rwxr-xr-x   0        0        0     5486 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/gcloud_setup.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/instance_setup.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/logger.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling_initial_results.ipynb
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling_latest_results.ipynb
--rw-r--r--   0        0        0   160310 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/push_benchmarks.ipynb
--rw-r--r--   0        0        0   862420 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/scheduler_benchmarks.ipynb
--rw-r--r--   0        0        0   147522 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/throughtput_benchmarks.ipynb
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/testing.py
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/throughput.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/benchmarks/utils.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/explore/control_flow.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/explore/scheduler.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-16.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-32.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-64.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/machine_configs/asv-testing-96.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/profiling_code.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/profiling_code_runner.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/profiling/view_profiling_results.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/benchmarks.json
--rw-r--r--   0        0        0    16442 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json
--rw-r--r--   0        0        0    32378 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json
--rw-r--r--   0        0        0    36602 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json
--rw-r--r--   0        0        0    49624 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json
--rw-r--r--   0        0        0    70610 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/Dockerfile
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/docker-compose.yaml
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/entrypoint.sh
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/slurm/slurm.conf
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/ssh/Dockerfile
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/ssh/docker-compose.yaml
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ci/ssh/ipcluster_config.py
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/Makefile
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/make.bat
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/requirements.txt
--rw-r--r--   0        0        0    17267 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/changelog.md
--rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/conf.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/index.md
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/links.txt
--rw-r--r--   0        0        0   234426 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/_static/IPyParallel-MPI-Example.png
--rw-r--r--   0        0        0    69226 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/_static/basic.mp4
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/api/ipyparallel.rst
--rw-r--r--   0        0        0    26434 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Cluster API.ipynb
--rw-r--r--   0        0        0   279116 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Data Publication API.ipynb
--rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Futures.ipynb
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Index.ipynb
--rw-r--r--   0        0        0    67353 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb
--rw-r--r--   0        0        0    62592 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb
--rw-r--r--   0        0        0   165516 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Monte Carlo Options.ipynb
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Parallel Decorator and map.ipynb
--rw-r--r--   0        0        0  3554371 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Parallel Magics.ipynb
--rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Using Dill.ipynb
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/Using MPI with IPython Parallel.ipynb
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/customresults.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/dagdeps.py
--rw-r--r--   0        0        0    42291 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/dask.ipynb
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/dependencies.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/fetchparse.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/iopubwatcher.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/itermapresult.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/joblib.ipynb
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/nwmerge.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/phistogram.py
--rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/progress.ipynb
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/task_mod.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/task_profiler.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/throughput.py
--rw-r--r--   0        0        0   329806 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/visualizing-tasks.ipynb
--rw-r--r--   0        0        0   439979 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/Broadcast view.ipynb
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/Dockerfile
--rw-r--r--   0        0        0    69566 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/MPI Broadcast.ipynb
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/docker-compose.yaml
--rw-r--r--   0        0        0    84423 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/broadcast/memmap Broadcast.ipynb
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/pwordfreq.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/wordfreq.py
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/bintree.py
--rwxr-xr-x   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/bintree_script.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/communicator.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/interengine/interengine.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/pi/parallelpi.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/pi/pidigits.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipy
--rw-r--r--   0        0        0    45443 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipynb
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/rmt/rmtkernel.py
--rwxr-xr-x   0        0        0    19532 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/RectPartitioner.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/communicator.py
--rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave-mpi.py
--rwxr-xr-x   0        0        0     7405 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave.py
--rwxr-xr-x   0        0        0    11642 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/examples/wave2D/wavesolver.py
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/connections.md
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/dag_dependencies.md
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/db.md
--rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/details.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/index.md
--rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/launchers.md
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/messages.md
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/mpi.md
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/security.md
--rw-r--r--   0        0        0    32144 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/allconnections.png
--rw-r--r--   0        0        0   303213 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/allconnections.svg
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.pdf
--rw-r--r--   0        0        0   202436 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.png
--rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.png
--rw-r--r--   0        0        0   283962 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.svg
--rw-r--r--   0        0        0    38554 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/hbfade.png
--rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/iopubfade.png
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.png
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.svg
--rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.png
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.svg
--rw-r--r--   0        0        0    30974 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.png
--rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.svg
--rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/notiffade.png
--rw-r--r--   0        0        0    41180 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.png
--rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.svg
--rw-r--r--   0        0        0    38260 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/queryfade.png
--rw-r--r--   0        0        0    40459 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/queuefade.png
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/simpledag.pdf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/reference/figs/simpledag.png
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/asyncresult.md
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/demos.md
--rw-r--r--   0        0        0    23931 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/direct.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/index.md
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/intro.md
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/magics.md
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/process.md
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/task.md
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.pdf
--rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.png
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.pdf
--rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.png
--rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.pdf
--rw-r--r--   0        0        0    50744 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.png
--rw-r--r--   0        0        0   128061 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.pdf
--rw-r--r--   0        0        0   115825 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.png
--rw-r--r--   0        0        0    41799 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.pdf
--rw-r--r--   0        0        0    36727 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.png
--rw-r--r--   0        0        0    74773 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.pdf
--rw-r--r--   0        0        0    73675 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.png
--rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/docs/source/tutorial/figs/wideView.png
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/__init__.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/_async.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/_version.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/datapub.py
--rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/error.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/joblib.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/logger.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/traitlets.py
--rw-r--r--   0        0        0    23239 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/baseapp.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/ipclusterapp.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/ipcontrollerapp.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/ipengineapp.py
--rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/iploggerapp.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/launcher.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/apps/logwatcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/__init__.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/_joblib.py
--rw-r--r--   0        0        0    42109 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/asyncresult.py
--rw-r--r--   0        0        0    91891 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/client.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/futures.py
--rw-r--r--   0        0        0    18716 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/magics.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/map.py
--rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/remotefunction.py
--rw-r--r--   0        0        0    54129 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/client/view.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/__main__.py
--rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/_winhpcjob.py
--rwxr-xr-x   0        0        0    23629 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/app.py
--rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/cluster.py
--rw-r--r--   0        0        0    84108 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/cluster/launcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/__main__.py
--rwxr-xr-x   0        0        0    44147 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/app.py
--rw-r--r--   0        0        0     8820 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/broadcast_scheduler.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/dependency.py
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/dictdb.py
--rwxr-xr-x   0        0        0    10768 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/heartmonitor.py
--rw-r--r--   0        0        0    55731 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/hub.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/mongodb.py
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/scheduler.py
--rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/sqlitedb.py
--rw-r--r--   0        0        0    27127 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/controller/task_scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/__main__.py
--rwxr-xr-x   0        0        0    33960 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/app.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/datapub.py
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/kernel.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/log.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/engine/nanny.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/package.json
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/schemas/ipyparallel-labextension/plugin.json
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/114.b63b1cb1deb6ab07694a.js
--rw-r--r--   0        0        0    25407 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/remoteEntry.f5bc00ef0248261af0b1.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/style.js
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/__init__.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/base.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/handlers.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/install.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/static/clusterlist.css
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/static/clusterlist.js
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/nbextension/static/main.js
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/__init__.py
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/canning.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/codeutil.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/serialize/serialize.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/_test_startup_crash.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/clienttest.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/conftest.py
--rw-r--r--   0        0        0     8255 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_apps.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_async.py
--rw-r--r--   0        0        0    19138 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_asyncresult.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_canning.py
--rw-r--r--   0        0        0    24230 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_client.py
--rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_cluster.py
--rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_db.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_dependency.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_executor.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_joblib.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_launcher.py
--rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_lbview.py
--rw-r--r--   0        0        0    19042 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_magics.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_mongodb.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_mpi.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_remotefunction.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_serialize.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_slurm.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_ssh.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_util.py
--rw-r--r--   0        0        0    29736 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_view.py
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/ipyparallel/tests/test_view_broadcast.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/jupyter-config/jupyter_notebook_config.d/ipyparallel.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/jupyter-config/jupyter_server_config.d/ipyparallel.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/jupyter-config/nbconfig/tree.d/ipyparallel.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/webpack.config.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/schema/plugin.json
--rw-r--r--   0        0        0    23367 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/clusters.tsx
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/commands.ts
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/dialog.tsx
--rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/index.ts
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/sidebar.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/src/svg.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/code-dark.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/code-light.svg
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/index.css
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/lab/style/logo.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/.gitignore
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/COPYING.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/hatch_build.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 ipyparallel-8.6.1/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.coveragerc
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.eslintignore
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.eslintrc.js
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.flake8
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.mailmap
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.prettierignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/asv.conf.json
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/install.json
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/package.json
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/readthedocs.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/tsconfig.json
+-rw-r--r--   0        0        0   215267 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/yarn.lock
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.binder/jupyter_config.json
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.binder/postBuild
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.binder/requirements.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.github/workflows/test-docs.yml
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/asv.conf.json
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/asv_normal.sh
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/asv_quick.sh
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/asv_runner.py
+-rw-r--r--   0        0        0   182323 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/async_benchmark.ipynb
+-rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/benchmark_result.py
+-rw-r--r--   0        0        0   669564 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/benchmark_results.ipynb
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/cluster_start.py
+-rw-r--r--   0        0        0    79070 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/depth_benchmark.ipynb
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/engines_test.py
+-rwxr-xr-x   0        0        0     5534 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/gcloud_setup.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/instance_setup.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/logger.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/profiling_initial_results.ipynb
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/profiling_latest_results.ipynb
+-rw-r--r--   0        0        0   160310 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/push_benchmarks.ipynb
+-rw-r--r--   0        0        0   862420 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/scheduler_benchmarks.ipynb
+-rw-r--r--   0        0        0   147522 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/throughtput_benchmarks.ipynb
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/benchmarks/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/benchmarks/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/benchmarks/testing.py
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/benchmarks/throughput.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/benchmarks/utils.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/explore/control_flow.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/explore/scheduler.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/machine_configs/asv-testing-16.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/machine_configs/asv-testing-32.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/machine_configs/asv-testing-64.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/machine_configs/asv-testing-96.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/profiling/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/profiling/profiling_code.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/profiling/profiling_code_runner.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/profiling/view_profiling_results.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/results/benchmarks.json
+-rw-r--r--   0        0        0    16442 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json
+-rw-r--r--   0        0        0    32378 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json
+-rw-r--r--   0        0        0    36602 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json
+-rw-r--r--   0        0        0    49624 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json
+-rw-r--r--   0        0        0    70610 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ci/slurm/Dockerfile
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ci/slurm/docker-compose.yaml
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ci/slurm/entrypoint.sh
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ci/slurm/slurm.conf
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ci/ssh/Dockerfile
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ci/ssh/docker-compose.yaml
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ci/ssh/ipcluster_config.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/Makefile
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/make.bat
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/requirements.txt
+-rw-r--r--   0        0        0    20305 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/changelog.md
+-rw-r--r--   0        0        0    12760 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/index.md
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/links.txt
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/redirects.txt
+-rw-r--r--   0        0        0   234426 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/_static/IPyParallel-MPI-Example.png
+-rw-r--r--   0        0        0    69226 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/_static/basic.mp4
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/api/ipyparallel.rst
+-rw-r--r--   0        0        0    26434 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Cluster API.ipynb
+-rw-r--r--   0        0        0   279116 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Data Publication API.ipynb
+-rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Futures.ipynb
+-rw-r--r--   0        0        0    67353 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb
+-rw-r--r--   0        0        0    62592 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb
+-rw-r--r--   0        0        0   165516 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Monte Carlo Options.ipynb
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Parallel Decorator and map.ipynb
+-rw-r--r--   0        0        0  3554371 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Parallel Magics.ipynb
+-rw-r--r--   0        0        0    27925 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Using Dill.ipynb
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/Using MPI with IPython Parallel.ipynb
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/customresults.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/dagdeps.py
+-rw-r--r--   0        0        0    42291 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/dask.ipynb
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/dependencies.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/fetchparse.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/index.md
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/iopubwatcher.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/itermapresult.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/joblib.ipynb
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/nwmerge.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/phistogram.py
+-rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/progress.ipynb
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/task_mod.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/task_profiler.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/throughput.py
+-rw-r--r--   0        0        0   329806 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/visualizing-tasks.ipynb
+-rw-r--r--   0        0        0   439979 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/broadcast/Broadcast view.ipynb
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/broadcast/Dockerfile
+-rw-r--r--   0        0        0    69566 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/broadcast/MPI Broadcast.ipynb
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/broadcast/docker-compose.yaml
+-rw-r--r--   0        0        0    84423 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/broadcast/memmap Broadcast.ipynb
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/daVinci Word Count/pwordfreq.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/daVinci Word Count/wordfreq.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/interengine/bintree.py
+-rwxr-xr-x   0        0        0     2823 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/interengine/bintree_script.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/interengine/communicator.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/interengine/interengine.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/pi/parallelpi.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/pi/pidigits.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/rmt/rmt.ipy
+-rw-r--r--   0        0        0    45443 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/rmt/rmt.ipynb
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/rmt/rmtkernel.py
+-rwxr-xr-x   0        0        0    19532 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/wave2D/RectPartitioner.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/wave2D/communicator.py
+-rwxr-xr-x   0        0        0     7226 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/wave2D/parallelwave-mpi.py
+-rwxr-xr-x   0        0        0     7405 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/wave2D/parallelwave.py
+-rwxr-xr-x   0        0        0    11642 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/examples/wave2D/wavesolver.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/connections.md
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/dag_dependencies.md
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/db.md
+-rw-r--r--   0        0        0    21343 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/details.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/index.md
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/launchers.md
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/messages.md
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/mpi.md
+-rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/security.md
+-rw-r--r--   0        0        0    32144 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/allconnections.png
+-rw-r--r--   0        0        0   303213 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/allconnections.svg
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/dagdeps.pdf
+-rw-r--r--   0        0        0   202436 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/dagdeps.png
+-rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/frontend-kernel.png
+-rw-r--r--   0        0        0   283962 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/frontend-kernel.svg
+-rw-r--r--   0        0        0    38554 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/hbfade.png
+-rw-r--r--   0        0        0    39136 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/iopubfade.png
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/ipy_kernel_and_terminal.png
+-rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/ipy_kernel_and_terminal.svg
+-rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/nbconvert.png
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/nbconvert.svg
+-rw-r--r--   0        0        0    30974 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/notebook_components.png
+-rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/notebook_components.svg
+-rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/notiffade.png
+-rw-r--r--   0        0        0    41180 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/other_kernels.png
+-rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/other_kernels.svg
+-rw-r--r--   0        0        0    38260 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/queryfade.png
+-rw-r--r--   0        0        0    40459 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/queuefade.png
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/simpledag.pdf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/reference/figs/simpledag.png
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/asyncresult.md
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/demos.md
+-rw-r--r--   0        0        0    23931 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/direct.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/index.md
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/intro.md
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/magics.md
+-rw-r--r--   0        0        0    30400 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/process.md
+-rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/task.md
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/asian_call.pdf
+-rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/asian_call.png
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/asian_put.pdf
+-rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/asian_put.png
+-rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/mec_simple.pdf
+-rw-r--r--   0        0        0    50744 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/mec_simple.png
+-rw-r--r--   0        0        0   128061 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/parallel_pi.pdf
+-rw-r--r--   0        0        0   115825 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/parallel_pi.png
+-rw-r--r--   0        0        0    41799 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/single_digits.pdf
+-rw-r--r--   0        0        0    36727 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/single_digits.png
+-rw-r--r--   0        0        0    74773 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/two_digit_counts.pdf
+-rw-r--r--   0        0        0    73675 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/two_digit_counts.png
+-rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/docs/source/tutorial/figs/wideView.png
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/__init__.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/_async.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/_version.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/datapub.py
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/error.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/joblib.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/logger.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/traitlets.py
+-rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/__init__.py
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/baseapp.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/ipclusterapp.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/ipcontrollerapp.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/ipengineapp.py
+-rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/iploggerapp.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/launcher.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/apps/logwatcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/_joblib.py
+-rw-r--r--   0        0        0    42118 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/asyncresult.py
+-rw-r--r--   0        0        0    91846 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/client.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/futures.py
+-rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/magics.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/map.py
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/remotefunction.py
+-rw-r--r--   0        0        0    54130 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/client/view.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/cluster/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/cluster/__main__.py
+-rw-r--r--   0        0        0    10516 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/cluster/_winhpcjob.py
+-rwxr-xr-x   0        0        0    24501 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/cluster/app.py
+-rw-r--r--   0        0        0    36572 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/cluster/cluster.py
+-rw-r--r--   0        0        0    84806 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/cluster/launcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/__main__.py
+-rwxr-xr-x   0        0        0    44163 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/app.py
+-rw-r--r--   0        0        0     8820 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/broadcast_scheduler.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/dependency.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/dictdb.py
+-rwxr-xr-x   0        0        0    10768 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/heartmonitor.py
+-rw-r--r--   0        0        0    55732 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/hub.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/mongodb.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/scheduler.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/sqlitedb.py
+-rw-r--r--   0        0        0    27127 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/controller/task_scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/engine/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/engine/__main__.py
+-rwxr-xr-x   0        0        0    33960 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/engine/app.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/engine/datapub.py
+-rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/engine/kernel.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/engine/log.py
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/engine/nanny.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/labextension/package.json
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/labextension/schemas/ipyparallel-labextension/plugin.json
+-rw-r--r--   0        0        0    26026 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/labextension/static/998.d38d80ac3e2fa7501089.js
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/labextension/static/remoteEntry.ccf2bfedaae5f1da1a90.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/labextension/static/style.js
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/nbextension/__init__.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/nbextension/base.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/nbextension/handlers.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/nbextension/install.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/nbextension/static/clusterlist.css
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/nbextension/static/clusterlist.js
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/nbextension/static/main.js
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/serialize/__init__.py
+-rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/serialize/canning.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/serialize/codeutil.py
+-rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/serialize/serialize.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/_test_startup_crash.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/clienttest.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/conftest.py
+-rw-r--r--   0        0        0     8256 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_apps.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_async.py
+-rw-r--r--   0        0        0    19293 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_asyncresult.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_canning.py
+-rw-r--r--   0        0        0    24231 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_client.py
+-rw-r--r--   0        0        0    12282 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_cluster.py
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_db.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_dependency.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_executor.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_joblib.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_launcher.py
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_lbview.py
+-rw-r--r--   0        0        0    19043 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_magics.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_mongodb.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_mpi.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_remotefunction.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_serialize.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_slurm.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_ssh.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_util.py
+-rw-r--r--   0        0        0    29737 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_view.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/ipyparallel/tests/test_view_broadcast.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/jupyter-config/jupyter_notebook_config.d/ipyparallel.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/jupyter-config/jupyter_server_config.d/ipyparallel.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/jupyter-config/nbconfig/tree.d/ipyparallel.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/webpack.config.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/schema/plugin.json
+-rw-r--r--   0        0        0    23393 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/src/clusters.tsx
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/src/commands.ts
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/src/dialog.tsx
+-rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/src/index.ts
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/src/sidebar.ts
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/src/svg.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/style/code-dark.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/style/code-light.svg
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/style/index.css
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/lab/style/logo.svg
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/.gitignore
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/COPYING.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/hatch_build.py
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 ipyparallel-8.7.0/PKG-INFO
```

### Comparing `ipyparallel-8.6.1/.eslintrc.js` & `ipyparallel-8.7.0/.eslintrc.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
         node: true,
     },
     root: true,
     extends: [
         "eslint:recommended",
         "plugin:@typescript-eslint/eslint-recommended",
         "plugin:@typescript-eslint/recommended",
-        "prettier/@typescript-eslint",
+        "prettier",
         "plugin:react/recommended",
     ],
     parser: "@typescript-eslint/parser",
     parserOptions: {
         project: "tsconfig.eslint.json",
     },
     plugins: ["@typescript-eslint"],
```

### Comparing `ipyparallel-8.6.1/.flake8` & `ipyparallel-8.7.0/.flake8`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/.mailmap` & `ipyparallel-8.7.0/.mailmap`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/.pre-commit-config.yaml` & `ipyparallel-8.7.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 ci:
   autoupdate_schedule: monthly
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.15.0
     hooks:
       - id: pyupgrade
         args:
           - --py36-plus
         exclude: setupbase.py
   - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         exclude: setupbase.py
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 24.1.1
     hooks:
       - id: black
         exclude: setupbase.py
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
   - repo: https://github.com/PyCQA/flake8
-    rev: "6.0.0"
+    rev: "7.0.0"
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: end-of-file-fixer
       - id: check-case-conflict
       - id: check-executables-have-shebangs
       - id: requirements-txt-fixer
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.37.0
+    rev: v9.0.0-alpha.2
     hooks:
       - id: eslint
         files: \.[jt]sx?$ # *.js, *.jsx, *.ts and *.tsx
         exclude: ipyparallel/nbextension/.*
         types: [file]
         additional_dependencies:
           - "@typescript-eslint/eslint-plugin@2.27.0"
```

### Comparing `ipyparallel-8.6.1/CONTRIBUTING.md` & `ipyparallel-8.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/package.json` & `ipyparallel-8.7.0/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9432367149758455%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.6', '@jupyterlab/apputils': '^4.1.6', "*

 * *                   "'@jupyterlab/codeeditor': '^4.0.6', '@jupyterlab/console': '^4.0.6', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.6', '@jupyterlab/nbformat': '^4.0.6', "*

 * *                   "'@jupyterlab/notebook': '^4.0.6', '@jupyterlab/services': '^7.0.6', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.6', '@jupyterlab/statedb': '^4.0.6', "*

 * *                   "'@jupyterlab/ui-components': ' […]*

```diff
@@ -1,52 +1,51 @@
 {
     "author": "Min Ragan-Kelley",
     "bugs": {
         "url": "https://github.com/ipython/ipyparallel/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codeeditor": "^3.0.0",
-        "@jupyterlab/console": "^3.0.0",
-        "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.6.3",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.6.3",
-        "@jupyterlab/statedb": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/domutils": "^1.2.3",
-        "@lumino/dragdrop": "^1.7.1",
-        "@lumino/messaging": "^1.4.3",
-        "@lumino/polling": "^1.0.4",
-        "@lumino/signaling": "^1.4.3",
-        "@lumino/widgets": "^1.17.0",
-        "react": "~17.0.0",
-        "react-dom": "~17.0.0"
+        "@jupyterlab/application": "^4.0.6",
+        "@jupyterlab/apputils": "^4.1.6",
+        "@jupyterlab/codeeditor": "^4.0.6",
+        "@jupyterlab/console": "^4.0.6",
+        "@jupyterlab/coreutils": "^6.0.6",
+        "@jupyterlab/nbformat": "^4.0.6",
+        "@jupyterlab/notebook": "^4.0.6",
+        "@jupyterlab/services": "^7.0.6",
+        "@jupyterlab/settingregistry": "^4.0.6",
+        "@jupyterlab/statedb": "^4.0.6",
+        "@jupyterlab/ui-components": "^4.0.6",
+        "@lumino/algorithm": "^2.0.1",
+        "@lumino/commands": "^2.1.3",
+        "@lumino/coreutils": "^2.1.2",
+        "@lumino/domutils": "^2.0.1",
+        "@lumino/dragdrop": "^2.1.3",
+        "@lumino/messaging": "^2.0.1",
+        "@lumino/polling": "^2.1.2",
+        "@lumino/signaling": "^2.1.2",
+        "@lumino/widgets": "^2.3.0",
+        "react": "~18.2.0",
+        "react-dom": "~18.2.0"
     },
     "description": "A JupyterLab extension for IPython Parallel.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.10",
-        "@types/react": "~17.0.0",
-        "@types/react-dom": "~17.0.0",
-        "@typescript-eslint/eslint-plugin": "^5.18.0",
-        "@typescript-eslint/parser": "^5.18.0",
-        "eslint": "^8.37.0",
-        "eslint-config-prettier": "^8.5.0",
-        "eslint-plugin-prettier": "^4.0.0",
-        "eslint-plugin-react": "^7.21.5",
+        "@jupyterlab/builder": "^4.0.6",
+        "@types/react": "~18.2.24",
+        "@types/react-dom": "~18.2.8",
+        "@typescript-eslint/eslint-plugin": "^6.7.3",
+        "@typescript-eslint/parser": "^6.7.3",
+        "eslint": "^8.50.0",
+        "eslint-config-prettier": "^9.0.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "eslint-plugin-react": "^7.33.2",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.3.5",
-        "yarn": "^1.22.0"
+        "prettier": "^3.0.3",
+        "rimraf": "^5.0.5",
+        "typescript": "~5.2.2"
     },
     "files": [
         "lab/lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "lab/schema/*.json",
         "lab/style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ipython/ipyparallel",
@@ -91,9 +90,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.6.1"
+    "version": "8.7.0"
 }
```

### Comparing `ipyparallel-8.6.1/tsconfig.json` & `ipyparallel-8.7.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/.binder/postBuild` & `ipyparallel-8.7.0/.binder/postBuild`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/.github/workflows/release.yml` & `ipyparallel-8.7.0/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -16,20 +16,21 @@
     ${{ github.workflow }}-
     ${{ github.ref_type }}-
     ${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 jobs:
   build-release:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
-          python-version: 3.8
+          python-version: 3.11
+          cache: pip
 
       - name: install build package
         run: |
           pip install --upgrade pip
           pip install build
           pip freeze
 
@@ -37,29 +38,36 @@
         run: |
           python -m build --sdist --wheel .
           ls -l dist
 
       - name: verify wheel
         run: |
           cd dist
-          pip install ./*.whl jupyterlab==3.*
+          pip install ./*.whl jupyterlab==4.*
           ipcluster --help-all
           ipcontroller --help-all
           ipengine --help-all
           jupyter labextension list 2>&1 | grep ipyparallel
           jupyter server extension list 2>&1 | grep ipyparallel
 
       # ref: https://github.com/actions/upload-artifact#readme
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: ipyparallel-${{ github.sha }}
           path: "dist/*"
           if-no-files-found: error
 
-      - name: Publish to PyPI
-        if: startsWith(github.ref, 'refs/tags/')
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-        run: |
-          pip install twine
-          twine upload --skip-existing dist/*
+  upload-pypi:
+    permissions:
+      id-token: write
+    environment: release
+    runs-on: ubuntu-22.04
+    if: startsWith(github.ref, 'refs/tags/')
+    needs:
+      - build-release
+    steps:
+      - uses: actions/download-artifact@v4
+        with:
+          path: dist
+          merge-multiple: true
+      - name: Publish wheels to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `ipyparallel-8.6.1/.github/workflows/test.yml` & `ipyparallel-8.7.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,42 +29,42 @@
       fail-fast: false
       matrix:
         include:
           - python: "3.9"
             cluster_type: ssh
           - python: "3.8"
             cluster_type: mpi
-          - python: "3.7"
+          - python: "3.10"
             cluster_type: slurm
             container: slurmctld
-          - python: "3.7"
+          - python: "3.8"
           - python: "3.10"
             env:
               IPP_CONTROLLER_IP: "*"
           - python: "3.9"
             env:
               IPP_ENABLE_CURVE: "1"
           - python: "3.8"
             runs_on: windows-2019
           - python: "3.9"
-            runs_on: macos-10.15
+            runs_on: macos-11
           - python: "3.11"
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Cache conda environment
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: |
             ~/conda
           key: conda
 
       - name: Cache node_modules
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: |
             node_modules
           key: ${{ runner.os }}-yarn-${{ hashFiles('yarn.lock') }}
           restore-keys: |
             ${{ runner.os }}-yarn-
 
@@ -107,15 +107,15 @@
           eval "$(./bin/micromamba shell hook -s posix)"
           micromamba activate
           micromamba install -y -c conda-forge mpich mpi4py python=${{ matrix.python }}
           echo "PATH=$MAMBA_ROOT_PREFIX/bin:$PATH" >> $GITHUB_ENV
 
       - name: Install Python ${{ matrix.python }}
         if: ${{ matrix.cluster_type != 'mpi' }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
 
       - name: Install ipyparallel itself
         run: |
           pip install --upgrade pip
           pip install --no-deps .
@@ -150,15 +150,15 @@
       - name: Fixup coverage permissions ${{ matrix.container }}
         if: ${{ matrix.container }}
         run: |
           ls -l .coverage*
           ${EXEC} chmod -R a+rw .coverage*
 
       - name: Submit codecov report
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
 
       - name: Report on slurm
         if: ${{ matrix.cluster_type == 'slurm' && failure() }}
         run: |
           set -x
           docker ps -a
           docker logs slurmctld
```

### Comparing `ipyparallel-8.6.1/benchmarks/asv_runner.py` & `ipyparallel-8.7.0/benchmarks/asv_runner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/async_benchmark.ipynb` & `ipyparallel-8.7.0/benchmarks/async_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/benchmark_result.py` & `ipyparallel-8.7.0/benchmarks/benchmark_result.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/benchmark_results.ipynb` & `ipyparallel-8.7.0/benchmarks/benchmark_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/cluster_start.py` & `ipyparallel-8.7.0/benchmarks/cluster_start.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,36 +15,44 @@
         f'--HubFactory.db_class=NoDB'
     )
     print(ipcontroller_cmd)
     ipengine_cmd = f'{path}ipengine --profile=asv ' f'--cluster-id=depth_{depth} '
     ps = [
         Popen(
             ipcontroller_cmd.split(),
-            stdout=open('ipcontroller_output.log', 'a+')
-            if log_output_to_file
-            else sys.stdout,
-            stderr=open('ipcontroller_error_output.log', 'a+')
-            if log_output_to_file
-            else sys.stdout,
+            stdout=(
+                open('ipcontroller_output.log', 'a+')
+                if log_output_to_file
+                else sys.stdout
+            ),
+            stderr=(
+                open('ipcontroller_error_output.log', 'a+')
+                if log_output_to_file
+                else sys.stdout
+            ),
             stdin=sys.stdin,
         )
     ]
     time.sleep(2)
     client = ipp.Client(profile='asv', cluster_id=f'depth_{depth}')
     print(ipengine_cmd)
     for i in range(number_of_engines):
         ps.append(
             Popen(
                 ipengine_cmd.split(),
-                stdout=open('ipengine_output.log', 'a+')
-                if log_output_to_file
-                else sys.stdout,
-                stderr=open('ipengine_error_output.log', 'a+')
-                if log_output_to_file
-                else sys.stdout,
+                stdout=(
+                    open('ipengine_output.log', 'a+')
+                    if log_output_to_file
+                    else sys.stdout
+                ),
+                stderr=(
+                    open('ipengine_error_output.log', 'a+')
+                    if log_output_to_file
+                    else sys.stdout
+                ),
                 stdin=sys.stdin,
             )
         )
         if i % 10 == 0:
             wait_for(lambda: len(client) >= i - 10)
         if i % 20 == 0:
             time.sleep(2)
```

### Comparing `ipyparallel-8.6.1/benchmarks/depth_benchmark.ipynb` & `ipyparallel-8.7.0/benchmarks/depth_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/gcloud_setup.py` & `ipyparallel-8.7.0/benchmarks/gcloud_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,23 @@
         if INSTANCE_NAME_PREFIX in name
     ]
 
 
 def gcloud_run(*args, block=True):
     cmd = ["gcloud", "compute"] + list(args)
     print(f'$ {" ".join(cmd)}')
-    check_call(
-        cmd
-        # stdout=open(get_gcloud_log_file_name(instance_name) + ".log", "a+"),
-        # stderr=open(f"{get_gcloud_log_file_name(instance_name)}_error.out", "a+"),
-    ) if block else Popen(cmd)
+    (
+        check_call(
+            cmd
+            # stdout=open(get_gcloud_log_file_name(instance_name) + ".log", "a+"),
+            # stderr=open(f"{get_gcloud_log_file_name(instance_name)}_error.out", "a+"),
+        )
+        if block
+        else Popen(cmd)
+    )
 
 
 def copy_files_to_instance(instance_name, *file_names, directory="~"):
     for file_name in file_names:
         gcloud_run("scp", file_name, f"{instance_name}:{directory}", f"--zone={ZONE}")
```

### Comparing `ipyparallel-8.6.1/benchmarks/instance_setup.py` & `ipyparallel-8.7.0/benchmarks/instance_setup.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/logger.py` & `ipyparallel-8.7.0/benchmarks/logger.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/profiling_initial_results.ipynb` & `ipyparallel-8.7.0/benchmarks/profiling_initial_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/profiling_latest_results.ipynb` & `ipyparallel-8.7.0/benchmarks/profiling_latest_results.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/push_benchmarks.ipynb` & `ipyparallel-8.7.0/benchmarks/push_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/scheduler_benchmarks.ipynb` & `ipyparallel-8.7.0/benchmarks/scheduler_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/throughtput_benchmarks.ipynb` & `ipyparallel-8.7.0/benchmarks/throughtput_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/benchmarks/throughput.py` & `ipyparallel-8.7.0/benchmarks/benchmarks/throughput.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/benchmarks/utils.py` & `ipyparallel-8.7.0/benchmarks/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/explore/control_flow.py` & `ipyparallel-8.7.0/benchmarks/explore/control_flow.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/profiling/profiling_code.py` & `ipyparallel-8.7.0/benchmarks/profiling/profiling_code.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/profiling/profiling_code_runner.py` & `ipyparallel-8.7.0/benchmarks/profiling/profiling_code_runner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/profiling/view_profiling_results.py` & `ipyparallel-8.7.0/benchmarks/profiling/view_profiling_results.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/results/benchmarks.json` & `ipyparallel-8.7.0/benchmarks/results/benchmarks.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json` & `ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingBroadcast.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json` & `ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-04-28/CoalescingPush.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json` & `ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-05-12-19-52-58/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json` & `ipyparallel-8.7.0/benchmarks/results/asv-testing-64-2020-05-19-00-04-55/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json` & `ipyparallel-8.7.0/benchmarks/results/asv_testing-16-2020-04-29-20-02-25/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json` & `ipyparallel-8.7.0/benchmarks/results/asv_testing-16-2020-05-04-17-43/results.json`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ci/slurm/Dockerfile` & `ipyparallel-8.7.0/ci/slurm/Dockerfile`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ci/slurm/docker-compose.yaml` & `ipyparallel-8.7.0/ci/slurm/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ci/slurm/slurm.conf` & `ipyparallel-8.7.0/ci/slurm/slurm.conf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ci/ssh/Dockerfile` & `ipyparallel-8.7.0/ci/ssh/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,18 @@
     rm -f /etc/apt/apt.conf.d/docker-clean \
  && apt-get update \
  && apt-get -y install wget openssh-server
 
 ENV MAMBA_ROOT_PREFIX=/opt/conda
 ENV PATH=$MAMBA_ROOT_PREFIX/bin:$PATH
 ENV IPP_DISABLE_JS=1
-RUN wget -qO- https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba \
- && mv bin/micromamba /usr/local/bin/micromamba
+# x86_64 -> 64, aarch64 unmodified
+RUN ARCH=$(uname -m | sed s@x86_@@) \
+ && wget -qO- https://github.com/mamba-org/micromamba-releases/releases/latest/download/micromamba-linux-${ARCH} > /usr/local/bin/micromamba \
+ && chmod +x /usr/local/bin/micromamba
 
 RUN --mount=type=cache,target=${MAMBA_ROOT_PREFIX}/pkgs \
     micromamba install -y -p $MAMBA_ROOT_PREFIX -c conda-forge \
         python=3.8 \
         pip \
         ipyparallel
```

### Comparing `ipyparallel-8.6.1/ci/ssh/ipcluster_config.py` & `ipyparallel-8.7.0/ci/ssh/ipcluster_config.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/changelog.md` & `ipyparallel-8.7.0/docs/source/changelog.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,51 @@
 (changelog)=
 
 # Changelog
 
 Changes in IPython Parallel
 
+## 8.7
+
+### 8.7.0 - 2024-03-04
+
+([full changelog](https://github.com/ipython/ipyparallel/compare/8.6.1...8.7.0))
+
+8.7 is a small release, with a few improvements and updates, mostly related to compatibility with different versions of JupyterLab, Notebook, and Jupyter Server.
+
+Highlights:
+
+- JupyterLab 4 compatibility for the lab extension
+- Improved logging and deprecation messages for different versions of Jupyter Server and Notebook
+
+#### New features added
+
+- Update labextension to jupyterlab 4 [#833](https://github.com/ipython/ipyparallel/pull/833) ([@minrk](https://github.com/minrk))
+- add `ControllerLauncher.connection_info_timeout` config [#872](https://github.com/ipython/ipyparallel/pull/872) ([@minrk](https://github.com/minrk))
+
+#### Enhancements made
+
+- log launcher output at warning-level in case of nonzero exit code [#866](https://github.com/ipython/ipyparallel/pull/866) ([@minrk](https://github.com/minrk))
+- improve deprecation messaging around `ipcluster nbextension` [#835](https://github.com/ipython/ipyparallel/pull/835) ([@minrk](https://github.com/minrk))
+
+#### Bugs fixed
+
+- Use pre-3.10 serialization code on PyPy3.10 [#846](https://github.com/ipython/ipyparallel/pull/846) ([@mgorny](https://github.com/mgorny), [@minrk](https://github.com/minrk))
+- fallback import when using notebook and jupyter_server is unavailable [#808](https://github.com/ipython/ipyparallel/pull/808) ([@minrk](https://github.com/minrk))
+- don't propagate logs in IPython [#797](https://github.com/ipython/ipyparallel/pull/797) ([@minrk](https://github.com/minrk))
+
+#### Contributors to this release
+
+The following people contributed discussions, new ideas, code and documentation contributions, and review.
+See [our definition of contributors](https://github-activity.readthedocs.io/en/latest/#how-does-this-tool-define-contributions-in-the-reports).
+
+([GitHub contributors page for this release](https://github.com/ipython/ipyparallel/graphs/contributors?from=2023-04-14&to=2024-03-04&type=c))
+
+@ellert ([activity](https://github.com/search?q=repo%3Aipython%2Fipyparallel+involves%3Aellert+updated%3A2023-04-14..2024-03-04&type=Issues)) | @hroncok ([activity](https://github.com/search?q=repo%3Aipython%2Fipyparallel+involves%3Ahroncok+updated%3A2023-04-14..2024-03-04&type=Issues)) | @mgorny ([activity](https://github.com/search?q=repo%3Aipython%2Fipyparallel+involves%3Amgorny+updated%3A2023-04-14..2024-03-04&type=Issues)) | @minrk ([activity](https://github.com/search?q=repo%3Aipython%2Fipyparallel+involves%3Aminrk+updated%3A2023-04-14..2024-03-04&type=Issues)) | @ottointhesky ([activity](https://github.com/search?q=repo%3Aipython%2Fipyparallel+involves%3Aottointhesky+updated%3A2023-04-14..2024-03-04&type=Issues)) | @tornaria ([activity](https://github.com/search?q=repo%3Aipython%2Fipyparallel+involves%3Atornaria+updated%3A2023-04-14..2024-03-04&type=Issues)) | @WernerFS ([activity](https://github.com/search?q=repo%3Aipython%2Fipyparallel+involves%3AWernerFS+updated%3A2023-04-14..2024-03-04&type=Issues))
+
 ## 8.6
 
 ### 8.6.1
 
 ([full changelog](https://github.com/ipython/ipyparallel/compare/8.6.0...8.6.1))
 
 ### Bugs fixed
@@ -238,15 +276,15 @@
 - Remove dependency on deprecated ipython-genutils
 - New dependencies on psutil, entrypoints, tqdm
 
 New features:
 
 - New {class}`.Cluster` API for managing clusters from Python,
   including support for signaling and restarting engines.
-  See [docs](../examples/Cluster%20API.ipynb) for more.
+  See [docs](./examples/Cluster%20API.ipynb) for more.
 - New `ipcluster list` and `ipcluster clean` commands derived from the Cluster API.
 - New {meth}`.Client.send_signal` for sending signals to single engines.
 - New KernelNanny process for signaling and monitoring engines
   for improved responsiveness of handing engine crashes.
 - New prototype {class}`.BroadcastScheduler` with vastly improved scaling in 'do-on-all' operations
   on large numbers of engines,
   c/o Tom-Olav Bøyum's [Master's thesis][] at University of Oslo.
@@ -258,15 +296,15 @@
 - Launchers registered via entrypoints for better support of third-party Launchers.
 - New JupyterLab extension (enabled by default) based on dask-labextension
   for managing clusters.
 - {meth}`.LoadBalancedView.imap` consumes inputs as-needed,
   producing a generator of results instead of an AsyncMapResult,
   allowing for consumption of very large or infinite mapping inputs.
 
-[broadcast view documentation]: ../examples/broadcast/Broadcast%20view.ipynb
+[broadcast view documentation]: ./examples/broadcast/Broadcast%20view.ipynb
 [master's thesis]: https://urn.nb.no/URN:NBN:no-84589
 
 Improvements and other fixes:
 
 - Greatly improved performance of heartbeat and registration with large numbers of engines,
   tested with 5000 engines and default configuration.
 - Single `IPController.ports` configuration to specify the pool of ports for the controller to use,
@@ -416,15 +454,15 @@
 ipcluster nbextension enable
 ```
 
 which does all three steps above.
 
 ### Slurm support
 
-[Slurm](https://hpc.llnl.gov/training/tutorials/livermore-computing-linux-commodity-clusters-overview-part-one) support is added to ipcluster.
+[Slurm](https://hpc.llnl.gov/documentation/tutorials/livermore-computing-linux-commodity-clusters-overview-part-two) support is added to ipcluster.
 
 ### 5.1.0
 
 [5.1.0 on GitHub](https://github.com/ipython/ipyparallel/milestones/5.1)
 
 ## 5.0
```

### Comparing `ipyparallel-8.6.1/docs/source/conf.py` & `ipyparallel-8.7.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,35 @@
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
     'sphinx.ext.inheritance_diagram',
     'sphinx.ext.intersphinx',
     'sphinx.ext.napoleon',
-    'myst_parser',
-    'nbsphinx',
+    "sphinxext.rediraffe",
+    # 'myst_parser',
+    'myst_nb',
     'IPython.sphinxext.ipython_console_highlighting',
     'autodoc_traits',
 ]
 
 myst_enable_extensions = [
     'colon_fence',
     'deflist',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-source_suffix = ['.md', '.rst']
+source_suffix = {
+    ".rst": "restructuredtext",
+    ".ipynb": "myst-nb",
+}
 
 from traitlets.config import LoggingConfigurable
 
 # exclude members inherited from HasTraits by default
 autodoc_default_options = {
     'members': None,
     "exclude-members": ','.join(dir(LoggingConfigurable)),
@@ -84,17 +88,16 @@
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 from datetime import date
 
-today = date.today()
 project = 'ipyparallel'
-copyright = '%04d, The IPython Development Team' % today.year
+copyright = '%04d, The IPython Development Team' % date.today().year
 author = 'The IPython Development Team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -359,11 +362,32 @@
     'python': ('https://docs.python.org/3/', None),
     'ipython': ('https://ipython.readthedocs.io/en/stable/', None),
     'pymongo': ('https://pymongo.readthedocs.io/en/stable/', None),
     'distributed': ('https://distributed.readthedocs.io/en/stable/', None),
     'jupyterclient': ('https://jupyter-client.readthedocs.io/en/stable/', None),
 }
 
+import os
+
+rediraffe_branch = os.environ.get("REDIRAFFE_BRANCH", "main")
+rediraffe_redirects = "redirects.txt"
+
+# allow 80% match for autogenerated redirects
+rediraffe_auto_redirect_perc = 80
+
 
-# nbsphinx config
-# https://nbsphinx.readthedocs.io/en/latest/usage.html
-nbsphinx_execute = 'auto'
+linkcheck_ignore = [
+    r"https://github.com/[^/]*$",  # too many github usernames / searches in changelog
+    "https://github.com/ipython/ipyparallel/pull/",  # too many PRs in changelog
+    "https://github.com/search",  # github search links
+    "https://github.com/ipython/ipyparallel/compare/",  # too many comparisons in changelog
+    r"https?://(localhost|127.0.0.1).*",  # ignore localhost references in auto-links
+]
+
+# myst_nb execution
+nb_execution_mode = "off"
+
+# avoid warning during linkcheck about image-only output
+nb_mime_priority_overrides = [
+    ("linkcheck", "text/html", 10),
+    ("linkcheck", "image/png", 99),
+]
```

### Comparing `ipyparallel-8.6.1/docs/source/index.md` & `ipyparallel-8.7.0/docs/source/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 tutorial/index
 reference/index
 ```
 
 ```{toctree}
 :maxdepth: 2
 
-examples/Index
+examples/index
 ```
 
 ```{toctree}
 :maxdepth: 1
 
 changelog
 ```
```

### Comparing `ipyparallel-8.6.1/docs/source/links.txt` & `ipyparallel-8.7.0/docs/source/links.txt`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/_static/IPyParallel-MPI-Example.png` & `ipyparallel-8.7.0/docs/source/_static/IPyParallel-MPI-Example.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/_static/basic.mp4` & `ipyparallel-8.7.0/docs/source/_static/basic.mp4`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/api/ipyparallel.rst` & `ipyparallel-8.7.0/docs/source/api/ipyparallel.rst`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Cluster API.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Cluster API.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Data Publication API.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Data Publication API.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Futures.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Futures.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Monitoring an MPI Simulation - 1.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Monitoring an MPI Simulation - 2.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Monte Carlo Options.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Monte Carlo Options.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Parallel Decorator and map.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Parallel Decorator and map.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Parallel Magics.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Parallel Magics.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/Using Dill.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Using Dill.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999003189792663%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(5, 'Another is "*

 * *            "[cloudpickle](https://github.com/cloudpipe/cloudpickle).\\n')], delete: [5]}}}"}*

```diff
@@ -12,15 +12,15 @@
             "metadata": {},
             "source": [
                 "ipyparallel doesn't do much in the way of serialization.\n",
                 "It has custom zero-copy handling of numpy arrays,\n",
                 "but other than that, it doesn't do anything other than the bare minimum to make basic interactively defined functions and classes sendable.\n",
                 "\n",
                 "There are a few projects that extend pickle to make just about anything sendable, and one of these is [dill](https://dill.readthedocs.io).\n",
-                "Another is [cloudpickle](https://cloudpickle.readthedocs.io).\n",
+                "Another is [cloudpickle](https://github.com/cloudpipe/cloudpickle).\n",
                 "\n",
                 "To install dill:\n",
                 "        \n",
                 "    pip install dill"
             ]
         },
         {
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/Using MPI with IPython Parallel.ipynb` & `ipyparallel-8.7.0/docs/source/examples/Using MPI with IPython Parallel.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995614035087719%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'Our documentation describes [how to create an MPI "*

 * *            "profile](https://ipyparallel.readthedocs.io/en/stable/tutorial/process.html#using-ipython-parallel-with-mpi)\\n'), "*

 * *            "(4, 'and explains [basic MPI usage of the IPython "*

 * *            "cluster](https://ipyparallel.readthedocs.io/en/stable/reference/mpi.html).\\n')], "*

 * *            'delete: [4, 3]}}}'}*

```diff
@@ -10,16 +10,16 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This example assumes you've started a cluster of N engines (4 in this example) as part\n",
                 "of an MPI world.  \n",
                 "\n",
-                "Our documentation describes [how to create an MPI profile](https://ipyparallel.readthedocs.io/en/stable/process.html#using-ipcluster-in-mpiexec-mpirun-mode)\n",
-                "and explains [basic MPI usage of the IPython cluster](https://ipyparallel.readthedocs.io/en/stable/mpi.html).\n",
+                "Our documentation describes [how to create an MPI profile](https://ipyparallel.readthedocs.io/en/stable/tutorial/process.html#using-ipython-parallel-with-mpi)\n",
+                "and explains [basic MPI usage of the IPython cluster](https://ipyparallel.readthedocs.io/en/stable/reference/mpi.html).\n",
                 "\n",
                 "\n",
                 "For the simplest possible way to start 4 engines that belong to the same MPI world, \n",
                 "you can run this in a terminal:\n",
                 "\n",
                 "<pre>\n",
                 "ipcluster start --engines=MPI -n 4\n",
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/customresults.py` & `ipyparallel-8.7.0/docs/source/examples/customresults.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 This just submits a bunch of jobs, waits on the results, and prints the stdout
 and results of each as they finish.
 
 Authors
 -------
 * MinRK
 """
+
 import random
 
 import ipyparallel as ipp
 
 # create client & views
 rc = ipp.Client()
 dv = rc[:]
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/dagdeps.py` & `ipyparallel-8.7.0/docs/source/examples/dagdeps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This demo uses networkx to generate the graph.
 
 Authors
 -------
 * MinRK
 """
+
 from random import randint
 
 import networkx as nx
 
 import ipyparallel as parallel
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/dask.ipynb` & `ipyparallel-8.7.0/docs/source/examples/dask.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/dependencies.py` & `ipyparallel-8.7.0/docs/source/examples/dependencies.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/fetchparse.py` & `ipyparallel-8.7.0/docs/source/examples/fetchparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 This module gives an example of how the task interface to the
 IPython controller works.  Before running this script start the IPython controller
 and some engines using something like::
 
     ipcluster start -n 4
 """
+
 import sys
 import time
 
 import bs4  # noqa this isn't necessary, but it helps throw the dependency error earlier
 
 import ipyparallel as ipp
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/iopubwatcher.py` & `ipyparallel-8.7.0/docs/source/examples/iopubwatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 You can use the zeromq SUBSCRIBE mechanism to only receive information from specific engines,
 and easily filter by message type.
 
 Authors
 -------
 * MinRK
 """
+
 import json
 import sys
 
 import zmq
 from ipykernel.connect import find_connection_file
 from jupyter_client.session import Session
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/itermapresult.py` & `ipyparallel-8.7.0/docs/source/examples/itermapresult.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if you call `map(...ordered=False)`, then results will be provided to the iterator
 on a first come first serve basis.
 
 Authors
 -------
 * MinRK
 """
+
 import time
 
 import ipyparallel as ipp
 
 # create client & view
 rc = ipp.Client()
 dv = rc[:]
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/joblib.ipynb` & `ipyparallel-8.7.0/docs/source/examples/joblib.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/nwmerge.py` & `ipyparallel-8.7.0/docs/source/examples/nwmerge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Example showing how to merge multiple remote data streams.
 """
+
 # Slightly modified version of:
 # https://aspn.activestate.com/ASPN/Cookbook/Python/Recipe/511509
 import heapq
 
 import ipyparallel as ipp
 from ipyparallel.error import RemoteError
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/phistogram.py` & `ipyparallel-8.7.0/docs/source/examples/phistogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parallel histogram function"""
+
 from ipyparallel import Reference
 
 
 def phistogram(view, a, bins=10, rng=None, normed=False):
     """Compute the histogram of a remote array a.
 
     Parameters
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/progress.ipynb` & `ipyparallel-8.7.0/docs/source/examples/progress.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/task_profiler.py` & `ipyparallel-8.7.0/docs/source/examples/task_profiler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/throughput.py` & `ipyparallel-8.7.0/docs/source/examples/throughput.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/visualizing-tasks.ipynb` & `ipyparallel-8.7.0/docs/source/examples/visualizing-tasks.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/broadcast/Broadcast view.ipynb` & `ipyparallel-8.7.0/docs/source/examples/broadcast/Broadcast view.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/broadcast/MPI Broadcast.ipynb` & `ipyparallel-8.7.0/docs/source/examples/broadcast/MPI Broadcast.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/broadcast/docker-compose.yaml` & `ipyparallel-8.7.0/docs/source/examples/broadcast/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/broadcast/memmap Broadcast.ipynb` & `ipyparallel-8.7.0/docs/source/examples/broadcast/memmap Broadcast.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/pwordfreq.py` & `ipyparallel-8.7.0/docs/source/examples/daVinci Word Count/pwordfreq.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/daVinci Word Count/wordfreq.py` & `ipyparallel-8.7.0/docs/source/examples/daVinci Word Count/wordfreq.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/interengine/bintree.py` & `ipyparallel-8.7.0/docs/source/examples/interengine/bintree.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 BinaryTree inter-engine communication class
 
 use from bintree_script.py
 
 Provides parallel [all]reduce functionality
 
 """
+
 import re
 import socket
 from functools import reduce
 
 import zmq
 
 from ipyparallel.serialize import deserialize_object, serialize_object
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/interengine/bintree_script.py` & `ipyparallel-8.7.0/docs/source/examples/interengine/bintree_script.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/interengine/communicator.py` & `ipyparallel-8.7.0/docs/source/examples/interengine/communicator.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/interengine/interengine.py` & `ipyparallel-8.7.0/docs/source/examples/interengine/interengine.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/pi/parallelpi.py` & `ipyparallel-8.7.0/docs/source/examples/pi/parallelpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 The dataset we have been using for this is the 200 million digit one here:
 ftp://pi.super-computing.org/.2/pi200m/
 
 and the files used will be downloaded if they are not in the working directory
 of the IPython engines.
 """
+
 from timeit import default_timer as clock
 
 from matplotlib import pyplot as plt
 from pidigits import (
     compute_two_digit_freqs,
     fetch_pi_file,
     plot_two_digit_freqs,
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/pi/pidigits.py` & `ipyparallel-8.7.0/docs/source/examples/pi/pidigits.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 straightforward.
 
 This focuses on computing the number of times that
 all 1, 2, n digits sequences occur in the digits of pi.
 If the digits of pi are truly random, these frequencies
 should be equal.
 """
+
 import os
 from urllib.request import urlretrieve
 
 import numpy as np
 from matplotlib import pyplot as plt
 
 # Top-level functions
```

### Comparing `ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipy` & `ipyparallel-8.7.0/docs/source/examples/rmt/rmt.ipy`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/rmt/rmt.ipynb` & `ipyparallel-8.7.0/docs/source/examples/rmt/rmt.ipynb`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/rmt/rmtkernel.py` & `ipyparallel-8.7.0/docs/source/examples/rmt/rmtkernel.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/wave2D/RectPartitioner.py` & `ipyparallel-8.7.0/docs/source/examples/wave2D/RectPartitioner.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/wave2D/communicator.py` & `ipyparallel-8.7.0/docs/source/examples/wave2D/communicator.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave-mpi.py` & `ipyparallel-8.7.0/docs/source/examples/wave2D/parallelwave-mpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/wave2D/parallelwave.py` & `ipyparallel-8.7.0/docs/source/examples/wave2D/parallelwave.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/examples/wave2D/wavesolver.py` & `ipyparallel-8.7.0/docs/source/examples/wave2D/wavesolver.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/connections.md` & `ipyparallel-8.7.0/docs/source/reference/connections.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/dag_dependencies.md` & `ipyparallel-8.7.0/docs/source/reference/dag_dependencies.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/db.md` & `ipyparallel-8.7.0/docs/source/reference/db.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 However, since we have this DB backend, we provide a direct query method in the {class}`~.Client`
 for users who want deeper introspection into their task history. The {meth}`db_query` method of
 the Client is modeled after MongoDB queries, so if you have used MongoDB it should look
 familiar. In fact, when the MongoDB backend is in use, the query is relayed directly.
 When using other backends, the interface is emulated and only a subset of queries is possible.
 
 ```{seealso}
-MongoDB [query docs](https://docs.mongodb.com/manual/tutorial/query-documents/)
+MongoDB [query docs](https://www.mongodb.com/docs/manual/tutorial/query-documents/)
 ```
 
 {meth}`Client.db_query` takes a dictionary query object, with keys from the TaskRecord key list,
 and values of either exact values to test, or MongoDB queries, which are dicts of The form:
 `{'operator' : 'argument(s)'}`. There is also an optional `keys` argument, that specifies
 which subset of keys should be retrieved. The default is to retrieve all keys excluding the
 request and result buffers. {meth}`db_query` returns a list of TaskRecord dicts. Also like
```

### Comparing `ipyparallel-8.6.1/docs/source/reference/details.md` & `ipyparallel-8.7.0/docs/source/reference/details.md`

 * *Files 0% similar despite different names*

```diff
@@ -650,25 +650,26 @@
 What keyword arguments are available depends on the view being used.
 
 ```{eval-rst}
 .. class:: ipyparallel.DirectView
    :noindex:
 
    .. automethod:: map
+      :noindex:
 ```
 
 ```{eval-rst}
 .. class:: ipyparallel.LoadBalancedView
    :noindex:
 
    .. automethod:: map
+      :noindex:
 
    .. automethod:: imap
-
-
+      :noindex:
 ```
 
 ## Decorators and RemoteFunctions
 
 ```{note}
 TODO: write this section
 ```
```

### Comparing `ipyparallel-8.6.1/docs/source/reference/launchers.md` & `ipyparallel-8.7.0/docs/source/reference/launchers.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 principally `profile_dir` and `cluster_id` are typically used to locate the connection files necessary for these two communicate,
 though explicit paths can be added to arguments.
 
 Launchers are used through the {class}`~.Cluster` API,
 which manages one ControllerLauncher and zero to many EngineLaunchers,
 each representing a set of engines.
 
-Launchers are registered via entry points ([more below](#entrypoints)),
+Launchers are registered via entry points ([more below](entrypoints)),
 and can be selected via short lowercase string naming the kind of launcher, e.g. 'mpi' or 'local':
 
 ```python
 import ipyparallel as ipp
 c = ipp.Cluster(engines="mpi")
 ```
 
@@ -49,17 +49,19 @@
 ## Writing your own Launcher(s)
 
 If you want to write your own launcher,
 the best place to start is to look at the Launcher classes that ship with IPython Parallel.
 
 There are three key methods to implement:
 
-- [`start()`](#writing-start)
-- [`stop()`](#writing-stop)
-- [`from_dict()`](#writing-from-dict)
+- [`start()`](writing-start)
+- [`stop()`](writing-stop)
+- [`from_dict()`](writing-from-dict)
+
+(writing-start)=
 
 ### Writing start
 
 A start method on a launcher should do the following:
 
 1. request the process(es) to be started
 2. start monitoring to notice when the process exits, such that {meth}`.notify_stop` will be called when the process exits.
@@ -75,14 +77,16 @@
 _ControllerLauncher.start_ is always called with no arguments,
 whereas `EngineLauncher.start` is called with `n`,
 which is an integer or None. If `n` is an integer,
 this many engines should be started.
 If `n` is None, a 'default' number should be used,
 e.g. the number of CPUs on a host.
 
+(writing-stop)=
+
 ### Writing stop
 
 A stop method should request that the process(es) stop,
 and return only after everything is stopped and cleaned up.
 Exactly how to collect these resources will depend greatly on how the resources were requested in `start`.
 
 ### Serializing Launchers
@@ -114,14 +118,16 @@
 def start(self):
     process = start_process(self.args, ...)
     self.pid = process.pid
 ```
 
 Mark whatever properties are required to reconstruct your object from disk with this metadata.
 
+(writing-from-dict)=
+
 #### writing from_dict
 
 {meth}`~.BaseLauncher.from_dict` should be a class method which returns an instance of your Launcher class, loaded from dict.
 
 Most `from_dict` methods will look similar to this:
 
 ```{literalinclude} ../../../ipyparallel/cluster/launcher.py
@@ -150,15 +156,15 @@
 Some useful additional methods to implement, if the base class implementations do not work for you:
 
 - {meth}`~.ControllerLauncher.get_connection_info`
 - {meth}`~.BaseLauncher.get_output`
 
 TODO: write more docs on these
 
-=(entrypoints)
+(entrypoints)=
 
 ## Registering your Launcher via entrypoints
 
 Once you have defined your launcher, you can 'register' it for discovery
 via entrypoints. In your setup.py:
 
 ```python
```

### Comparing `ipyparallel-8.6.1/docs/source/reference/messages.md` & `ipyparallel-8.7.0/docs/source/reference/messages.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/mpi.md` & `ipyparallel-8.7.0/docs/source/reference/mpi.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/security.md` & `ipyparallel-8.7.0/docs/source/reference/security.md`

 * *Files 1% similar despite different names*

```diff
@@ -377,10 +377,9 @@
 ipc file permissions,
 and and/or SSH tunneled TCP/IP channels,
 address the core potential vulnerabilities in the system,
 while still enabling user's to use the system in open networks.
 
 [openssh]: https://www.openssh.com
 [paramiko]: https://www.lag.net/paramiko
-[hmac]: https://tools.ietf.org/html/rfc2104
-[rfc5246]: https://tools.ietf.org/html/rfc5246
+[hmac]: https://datatracker.ietf.org/doc/html/rfc2104
 [curvezmq]: https://rfc.zeromq.org/spec/26/
```

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/allconnections.png` & `ipyparallel-8.7.0/docs/source/reference/figs/allconnections.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/allconnections.svg` & `ipyparallel-8.7.0/docs/source/reference/figs/allconnections.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.pdf` & `ipyparallel-8.7.0/docs/source/reference/figs/dagdeps.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/dagdeps.png` & `ipyparallel-8.7.0/docs/source/reference/figs/dagdeps.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.png` & `ipyparallel-8.7.0/docs/source/reference/figs/frontend-kernel.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/frontend-kernel.svg` & `ipyparallel-8.7.0/docs/source/reference/figs/frontend-kernel.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/hbfade.png` & `ipyparallel-8.7.0/docs/source/reference/figs/hbfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/iopubfade.png` & `ipyparallel-8.7.0/docs/source/reference/figs/iopubfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.png` & `ipyparallel-8.7.0/docs/source/reference/figs/ipy_kernel_and_terminal.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/ipy_kernel_and_terminal.svg` & `ipyparallel-8.7.0/docs/source/reference/figs/ipy_kernel_and_terminal.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.png` & `ipyparallel-8.7.0/docs/source/reference/figs/nbconvert.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/nbconvert.svg` & `ipyparallel-8.7.0/docs/source/reference/figs/nbconvert.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.png` & `ipyparallel-8.7.0/docs/source/reference/figs/notebook_components.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/notebook_components.svg` & `ipyparallel-8.7.0/docs/source/reference/figs/notebook_components.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/notiffade.png` & `ipyparallel-8.7.0/docs/source/reference/figs/notiffade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.png` & `ipyparallel-8.7.0/docs/source/reference/figs/other_kernels.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/other_kernels.svg` & `ipyparallel-8.7.0/docs/source/reference/figs/other_kernels.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/queryfade.png` & `ipyparallel-8.7.0/docs/source/reference/figs/queryfade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/queuefade.png` & `ipyparallel-8.7.0/docs/source/reference/figs/queuefade.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/simpledag.pdf` & `ipyparallel-8.7.0/docs/source/reference/figs/simpledag.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/reference/figs/simpledag.png` & `ipyparallel-8.7.0/docs/source/reference/figs/simpledag.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/asyncresult.md` & `ipyparallel-8.7.0/docs/source/tutorial/asyncresult.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/demos.md` & `ipyparallel-8.7.0/docs/source/tutorial/demos.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/direct.md` & `ipyparallel-8.7.0/docs/source/tutorial/direct.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/intro.md` & `ipyparallel-8.7.0/docs/source/tutorial/intro.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Overview and getting started
 
 ## Examples
 
 We have various example scripts and notebooks for using ipyparallel in our
 {file}`docs/source/examples` directory, as covered in the [examples][] section.
 
-[examples]: ../examples/Index.ipynb
+[examples]: ../examples/index.md
 
 ## Introduction
 
 This section gives an overview of IPython's
 architecture for parallel and distributed computing. This architecture
 abstracts out parallelism in a general way, enabling IPython to
 support many different styles of parallelism, including:
```

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/magics.md` & `ipyparallel-8.7.0/docs/source/tutorial/magics.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/process.md` & `ipyparallel-8.7.0/docs/source/tutorial/process.md`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,16 @@
 have not yet supported
 ```
 
 ### Writing custom Launchers
 
 TODO: example writing custom Launchers
 
+(ipcluster-mpi)=
+
 ### Using IPython Parallel with MPI
 
 The mpiexec/mpirun mode is useful if:
 
 1. You have MPI installed.
 2. Your systems are configured to use the {command}`mpiexec` or
    {command}`mpirun` commands to start MPI processes.
@@ -335,14 +337,17 @@
 c.IPController.ip = '*'
 ```
 
 You can now run the cluster with:
 
 ```python
 cluster = Cluster(profile="pbs")
+```
+
+```
 $ ipcluster start --profile=pbs -n 128
 ```
 
 ### Starting a cluster with SSH
 
 The SSH mode uses {command}`ssh` to execute {command}`ipengine` on remote
 nodes and {command}`ipcontroller` can be run remotely as well, or on localhost.
```

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/task.md` & `ipyparallel-8.7.0/docs/source/tutorial/task.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.pdf` & `ipyparallel-8.7.0/docs/source/tutorial/figs/asian_call.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_call.png` & `ipyparallel-8.7.0/docs/source/tutorial/figs/asian_call.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.pdf` & `ipyparallel-8.7.0/docs/source/tutorial/figs/asian_put.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/asian_put.png` & `ipyparallel-8.7.0/docs/source/tutorial/figs/asian_put.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.pdf` & `ipyparallel-8.7.0/docs/source/tutorial/figs/mec_simple.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/mec_simple.png` & `ipyparallel-8.7.0/docs/source/tutorial/figs/mec_simple.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.pdf` & `ipyparallel-8.7.0/docs/source/tutorial/figs/parallel_pi.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/parallel_pi.png` & `ipyparallel-8.7.0/docs/source/tutorial/figs/parallel_pi.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.pdf` & `ipyparallel-8.7.0/docs/source/tutorial/figs/single_digits.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/single_digits.png` & `ipyparallel-8.7.0/docs/source/tutorial/figs/single_digits.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.pdf` & `ipyparallel-8.7.0/docs/source/tutorial/figs/two_digit_counts.pdf`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/two_digit_counts.png` & `ipyparallel-8.7.0/docs/source/tutorial/figs/two_digit_counts.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/docs/source/tutorial/figs/wideView.png` & `ipyparallel-8.7.0/docs/source/tutorial/figs/wideView.png`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/__init__.py` & `ipyparallel-8.7.0/ipyparallel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The IPython ZMQ-based parallel computing interface."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 # export return_when constants
 import os
 from concurrent.futures import ALL_COMPLETED  # noqa
 from concurrent.futures import FIRST_COMPLETED  # noqa
 from concurrent.futures import FIRST_EXCEPTION  # noqa
```

### Comparing `ipyparallel-8.6.1/ipyparallel/_async.py` & `ipyparallel-8.7.0/ipyparallel/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Async utilities"""
+
 import asyncio
 import concurrent.futures
 import inspect
 import threading
 from functools import partial
 
 from tornado.ioloop import IOLoop
```

### Comparing `ipyparallel-8.6.1/ipyparallel/_version.py` & `ipyparallel-8.7.0/ipyparallel/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-__version__ = "8.6.1"
+__version__ = "8.7.0"
 
 # matches tbump regex in pyproject.toml
 _version_regex = re.compile(
     r'''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `ipyparallel-8.6.1/ipyparallel/error.py` & `ipyparallel-8.7.0/ipyparallel/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Classes and functions for kernel related errors and exceptions.
 
 Inheritance diagram:
 
 .. inheritance-diagram:: ipyparallel.error
     :parts: 3
 """
+
 import builtins
 import sys
 import traceback
 
 __docformat__ = "restructuredtext en"
```

### Comparing `ipyparallel-8.6.1/ipyparallel/joblib.py` & `ipyparallel-8.7.0/ipyparallel/joblib.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 At this point, you can use it with::
 
     with parallel_backend('ipyparallel'):
         Parallel(n_jobs=2)(delayed(some_function)(i) for i in range(10))
 
 .. versionadded:: 5.1
 """
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 from joblib.parallel import register_parallel_backend
 
 from .client._joblib import IPythonParallelBackend
```

### Comparing `ipyparallel-8.6.1/ipyparallel/traitlets.py` & `ipyparallel-8.7.0/ipyparallel/traitlets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom ipyparallel trait types"""
+
 import entrypoints
 from traitlets import List, TraitError, Type
 
 
 class Launcher(Type):
     """Entry point-extended Type
```

### Comparing `ipyparallel-8.6.1/ipyparallel/util.py` & `ipyparallel-8.7.0/ipyparallel/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Some generic utilities for dealing with classes, urls, and serialization."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import asyncio
 import functools
 import inspect
 import logging
 import os
@@ -484,17 +485,17 @@
         return
     from distributed import Nanny, Worker
 
     if nanny:
         w = Nanny(address, **kwargs)
     else:
         w = Worker(address, **kwargs)
-    shell.user_ns['dask_worker'] = shell.user_ns[
-        'distributed_worker'
-    ] = kernel.distributed_worker = w
+    shell.user_ns['dask_worker'] = shell.user_ns['distributed_worker'] = (
+        kernel.distributed_worker
+    ) = w
     kernel.io_loop.add_callback(w.start)
 
 
 def stop_distributed_worker():
     """Task function for stopping the the distributed worker on an engine."""
     shell = get_ipython()
     kernel = shell.kernel
@@ -587,15 +588,15 @@
     elif a.tzinfo is not None and b.tzinfo is None:
         b = b.replace(tzinfo=tzlocal())
     return a - b
 
 
 def utcnow():
     """Timezone-aware UTC timestamp"""
-    return datetime.utcnow().replace(tzinfo=utc)
+    return datetime.now(utc)
 
 
 def _v(version_s):
     return tuple(int(s) for s in re.findall(r"\d+", version_s))
 
 
 def _patch_jupyter_client_dates():
```

### Comparing `ipyparallel-8.6.1/ipyparallel/apps/baseapp.py` & `ipyparallel-8.7.0/ipyparallel/apps/baseapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The Base Application class for ipyparallel apps
 """
+
 import logging
 import os
 import re
 import sys
 
 import traitlets
 from IPython.core.application import BaseIPythonApplication
```

### Comparing `ipyparallel-8.6.1/ipyparallel/apps/iploggerapp.py` & `ipyparallel-8.7.0/ipyparallel/apps/iploggerapp.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/apps/logwatcher.py` & `ipyparallel-8.7.0/ipyparallel/apps/logwatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A logger object that consolidates messages incoming from ipcluster processes.
 """
+
 import logging
 
 import zmq
 from jupyter_client.localinterfaces import localhost
 from tornado import ioloop
 from traitlets import Instance, List, Unicode
 from traitlets.config.configurable import LoggingConfigurable
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/_joblib.py` & `ipyparallel-8.7.0/ipyparallel/client/_joblib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """joblib parallel backend for IPython Parallel"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 from joblib.parallel import AutoBatchingMixin, ParallelBackendBase
 
 import ipyparallel as ipp
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/asyncresult.py` & `ipyparallel-8.7.0/ipyparallel/client/asyncresult.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """AsyncResult objects for the client"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import concurrent.futures
 import sys
 import threading
 import time
 import warnings
@@ -313,15 +314,14 @@
             If `timeout` is not ``None`` and the result does not arrive within
             `timeout` seconds then ``TimeoutError`` is raised. If the
             remote call raised an exception then that exception will be reraised
             by get() inside a `RemoteError`.
         return_exceptions : bool [default False]
             If True, return Exceptions instead of raising them.
         return_when : None, ALL_COMPLETED, or FIRST_EXCEPTION
-
             FIRST_COMPLETED is not supported, and treated the same as ALL_COMPLETED.
             See :py:func:`concurrent.futures.wait` for documentation.
 
             When return_when=FIRST_EXCEPTION, will raise immediately on the first exception,
             rather than waiting for all results to finish before reporting errors.
 
         .. versionchanged:: 8.0
@@ -624,15 +624,16 @@
         """result property as a dict."""
         return self.get_dict()
 
     def __dict__(self):
         return self.get_dict(0)
 
     def abort(self):
-        """Abort my tasks, if possible.
+        """
+        Abort my tasks, if possible.
 
         Only tasks that have not started yet can be aborted.
 
         Raises RuntimeError if already done.
         """
         if self.ready():
             raise RuntimeError("Can't abort, I am already done!")
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/client.py` & `ipyparallel-8.7.0/ipyparallel/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A semi-synchronous Client for IPython parallel"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import asyncio
 import json
 import os
 import re
 import socket
@@ -1346,15 +1347,14 @@
 
     # --------------------------------------------------------------------------
     # Begin public methods
     # --------------------------------------------------------------------------
 
     @property
     def ids(self):
-        """Always up-to-date ids property."""
         # always copy:
         return list(self._ids)
 
     def activate(self, targets='all', suffix=''):
         """Create a DirectView and register it with IPython magics
 
         Defines the magics `%px, %autopx, %pxresult, %%px`
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/futures.py` & `ipyparallel-8.7.0/ipyparallel/client/futures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Future-related utils"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import sys
 from concurrent.futures import Future
 from threading import Event
 
 from tornado.log import app_log
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/magics.py` & `ipyparallel-8.7.0/ipyparallel/client/magics.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 {RESULT_DOC}
 
 ``%pxconfig``
 
 {CONFIG_DOC}
 
 """
+
 import time
 from contextlib import contextmanager
 
 
 # Python 3.6 doesn't have nullcontext, so we define our own
 @contextmanager
 def nullcontext():
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/map.py` & `ipyparallel-8.7.0/ipyparallel/client/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Classes used in scattering and gathering sequences.
 
 Scattering consists of partitioning a sequence and sending the various
 pieces to individual nodes in a cluster.
 """
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import sys
 from itertools import chain, islice
 
 numpy = None
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/remotefunction.py` & `ipyparallel-8.7.0/ipyparallel/client/remotefunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Remote Functions and decorators for Views."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import sys
 import warnings
 from inspect import signature
 
 from decorator import decorator
```

### Comparing `ipyparallel-8.6.1/ipyparallel/client/view.py` & `ipyparallel-8.7.0/ipyparallel/client/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Views of remote engines."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import builtins
 import concurrent.futures
 import inspect
 import secrets
 import threading
```

### Comparing `ipyparallel-8.6.1/ipyparallel/cluster/_winhpcjob.py` & `ipyparallel-8.7.0/ipyparallel/cluster/_winhpcjob.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Job and task components for writing .xml files that the Windows HPC Server
 2008 can use to start jobs.
 """
+
 import os
 import re
 import uuid
 from xml.etree import ElementTree as ET
 
 from traitlets import Bool, Enum, Instance, Integer, List, Unicode
 from traitlets.config.configurable import Configurable
```

### Comparing `ipyparallel-8.6.1/ipyparallel/cluster/app.py` & `ipyparallel-8.7.0/ipyparallel/cluster/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -623,15 +623,21 @@
 
 
 class IPClusterNBExtension(BaseParallelApplication):
     """Enable/disable ipcluster tab extension in Jupyter notebook"""
 
     name = 'ipcluster-nbextension'
 
-    description = """Enable/disable IPython clusters tab in Jupyter notebook
+    description = """(DEPRECATED) Enable/disable IPython clusters tab in classic Jupyter notebook
+
+    Only for the deprecated jupyter-notebook < 7.0.
+
+    For current jupyter-server implementations (jupyterlab and jupyter-notebook 7):
+
+        jupyter server extension enable ipyparallel
 
     for Jupyter Notebook >= 4.2, you can use the new nbextension API:
 
     jupyter serverextension enable --py ipyparallel
     jupyter nbextension install --py ipyparallel
     jupyter nbextension enable --py ipyparallel
     """
@@ -650,24 +656,44 @@
                 {'IPClusterNBExtension': {'user': True}},
                 'Apply the operation only for the given user',
             )
         }
     )
 
     def start(self):
-        from ipyparallel.nbextension.install import install_extensions
-
         if len(self.extra_args) != 1:
             self.exit("Must specify 'enable' or 'disable'")
         action = self.extra_args[0].lower()
+
+        print(
+            "WARNING: `ipcluster nbextension` is deprecated. Use `jupyter server extension enable ipyparallel`",
+            file=sys.stderr,
+        )
+
+        from ipyparallel.util import _v
+
+        try:
+            import notebook
+        except ImportError:
+            self.exit(
+                "Deprecated `ipcluster nbextension` requires `notebook<7`, no `notebook` package found."
+            )
+
+        if _v(notebook.__version__) >= _v('7'):
+            self.exit(
+                "Deprecated `ipcluster nbextension` requires `notebook<7`, found `notebook=={notebook.__version__}`."
+            )
+
+        from ipyparallel.nbextension.install import install_extensions
+
         if action == 'enable':
-            print("Enabling IPython clusters tab")
+            print("Enabling IPython clusters tab", file=sys.stderr)
             install_extensions(enable=True, user=self.user)
         elif action == 'disable':
-            print("Disabling IPython clusters tab")
+            print("Disabling IPython clusters tab", file=sys.stderr)
             install_extensions(enable=False, user=self.user)
         else:
             self.exit("Must specify 'enable' or 'disable', not '%s'" % action)
 
 
 class IPCluster(BaseParallelApplication):
     name = 'ipcluster'
```

### Comparing `ipyparallel-8.6.1/ipyparallel/cluster/cluster.py` & `ipyparallel-8.7.0/ipyparallel/cluster/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Cluster class
 
 defines the basic interface to a single IPython Parallel cluster
 
 starts/stops/polls controllers, engines, etc.
 """
+
 import asyncio
 import atexit
 import glob
 import inspect
 import json
 import logging
 import os
@@ -266,14 +267,15 @@
         if self.parent and self.parent is IPython.get_ipython():
             # log to stdout in an IPython session
             log = logging.getLogger(f"{__name__}.{self.cluster_id}")
             log.setLevel(self.log_level)
 
             handler = logging.StreamHandler(sys.stdout)
             log.handlers = [handler]
+            log.propagate = False
             return log
         elif self.parent and getattr(self.parent, 'log', None) is not None:
             return self.parent.log
         elif Application.initialized():
             return Application.instance().log
         else:
             # set up our own logger
```

### Comparing `ipyparallel-8.6.1/ipyparallel/cluster/launcher.py` & `ipyparallel-8.7.0/ipyparallel/cluster/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Facilities for launching IPython Parallel processes asynchronously."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import asyncio
 import copy
 import inspect
 import json
 import logging
@@ -323,16 +324,20 @@
         # override in subclasses to retrieve output
         return ""
 
     def _log_output(self, stop_data=None):
         output = self.get_output(remove=True)
         if self.output_limit:
             output = "".join(output.splitlines(True)[-self.output_limit :])
+
+        log = self.log.debug
+        if stop_data and stop_data.get("exit_code", 0) != 0:
+            log = self.log.warning
         if output:
-            self.log.debug(f"Output for {self.identifier}:\n{output}")
+            log("Output for %s:\n%s", self.identifier, output)
 
 
 class ControllerLauncher(BaseLauncher):
     """Base class for launching ipcontroller"""
 
     name = Unicode("ipcontroller")
 
@@ -344,19 +349,34 @@
     # Command line arguments to ipcontroller.
     controller_args = List(
         Unicode(),
         config=True,
         help="""command-line args to pass to ipcontroller""",
     )
 
-    async def get_connection_info(self, timeout=60):
+    connection_info_timeout = Float(
+        60,
+        config=True,
+        help="""
+        Default timeout (in seconds) for get_connection_info
+        
+        .. versionadded:: 8.7
+        """,
+    )
+
+    async def get_connection_info(self, timeout=None):
         """Retrieve connection info for the controller
 
         Default implementation assumes profile_dir and cluster_id are local.
+
+        .. versionchanged:: 8.7
+            Accept `timeout=None` (default) to use `.connection_info_timeout` config.
         """
+        if timeout is None:
+            timeout = self.connection_info_timeout
         connection_files = self.connection_files
         paths = list(connection_files.values())
         start_time = time.monotonic()
         if timeout >= 0:
             deadline = start_time + timeout
         else:
             deadline = None
@@ -790,14 +810,19 @@
                     if engine['exit_code']:
                         # save the first nonzero exit code
                         self.stop_data['exit_code'] = engine['exit_code']
                         break
 
             self.notify_stop(self.stop_data)
 
+    def _log_output(self, stop_data=None):
+        # avoid double-logging output, already logged by each engine
+        # that will be a lot if all 100 engines fail!
+        pass
+
     def get_output(self, remove=False):
         """Get the output of all my child Launchers"""
         for identifier, launcher in self.launchers.items():
             # remaining launchers
             self.outputs[identifier] = launcher.get_output(remove=remove)
 
         joined_output = []
@@ -862,17 +887,21 @@
     def start(self, n=1):
         """Start n instances of the program using mpiexec."""
         self.n = n
         return super().start()
 
     def _log_output(self, stop_data):
         """Try to log mpiexec error output, if any, at warning level"""
-        super()._log_output()
-        if self.log.getEffectiveLevel() <= logging.DEBUG:
+        super()._log_output(stop_data)
+
+        if stop_data and self.stop_data.get("exit_code", 0) != 0:
+            # if this is True, super()._log_output would have already logged the full output
+            # no need to extract from MPI
             return
+
         output = self.get_output(remove=False)
         mpiexec_lines = []
 
         in_mpi = False
         after_mpi = False
         mpi_tail = 0
         for line in output.splitlines(True):
@@ -1584,17 +1613,14 @@
         submit_command. """,
     )
     job_file_name = Unicode(
         'ipython_job.xml',
         config=True,
         help="The filename of the instantiated job script.",
     )
-    # The full path to the instantiated job script. This gets made dynamically
-    # by combining the work_dir with the job_file_name.
-    job_file = Unicode('')
     scheduler = Unicode(
         '', config=True, help="The hostname of the scheduler to submit the job to."
     )
     job_cmd = Unicode(config=True, help="The command for submitting jobs.")
 
     @default("job_cmd")
     def _default_job(self):
```

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/app.py` & `ipyparallel-8.7.0/ipyparallel/controller/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -919,17 +919,17 @@
             parent=self,
         )
 
         if self.write_connection_files:
             # save to new json config files
             base = {
                 'key': self.session.key.decode('ascii'),
-                'curve_serverkey': self.curve_publickey.decode("ascii")
-                if self.enable_curve
-                else None,
+                'curve_serverkey': (
+                    self.curve_publickey.decode("ascii") if self.enable_curve else None
+                ),
                 'location': self.location,
                 'pack': self.session.packer,
                 'unpack': self.session.unpacker,
                 'signature_scheme': self.session.signature_scheme,
             }
 
             cdict = {'ssh': self.ssh_server}
@@ -978,17 +978,17 @@
         return {
             'scheduler_class': scheduler_class,
             'in_addr': in_addr or self.client_url(scheduler_name),
             'out_addr': out_addr or self.engine_url(scheduler_name),
             'mon_addr': monitor_url,
             'not_addr': disambiguate_url(self.client_url('notification')),
             'reg_addr': disambiguate_url(self.client_url('registration')),
-            'identity': identity
-            if identity is not None
-            else bytes(scheduler_name, 'utf8'),
+            'identity': (
+                identity if identity is not None else bytes(scheduler_name, 'utf8')
+            ),
             'logname': logname,
             'loglevel': self.log_level,
             'log_url': self.log_url,
             'config': dict(self.config),
             'curve_secretkey': self.curve_secretkey if self.enable_curve else None,
             'curve_publickey': self.curve_publickey if self.enable_curve else None,
         }
```

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/broadcast_scheduler.py` & `ipyparallel-8.7.0/ipyparallel/controller/broadcast_scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/dependency.py` & `ipyparallel-8.7.0/ipyparallel/controller/dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Dependency utilities
 """
+
 from types import ModuleType
 
 from ipyparallel.client.asyncresult import AsyncResult
 from ipyparallel.error import UnmetDependency
 from ipyparallel.serialize import can
 from ipyparallel.util import interactive
```

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/dictdb.py` & `ipyparallel-8.7.0/ipyparallel/controller/dictdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 * client's outstanding: client_uuid = uuid && completed is None
 * MIA: arrived is None (and completed is None)
 
 DictDB supports a subset of mongodb operators::
 
     $lt,$gt,$lte,$gte,$ne,$in,$nin,$all,$mod,$exists
 """
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import copy
 from copy import deepcopy
 from datetime import datetime
 
 from traitlets import Dict, Float, Integer, Unicode
```

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/heartmonitor.py` & `ipyparallel-8.7.0/ipyparallel/controller/heartmonitor.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/hub.py` & `ipyparallel-8.7.0/ipyparallel/controller/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The IPython Controller Hub with 0MQ
 
 This is the master object that handles connections from engines and clients,
 and monitors traffic through the various queues.
 """
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import inspect
 import json
 import os
 import sys
 import time
```

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/mongodb.py` & `ipyparallel-8.7.0/ipyparallel/controller/mongodb.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/scheduler.py` & `ipyparallel-8.7.0/ipyparallel/controller/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The Python scheduler for rich scheduling.
 
 The Pure ZMQ scheduler does not allow routing schemes other than LRU,
 nor does it check msg_id DAG dependencies. For those, a slightly slower
 Python Scheduler exists.
 """
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import logging
 
 import jupyter_client.session
 import traitlets.log
 import zmq
```

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/sqlitedb.py` & `ipyparallel-8.7.0/ipyparallel/controller/sqlitedb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A TaskRecord backend using sqlite3"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import json
 import os
 
 try:
     import cPickle as pickle
```

### Comparing `ipyparallel-8.6.1/ipyparallel/controller/task_scheduler.py` & `ipyparallel-8.7.0/ipyparallel/controller/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/engine/app.py` & `ipyparallel-8.7.0/ipyparallel/engine/app.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/engine/datapub.py` & `ipyparallel-8.7.0/ipyparallel/engine/datapub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Publishing native (typically pickled) objects."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 from ipykernel.jsonutil import json_clean
 from jupyter_client.session import Session, extract_header
 from traitlets import Any, CBytes, Dict, Instance
 from traitlets.config import Configurable
```

### Comparing `ipyparallel-8.6.1/ipyparallel/engine/kernel.py` & `ipyparallel-8.7.0/ipyparallel/engine/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """IPython kernel for parallel computing"""
+
 import asyncio
 import inspect
 import sys
 from functools import partial
 
 import ipykernel
 from ipykernel.ipkernel import IPythonKernel
```

### Comparing `ipyparallel-8.6.1/ipyparallel/engine/log.py` & `ipyparallel-8.7.0/ipyparallel/engine/log.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/engine/nanny.py` & `ipyparallel-8.7.0/ipyparallel/engine/nanny.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 This has overlapping functionality with the Cluster API,
 but has key differences, justifying both existing:
 
 - addressing single engines is not feasible with the Cluster API,
   only engine *sets*
 - Cluster API can efficiently signal all engines via mpiexec
 """
+
 import asyncio
 import logging
 import os
 import pickle
 import signal
 import sys
 from subprocess import PIPE, Popen
```

### Comparing `ipyparallel-8.6.1/ipyparallel/labextension/package.json` & `ipyparallel-8.7.0/ipyparallel/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9425422705314008%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.6', '@jupyterlab/apputils': '^4.1.6', "*

 * *                   "'@jupyterlab/codeeditor': '^4.0.6', '@jupyterlab/console': '^4.0.6', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.6', '@jupyterlab/nbformat': '^4.0.6', "*

 * *                   "'@jupyterlab/notebook': '^4.0.6', '@jupyterlab/services': '^7.0.6', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.6', '@jupyterlab/statedb': '^4.0.6', "*

 * *                   "'@jupyterlab/ui-components': ' […]*

```diff
@@ -1,63 +1,62 @@
 {
     "author": "Min Ragan-Kelley",
     "bugs": {
         "url": "https://github.com/ipython/ipyparallel/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codeeditor": "^3.0.0",
-        "@jupyterlab/console": "^3.0.0",
-        "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.6.3",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.6.3",
-        "@jupyterlab/statedb": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/domutils": "^1.2.3",
-        "@lumino/dragdrop": "^1.7.1",
-        "@lumino/messaging": "^1.4.3",
-        "@lumino/polling": "^1.0.4",
-        "@lumino/signaling": "^1.4.3",
-        "@lumino/widgets": "^1.17.0",
-        "react": "~17.0.0",
-        "react-dom": "~17.0.0"
+        "@jupyterlab/application": "^4.0.6",
+        "@jupyterlab/apputils": "^4.1.6",
+        "@jupyterlab/codeeditor": "^4.0.6",
+        "@jupyterlab/console": "^4.0.6",
+        "@jupyterlab/coreutils": "^6.0.6",
+        "@jupyterlab/nbformat": "^4.0.6",
+        "@jupyterlab/notebook": "^4.0.6",
+        "@jupyterlab/services": "^7.0.6",
+        "@jupyterlab/settingregistry": "^4.0.6",
+        "@jupyterlab/statedb": "^4.0.6",
+        "@jupyterlab/ui-components": "^4.0.6",
+        "@lumino/algorithm": "^2.0.1",
+        "@lumino/commands": "^2.1.3",
+        "@lumino/coreutils": "^2.1.2",
+        "@lumino/domutils": "^2.0.1",
+        "@lumino/dragdrop": "^2.1.3",
+        "@lumino/messaging": "^2.0.1",
+        "@lumino/polling": "^2.1.2",
+        "@lumino/signaling": "^2.1.2",
+        "@lumino/widgets": "^2.3.0",
+        "react": "~18.2.0",
+        "react-dom": "~18.2.0"
     },
     "description": "A JupyterLab extension for IPython Parallel.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.10",
-        "@types/react": "~17.0.0",
-        "@types/react-dom": "~17.0.0",
-        "@typescript-eslint/eslint-plugin": "^5.18.0",
-        "@typescript-eslint/parser": "^5.18.0",
-        "eslint": "^8.37.0",
-        "eslint-config-prettier": "^8.5.0",
-        "eslint-plugin-prettier": "^4.0.0",
-        "eslint-plugin-react": "^7.21.5",
+        "@jupyterlab/builder": "^4.0.6",
+        "@types/react": "~18.2.24",
+        "@types/react-dom": "~18.2.8",
+        "@typescript-eslint/eslint-plugin": "^6.7.3",
+        "@typescript-eslint/parser": "^6.7.3",
+        "eslint": "^8.50.0",
+        "eslint-config-prettier": "^9.0.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "eslint-plugin-react": "^7.33.2",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.3.5",
-        "yarn": "^1.22.0"
+        "prettier": "^3.0.3",
+        "rimraf": "^5.0.5",
+        "typescript": "~5.2.2"
     },
     "files": [
         "lab/lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "lab/schema/*.json",
         "lab/style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ipython/ipyparallel",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f5bc00ef0248261af0b1.js"
+            "load": "static/remoteEntry.ccf2bfedaae5f1da1a90.js"
         },
         "extension": true,
         "outputDir": "ipyparallel/labextension",
         "schemaDir": "lab/schema",
         "webpackConfig": "lab/webpack.config.js"
     },
     "keywords": [
@@ -95,9 +94,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.6.1"
+    "version": "8.7.0"
 }
```

### Comparing `ipyparallel-8.6.1/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig` & `ipyparallel-8.7.0/ipyparallel/labextension/schemas/ipyparallel-labextension/package.json.orig`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9432367149758455%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.6', '@jupyterlab/apputils': '^4.1.6', "*

 * *                   "'@jupyterlab/codeeditor': '^4.0.6', '@jupyterlab/console': '^4.0.6', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.6', '@jupyterlab/nbformat': '^4.0.6', "*

 * *                   "'@jupyterlab/notebook': '^4.0.6', '@jupyterlab/services': '^7.0.6', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.6', '@jupyterlab/statedb': '^4.0.6', "*

 * *                   "'@jupyterlab/ui-components': ' […]*

```diff
@@ -1,52 +1,51 @@
 {
     "author": "Min Ragan-Kelley",
     "bugs": {
         "url": "https://github.com/ipython/ipyparallel/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codeeditor": "^3.0.0",
-        "@jupyterlab/console": "^3.0.0",
-        "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.6.3",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.6.3",
-        "@jupyterlab/statedb": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/domutils": "^1.2.3",
-        "@lumino/dragdrop": "^1.7.1",
-        "@lumino/messaging": "^1.4.3",
-        "@lumino/polling": "^1.0.4",
-        "@lumino/signaling": "^1.4.3",
-        "@lumino/widgets": "^1.17.0",
-        "react": "~17.0.0",
-        "react-dom": "~17.0.0"
+        "@jupyterlab/application": "^4.0.6",
+        "@jupyterlab/apputils": "^4.1.6",
+        "@jupyterlab/codeeditor": "^4.0.6",
+        "@jupyterlab/console": "^4.0.6",
+        "@jupyterlab/coreutils": "^6.0.6",
+        "@jupyterlab/nbformat": "^4.0.6",
+        "@jupyterlab/notebook": "^4.0.6",
+        "@jupyterlab/services": "^7.0.6",
+        "@jupyterlab/settingregistry": "^4.0.6",
+        "@jupyterlab/statedb": "^4.0.6",
+        "@jupyterlab/ui-components": "^4.0.6",
+        "@lumino/algorithm": "^2.0.1",
+        "@lumino/commands": "^2.1.3",
+        "@lumino/coreutils": "^2.1.2",
+        "@lumino/domutils": "^2.0.1",
+        "@lumino/dragdrop": "^2.1.3",
+        "@lumino/messaging": "^2.0.1",
+        "@lumino/polling": "^2.1.2",
+        "@lumino/signaling": "^2.1.2",
+        "@lumino/widgets": "^2.3.0",
+        "react": "~18.2.0",
+        "react-dom": "~18.2.0"
     },
     "description": "A JupyterLab extension for IPython Parallel.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.10",
-        "@types/react": "~17.0.0",
-        "@types/react-dom": "~17.0.0",
-        "@typescript-eslint/eslint-plugin": "^5.18.0",
-        "@typescript-eslint/parser": "^5.18.0",
-        "eslint": "^8.37.0",
-        "eslint-config-prettier": "^8.5.0",
-        "eslint-plugin-prettier": "^4.0.0",
-        "eslint-plugin-react": "^7.21.5",
+        "@jupyterlab/builder": "^4.0.6",
+        "@types/react": "~18.2.24",
+        "@types/react-dom": "~18.2.8",
+        "@typescript-eslint/eslint-plugin": "^6.7.3",
+        "@typescript-eslint/parser": "^6.7.3",
+        "eslint": "^8.50.0",
+        "eslint-config-prettier": "^9.0.0",
+        "eslint-plugin-prettier": "^5.0.0",
+        "eslint-plugin-react": "^7.33.2",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.3.5",
-        "yarn": "^1.22.0"
+        "prettier": "^3.0.3",
+        "rimraf": "^5.0.5",
+        "typescript": "~5.2.2"
     },
     "files": [
         "lab/lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "lab/schema/*.json",
         "lab/style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ipython/ipyparallel",
@@ -91,9 +90,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lab/lib/index.d.ts",
-    "version": "8.6.1"
+    "version": "8.7.0"
 }
```

### Comparing `ipyparallel-8.6.1/ipyparallel/labextension/static/592.2265e4df71d8ba0dbbf6.js` & `ipyparallel-8.7.0/ipyparallel/labextension/static/998.d38d80ac3e2fa7501089.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
+"use strict";
 (self.webpackChunkipyparallel_labextension = self.webpackChunkipyparallel_labextension || []).push([
-    [592], {
-        592: (e, t, n) => {
-            "use strict";
+    [998], {
+        998: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => B
+                default: () => H
             });
-            var s = n(142),
-                i = n(687),
-                r = n(282),
-                a = n(38),
-                o = n(933),
-                l = n(123),
-                c = n(502),
-                u = n(840),
-                d = n(832),
-                p = n(33),
-                h = n(820),
-                g = n(918),
-                m = n(526),
-                C = n(520),
-                v = n(694),
-                f = n(358),
-                y = n(271);
+            var s = n(351),
+                i = n(750),
+                r = n(824),
+                a = n(991),
+                o = n(943),
+                l = n(445),
+                c = n(448),
+                u = n(901),
+                d = n(882),
+                p = n(403),
+                h = n(810),
+                g = n(697),
+                m = n(930),
+                C = n(593),
+                v = n(359),
+                f = n(797),
+                y = n(29);
             class w extends y.Component {
                 constructor(e) {
                     let t;
                     super(e), t = e.initialModel, this.state = {
                         model: t
                     }
                 }
@@ -99,20 +99,20 @@
                         placeholder: "auto",
                         onChange: e => {
                             this.onScaleChanged(e)
                         }
                     }))))
                 }
             }
-            var b, _ = n(456);
+            var b, _ = n(745);
             ! function(e) {
                 e.injectClientCode = "ipyparallel:inject-client-code", e.newCluster = "ipyparallel:new-cluster", e.startCluster = "ipyparallel:start-cluster", e.stopCluster = "ipyparallel:stop-cluster", e.scaleCluster = "ipyparallel:scale-cluster", e.toggleAutoStartClient = "ipyparallel:toggle-auto-start-client"
             }(b || (b = {}));
             const I = "ipyparallel/clusters";
-            class E extends d.Widget {
+            class L extends d.Widget {
                 constructor(e) {
                     super(), this._dragData = null, this._clusters = [], this._activeClusterChanged = new u.Signal(this), this._serverErrorShown = !1, this._isReady = !0, this.addClass("ipp-ClusterManager"), this._serverSettings = h.ServerConnection.makeSettings(), this._injectClientCodeForCluster = e.injectClientCodeForCluster, this._getClientCodeForCluster = e.getClientCodeForCluster, this._registry = e.registry, this._setActiveById = e => {
                         const t = this._clusters.find((t => t.id === e));
                         if (!t) return;
                         const n = this._activeCluster;
                         n && n.id === t.id || (this._activeCluster = t, this._activeClusterChanged.emit({
                             name: "cluster",
@@ -194,23 +194,23 @@
                     if (!this._clusters.find((t => t.id === e))) throw Error(`Cannot find cluster ${e}`);
                     return await this._scaleById(e)
                 }
                 dispose() {
                     this.isDisposed || (this._poll.dispose(), super.dispose())
                 }
                 onUpdateRequest(e) {
-                    this.isVisible && _.render(y.createElement(L, {
+                    this.isVisible && (0, _.s)(this._clusterListing.node).render(y.createElement(x, {
                         clusters: this._clusters,
                         activeClusterId: this._activeCluster && this._activeCluster.id || "",
                         scaleById: e => this._scaleById(e),
                         startById: e => this._startById(e),
                         stopById: e => this._stopById(e),
                         setActiveById: this._setActiveById,
                         injectClientCodeForCluster: this._injectClientCodeForCluster
-                    }), this._clusterListing.node)
+                    }))
                 }
                 onAfterShow(e) {
                     this.update()
                 }
                 onAfterAttach(e) {
                     super.onAfterAttach(e);
                     let t = this._clusterListing.node;
@@ -344,31 +344,31 @@
                 }
                 _findCluster(e) {
                     const t = Array.from(this.node.querySelectorAll("li.ipp-ClusterListingItem"));
                     return g.ArrayExt.findFirstIndex(t, (t => C.ElementExt.hitTest(t, e.clientX, e.clientY)))
                 }
             }
 
-            function L(e) {
-                let t = e.clusters.map((t => y.createElement(x, {
+            function x(e) {
+                let t = e.clusters.map((t => y.createElement(E, {
                     isActive: t.id === e.activeClusterId,
                     key: t.id,
                     cluster: t,
                     scale: () => e.scaleById(t.id),
                     start: () => e.startById(t.id),
                     stop: () => e.stopById(t.id),
                     setActive: () => e.setActiveById(t.id),
                     injectClientCode: () => e.injectClientCodeForCluster(t)
                 })));
                 return y.createElement("div", null, y.createElement("ul", {
                     className: "ipp-ClusterListing-list"
                 }, t))
             }
 
-            function x(e) {
+            function E(e) {
                 const {
                     cluster: t,
                     isActive: n,
                     setActive: s,
                     scale: i,
                     start: r,
                     stop: a,
@@ -422,116 +422,123 @@
             }(S || (S = {}));
             class j extends d.Widget {
                 constructor(e) {
                     super(), this.addClass("ipp-Sidebar");
                     let t = this.layout = new d.PanelLayout;
                     const n = e.clientCodeInjector,
                         s = e.clientCodeGetter;
-                    this._clusters = new E({
+                    this._clusters = new L({
                         registry: e.registry,
                         injectClientCodeForCluster: n,
                         getClientCodeForCluster: s
                     }), t.addWidget(this._clusters)
                 }
                 get clusterManager() {
                     return this._clusters
                 }
             }
             var k = n(379),
                 M = n.n(k),
-                D = n(861);
-            M()(D.Z, {
-                insert: "head",
-                singleton: !1
-            }), D.Z.locals;
-            const N = "ipyparallel-labextension:plugin",
-                A = "IPython Parallel",
-                B = {
+                D = n(795),
+                A = n.n(D),
+                N = n(569),
+                P = n.n(N),
+                B = n(565),
+                R = n.n(B),
+                T = n(216),
+                $ = n.n(T),
+                F = n(589),
+                W = n.n(F),
+                U = n(861),
+                z = {};
+            z.styleTagTransform = W(), z.setAttributes = R(), z.insert = P().bind(null, "head"), z.domAPI = A(), z.insertStyleElement = $(), M()(U.Z, z), U.Z && U.Z.locals && U.Z.locals;
+            const q = "ipyparallel-labextension:plugin",
+                O = "IPython Parallel",
+                H = {
                     activate: async function(e, t, n, i, r, a) {
                         const o = "ipp-cluster-launcher",
                             l = !!a,
                             d = "tree" == s.PageConfig.getOption("retroPage"),
-                            p = s => {
-                                const i = P.getCurrentEditor(e, n, t);
-                                i && P.injectClientCode(s, i)
-                            },
-                            h = new j({
+                            p = async s => {
+                                const i = await V.getCurrentEditor(e, n, t);
+                                i && V.injectClientCode(s, i)
+                            }, h = new j({
                                 clientCodeInjector: p,
-                                clientCodeGetter: P.getClientCode,
+                                clientCodeGetter: V.getClientCode,
                                 registry: e.commands
                             });
                         if (h.id = o, h.title.icon = new c.LabIcon({
                                 name: "ipyparallel:logo",
                                 svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   xmlns="http://www.w3.org/2000/svg"\n   version="1.1"\n   viewBox="0 0 20 20"\n   height="20"\n   width="20">\n   \x3c!-- text: IP in Source Code Pro --\x3e\n    <g\n       aria-label="IP">\n      <path\n         class="jp-icon3 jp-icon-selectable"\n         fill="#616161"\n         d="m 1.619125,15.248 v -1.136 h 2.608 V 5.8720001 h -2.608 v -1.12 h 6.56 v 1.12 h -2.608 V 14.112 h 2.608 v 1.136 z" />\n      <path\n         class="jp-icon3 jp-icon-selectable"\n         fill="#616161"\n         d="M 11.324875,15.248 V 4.7520001 h 3.168 q 1.168,0 2.032,0.288 0.88,0.288 1.36,0.976 0.496,0.672 0.496,1.824 0,1.104 -0.496,1.824 -0.48,0.7199999 -1.36,1.0719999 -0.88,0.352 -2.032,0.352 h -1.84 v 4.16 z m 1.328,-5.248 h 1.68 q 1.376,0 2.032,-0.5119999 0.672,-0.528 0.672,-1.648 0,-1.136 -0.672,-1.568 -0.672,-0.448 -2.032,-0.448 h -1.68 z" />\n  </g>\n</svg>\n'
                             }), l) a.add(h, "left", {
                             rank: 200
-                        }), h.title.caption = A;
+                        }), h.title.caption = O;
                         else if (d) {
                             const t = e.shell.currentWidget;
-                            t.addWidget(h), t.tabBar.addTab(h.title), h.title.label = A
+                            t.addWidget(h), t.tabBar.addTab(h.title), h.title.label = O
                         }
                         h.clusterManager.activeClusterChanged.connect((async () => {
                             const e = h.clusterManager.activeCluster;
                             return r.save(o, {
                                 cluster: e ? e.id : ""
                             })
                         }));
                         const g = async e => {
                             if (!e) return;
                             const t = h.clusterManager.activeCluster;
-                            return t && await P.shouldUseKernel(e.kernel) ? P.createClientForKernel(t, e.kernel) : void 0
+                            return t && await V.shouldUseKernel(e.kernel) ? V.createClientForKernel(t, e.kernel) : void 0
                         }, m = [n, t], C = async e => {
                             if (e.session && e.session.kernel && "restarting" === e.session.kernel.status) return g(e.session)
                         }, v = (e, t) => {
                             t.sessionContext.statusChanged.connect(C)
                         }, f = () => {
                             m.forEach((e => {
                                 e.forEach((async e => {
                                     const t = e.sessionContext.session;
-                                    if (t && await P.shouldUseKernel(t.kernel)) return g(t)
+                                    if (t && await V.shouldUseKernel(t.kernel)) return g(t)
                                 }))
                             }))
                         };
-                        Promise.all([i.load(N), r.fetch(o)]).then((async e => {
+                        Promise.all([i.load(q), r.fetch(o)]).then((async e => {
                             const t = e[0];
                             if (!t) return void console.warn("Unable to retrieve ipp-labextension settings");
                             const n = e[1],
                                 s = n ? n.cluster : "",
                                 i = () => {
                                     u.Signal.clearData(v), u.Signal.clearData(C), u.Signal.clearData(f)
                                 };
                             i(), t.changed.connect(i), s && (await h.clusterManager.refresh(), h.clusterManager.setActiveCluster(s))
                         })), e.commands.addCommand(b.injectClientCode, {
                             label: "Inject IPython Client Connection Code",
-                            execute: () => {
-                                const t = P.clusterFromClick(e, h.clusterManager);
-                                t && p(t)
+                            execute: async () => {
+                                const t = V.clusterFromClick(e, h.clusterManager);
+                                if (t) return await p(t)
                             }
                         }), e.commands.addCommand(b.newCluster, {
                             label: e => e.isPalette ? "Create New Cluster" : "NEW",
                             execute: () => h.clusterManager.create(),
                             iconClass: e => e.isPalette ? "" : "jp-AddIcon jp-Icon jp-Icon-16",
                             isEnabled: () => h.clusterManager.isReady,
                             caption: () => h.clusterManager.isReady ? "Start New Cluster" : "Cluster starting..."
                         }), e.commands.addCommand(b.startCluster, {
                             label: "Start Cluster",
                             execute: () => {
-                                const t = P.clusterFromClick(e, h.clusterManager);
+                                const t = V.clusterFromClick(e, h.clusterManager);
                                 if (t) return h.clusterManager.start(t.id)
                             }
                         }), e.commands.addCommand(b.stopCluster, {
                             label: "Shutdown Cluster",
                             execute: () => {
-                                const t = P.clusterFromClick(e, h.clusterManager);
+                                const t = V.clusterFromClick(e, h.clusterManager);
                                 if (t) return h.clusterManager.stop(t.id)
                             }
                         }), e.commands.addCommand(b.scaleCluster, {
                             label: "Scale Cluster…",
                             execute: () => {
-                                const t = P.clusterFromClick(e, h.clusterManager);
+                                const t = V.clusterFromClick(e, h.clusterManager);
                                 if (t) return h.clusterManager.scale(t.id)
                             }
                         }), e.contextMenu.addItem({
                             command: b.injectClientCode,
                             selector: ".ipp-ClusterListingItem",
                             rank: 10
                         }), e.contextMenu.addItem({
@@ -544,20 +551,20 @@
                             rank: 2
                         }), e.contextMenu.addItem({
                             command: b.startCluster,
                             selector: ".ipp-ClusterListing-list",
                             rank: 1
                         })
                     },
-                    id: N,
+                    id: q,
                     requires: [r.IConsoleTracker, l.INotebookTracker, a.ISettingRegistry, o.IStateDB],
                     optional: [i.ILabShell],
                     autoStart: !0
                 };
-            var P;
+            var V;
             ! function(e) {
                 function t(e) {
                     return `import ipyparallel as ipp\n\ncluster = ipp.Cluster.from_file("${e.cluster_file}")\nrc = cluster.connect_client_sync()\nrc`
                 }
                 e.id = 0, e.shouldUseKernel = async function(e) {
                     if (!e) return !1;
                     const t = await e.spec;
@@ -572,229 +579,238 @@
                             "display_data" === t.header.msg_type && e(void 0)
                         }
                     }))
                 }, e.injectClientCode = function(e, n) {
                     const s = n.getCursorPosition(),
                         i = n.getOffsetAt(s),
                         r = t(e);
-                    n.model.value.insert(i, r)
+                    n.model.sharedModel.updateSource(i, i, r)
                 }, e.getClientCode = t, e.getCurrentKernel = function(e, t, n) {
                     var s, i, r, a;
                     let o, l = e.currentWidget;
                     return l && t.has(l) ? o = null === (s = l.sessionContext.session) || void 0 === s ? void 0 : s.kernel : l && n.has(l) ? o = null === (i = l.sessionContext.session) || void 0 === i ? void 0 : i.kernel : t.currentWidget ? o = null === (r = t.currentWidget.sessionContext.session) || void 0 === r ? void 0 : r.kernel : n.currentWidget && (o = null === (a = n.currentWidget.sessionContext.session) || void 0 === a ? void 0 : a.kernel), o
-                }, e.getCurrentEditor = function(e, t, n) {
+                }, e.getCurrentEditor = async function(e, t, n) {
                     let s, i = e.shell.currentWidget;
                     if (i && t.has(i)) {
                         l.NotebookActions.insertAbove(i.content);
                         const e = i.content.activeCell;
-                        s = e && e.editor
+                        await e.ready, s = e && e.editor
                     } else if (i && n.has(i)) {
                         const e = i.console.promptCell;
-                        s = e && e.editor
+                        await e.ready, s = e && e.editor
                     } else if (t.currentWidget) {
                         const e = t.currentWidget;
                         l.NotebookActions.insertAbove(e.content);
                         const n = e.content.activeCell;
-                        s = n && n.editor
+                        await n.ready, s = n && n.editor
                     } else if (n.currentWidget) {
                         const e = n.currentWidget.console.promptCell;
-                        s = e && e.editor
+                        await e.ready, s = e && e.editor
                     }
                     return s
                 }, e.clusterFromClick = function(e, t) {
                     const n = e.contextMenuHitTest((e => !!e.dataset.clusterId));
                     if (!n) return;
                     const s = n.dataset.clusterId;
                     return t.clusters.find((e => e.id === s))
                 }
-            }(P || (P = {}))
+            }(V || (V = {}))
         },
         861: (e, t, n) => {
-            "use strict";
             n.d(t, {
                 Z: () => g
             });
-            var s = n(645),
+            var s = n(81),
                 i = n.n(s),
-                r = n(667),
+                r = n(645),
                 a = n.n(r),
-                o = n(825),
+                o = n(667),
                 l = n.n(o),
-                c = n(618),
-                u = n.n(c),
-                d = i()((function(e) {
-                    return e[1]
-                })),
-                p = a()(l()),
-                h = a()(u());
-            d.push([e.id, ':root {\n  --ipp-launch-button-height: 24px;\n}\n\n/**\n * Rules related to the overall sidebar panel.\n */\n\n.ipp-Sidebar {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size1);\n  overflow: auto;\n}\n\n/**\n * Rules related to the cluster manager.\n */\n\n.ipp-ClusterManager .jp-Toolbar {\n  align-items: center;\n}\n\n.ipp-ClusterManager .jp-Toolbar .ipp-ClusterManager-label {\n  flex: 0 0 auto;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n  font-size: var(--jp-ui-font-size0);\n  padding: 8px 8px 8px 12px;\n  margin: 0px;\n}\n\n.ipp-ClusterManager button.jp-Button > span {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n}\n\n.ipp-ClusterListing ul.ipp-ClusterListing-list {\n  list-style-type: none;\n  padding: 0;\n  margin: 0;\n}\n\n.ipp-ClusterListingItem {\n  display: inline-block;\n  list-style-type: none;\n  padding: 8px;\n  width: 100%;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  cursor: grab;\n}\n\n.ipp-ClusterListingItem-drag {\n  opacity: 0.7;\n  color: var(--jp-ui-font-color1);\n  cursor: grabbing;\n  max-width: 260px;\n  transform: translateX(-50%) translateY(-50%);\n}\n\n.ipp-ClusterListingItem-title {\n  margin: 0px;\n  font-size: var(--jp-ui-font-size2);\n}\n\n.ipp-ClusterListingItem-link a {\n  text-decoration: none;\n  color: var(--jp-content-link-color);\n}\n\n.ipp-ClusterListingItem-link a:hover {\n  text-decoration: underline;\n}\n\n.ipp-ClusterListingItem-link a:visited {\n  color: var(--jp-content-link-color);\n}\n\n.ipp-ClusterListingItem:hover {\n  background: var(--jp-layout-color2);\n}\n\n.ipp-ClusterListingItem.jp-mod-active {\n  color: white;\n  background: var(--jp-brand-color0);\n}\n\n.ipp-ClusterListingItem.jp-mod-active a,\n.ipp-ClusterListingItem.jp-mod-active a:visited {\n  color: white;\n}\n\n.ipp-ClusterListingItem button.jp-mod-styled {\n  background-color: transparent;\n}\n\n.ipp-ClusterListingItem button.jp-mod-styled:hover {\n  background-color: var(--jp-layout-color3);\n}\n\n.ipp-ClusterListingItem.jp-mod-active button.jp-mod-styled:hover {\n  background-color: var(--jp-brand-color1);\n}\n\n.ipp-ClusterListingItem-button-panel {\n  display: flex;\n  align-content: center;\n}\n\nbutton.ipp-ClusterListingItem-stop {\n  color: var(--jp-warn-color1);\n  font-weight: 600;\n}\n\nbutton.ipp-ClusterListingItem-scale {\n  color: var(--jp-accent-color1);\n  font-weight: 600;\n}\n\nbutton.ipp-ClusterListingItem-start {\n  color: var(--jp-accent-color1);\n  font-weight: 600;\n}\n\nbutton.ipp-hidden {\n  display: none;\n}\n\n.ipp-ClusterListingItem button.ipp-ClusterListingItem-code.jp-mod-styled {\n  margin: 0 4px 0 4px;\n  background-repeat: no-repeat;\n  background-position: center;\n}\n\n/**\n * Rules for the scaling dialog.\n */\n\n.ipp-DialogHeader {\n  font-size: var(--jp-ui-font-size2);\n}\n\n.ipp-DialogSection {\n  margin-left: 24px;\n}\n\n.ipp-DialogSection-item {\n  display: flex;\n  align-items: center;\n  justify-content: space-around;\n  margin: 12px 0 12px 0;\n}\n\n.ipp-DialogHeader input[type="checkbox"] {\n  position: relative;\n  top: 4px;\n  left: 4px;\n  margin: 0 0 0 8px;\n}\n\n.ipp-DialogSection input[type="number"] {\n  width: 72px;\n}\n\n.ipp-DialogSection-label.ipp-mod-disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n.ipp-DialogSection input[type="number"]:disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n/**\n * Rules for the logos.\n */\n\n.ipp-SearchIcon {\n  background-image: var(--jp-icon-search);\n}\n\n[data-jp-theme-light="true"] .ipp-CodeIcon {\n  background-image: url(' + p + ');\n}\n\n[data-jp-theme-light="false"] .ipp-CodeIcon {\n  background-image: url(' + h + ");\n}\n\n.ipp-ClusterListingItem.jp-mod-active .ipp-CodeIcon {\n  background-image: url(" + h + ");\n}\n", ""]);
+                c = new URL(n(1), n.b),
+                u = new URL(n(362), n.b),
+                d = a()(i()),
+                p = l()(c),
+                h = l()(u);
+            d.push([e.id, `:root {\n  --ipp-launch-button-height: 24px;\n}\n\n/**\n * Rules related to the overall sidebar panel.\n */\n\n.ipp-Sidebar {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size1);\n  overflow: auto;\n}\n\n/**\n * Rules related to the cluster manager.\n */\n\n.ipp-ClusterManager .jp-Toolbar {\n  align-items: center;\n}\n\n.ipp-ClusterManager .jp-Toolbar .ipp-ClusterManager-label {\n  flex: 0 0 auto;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n  font-size: var(--jp-ui-font-size0);\n  padding: 8px 8px 8px 12px;\n  margin: 0px;\n}\n\n.ipp-ClusterManager button.jp-Button > span {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n}\n\n.ipp-ClusterListing ul.ipp-ClusterListing-list {\n  list-style-type: none;\n  padding: 0;\n  margin: 0;\n}\n\n.ipp-ClusterListingItem {\n  display: inline-block;\n  list-style-type: none;\n  padding: 8px;\n  width: 100%;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  cursor: grab;\n}\n\n.ipp-ClusterListingItem-drag {\n  opacity: 0.7;\n  color: var(--jp-ui-font-color1);\n  cursor: grabbing;\n  max-width: 260px;\n  transform: translateX(-50%) translateY(-50%);\n}\n\n.ipp-ClusterListingItem-title {\n  margin: 0px;\n  font-size: var(--jp-ui-font-size2);\n}\n\n.ipp-ClusterListingItem-link a {\n  text-decoration: none;\n  color: var(--jp-content-link-color);\n}\n\n.ipp-ClusterListingItem-link a:hover {\n  text-decoration: underline;\n}\n\n.ipp-ClusterListingItem-link a:visited {\n  color: var(--jp-content-link-color);\n}\n\n.ipp-ClusterListingItem:hover {\n  background: var(--jp-layout-color2);\n}\n\n.ipp-ClusterListingItem.jp-mod-active {\n  color: white;\n  background: var(--jp-brand-color0);\n}\n\n.ipp-ClusterListingItem.jp-mod-active a,\n.ipp-ClusterListingItem.jp-mod-active a:visited {\n  color: white;\n}\n\n.ipp-ClusterListingItem button.jp-mod-styled {\n  background-color: transparent;\n}\n\n.ipp-ClusterListingItem button.jp-mod-styled:hover {\n  background-color: var(--jp-layout-color3);\n}\n\n.ipp-ClusterListingItem.jp-mod-active button.jp-mod-styled:hover {\n  background-color: var(--jp-brand-color1);\n}\n\n.ipp-ClusterListingItem-button-panel {\n  display: flex;\n  align-content: center;\n}\n\nbutton.ipp-ClusterListingItem-stop {\n  color: var(--jp-warn-color1);\n  font-weight: 600;\n}\n\nbutton.ipp-ClusterListingItem-scale {\n  color: var(--jp-accent-color1);\n  font-weight: 600;\n}\n\nbutton.ipp-ClusterListingItem-start {\n  color: var(--jp-accent-color1);\n  font-weight: 600;\n}\n\nbutton.ipp-hidden {\n  display: none;\n}\n\n.ipp-ClusterListingItem button.ipp-ClusterListingItem-code.jp-mod-styled {\n  margin: 0 4px 0 4px;\n  background-repeat: no-repeat;\n  background-position: center;\n}\n\n/**\n * Rules for the scaling dialog.\n */\n\n.ipp-DialogHeader {\n  font-size: var(--jp-ui-font-size2);\n}\n\n.ipp-DialogSection {\n  margin-left: 24px;\n}\n\n.ipp-DialogSection-item {\n  display: flex;\n  align-items: center;\n  justify-content: space-around;\n  margin: 12px 0 12px 0;\n}\n\n.ipp-DialogHeader input[type="checkbox"] {\n  position: relative;\n  top: 4px;\n  left: 4px;\n  margin: 0 0 0 8px;\n}\n\n.ipp-DialogSection input[type="number"] {\n  width: 72px;\n}\n\n.ipp-DialogSection-label.ipp-mod-disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n.ipp-DialogSection input[type="number"]:disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n/**\n * Rules for the logos.\n */\n\n.ipp-SearchIcon {\n  background-image: var(--jp-icon-search);\n}\n\n[data-jp-theme-light="true"] .ipp-CodeIcon {\n  background-image: url(${p});\n}\n\n[data-jp-theme-light="false"] .ipp-CodeIcon {\n  background-image: url(${h});\n}\n\n.ipp-ClusterListingItem.jp-mod-active .ipp-CodeIcon {\n  background-image: url(${h});\n}\n`, ""]);
             const g = d
         },
         645: e => {
-            "use strict";
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
-                        var n = e(t);
-                        return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
+                        var n = "",
+                            s = void 0 !== t[5];
+                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), s && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), s && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, n, s) {
+                }, t.i = function(e, n, s, i, r) {
                     "string" == typeof e && (e = [
-                        [null, e, ""]
+                        [null, e, void 0]
                     ]);
-                    var i = {};
+                    var a = {};
                     if (s)
-                        for (var r = 0; r < this.length; r++) {
-                            var a = this[r][0];
-                            null != a && (i[a] = !0)
-                        }
-                    for (var o = 0; o < e.length; o++) {
-                        var l = [].concat(e[o]);
-                        s && i[l[0]] || (n && (l[2] ? l[2] = "".concat(n, " and ").concat(l[2]) : l[2] = n), t.push(l))
+                        for (var o = 0; o < this.length; o++) {
+                            var l = this[o][0];
+                            null != l && (a[l] = !0)
+                        }
+                    for (var c = 0; c < e.length; c++) {
+                        var u = [].concat(e[c]);
+                        s && a[u[0]] || (void 0 !== r && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = r), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), i && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = i) : u[4] = "".concat(i)), t.push(u))
                     }
                 }, t
             }
         },
         667: e => {
-            "use strict";
             e.exports = function(e, t) {
-                return t || (t = {}), "string" != typeof(e = e && e.__esModule ? e.default : e) ? e : (/^['"].*['"]$/.test(e) && (e = e.slice(1, -1)), t.hash && (e += t.hash), /["'() \t\n]/.test(e) || t.needQuotes ? '"'.concat(e.replace(/"/g, '\\"').replace(/\n/g, "\\n"), '"') : e)
+                return t || (t = {}), e ? (e = String(e.__esModule ? e.default : e), /^['"].*['"]$/.test(e) && (e = e.slice(1, -1)), t.hash && (e += t.hash), /["'() \t\n]|(%20)/.test(e) || t.needQuotes ? '"'.concat(e.replace(/"/g, '\\"').replace(/\n/g, "\\n"), '"') : e) : e
             }
         },
-        379: (e, t, n) => {
-            "use strict";
-            var s, i = function() {
-                    var e = {};
-                    return function(t) {
-                        if (void 0 === e[t]) {
-                            var n = document.querySelector(t);
-                            if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
-                                n = n.contentDocument.head
-                            } catch (e) {
-                                n = null
-                            }
-                            e[t] = n
-                        }
-                        return e[t]
-                    }
-                }(),
-                r = [];
+        81: e => {
+            e.exports = function(e) {
+                return e[1]
+            }
+        },
+        745: (e, t, n) => {
+            var s = n(704);
+            t.s = s.createRoot, s.hydrateRoot
+        },
+        379: e => {
+            var t = [];
 
-            function a(e) {
-                for (var t = -1, n = 0; n < r.length; n++)
-                    if (r[n].identifier === e) {
-                        t = n;
+            function n(e) {
+                for (var n = -1, s = 0; s < t.length; s++)
+                    if (t[s].identifier === e) {
+                        n = s;
                         break
-                    } return t
+                    } return n
             }
 
-            function o(e, t) {
-                for (var n = {}, s = [], i = 0; i < e.length; i++) {
-                    var o = e[i],
-                        l = t.base ? o[0] + t.base : o[0],
-                        c = n[l] || 0,
-                        u = "".concat(l, " ").concat(c);
-                    n[l] = c + 1;
-                    var d = a(u),
-                        p = {
-                            css: o[1],
-                            media: o[2],
-                            sourceMap: o[3]
-                        }; - 1 !== d ? (r[d].references++, r[d].updater(p)) : r.push({
-                        identifier: u,
-                        updater: m(p, t),
-                        references: 1
-                    }), s.push(u)
+            function s(e, s) {
+                for (var r = {}, a = [], o = 0; o < e.length; o++) {
+                    var l = e[o],
+                        c = s.base ? l[0] + s.base : l[0],
+                        u = r[c] || 0,
+                        d = "".concat(c, " ").concat(u);
+                    r[c] = u + 1;
+                    var p = n(d),
+                        h = {
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3],
+                            supports: l[4],
+                            layer: l[5]
+                        };
+                    if (-1 !== p) t[p].references++, t[p].updater(h);
+                    else {
+                        var g = i(h, s);
+                        s.byIndex = o, t.splice(o, 0, {
+                            identifier: d,
+                            updater: g,
+                            references: 1
+                        })
+                    }
+                    a.push(d)
                 }
-                return s
+                return a
             }
 
-            function l(e) {
-                var t = document.createElement("style"),
-                    s = e.attributes || {};
-                if (void 0 === s.nonce) {
-                    var r = n.nc;
-                    r && (s.nonce = r)
-                }
-                if (Object.keys(s).forEach((function(e) {
-                        t.setAttribute(e, s[e])
-                    })), "function" == typeof e.insert) e.insert(t);
-                else {
-                    var a = i(e.insert || "head");
-                    if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    a.appendChild(t)
-                }
-                return t
+            function i(e, t) {
+                var n = t.domAPI(t);
+                return n.update(e),
+                    function(t) {
+                        if (t) {
+                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
+                            n.update(e = t)
+                        } else n.remove()
+                    }
             }
-            var c, u = (c = [], function(e, t) {
-                return c[e] = t, c.filter(Boolean).join("\n")
-            });
-
-            function d(e, t, n, s) {
-                var i = n ? "" : s.media ? "@media ".concat(s.media, " {").concat(s.css, "}") : s.css;
-                if (e.styleSheet) e.styleSheet.cssText = u(t, i);
-                else {
-                    var r = document.createTextNode(i),
-                        a = e.childNodes;
-                    a[t] && e.removeChild(a[t]), a.length ? e.insertBefore(r, a[t]) : e.appendChild(r)
+            e.exports = function(e, i) {
+                var r = s(e = e || [], i = i || {});
+                return function(e) {
+                    e = e || [];
+                    for (var a = 0; a < r.length; a++) {
+                        var o = n(r[a]);
+                        t[o].references--
+                    }
+                    for (var l = s(e, i), c = 0; c < r.length; c++) {
+                        var u = n(r[c]);
+                        0 === t[u].references && (t[u].updater(), t.splice(u, 1))
+                    }
+                    r = l
                 }
             }
-
-            function p(e, t, n) {
-                var s = n.css,
-                    i = n.media,
-                    r = n.sourceMap;
-                if (i ? e.setAttribute("media", i) : e.removeAttribute("media"), r && "undefined" != typeof btoa && (s += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), e.styleSheet) e.styleSheet.cssText = s;
-                else {
-                    for (; e.firstChild;) e.removeChild(e.firstChild);
-                    e.appendChild(document.createTextNode(s))
-                }
+        },
+        569: e => {
+            var t = {};
+            e.exports = function(e, n) {
+                var s = function(e) {
+                    if (void 0 === t[e]) {
+                        var n = document.querySelector(e);
+                        if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                            n = n.contentDocument.head
+                        } catch (e) {
+                            n = null
+                        }
+                        t[e] = n
+                    }
+                    return t[e]
+                }(e);
+                if (!s) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                s.appendChild(n)
             }
-            var h = null,
-                g = 0;
-
-            function m(e, t) {
-                var n, s, i;
-                if (t.singleton) {
-                    var r = g++;
-                    n = h || (h = l(t)), s = d.bind(null, n, r, !1), i = d.bind(null, n, r, !0)
-                } else n = l(t), s = p.bind(null, n, t), i = function() {
-                    ! function(e) {
-                        if (null === e.parentNode) return !1;
-                        e.parentNode.removeChild(e)
-                    }(n)
+        },
+        216: e => {
+            e.exports = function(e) {
+                var t = document.createElement("style");
+                return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
+            }
+        },
+        565: (e, t, n) => {
+            e.exports = function(e) {
+                var t = n.nc;
+                t && e.setAttribute("nonce", t)
+            }
+        },
+        795: e => {
+            e.exports = function(e) {
+                if ("undefined" == typeof document) return {
+                    update: function() {},
+                    remove: function() {}
                 };
-                return s(e),
-                    function(t) {
-                        if (t) {
-                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                            s(e = t)
-                        } else i()
+                var t = e.insertStyleElement(e);
+                return {
+                    update: function(n) {
+                        ! function(e, t, n) {
+                            var s = "";
+                            n.supports && (s += "@supports (".concat(n.supports, ") {")), n.media && (s += "@media ".concat(n.media, " {"));
+                            var i = void 0 !== n.layer;
+                            i && (s += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), s += n.css, i && (s += "}"), n.media && (s += "}"), n.supports && (s += "}");
+                            var r = n.sourceMap;
+                            r && "undefined" != typeof btoa && (s += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), t.styleTagTransform(s, e, t.options)
+                        }(t, e, n)
+                    },
+                    remove: function() {
+                        ! function(e) {
+                            if (null === e.parentNode) return !1;
+                            e.parentNode.removeChild(e)
+                        }(t)
                     }
+                }
             }
+        },
+        589: e => {
             e.exports = function(e, t) {
-                (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === s && (s = Boolean(window && document && document.all && !window.atob)), s));
-                var n = o(e = e || [], t);
-                return function(e) {
-                    if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                        for (var s = 0; s < n.length; s++) {
-                            var i = a(n[s]);
-                            r[i].references--
-                        }
-                        for (var l = o(e, t), c = 0; c < n.length; c++) {
-                            var u = a(n[c]);
-                            0 === r[u].references && (r[u].updater(), r.splice(u, 1))
-                        }
-                        n = l
-                    }
+                if (t.styleSheet) t.styleSheet.cssText = e;
+                else {
+                    for (; t.firstChild;) t.removeChild(t.firstChild);
+                    t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        618: e => {
-            e.exports = "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='%23E0E0E0' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath fill='none' d='M0 0h24v24H0V0z'/%3E%3Cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3E%3C/svg%3E"
+        362: e => {
+            e.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='%23E0E0E0' width='24' height='24' viewBox='0 0 24 24'%3e%3cpath fill='none' d='M0 0h24v24H0V0z'/%3e%3cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3e%3c/svg%3e"
         },
-        825: e => {
-            e.exports = "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='%23616161' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath fill='none' d='M0 0h24v24H0V0z'/%3E%3Cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3E%3C/svg%3E"
+        1: e => {
+            e.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='%23616161' width='24' height='24' viewBox='0 0 24 24'%3e%3cpath fill='none' d='M0 0h24v24H0V0z'/%3e%3cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3e%3c/svg%3e"
         }
     }
 ]);
```

### Comparing `ipyparallel-8.6.1/ipyparallel/labextension/static/remoteEntry.f5bc00ef0248261af0b1.js` & `ipyparallel-8.7.0/ipyparallel/labextension/static/remoteEntry.ccf2bfedaae5f1da1a90.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, l, i, u, f, s, d, p, c, h, v, b, m, g = {
+    var e, r, t, n, a, o, i, l, u, s, f, d, p, c, h, v, b = {
             61: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(60), t.e(592)]).then((() => () => t(592))),
-                        "./extension": () => Promise.all([t.e(60), t.e(592)]).then((() => () => t(592)))
+                        "./index": () => t.e(998).then((() => () => t(998))),
+                        "./extension": () => t.e(998).then((() => () => t(998)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -20,278 +20,266 @@
                     };
                 t.d(r, {
                     get: () => a,
                     init: () => o
                 })
             }
         },
-        y = {};
+        g = {};
 
-    function w(e) {
-        var r = y[e];
+    function m(e) {
+        var r = g[e];
         if (void 0 !== r) return r.exports;
-        var t = y[e] = {
+        var t = g[e] = {
             id: e,
             exports: {}
         };
-        return g[e](t, t.exports, w), t.exports
+        return b[e](t, t.exports, m), t.exports
     }
-    w.m = g, w.c = y, w.n = e => {
+    m.m = b, m.c = g, m.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return w.d(r, {
+        return m.d(r, {
             a: r
         }), r
-    }, w.d = (e, r) => {
-        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
+    }, m.d = (e, r) => {
+        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        60: "549e6d23fd01f935aa18",
-        114: "b63b1cb1deb6ab07694a",
-        592: "2265e4df71d8ba0dbbf6"
-    } [e] + ".js?v=" + {
-        60: "549e6d23fd01f935aa18",
-        114: "b63b1cb1deb6ab07694a",
-        592: "2265e4df71d8ba0dbbf6"
-    } [e], w.g = function() {
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".d38d80ac3e2fa7501089.js?v=d38d80ac3e2fa7501089", m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyparallel-labextension:", w.l = (t, n, a, o) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyparallel-labextension:", m.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var l, i;
+            var i, l;
             if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        l = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var f = u[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
+                        i = f;
                         break
                     }
                 }
-            l || (i = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, w.nc && l.setAttribute("nonce", w.nc), l.setAttribute("data-webpack", r + a), l.src = t), e[t] = [n];
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    l.onerror = l.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
-                    if (delete e[t], l.parentNode && l.parentNode.removeChild(l), a && a.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
-                    target: l
+                    target: i
                 }), 12e4);
-            l.onerror = d.bind(null, l.onerror), l.onload = d.bind(null, l.onload), i && document.head.appendChild(l)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
-    }, w.r = e => {
+    }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        w.S = {};
+        m.S = {};
         var e = {},
             r = {};
-        w.I = (t, n) => {
+        m.I = (t, n) => {
             n || (n = []);
             var a = r[t];
             if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
                 if (n.push(a), e[t]) return e[t];
-                w.o(w.S, t) || (w.S[t] = {});
-                var o = w.S[t],
-                    l = "ipyparallel-labextension",
-                    i = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            i = a[r];
-                        (!i || !i.loaded && (!n != !i.eager ? n : l > i.from)) && (a[r] = {
-                            get: t,
-                            from: l,
-                            eager: !!n
-                        })
-                    },
-                    u = [];
-                return "default" === t && (i("@lumino/polling", "1.11.4", (() => Promise.all([w.e(114), w.e(60)]).then((() => () => w(114))))), i("ipyparallel-labextension", "8.6.1", (() => Promise.all([w.e(60), w.e(592)]).then((() => () => w(592)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                m.o(m.S, t) || (m.S[t] = {});
+                var o = m.S[t],
+                    i = "ipyparallel-labextension",
+                    l = [];
+                return "default" === t && ((e, r, t, n) => {
+                    var a = o[e] = o[e] || {},
+                        l = a[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (a[r] = {
+                        get: () => m.e(998).then((() => () => m(998))),
+                        from: i,
+                        eager: !1
+                    })
+                })("ipyparallel-labextension", "8.7.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        w.g.importScripts && (e = w.g.location + "");
-        var r = w.g.document;
+        m.g.importScripts && (e = m.g.location + "");
+        var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var a = e[n],
                 o = (typeof a)[0];
             if (n >= r.length) return "u" == o;
-            var l = r[n],
-                i = (typeof l)[0];
-            if (o != i) return "o" == o && "n" == i || "s" == i || "u" == o;
-            if ("o" != o && "u" != o && a != l) return a < l;
+            var i = r[n],
+                l = (typeof i)[0];
+            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
     }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(i = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, i);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
-        var l = [];
+        var i = [];
         for (o = 1; o < e.length; o++) {
-            var i = e[o];
-            l.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? l.pop() + " " + l.pop() : a(i))
+            var l = e[o];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
         }
         return u();
 
         function u() {
-            return l.pop().replace(/^\((.+)\)$/, "$1")
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
-            for (var l = 0, i = 1, u = !0;; i++, l++) {
-                var f, s, d = i < e.length ? (typeof e[i])[0] : "";
-                if (l >= r.length || "o" == (s = (typeof(f = r[l]))[0])) return !u || ("u" == d ? i > n && !a : "" == d != a);
-                if ("u" == s) {
+            for (var i = 0, l = 1, u = !0;; l++, i++) {
+                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
+                if ("u" == f) {
                     if (!u || "u" != d) return !1
                 } else if (u)
-                    if (d == s)
-                        if (i <= n) {
-                            if (f != e[i]) return !1
+                    if (d == f)
+                        if (l <= n) {
+                            if (s != e[l]) return !1
                         } else {
-                            if (a ? f > e[i] : f < e[i]) return !1;
-                            f != e[i] && (u = !1)
+                            if (a ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
-                    if (a || i <= n) return !1;
-                    u = !1, i--
+                    if (a || l <= n) return !1;
+                    u = !1, l--
                 } else {
-                    if (i <= n || s < d != a) return !1;
+                    if (l <= n || f < d != a) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, i--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
-        for (l = 1; l < e.length; l++) {
-            var h = e[l];
+        for (i = 1; i < e.length; i++) {
+            var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
-    }, l = (e, r) => {
-        var t = w.S[e];
-        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
-        return t
     }, i = (e, r) => {
+        var t = m.S[e];
+        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        return t
+    }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
-        var a = i(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(u(e, t, a, n)), d(e[t][a])
-    }, s = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, d = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
-        var o = w.I(r);
-        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (l(e, t), f(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
-        var o = r && w.o(r, t) && s(r, t, n);
-        return o ? d(o) : a()
-    })), v = {}, b = {
-        526: () => c("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        840: () => c("default", "@lumino/signaling", [1, 1, 10, 0]),
-        33: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
-        123: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        271: () => c("default", "react", [1, 17, 0, 1]),
-        282: () => c("default", "@jupyterlab/console", [1, 3, 6, 3]),
-        358: () => h("default", "@lumino/polling", [1, 1, 0, 4], (() => w.e(114).then((() => () => w(114))))),
-        456: () => c("default", "react-dom", [1, 17, 0, 1]),
-        502: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
-        520: () => c("default", "@lumino/domutils", [1, 1, 8, 0]),
-        687: () => c("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        694: () => c("default", "@lumino/dragdrop", [1, 1, 13, 0]),
-        820: () => c("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        832: () => c("default", "@lumino/widgets", [1, 1, 37, 2]),
-        918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        933: () => c("default", "@jupyterlab/statedb", [1, 3, 6, 3])
-    }, m = {
-        60: [526, 840],
-        592: [33, 38, 123, 142, 271, 282, 358, 456, 502, 520, 687, 694, 820, 832, 918, 933]
-    }, w.f.consumes = (e, r) => {
-        w.o(m, e) && m[e].forEach((e => {
-            if (w.o(v, e)) return r.push(v[e]);
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
+        var a = l(e, t);
+        return o(n, a) || f(u(e, t, a, n)), d(e[t][a])
+    }, f = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
+        var o = m.I(r);
+        return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
+        351: () => p("default", "@jupyterlab/coreutils", [1, 6, 1, 2]),
+        750: () => p("default", "@jupyterlab/application", [1, 4, 1, 2]),
+        824: () => p("default", "@jupyterlab/console", [1, 4, 1, 2]),
+        991: () => p("default", "@jupyterlab/settingregistry", [1, 4, 1, 2]),
+        943: () => p("default", "@jupyterlab/statedb", [1, 4, 1, 2]),
+        445: () => p("default", "@jupyterlab/notebook", [1, 4, 1, 2]),
+        448: () => p("default", "@jupyterlab/ui-components", [1, 4, 1, 2]),
+        901: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
+        882: () => p("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
+        403: () => p("default", "@jupyterlab/apputils", [1, 4, 2, 2]),
+        810: () => p("default", "@jupyterlab/services", [1, 7, 1, 2]),
+        697: () => p("default", "@lumino/algorithm", [1, 2, 0, 0]),
+        930: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        593: () => p("default", "@lumino/domutils", [1, 2, 0, 0]),
+        359: () => p("default", "@lumino/dragdrop", [1, 2, 0, 0]),
+        797: () => p("default", "@lumino/polling", [1, 2, 0, 0]),
+        29: () => p("default", "react", [1, 18, 2, 0]),
+        704: () => p("default", "react-dom", [1, 18, 2, 0])
+    }, v = {
+        998: [351, 750, 824, 991, 943, 445, 448, 901, 882, 403, 810, 697, 930, 593, 359, 797, 29, 704]
+    }, m.f.consumes = (e, r) => {
+        m.o(v, e) && v[e].forEach((e => {
+            if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    v[e] = 0, w.m[e] = t => {
-                        delete w.c[e], t.exports = r()
+                    c[e] = 0, m.m[e] = t => {
+                        delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete v[e], w.m[e] = t => {
-                        throw delete w.c[e], r
+                    delete c[e], m.m[e] = t => {
+                        throw delete m.c[e], r
                     }
                 };
             try {
-                var a = b[e]();
-                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
+                var a = h[e]();
+                a.then ? r.push(c[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
+        m.b = document.baseURI || self.location.href;
         var e = {
             489: 0
         };
-        w.f.j = (r, t) => {
-            var n = w.o(e, r) ? e[r] : void 0;
+        m.f.j = (r, t) => {
+            var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (60 != r) {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
-                var o = w.p + w.u(r),
-                    l = new Error;
-                w.l(o, (t => {
-                    if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        l.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", l.name = "ChunkLoadError", l.type = a, l.request = o, n[1](l)
-                    }
-                }), "chunk-" + r, r)
-            } else e[r] = 0
+                else {
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
+                    var o = m.p + m.u(r),
+                        i = new Error;
+                    m.l(o, (t => {
+                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var a = t && ("load" === t.type ? "missing" : t.type),
+                                o = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        }
+                    }), "chunk-" + r, r)
+                }
         };
         var r = (r, t) => {
-                var n, a, [o, l, i] = t,
+                var n, a, [o, i, l] = t,
                     u = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (n in l) w.o(l, n) && (w.m[n] = l[n]);
-                    i && i(w)
+                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
+                    l && l(m)
                 }
-                for (r && r(t); u < o.length; u++) a = o[u], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); u < o.length; u++) a = o[u], m.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkipyparallel_labextension = self.webpackChunkipyparallel_labextension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), w.nc = void 0;
-    var j = w(61);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["ipyparallel-labextension"] = j
+    })(), m.nc = void 0;
+    var y = m(61);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["ipyparallel-labextension"] = y
 })();
```

### Comparing `ipyparallel-8.6.1/ipyparallel/labextension/static/third-party-licenses.json` & `ipyparallel-8.7.0/ipyparallel/labextension/static/third-party-licenses.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'packages'": "{0: {'name': 'css-loader', 'versionInfo': '6.8.1', 'licenseId': 'MIT', "*

 * *               '\'extractedText\': "Copyright JS Foundation and other contributors\\n\\nPermission '*

 * *               'is hereby granted, free of charge, to any person obtaining\\na copy of this '*

 * *               "software and associated documentation files (the\\n'Software'), to deal in the "*

 * *               'Software without restriction, including\\nwithout limitation the rights to use, '*

 * *               'copy, modify, mer […]*

```diff
@@ -1,22 +1,22 @@
 {
     "packages": [
         {
-            "extractedText": "",
-            "licenseId": "BSD-3-Clause",
-            "name": "@lumino/polling",
-            "versionInfo": "1.11.4"
-        },
-        {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.8.1"
+        },
+        {
+            "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "react-dom",
+            "versionInfo": "18.2.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.3"
         }
     ]
 }
```

### Comparing `ipyparallel-8.6.1/ipyparallel/nbextension/base.py` & `ipyparallel-8.7.0/ipyparallel/nbextension/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Place to put the base Handler"""
+
 import warnings
 from functools import lru_cache
 
 _APIHandler = None
 
 
 @lru_cache()
```

### Comparing `ipyparallel-8.6.1/ipyparallel/nbextension/handlers.py` & `ipyparallel-8.7.0/ipyparallel/nbextension/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Tornado handlers for IPython cluster web service."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import json
 import os
 
-from jupyter_server.utils import url_path_join as ujoin
+try:
+    from jupyter_server.utils import url_path_join as ujoin
+except ImportError:
+    # fallback on legacy Notebook server
+    from notebook.utils import url_path_join as ujoin
+
 from tornado import web
 
 from ..cluster import ClusterManager
 from ..util import abbreviate_profile_dir
 from .base import get_api_handler
 
 static = os.path.join(os.path.dirname(__file__), 'static')
```

### Comparing `ipyparallel-8.6.1/ipyparallel/nbextension/install.py` & `ipyparallel-8.7.0/ipyparallel/nbextension/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""Install the IPython clusters tab in the Jupyter notebook dashboard"""
+"""Install the IPython clusters tab in the Jupyter notebook dashboard
+
+Only applicable for notebook < 7
+"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 from jupyter_core.paths import jupyter_config_dir
 from notebook.services.config import ConfigManager as FrontendConfigManager
 from traitlets.config.manager import BaseJSONConfigManager
```

### Comparing `ipyparallel-8.6.1/ipyparallel/nbextension/static/clusterlist.js` & `ipyparallel-8.7.0/ipyparallel/nbextension/static/clusterlist.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/nbextension/static/main.js` & `ipyparallel-8.7.0/ipyparallel/nbextension/static/main.js`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/serialize/__init__.py` & `ipyparallel-8.7.0/ipyparallel/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/serialize/canning.py` & `ipyparallel-8.7.0/ipyparallel/serialize/canning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pickle-related utilities.."""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import copy
 import functools
 import sys
 from types import FunctionType
```

### Comparing `ipyparallel-8.6.1/ipyparallel/serialize/codeutil.py` & `ipyparallel-8.7.0/ipyparallel/serialize/codeutil.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Any process that import this module will be able to pickle code objects.  This
 includes the func_code attribute of any function.  Once unpickled, new
 functions can be built using new.function(code, globals()).  Eventually
 we need to automate all of this so that functions themselves can be pickled.
 
 Reference: A. Tremols, P Cogolo, "Python Cookbook," p 302-305
 """
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import copyreg
 import inspect
 import sys
 import types
 
@@ -23,15 +24,16 @@
 # (they _almost_ all match, and new ones probably will)
 _code_attr_map = {
     "codestring": "code",
     "constants": "consts",
 }
 # pass every supported arg to the code constructor
 # this should be more forward-compatible
-if sys.version_info >= (3, 10):
+# (broken on pypy: https://github.com/ipython/ipyparallel/issues/845)
+if sys.version_info >= (3, 10) and not hasattr(sys, "pypy_version_info"):
     _code_attr_names = tuple(
         _code_attr_map.get(name, name)
         for name, param in inspect.signature(types.CodeType).parameters.items()
         if param.POSITIONAL_ONLY or param.POSITIONAL_OR_KEYWORD
     )
 else:
     # can't inspect types.CodeType on Python < 3.10
```

### Comparing `ipyparallel-8.6.1/ipyparallel/serialize/serialize.py` & `ipyparallel-8.7.0/ipyparallel/serialize/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """serialization utilities for apply messages"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 try:
     import cPickle
 
     pickle = cPickle
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/__init__.py` & `ipyparallel-8.7.0/ipyparallel/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """toplevel setup/teardown for parallel tests."""
+
 import asyncio
 import os
 import time
 from subprocess import Popen
 
 from IPython.paths import get_ipython_dir
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/clienttest.py` & `ipyparallel-8.7.0/ipyparallel/tests/clienttest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """base class for parallel client tests"""
+
 import os
 import signal
 import sys
 import time
 import warnings
 from contextlib import contextmanager
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/conftest.py` & `ipyparallel-8.7.0/ipyparallel/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pytest fixtures"""
+
 import inspect
 import logging
 import os
 import sys
 from contextlib import contextmanager
 from pathlib import Path
 from subprocess import check_call, check_output
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_apps.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test CLI application behavior"""
+
 import glob
 import json
 import os
 import sys
 import time
 import types
 from subprocess import Popen, check_call, check_output
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_async.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """tests for async utilities"""
+
 import pytest
 
 from ipyparallel._async import AsyncFirst
 
 
 class A(AsyncFirst):
     a = 5
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_asyncresult.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_asyncresult.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for asyncresult.py"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import os
 import time
 from datetime import datetime
 
 import pytest
@@ -391,21 +392,24 @@
         d = dir(ar)
         assert 'stdout' in d
         assert 'get' in d
 
     def test_wait_for_send(self):
         view = self.client[-1]
         view.track = True
+
         with pytest.raises(TimeoutError):
             # this test can fail if the send happens too quickly
             # e.g. the IO thread takes control for too long,
             # so run the test a few times
-            for i in range(10):
+            for i in range(3):
                 if i > 0:
                     print("Retrying test_wait_for_send")
+                # inject delay in io loop so send doesn't complete immediately
+                self.client._io_loop.add_callback(lambda: time.sleep(0.5))
                 data = os.urandom(10 * 1024 * 1024)
                 ar = view.apply_async(lambda x: x, data)
                 ar.wait_for_send(0)
         ar.wait_for_send(10)
 
     def test_return_exceptions(self):
         view = self.client.load_balanced_view()
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_canning.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_canning.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_client.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for parallel client.py"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import os
 import signal
 import socket
 import sys
 import time
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_cluster.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_db.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for db backends"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import logging
 import os
 import tempfile
 import time
 from datetime import datetime, timedelta
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_dependency.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for dependency.py"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import ipyparallel as ipp
 from ipyparallel.serialize import can, uncan
 from ipyparallel.util import interactive
 
 from .clienttest import ClusterTestCase, raises_remote
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_executor.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for Executor API"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import time
 
 from ipyparallel.client.view import LazyMapIterator, LoadBalancedView
 
 from .clienttest import ClusterTestCase
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_joblib.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_joblib.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_launcher.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for launchers
 
 Doesn't actually start any subprocesses, but goes through the motions of constructing
 objects, which should test basic config.
 """
+
 import logging
 import os
 import sys
 import time
 from subprocess import Popen
 
 import entrypoints
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_lbview.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_lbview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """test LoadBalancedView objects"""
+
 import time
 from itertools import count
 
 import pytest
 
 import ipyparallel as ipp
 from ipyparallel import error
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_magics.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_magics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test Parallel magics"""
+
 import re
 import signal
 import sys
 import time
 
 import pytest
 from IPython import get_ipython
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_mongodb.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_mongodb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for mongodb backend"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import os
 from unittest import TestCase
 
 import pytest
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_mpi.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_remotefunction.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_remotefunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for remote functions"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import ipyparallel as ipp
 
 from .clienttest import ClusterTestCase
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_serialize.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """test serialization tools"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import pickle
 from collections import namedtuple
 
 import pytest
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_slurm.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_slurm.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_ssh.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_util.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import socket
-from unittest import mock
 
+import pytest
 from jupyter_client.localinterfaces import localhost, public_ips
 
 from ipyparallel import util
 
 
-@mock.patch('warnings.warn')
-def test_disambiguate_ip(warn_mock):
+def test_disambiguate_ip():
     # garbage in, garbage out
     public_ip = public_ips()[0]
     assert util.disambiguate_ip_address('garbage') == 'garbage'
     assert util.disambiguate_ip_address('0.0.0.0', socket.gethostname()) == localhost()
     wontresolve = 'this.wontresolve.dns'
-    assert util.disambiguate_ip_address('0.0.0.0', wontresolve) == wontresolve
-    assert warn_mock.called_once_with(
-        'IPython could not determine IPs for {}: '
-        '[Errno -2] Name or service not known'.format(wontresolve),
-        RuntimeWarning,
-    )
+    with pytest.warns(
+        RuntimeWarning, match=f"IPython could not determine IPs for {wontresolve}"
+    ):
+        assert util.disambiguate_ip_address('0.0.0.0', wontresolve) == wontresolve
     assert util.disambiguate_ip_address('0.0.0.0', public_ip) == localhost()
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_view.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """test View objects"""
+
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 import base64
 import platform
 import sys
 import time
 from collections import namedtuple
```

### Comparing `ipyparallel-8.6.1/ipyparallel/tests/test_view_broadcast.py` & `ipyparallel-8.7.0/ipyparallel/tests/test_view_broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """test BroadcastView objects"""
+
 import pytest
 
 from . import test_view
 
 needs_map = pytest.mark.xfail(reason="map not yet implemented")
 
 
@@ -23,16 +24,16 @@
                 self._broadcast_view_used = True
                 return self.client.broadcast_view(
                     targets, is_coalescing=self.is_coalescing
                 )
 
         self.client.direct_view = broadcast_or_direct
 
-    def teardown(self):
-        super().teardown()
+    def teardown_method(self):
+        super().teardown_method()
         # note that a test didn't use a broadcast view
         if not self._broadcast_view_used:
             pytest.skip("No broadcast view used")
 
     @needs_map
     def test_map(self):
         pass
```

### Comparing `ipyparallel-8.6.1/lab/src/clusters.tsx` & `ipyparallel-8.7.0/lab/src/clusters.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import { ISignal, Signal } from "@lumino/signaling";
 
 import { Widget, PanelLayout } from "@lumino/widgets";
 
 import { newClusterDialog, INewCluster } from "./dialog";
 
 import * as React from "react";
-import * as ReactDOM from "react-dom";
+import { createRoot } from "react-dom/client";
 import { CommandRegistry } from "@lumino/commands";
 
 import { CommandIDs } from "./commands";
 
 /**
  * A refresh interval (in ms) for polling the backend cluster manager.
  */
@@ -246,16 +246,16 @@
    * Handle an update request.
    */
   protected onUpdateRequest(msg: Message): void {
     // Don't bother if the sidebar is not visible
     if (!this.isVisible) {
       return;
     }
-
-    ReactDOM.render(
+    const root = createRoot(this._clusterListing.node);
+    root.render(
       <ClusterListing
         clusters={this._clusters}
         activeClusterId={(this._activeCluster && this._activeCluster.id) || ""}
         scaleById={(id: string) => {
           return this._scaleById(id);
         }}
         startById={(id: string) => {
@@ -263,15 +263,14 @@
         }}
         stopById={(id: string) => {
           return this._stopById(id);
         }}
         setActiveById={this._setActiveById}
         injectClientCodeForCluster={this._injectClientCodeForCluster}
       />,
-      this._clusterListing.node,
     );
   }
 
   /**
    * Rerender after showing.
    */
   protected onAfterShow(msg: Message): void {
```

### Comparing `ipyparallel-8.6.1/lab/src/commands.ts` & `ipyparallel-8.7.0/lab/src/commands.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/lab/src/dialog.tsx` & `ipyparallel-8.7.0/lab/src/dialog.tsx`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/lab/src/index.ts` & `ipyparallel-8.7.0/lab/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
   labShell?: ILabShell | null,
 ): Promise<void> {
   const id = "ipp-cluster-launcher";
 
   const isLab = !!labShell;
   const isRetroTree = PageConfig.getOption("retroPage") == "tree";
 
-  const clientCodeInjector = (model: IClusterModel) => {
-    const editor = Private.getCurrentEditor(
+  const clientCodeInjector = async (model: IClusterModel) => {
+    const editor = await Private.getCurrentEditor(
       app,
       notebookTracker,
       consoleTracker,
     );
     if (!editor) {
       return;
     }
@@ -242,20 +242,20 @@
 
   // Add a command to inject client connection code for a given cluster model.
   // This looks for a cluster model in the application context menu,
   // and looks for an editor among the currently active notebooks and consoles.
   // If either is not found, it bails.
   app.commands.addCommand(CommandIDs.injectClientCode, {
     label: "Inject IPython Client Connection Code",
-    execute: () => {
+    execute: async () => {
       const cluster = Private.clusterFromClick(app, sidebar.clusterManager);
       if (!cluster) {
         return;
       }
-      clientCodeInjector(cluster);
+      return await clientCodeInjector(cluster);
     },
   });
 
   // Add a command to launch a new cluster.
   app.commands.addCommand(CommandIDs.newCluster, {
     label: (args) => (args["isPalette"] ? "Create New Cluster" : "NEW"),
     execute: () => sidebar.clusterManager.create(),
@@ -409,15 +409,15 @@
   export function injectClientCode(
     cluster: IClusterModel,
     editor: CodeEditor.IEditor,
   ): void {
     const cursor = editor.getCursorPosition();
     const offset = editor.getOffsetAt(cursor);
     const code = getClientCode(cluster);
-    editor.model.value.insert(offset, code);
+    editor.model.sharedModel.updateSource(offset, offset, code);
   }
 
   /**
    * Get code to connect to a given cluster.
    */
   export function getClientCode(cluster: IClusterModel): string {
     return `import ipyparallel as ipp
@@ -456,38 +456,42 @@
 
   /**
    * Get the currently focused editor in the application,
    * checking both notebooks and consoles.
    * In the case of a notebook, it creates a new cell above the currently
    * active cell and then returns that.
    */
-  export function getCurrentEditor(
+  export async function getCurrentEditor(
     app: JupyterFrontEnd,
     notebookTracker: INotebookTracker,
     consoleTracker: IConsoleTracker,
-  ): CodeEditor.IEditor | null | undefined {
+  ): Promise<CodeEditor.IEditor | null | undefined> {
     // Get a handle on the most relevant kernel,
     // whether it is attached to a notebook or a console.
     let current = app.shell.currentWidget;
     let editor: CodeEditor.IEditor | null | undefined;
     if (current && notebookTracker.has(current)) {
       NotebookActions.insertAbove((current as NotebookPanel).content);
       const cell = (current as NotebookPanel).content.activeCell;
+      await cell.ready;
       editor = cell && cell.editor;
     } else if (current && consoleTracker.has(current)) {
       const cell = (current as ConsolePanel).console.promptCell;
+      await cell.ready;
       editor = cell && cell.editor;
     } else if (notebookTracker.currentWidget) {
       const current = notebookTracker.currentWidget;
       NotebookActions.insertAbove(current.content);
       const cell = current.content.activeCell;
+      await cell.ready;
       editor = cell && cell.editor;
     } else if (consoleTracker.currentWidget) {
       const current = consoleTracker.currentWidget;
       const cell = current.console.promptCell;
+      await cell.ready;
       editor = cell && cell.editor;
     }
     return editor;
   }
 
   /**
    * Get a cluster model based on the application context menu click node.
```

### Comparing `ipyparallel-8.6.1/lab/src/sidebar.ts` & `ipyparallel-8.7.0/lab/src/sidebar.ts`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/lab/style/index.css` & `ipyparallel-8.7.0/lab/style/index.css`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/lab/style/logo.svg` & `ipyparallel-8.7.0/lab/style/logo.svg`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/COPYING.md` & `ipyparallel-8.7.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/README.md` & `ipyparallel-8.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyparallel-8.6.1/hatch_build.py` & `ipyparallel-8.7.0/hatch_build.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom build script for hatch backend"""
+
 import glob
 import os
 import subprocess
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
```

### Comparing `ipyparallel-8.6.1/pyproject.toml` & `ipyparallel-8.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = [
-  "jupyterlab>=3.0.0,==3.*",
-  "hatchling>=0.25"
+  "jupyterlab==4.*",
+  "hatchling>=0.25",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ipyparallel"
-version = "8.6.1"
+version = "8.7.0"
 authors = [{name = "IPython Development Team", email = "ipython-dev@scipy.org"}]
 license = {file = "COPYING.md"}
 readme = "README.md"
 description = "Interactive Parallel Computing with IPython"
 keywords = [
     "Interactive",
     "Interpreter",
@@ -30,15 +30,15 @@
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 urls = {Homepage = "https://ipython.org"}
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "entrypoints",
     "decorator",
     "pyzmq>=18",
     "traitlets>=4.3",
     "ipython>=4",
     "jupyter_client",
@@ -141,15 +141,15 @@
 ]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/jupyterhub/jupyterhub"
 
 [tool.tbump.version]
-current = "8.6.1"
+current = "8.7.0"
 
 # pep440 regex
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
```

### Comparing `ipyparallel-8.6.1/PKG-INFO` & `ipyparallel-8.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyparallel
-Version: 8.6.1
+Version: 8.7.0
 Summary: Interactive Parallel Computing with IPython
 Project-URL: Homepage, https://ipython.org
 Author-email: IPython Development Team <ipython-dev@scipy.org>
 License: # Licensing terms
         
         Traitlets is adapted from enthought.traits, Copyright (c) Enthought, Inc.,
         under the terms of the Modified BSD License.
@@ -77,15 +77,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: decorator
 Requires-Dist: entrypoints
 Requires-Dist: ipykernel>=4.4
 Requires-Dist: ipython>=4
 Requires-Dist: jupyter-client
 Requires-Dist: psutil
 Requires-Dist: python-dateutil>=2.1
```

