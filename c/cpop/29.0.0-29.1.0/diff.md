# Comparing `tmp/cpop-29.0.0.tar.gz` & `tmp/cpop-29.1.0.tar.gz`

## Comparing `cpop-29.0.0.tar` & `cpop-29.1.0.tar`

### file list

```diff
@@ -1,21 +1,176 @@
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-29.0.0/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-29.0.0/cpop/data.pyx
--rwxr-xr-x   0        0        0     4280 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/__main__.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/config.yaml
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/dirs.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/exc.py
--rw-r--r--   0        0        0    23473 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/hub.py
--rw-r--r--   0        0        0    11479 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/loader.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/ref.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/scanner.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/verify.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/log/async.py
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/config.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/contract.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/dyne.py
--rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/sub.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-29.0.0/pop/mods/test.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-29.0.0/.gitignore
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 cpop-29.0.0/README.rst
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 cpop-29.0.0/pyproject.toml
--rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 cpop-29.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 cpop-29.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-29.1.0/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-29.1.0/src/cpop/data.pyx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/src/hub/__init__.py
+-rwxr-xr-x   0        0        0     4790 2020-02-02 00:00:00.000000 cpop-29.1.0/src/hub/__main__.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/config.yaml
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/dirs.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/exc.py
+-rw-r--r--   0        0        0    22326 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/hub.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/loader.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/ref.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/scanner.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/verify.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/log/async.py
+-rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/config.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/sub.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/test.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/test.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/testing.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/csigs/sigs.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/csigs/contracts/sigs.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/external_module/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/__init__.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_bench.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_coro.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_fail.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/falias_func.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/falias_wrap.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/proc.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/vtrue.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/alias_bad/init.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/alias_clash/init.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/README.rst
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/ca/config.yaml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/ca/contract_alias/init.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/init.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/clash.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/dup1.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/dup2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/float.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/init.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/invalid.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/neg.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/neg_last.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/pos.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/pos_first.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/zero.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/nest/init.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/config/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-29.1.0/.gitignore
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 cpop-29.1.0/README.rst
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 cpop-29.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 cpop-29.1.0/PKG-INFO
```

### Comparing `cpop-29.0.0/cpop/contract.pyx` & `cpop-29.1.0/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/cpop/data.pyx` & `cpop-29.1.0/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/pop/__main__.py` & `cpop-29.1.0/src/hub/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,70 +5,90 @@
 from collections.abc import Iterable
 from pprint import pprint
 
 import cpop.contract
 import cpop.data
 import pop.hub
 
+try:
+    import uvloop
+
+    HAS_UVLOOP = True
+except ImportError:
+    HAS_UVLOOP = False
+
 
 def save_hub_state(hub, state_file: pathlib.Path):
     # Manually retrieve the state using __getstate__
     state = hub.__getstate__()
     state_file.parent.mkdir(parents=True, exist_ok=True)
     with state_file.open("wb") as f:
         pickle.dump(state, f)
 
 
-def load_hub_state(hub, state_file: pathlib.Path):
+async def load_hub_state(hub, state_file: pathlib.Path, cli: str):
     if state_file.exists():
         try:
-            with state_file.open("rb") as f:
-                state = pickle.load(f)
+            async with hub.lib.aiofiles.open(state_file, "rb") as f:
+                state = pickle.loads(await f.read())
         except:
             return
+
+        if not state:
+            return
+
         if hub._init_kwargs != state["init_kwargs"]:
-            hub.__init__(**state["init_kwargs"])
-        hub.__setstate__(state)
-        return hub
+            cli = state["init_kwargs"].pop("cli", cli)
+            state["init_kwargs"].pop("load_config", None)
+            await hub.__ainit__(cli=cli, **state["init_kwargs"], load_config=False)
+
+        # Now that the hub has started, run all those waiting init tasks
+        await asyncio.gather(*hub._tasks)
 
 
 def main():
-    # Create the hub, loading all dynes and starting the loop
-    hub = pop.hub.Hub(cli="pop_cli")
+    # Initialize the event loop
+    if HAS_UVLOOP:
+        asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
+
+    asyncio.run(amain())
+
+
+async def amain():
+    hub = await pop.hub.AsyncHub(cli="pop_cli")
 
     original_opt = hub.OPT
     ref = original_opt.pop_cli.ref
-
-    safe_env = {"hub":cpop.data.NamespaceDict(lib=hub.lib)}
+    cli = original_opt.pop_cli.cli or ref.split(".")[0]
 
     # Try to get a saved hub
     if original_opt.pop_cli.hub_state:
         hub_state = original_opt.pop_cli.hub_state
+
+        # Evaluate a reference the hub as the hub_state
         if hub_state.startswith('f"'):
+            safe_env = {"hub": cpop.data.NamespaceDict(lib=hub.lib)}
             hub_state = eval(hub_state, safe_env)
 
         hub_state_file = pathlib.Path(hub_state).expanduser()
-        new_hub = load_hub_state(hub, hub_state_file)
+        await load_hub_state(hub, hub_state_file, cli)
     else:
         hub_state_file = None
-        new_hub = None
-
-    # Successfully loaded a hub from a file
-    if new_hub is not None:
-        hub = new_hub
 
     args = []
     kwargs = {}
 
     # Override hub.OPT with the the new cli
     cli = original_opt.pop_cli.cli or ref.split(".")[0]
     if cli:
         # Pass all remaining args onto the new parser
 
-        hub._opt = hub._sync.pop.config.load(
+        hub._opt = await hub.pop.config.load(
             cli=cli, parser_args=tuple(original_opt.pop_cli.args)
         )
     else:
         # We are using the pop cli, treat all the extra args as parameters for the called function
         PLACEHOLDER = object()
         hold = PLACEHOLDER
         for arg in original_opt.pop_cli.args:
@@ -108,17 +128,15 @@
     # Call the named reference on the hub
     # This allows you to do
     # $ pop idem.init.cli
     # This way you can have multiple entrypoints, or even alias the above command to "idem"
     if asyncio.iscoroutinefunction(finder) or isinstance(
         finder, (Callable, cpop.contract.Contracted)
     ):
-        ret = finder(*args, **kwargs)
-        while asyncio.iscoroutine(ret):
-            ret = hub._synchronize(ret)
+        ret = await finder(*args, **kwargs)
     else:
         ret = finder
 
     # TODO handle generator ret
 
     try:
         pprint(ret.__dict__)
```

### Comparing `cpop-29.0.0/pop/config.yaml` & `cpop-29.1.0/src/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/pop/dirs.py` & `cpop-29.1.0/src/pop/dirs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Find directories
 """
+
 import importlib.resources
 import os
 import pathlib
 import sys
 from collections import defaultdict
 from collections.abc import Iterable
 from typing import Any
 
-import yaml
-
 import cpop.data
+import yaml
 
 
 def dir_list(pypath: list[str] = None, static: list[str] = None) -> list[pathlib.Path]:
     """
     Return the directories to look for modules in, pypath specifies files
     relative to an installed python package, static is for static dirs
     :param pypath: One or many python paths which will be imported
@@ -65,15 +65,15 @@
             if sub.endswith(".egg-link"):
                 with open(full) as rfh:
                     dirs.add(pathlib.Path(rfh.read().strip()))
             elif full.is_dir():
                 dirs.add(full)
 
     # Set up the _dynamic return
-    ret =cpop.data.NamespaceDict(
+    ret = cpop.data.NamespaceDict(
         dyne=cpop.data.NamespaceDict(),
         config=cpop.data.NamespaceDict(),
         imports=cpop.data.NamespaceDict(),
     )
 
     # Iterate over namespaces in sys.path
     for dir_ in dirs:
@@ -81,33 +81,33 @@
         try:
             if not config_file.is_file():
                 continue
         except:
             continue
         dynes, configs, imports = parse_config(config_file)
         if dynes:
-           cpop.data.update(ret.dyne, dynes, merge_lists=True)
+            cpop.data.update(ret.dyne, dynes, merge_lists=True)
         if configs:
-           cpop.data.update(ret.config, configs, merge_lists=True)
+            cpop.data.update(ret.config, configs, merge_lists=True)
         if imports:
-           cpop.data.update(ret.imports, imports)
+            cpop.data.update(ret.imports, imports)
 
     return ret
 
 
 def parse_config(
     config_file: str,
 ) -> tuple[dict[str, object], dict[str, object], set[str]]:
-    dyne = defaultdict(lambda:cpop.data.NamespaceDict(paths=set()))
-    config =cpop.data.NamespaceDict(
+    dyne = defaultdict(lambda: cpop.data.NamespaceDict(paths=set()))
+    config = cpop.data.NamespaceDict(
         config=cpop.data.NamespaceDict(),
         cli_config=cpop.data.NamespaceDict(),
         subcommands=cpop.data.NamespaceDict(),
     )
-    imports =cpop.data.NamespaceDict()
+    imports = cpop.data.NamespaceDict()
 
     config_file = pathlib.Path(config_file)
     if not config_file.is_file():
         return dyne, config, imports
     with open(config_file) as f:
         pop_config = yaml.safe_load(f) or {}
 
@@ -121,15 +121,17 @@
     for section in ["config", "cli_config", "subcommands"]:
         section_data = pop_config.get(section)
         if not isinstance(section_data, dict):
             continue
         for namespace, data in section_data.items():
             if data is None:
                 continue
-            config[section].setdefault(namespace,cpop.data.NamespaceDict()).update(data)
+            config[section].setdefault(namespace, cpop.data.NamespaceDict()).update(
+                data
+            )
 
     # Handle python imports
     for imp in pop_config.get("import", []):
         base = imp.split(".", 1)[0]
         if base not in imports:
             imports[base] = importlib.import_module(base)
         if "." in imp:
```

### Comparing `cpop-29.0.0/pop/exc.py` & `cpop-29.1.0/src/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/pop/hub.py` & `cpop-29.1.0/src/pop/hub.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-import asyncio
 import importlib.machinery
 import os
 import secrets
 import sys
-from collections.abc import Coroutine
 from collections.abc import Iterable
 from types import ModuleType
 from typing import Any
 
 import cpop.contract
 import cpop.data
 import pop.dirs
 import pop.exc
 import pop.loader
 import pop.ref
 import pop.scanner
 import pop.verify
 
+try:
+    pass
+
+    HAS_UVLOOP = True
+except ImportError:
+    HAS_UVLOOP = False
+
 
 def ex_path(path: str) -> list[str]:
     """
     Take a path that is sent to the Sub and expand it if it is a string or not
     """
     if isinstance(path, str):
         return path.split(",")
@@ -40,130 +45,85 @@
     def __setattr__(self, item: str, value):
         if item.startswith("_"):
             object.__setattr__(self, item, value)
         else:
             self._attrs[item] = value
 
 
-class SyncWrapper:
-    """
-    Enable synchronous calls to asynchronous hub references.
-    I.e.:
-
-        hub._sync.pop.sub.add(dyne_name="dyne")
-    """
-
-    def __init__(self, hub: "Hub", target=None):
-        self._hub = hub
-        self._target = target
-
-    def __getitem__(self, name: str):
-        try:
-            return getattr(self, name)
-        except AttributeError as e:
-            raise KeyError(e)
-
-    def __getattr__(self, name: str):
-        if self._target is None:
-            new_target = getattr(self._hub, name)
-        else:
-            new_target = getattr(self._target, name)
-        return SyncWrapper(self._hub, new_target)
-
-    async def __self(self):
-        return self
-
-    def __call__(self, *args, **kwargs):
-        if not self._target:
-            return self.__self
-
-        if isinstance(self._target, cpop.contract.Contracted):
-            coroutine = self._target(*args, **kwargs)
-            return self._hub._synchronize(coroutine)
-        else:
-            raise TypeError(f"{self._target} is not a coroutine function")
-
-
 class Hub(PopMeta):
     """
     The redistributed pop central hub. All components of the system are
     rooted to the Hub.
     """
 
-    def __init__(self, loop: asyncio.AbstractEventLoop = None, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         subs = {}
         sub_alias = {}
         imports = {}
         PopMeta.__init__(self, [subs, sub_alias, imports])
+        self._tasks = []
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._dynamic = None
         self._dscan = False
         # Set up the conf OPT structure so it is always available
         self._opt = None
 
-        # Initialize the loop
-        if loop is None:
-            self._loop = asyncio.new_event_loop()
-        else:
-            self._loop = loop
-
-        asyncio.set_event_loop(self._loop)
-        self._loop.run_until_complete(self.__ainit__(*args, **kwargs))
-
     async def __ainit__(
         self,
         load_all_dynes: bool = True,
         load_all_subdirs: bool = True,
         recurse_subdirs: bool = True,
         pop_mods: list[str] = None,
         cli: str = None,
         logs: bool = True,
+        load_config: bool = True,
     ):
         self._init_kwargs = {
             k: v for k, v in locals().items() if k != "self" and not k.startswith("_")
         }
 
         # Add the dyne for python imports to live in to the hub
-        self._subs["lib"] = await AsyncSub(
-            self, subname="lib", dyne_name="lib", pypath=pop_mods
-        )
-        # Load all existing libraries onto hub.lib
-        self._subs["lib"]._imports.update(
-            {
-                base: mod
-                for base, mod in sys.modules.items()
-                if not base.startswith("_") and "." not in base
-            }
-        )
-
-        if pop_mods is None:
-            pop_mods = ["pop.mods"]
-
-        # Add the pop sub to the hub, this should always use pypath and
-        # Should never be made dynamic. This is a core system sub and should
-        # NOT be app-merged
-        self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
-        await self._subs["pop"]._load_all()
+        if "lib" not in self._subs:
+            self._subs["lib"] = await AsyncSub(
+                self, subname="lib", dyne_name="lib", pypath=pop_mods
+            )
+            # Load all existing libraries onto hub.lib
+            self._subs["lib"]._imports.update(
+                {
+                    base: mod
+                    for base, mod in sys.modules.items()
+                    if not base.startswith("_") and "." not in base
+                }
+            )
 
-        self._sync = SyncWrapper(self)
+        if "pop" not in self._subs:
+            if pop_mods is None:
+                pop_mods = ["pop.mods"]
+
+            # Add the pop sub to the hub, this should always use pypath and
+            # Should never be made dynamic. This is a core system sub and should
+            # NOT be app-merged
+            self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
+            await self._subs["pop"]._load_all()
 
         self._load_all_dynes = load_all_dynes
         self._load_all_subdirs = load_all_subdirs
         self._recurse_subdirs = recurse_subdirs
         if self._load_all_dynes:
             self._scan_dynamic()
             await self._load_all()
 
-            # Overwrite opt with config data
-            self._opt = await self.pop.config.load(cli=cli, **self._dynamic.config)
+            if load_config:
+                # Overwrite opt with config data
+                self._opt = await self.pop.config.load(cli=cli, **self._dynamic.config)
 
         # Set up a logger
-        if logs:
+        if load_config and "log" in self._subs and logs:
             await self.log[self._opt.log.log_plugin].setup(self._opt.log.copy())
 
     @property
     def OPT(self):
         return self._opt
 
     async def _load_all(self):
@@ -177,22 +137,14 @@
             await self.pop.sub.add(dyne_name=dyne)
             if not self._load_all_subdirs:
                 continue
             await self.pop.sub.load_subdirs(
                 self._subs[dyne], recurse=self._recurse_subdirs
             )
 
-    def _synchronize(self, coroutine: Coroutine):
-        """
-        Synchronous function to wait for a coroutine
-        """
-        while asyncio.iscoroutine(coroutine):
-            coroutine = self._loop.run_until_complete(coroutine)
-        return coroutine
-
     def __getstate__(self) -> dict:
         attrs = {}
         for k, v in self._attrs.items():
             if isinstance(v, pop.loader.BASE_TYPES):
                 attrs[k] = v
             elif isinstance(v, dict):
                 if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v.values()):
@@ -217,15 +169,18 @@
         for subname, modname in state["imports"].items():
             try:
                 self._imports[subname] = importlib.import_module(modname)
             except ModuleNotFoundError:
                 ...
         self._attrs.update(state["attrs"])
         self._sub_alias.update(aliases)
-        self._opt =cpop.data.freeze(opt)
+        self._opt = cpop.data.freeze(opt)
+
+        # Schedule the hub's async init function to run later
+        self._tasks.append(self.__ainit__())
         for name, data in subs.items():
             if name in self._subs:
                 sub = self._subs[name]
             else:
                 sub = Sub(hub=self, root=self, **data["init_kwargs"])
                 self._subs[name] = sub
 
@@ -345,15 +300,15 @@
         self._omit_class = omit_class
         self._omit_vars = omit_vars
         self._mod_basename = mod_basename
         self._stop_on_failures = stop_on_failures
         self._is_contract = is_contract
         self._process_init = init
 
-    async def __ainit__(self):
+    async def __ainit__(self, *args, **kwargs):
         await self._prepare()
 
     async def _prepare(self):
         self._dirs = pop.dirs.dir_list(
             self._pypath,
             self._static,
         )
@@ -479,17 +434,17 @@
                 ...
 
         for name, data in subs.items():
             sub = Sub(hub=self._hub, root=self, **data["init_kwargs"])
             sub.__setstate__(data)
             self._subs[name] = sub
 
-        # Initialize the Sub
-        self._hub._synchronize(self.__ainit__())
-        self._hub._synchronize(self._load_all())
+        # Initialize the Sub, put these functions on the hub to be gathered
+        self._hub._tasks.append(self.__ainit__())
+        self._hub._tasks.append(self._load_all())
 
         # Make sure all unique items make it back onto the loaded mod
         for item, data in loaded.items():
             try:
                 self._loaded[item].__setstate__(data["state"])
             except KeyError:
                 ...
@@ -655,12 +610,13 @@
 
 class AsyncInitWrapper:
     def __init__(self, cls):
         self.cls = cls
 
     async def __call__(self, *args, **kwargs):
         instance = self.cls(*args, **kwargs)
-        await instance.__ainit__()
+        await instance.__ainit__(*args, **kwargs)
         return instance
 
 
+AsyncHub = AsyncInitWrapper(Hub)
 AsyncSub = AsyncInitWrapper(Sub)
```

### Comparing `cpop-29.0.0/pop/loader.py` & `cpop-29.1.0/src/pop/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Load the files detected from the scanner
 """
+
 import asyncio
 import importlib.machinery
 import importlib.util
 import inspect
 import os
 import sys
 import types
@@ -303,15 +304,15 @@
     """
 
     def __init__(self, name: str):
         super().__init__(name)
         vars = {}
         funcs = {}
         classes = {}
-        self._attrs =cpop.data.MultidictCache([funcs, classes, vars])
+        self._attrs = cpop.data.MultidictCache([funcs, classes, vars])
         self._vars = vars
         self._funcs = funcs
         self._classes = classes
 
     def __getattr__(self, item: str):
         if item.startswith("_"):
             return self.__getattribute__(item)
```

### Comparing `cpop-29.0.0/pop/ref.py` & `cpop-29.1.0/src/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/pop/scanner.py` & `cpop-29.1.0/src/pop/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Used to scan the given directories for loadable files
 """
+
 import collections
 import os
 from collections.abc import Iterable
 from typing import Any
 
 PY_END = (".py", ".pyc", ".pyo")
```

### Comparing `cpop-29.0.0/pop/verify.py` & `cpop-29.1.0/src/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/pop/log/async.py` & `cpop-29.1.0/src/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/pop/mods/config.py` & `cpop-29.1.0/src/pop/mods/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     pop_config = config.get("pop", {}).get("config")
     config_file = (
         cli_opts.get("config")
         or hub.lib.os.environ.get("POP_CONFIG", pop_config.get("os"))
         or pop_config.get("default")
     )
     if config_file and hub.lib.os.path.exists(config_file):
-        with open(config_file) as fh:
-            config_data = hub.lib.yaml.safe_load(fh)
+        async with hub.lib.aiofiles.open(config_file, "r") as fh:
+            config_data = hub.lib.yaml.safe_load(await fh.read())
     else:
         config_data = {}
 
     OPT = await hub.pop.config.prioritize(
         cli=cli,
         cli_opts=cli_opts,
         config=config,
@@ -170,15 +170,15 @@
 async def prioritize(
     hub,
     cli: str,
     cli_opts: dict[str, any],
     config: dict[str, any],
     config_file_data: dict[str, any],
     global_clis: list[str],
-) ->cpop.data.ImmutableNamespaceDict:
+) -> cpop.data.ImmutableNamespaceDict:
     """
     Prioritize configuration data from various sources.
 
     The order of priority is:
     1. CLI options (highest priority)
     2. Configuration file data
     3. OS environment variables
```

### Comparing `cpop-29.0.0/pop/mods/contract.py` & `cpop-29.1.0/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/pop/mods/sub.py` & `cpop-29.1.0/src/pop/mods/sub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Control and add subsystems to the running daemon hub
 """
+
 import pop.hub
 
 
 async def add(
     hub: "pop.hub.Hub",
     dyne_name: str = None,
     *,
```

### Comparing `cpop-29.0.0/pop/mods/test.py` & `cpop-29.1.0/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/.gitignore` & `cpop-29.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-29.0.0/README.rst` & `cpop-29.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,20 +31,24 @@
 Now all it takes to create a pluggable application is a few lines of code.
 This is the root of every pop project.
 We create a hub, we add dynamic subsystems, and then we call them through the hub's namespace.
 
 .. code-block:: python
 
     import pop.hub
+    import asyncio
 
-    # Create the hub, which initializes its own event loop
-    hub = pop.hub.Hub()
+    loop = asyncio.get_event_loop()
+    asyncio.run(main(loop))
 
-    # Run the main coroutine, which uses the hub's event loop
-    hub._sync.my_sub.init.cli()
+
+    async def main(loop):
+        hub = await pop.hub.AsyncHub(loop=loop)
+
+        await hub.my_sub.init.cli()
 
 
 You can also initialize pop from the cli:
 
 .. code-block:: bash
 
     python -m hub my_sub.init.cli
@@ -161,14 +165,15 @@
 .. code-block:: bash
 
     pytest tests
 
 
 Release
 =======
+The following steps are how to release a project with hatch
 
 .. code-block:: bash
 
     pip install .\[build\]
     hatch build
     export HATCH_INDEX_USER="__token__"
     export HATCH_INDEX_AUTH="pypi-api-token"
```

### Comparing `cpop-29.0.0/pyproject.toml` & `cpop-29.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "29.0.0"
+version = "29.1.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
@@ -21,53 +21,48 @@
 ]
 requires-python = ">=3.10"
 dependencies = [
     "aiofiles",
     "aiologger",
     "argparse",
     "PyYaml",
+    "uvloop; sys_platform != 'win32'",
 ]
 
 [project.optional-dependencies]
 test = [
-    "nest-asyncio",
     "pytest",
     "pytest-asyncio",
 ]
 build = [
     "Cython",
     "hatch-cython",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = [
-    "src/pop",
     "src/cpop",
-]
-
-[tool.hatch.build.targets.sdist]
-packages = [
     "src/pop",
-    "src/cpop",
+    "src/hub",
 ]
 
 [project.scripts]
-hub = "pop.__main__:main"
+hub = "hub.__main__:main"
 
 [tool.hatch.build.targets.wheel.hooks.cython.options]
 include_numpy = false
 include_pyarrow = false
 include_pythran = false
 
 directives = { boundscheck = false, nonecheck = false, language_level = 3, binding = true }
 
 
 [tool.black]
 line-length = 88
-target-version = ['py310', 'py311', 'py312']
+target-version = ['py310']
 include = '\.pyi?$'
 exclude = '''
 (
 /(
     \.eggs
     | \.git
     | \.hg
```

### Comparing `cpop-29.0.0/PKG-INFO` & `cpop-29.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 29.0.0
+Version: 29.1.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: aiofiles
 Requires-Dist: aiologger
 Requires-Dist: argparse
 Requires-Dist: pyyaml
+Requires-Dist: uvloop; sys_platform != 'win32'
 Provides-Extra: build
 Requires-Dist: cython; extra == 'build'
 Requires-Dist: hatch-cython; extra == 'build'
 Provides-Extra: test
-Requires-Dist: nest-asyncio; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Description-Content-Type: text/x-rst
 
 ====
 cPOP
 ====
@@ -56,20 +56,24 @@
 Now all it takes to create a pluggable application is a few lines of code.
 This is the root of every pop project.
 We create a hub, we add dynamic subsystems, and then we call them through the hub's namespace.
 
 .. code-block:: python
 
     import pop.hub
+    import asyncio
 
-    # Create the hub, which initializes its own event loop
-    hub = pop.hub.Hub()
+    loop = asyncio.get_event_loop()
+    asyncio.run(main(loop))
 
-    # Run the main coroutine, which uses the hub's event loop
-    hub._sync.my_sub.init.cli()
+
+    async def main(loop):
+        hub = await pop.hub.AsyncHub(loop=loop)
+
+        await hub.my_sub.init.cli()
 
 
 You can also initialize pop from the cli:
 
 .. code-block:: bash
 
     python -m hub my_sub.init.cli
@@ -186,14 +190,15 @@
 .. code-block:: bash
 
     pytest tests
 
 
 Release
 =======
+The following steps are how to release a project with hatch
 
 .. code-block:: bash
 
     pip install .\[build\]
     hatch build
     export HATCH_INDEX_USER="__token__"
     export HATCH_INDEX_AUTH="pypi-api-token"
```

