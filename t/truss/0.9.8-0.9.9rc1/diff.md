# Comparing `tmp/truss-0.9.8.tar.gz` & `tmp/truss-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.9.8.tar", max compression
+gzip compressed data, was "truss-0.9.9rc1.tar", max compression
```

## Comparing `truss-0.9.8.tar` & `truss-0.9.9rc1.tar`

### file list

```diff
@@ -1,231 +1,232 @@
--rw-r--r--   0        0        0     5483 2024-04-03 15:02:20.047835 truss-0.9.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1842 2024-04-03 15:02:20.047835 truss-0.9.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2024-04-03 15:02:20.047835 truss-0.9.8/LICENSE
--rw-r--r--   0        0        0     5107 2024-04-03 15:02:20.047835 truss-0.9.8/README.md
--rw-r--r--   0        0        0      933 2024-04-03 15:02:20.047835 truss-0.9.8/context_builder.Dockerfile
--rw-r--r--   0        0        0     2651 2024-04-03 15:02:20.055836 truss-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      255 2024-04-03 15:02:20.055836 truss-0.9.8/truss/__init__.py
--rw-r--r--   0        0        0      252 2024-04-03 15:02:20.059836 truss-0.9.8/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2024-04-03 15:02:20.059836 truss-0.9.8/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2024-04-03 15:02:20.059836 truss-0.9.8/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0     4518 2024-04-03 15:02:20.059836 truss-0.9.8/truss/build.py
--rw-r--r--   0        0        0       51 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/__init__.py
--rw-r--r--   0        0        0    17836 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/cli.py
--rw-r--r--   0        0        0      115 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/console.py
--rw-r--r--   0        0        0      134 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/create.py
--rw-r--r--   0        0        0     3096 2024-04-03 15:02:20.059836 truss-0.9.8/truss/config/trt_llm.py
--rw-r--r--   0        0        0     3259 2024-04-03 15:02:20.059836 truss-0.9.8/truss/constants.py
--rw-r--r--   0        0        0     7425 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/cache_warmer.py
--rw-r--r--   0        0        0     1456 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0    18184 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     1561 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2120 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     5711 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2024-04-03 15:02:20.059836 truss-0.9.8/truss/decorators.py
--rw-r--r--   0        0        0     3641 2024-04-03 15:02:20.059836 truss-0.9.8/truss/docker.py
--rw-r--r--   0        0        0      643 2024-04-03 15:02:20.059836 truss-0.9.8/truss/errors.py
--rw-r--r--   0        0        0      824 2024-04-03 15:02:20.059836 truss-0.9.8/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2024-04-03 15:02:20.059836 truss-0.9.8/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     3934 2024-04-03 15:02:20.059836 truss-0.9.8/truss/model_inference.py
--rw-r--r--   0        0        0      510 2024-04-03 15:02:20.059836 truss-0.9.8/truss/notebook.py
--rw-r--r--   0        0        0    15195 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      139 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/constants.py
--rw-r--r--   0        0        0      908 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2110 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/hash.py
--rw-r--r--   0        0        0     2930 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/local_truss_patch_applier.py
--rw-r--r--   0        0        0      570 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/signature.py
--rw-r--r--   0        0        0     3410 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      960 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/types.py
--rw-r--r--   0        0        0      237 2024-04-03 15:02:20.059836 truss-0.9.8/truss/pytest.ini
--rw-r--r--   0        0        0      705 2024-04-03 15:02:20.059836 truss-0.9.8/truss/readme_generator.py
--rw-r--r--   0        0        0      176 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/__init__.py
--rw-r--r--   0        0        0     7198 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/api.py
--rw-r--r--   0        0        0      752 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/auth.py
--rw-r--r--   0        0        0     6952 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/core.py
--rw-r--r--   0        0        0      541 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/error.py
--rw-r--r--   0        0        0    11775 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/remote.py
--rw-r--r--   0        0        0     2665 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/service.py
--rw-r--r--   0        0        0     1951 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/utils/tar.py
--rw-r--r--   0        0        0      985 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/utils/transfer.py
--rw-r--r--   0        0        0     1854 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/remote_cli.py
--rw-r--r--   0        0        0     4219 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/remote_factory.py
--rw-r--r--   0        0        0     7474 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/truss_remote.py
--rw-r--r--   0        0        0     2482 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/__init__.py
--rw-r--r--   0        0        0     2275 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     1026 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/cache.Dockerfile.jinja
--rw-r--r--   0        0        0       87 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/cache_requirements.txt
--rw-r--r--   0        0        0     3819 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     5397 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     6317 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     4245 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2652 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0      998 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1842 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     7419 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     5930 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     2354 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      158 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       98 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/copy_cache_files.Dockerfile.jinja
--rw-r--r--   0        0        0       48 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2561 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     2382 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     5758 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/schema.py
--rw-r--r--   0        0        0     2340 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/termination_handler_middleware.py
--rw-r--r--   0        0        0    14186 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      727 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0    15698 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      263 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     3196 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1352 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/logging.py
--rw-r--r--   0        0        0     2163 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0     3318 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/serialization.py
--rw-r--r--   0        0        0     2396 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/util.py
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/README.md
--rw-r--r--   0        0        0     4779 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/model/model.py
--rw-r--r--   0        0        0      860 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/build_engine_utils.py
--rw-r--r--   0        0        0      387 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/constants.py
--rw-r--r--   0        0        0     5775 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/schema.py
--rw-r--r--   0        0        0     5498 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt
--rw-r--r--   0        0        0     9023 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py
--rw-r--r--   0        0        0     2034 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt
--rw-r--r--   0        0        0    10875 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py
--rw-r--r--   0        0        0     2737 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt
--rw-r--r--   0        0        0     4457 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt
--rw-r--r--   0        0        0     4797 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/triton_client.py
--rw-r--r--   0        0        0     1729 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/utils.py
--rw-r--r--   0        0        0      147 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/annotated_types_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/annotated_types_truss/model/__init__.py
--rw-r--r--   0        0        0      274 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/annotated_types_truss/model/model.py
--rw-r--r--   0        0        0    30286 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0      234 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/gcs_fix/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/gcs_fix/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/gcs_fix/model/model.py
--rw-r--r--   0        0        0     1394 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0       51 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1566 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0       57 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0       44 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_async_truss/config.yaml
--rw-r--r--   0        0        0      646 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_async_truss/model/model.py
--rw-r--r--   0        0        0      238 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_basic_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_basic_truss/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_basic_truss/model/model.py
--rw-r--r--   0        0        0       34 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_concurrency_truss/config.yaml
--rw-r--r--   0        0        0      547 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_concurrency_truss/model/model.py
--rw-r--r--   0        0        0      270 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/model/__init__.py
--rw-r--r--   0        0        0      850 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/model/model.py
--rw-r--r--   0        0        0       13 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/requirements.txt
--rw-r--r--   0        0        0      270 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/model/__init__.py
--rw-r--r--   0        0        0      903 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/model/model.py
--rw-r--r--   0        0        0       14 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/requirements.txt
--rw-r--r--   0        0        0      270 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/model/__init__.py
--rw-r--r--   0        0        0     1106 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/model/model.py
--rw-r--r--   0        0        0       13 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/requirements.txt
--rw-r--r--   0        0        0       64 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_async_generator_truss/config.yaml
--rw-r--r--   0        0        0      521 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_async_generator_truss/model/model.py
--rw-r--r--   0        0        0      206 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_read_timeout/config.yaml
--rw-r--r--   0        0        0      636 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_read_timeout/model/model.py
--rw-r--r--   0        0        0       49 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss/config.yaml
--rw-r--r--   0        0        0      606 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss/model/model.py
--rw-r--r--   0        0        0       59 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss_with_error/config.yaml
--rw-r--r--   0        0        0      673 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss_with_error/model/model.py
--rw-r--r--   0        0        0       38 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        6 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/packages/test_package/test.py
--rw-r--r--   0        0        0      352 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss_server_caching_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss_server_caching_truss/model/__init__.py
--rw-r--r--   0        0        0      448 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss_server_caching_truss/model/model.py
--rw-r--r--   0        0        0       67 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/user_package/__init__.py
--rw-r--r--   0        0        0      469 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/user_package/shared_processor.py
--rw-r--r--   0        0        0     2340 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/workflow.py
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/__init__.py
--rw-r--r--   0        0        0    17477 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/conftest.py
--rw-r--r--   0        0        0    10496 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      555 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/helpers.py
--rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0    19223 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0     1090 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      715 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     2604 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0     7658 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_api.py
--rw-r--r--   0        0        0      580 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_auth.py
--rw-r--r--   0        0        0     2589 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_core.py
--rw-r--r--   0        0        0     8243 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_remote.py
--rw-r--r--   0        0        0     4626 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/test_remote_factory.py
--rw-r--r--   0        0        0     2475 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/test_truss_remote.py
--rw-r--r--   0        0        0      283 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     6060 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     7513 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0     8326 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/test_server_integration.py
--rw-r--r--   0        0        0     1560 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/core/server/common/test_truss_server.py
--rw-r--r--   0        0        0      821 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2605 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/common/test_termination_handler_middleware.py
--rw-r--r--   0        0        0     3131 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     7941 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/test_schema.py
--rw-r--r--   0        0        0     1952 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_build.py
--rw-r--r--   0        0        0     9997 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0    15051 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_control_truss_patching.py
--rw-r--r--   0        0        0      517 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_docker.py
--rw-r--r--   0        0        0    29185 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0    13995 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_model_schema.py
--rw-r--r--   0        0        0     1483 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    28421 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0     1358 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_util.py
--rw-r--r--   0        0        0     1865 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_validation.py
--rw-r--r--   0        0        0     1748 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_workflows.py
--rw-r--r--   0        0        0     7480 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/util/test_path.py
--rw-r--r--   0        0        0    23145 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_config.py
--rw-r--r--   0        0        0     2843 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_gatherer.py
--rw-r--r--   0        0        0    37089 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_handle.py
--rw-r--r--   0        0        0     5568 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_spec.py
--rw-r--r--   0        0        0     2729 2024-04-03 15:02:20.063835 truss-0.9.8/truss/types.py
--rw-r--r--   0        0        0     3110 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/.truss_ignore
--rw-r--r--   0        0        0      379 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/data_structures.py
--rw-r--r--   0        0        0     2566 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/download.py
--rw-r--r--   0        0        0      553 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/jinja.py
--rw-r--r--   0        0        0     6183 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/path.py
--rw-r--r--   0        0        0     2868 2024-04-03 15:02:20.063835 truss-0.9.8/truss/validation.py
--rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 truss-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     5483 2024-04-03 21:50:07.351823 truss-0.9.9rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1842 2024-04-03 21:50:07.351823 truss-0.9.9rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2024-04-03 21:50:07.351823 truss-0.9.9rc1/LICENSE
+-rw-r--r--   0        0        0     5107 2024-04-03 21:50:07.351823 truss-0.9.9rc1/README.md
+-rw-r--r--   0        0        0      933 2024-04-03 21:50:07.351823 truss-0.9.9rc1/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2654 2024-04-04 22:25:14.462578 truss-0.9.9rc1/pyproject.toml
+-rw-r--r--   0        0        0      255 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/__init__.py
+-rw-r--r--   0        0        0      252 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0     4518 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/build.py
+-rw-r--r--   0        0        0       51 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/cli/__init__.py
+-rw-r--r--   0        0        0    19659 2024-04-04 23:11:00.558686 truss-0.9.9rc1/truss/cli/cli.py
+-rw-r--r--   0        0        0      115 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/cli/console.py
+-rw-r--r--   0        0        0      134 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/cli/create.py
+-rw-r--r--   0        0        0     3096 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/config/trt_llm.py
+-rw-r--r--   0        0        0     3259 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/constants.py
+-rw-r--r--   0        0        0     7425 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/image_builder/cache_warmer.py
+-rw-r--r--   0        0        0     1456 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0    18184 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     1561 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2120 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     5711 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/docker.py
+-rw-r--r--   0        0        0      643 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/errors.py
+-rw-r--r--   0        0        0      824 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     3934 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/notebook.py
+-rw-r--r--   0        0        0    15195 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      139 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/constants.py
+-rw-r--r--   0        0        0      908 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2110 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/hash.py
+-rw-r--r--   0        0        0     2930 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      570 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/signature.py
+-rw-r--r--   0        0        0     3410 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      960 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/readme_generator.py
+-rw-r--r--   0        0        0      176 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/remote/baseten/__init__.py
+-rw-r--r--   0        0        0     7767 2024-04-04 23:08:23.538679 truss-0.9.9rc1/truss/remote/baseten/api.py
+-rw-r--r--   0        0        0      752 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/remote/baseten/auth.py
+-rw-r--r--   0        0        0     7055 2024-04-04 22:16:40.358558 truss-0.9.9rc1/truss/remote/baseten/core.py
+-rw-r--r--   0        0        0      541 2024-04-03 21:50:07.371823 truss-0.9.9rc1/truss/remote/baseten/error.py
+-rw-r--r--   0        0        0    12334 2024-04-04 23:12:20.578689 truss-0.9.9rc1/truss/remote/baseten/remote.py
+-rw-r--r--   0        0        0     3462 2024-04-04 23:11:06.938686 truss-0.9.9rc1/truss/remote/baseten/service.py
+-rw-r--r--   0        0        0     1951 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/remote/baseten/utils/tar.py
+-rw-r--r--   0        0        0      985 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/remote/baseten/utils/transfer.py
+-rw-r--r--   0        0        0     1854 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/remote/remote_cli.py
+-rw-r--r--   0        0        0     4219 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/remote/remote_factory.py
+-rw-r--r--   0        0        0     7608 2024-04-04 23:10:42.998685 truss-0.9.9rc1/truss/remote/truss_remote.py
+-rw-r--r--   0        0        0     2482 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/__init__.py
+-rw-r--r--   0        0        0     2275 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     1026 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/cache.Dockerfile.jinja
+-rw-r--r--   0        0        0       87 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/cache_requirements.txt
+-rw-r--r--   0        0        0     3819 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     5397 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     6317 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     4245 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2652 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0      998 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1842 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     7419 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     5930 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     2354 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      158 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       98 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/copy_cache_files.Dockerfile.jinja
+-rw-r--r--   0        0        0       48 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2561 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     5758 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/schema.py
+-rw-r--r--   0        0        0     2340 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/termination_handler_middleware.py
+-rw-r--r--   0        0        0    14186 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0    16228 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      263 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     3196 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2024-04-03 21:50:07.375823 truss-0.9.9rc1/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     2163 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     2396 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/shared/util.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/README.md
+-rw-r--r--   0        0        0     4779 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/model/model.py
+-rw-r--r--   0        0        0      860 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/build_engine_utils.py
+-rw-r--r--   0        0        0      387 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/constants.py
+-rw-r--r--   0        0        0     5775 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/schema.py
+-rw-r--r--   0        0        0     5498 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt
+-rw-r--r--   0        0        0     9023 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py
+-rw-r--r--   0        0        0     2034 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt
+-rw-r--r--   0        0        0    10875 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py
+-rw-r--r--   0        0        0     2737 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt
+-rw-r--r--   0        0        0     4457 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt
+-rw-r--r--   0        0        0     4797 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/triton_client.py
+-rw-r--r--   0        0        0     1729 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/templates/trtllm/packages/utils.py
+-rw-r--r--   0        0        0      147 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/annotated_types_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/annotated_types_truss/model/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/annotated_types_truss/model/model.py
+-rw-r--r--   0        0        0    30286 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0      234 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/gcs_fix/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/gcs_fix/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/gcs_fix/model/model.py
+-rw-r--r--   0        0        0     1394 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0       51 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1566 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0       57 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-03 21:50:07.379823 truss-0.9.9rc1/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0       44 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_async_truss/config.yaml
+-rw-r--r--   0        0        0      646 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_async_truss/model/model.py
+-rw-r--r--   0        0        0      238 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_basic_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_basic_truss/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_basic_truss/model/model.py
+-rw-r--r--   0        0        0       34 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_concurrency_truss/config.yaml
+-rw-r--r--   0        0        0      547 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_concurrency_truss/model/model.py
+-rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v1/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v1/model/__init__.py
+-rw-r--r--   0        0        0      850 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v1/model/model.py
+-rw-r--r--   0        0        0       13 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v1/requirements.txt
+-rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v2/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v2/model/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v2/model/model.py
+-rw-r--r--   0        0        0       14 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_pyantic_v2/requirements.txt
+-rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_requirements_file_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_requirements_file_truss/model/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_requirements_file_truss/model/model.py
+-rw-r--r--   0        0        0       13 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_requirements_file_truss/requirements.txt
+-rw-r--r--   0        0        0       64 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_async_generator_truss/config.yaml
+-rw-r--r--   0        0        0      521 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_async_generator_truss/model/model.py
+-rw-r--r--   0        0        0      206 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_read_timeout/config.yaml
+-rw-r--r--   0        0        0      636 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_read_timeout/model/model.py
+-rw-r--r--   0        0        0       49 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_truss/config.yaml
+-rw-r--r--   0        0        0      606 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_truss/model/model.py
+-rw-r--r--   0        0        0       59 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_truss_with_error/config.yaml
+-rw-r--r--   0        0        0      673 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_streaming_truss_with_error/model/model.py
+-rw-r--r--   0        0        0       38 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        6 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss/packages/test_package/test.py
+-rw-r--r--   0        0        0      352 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss_server_caching_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss_server_caching_truss/model/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/test_truss_server_caching_truss/model/model.py
+-rw-r--r--   0        0        0       67 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/workflow_text_to_num/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/workflow_text_to_num/user_package/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/workflow_text_to_num/user_package/shared_processor.py
+-rw-r--r--   0        0        0     2340 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/test_data/workflow_text_to_num/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/tests/__init__.py
+-rw-r--r--   0        0        0    17477 2024-04-03 21:50:07.383823 truss-0.9.9rc1/truss/tests/conftest.py
+-rw-r--r--   0        0        0    10496 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      555 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0    19223 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0     1090 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      715 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     2604 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0     7658 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/remote/baseten/test_api.py
+-rw-r--r--   0        0        0      580 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/remote/baseten/test_auth.py
+-rw-r--r--   0        0        0     2589 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/remote/baseten/test_core.py
+-rw-r--r--   0        0        0     8243 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/remote/baseten/test_remote.py
+-rw-r--r--   0        0        0     4626 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/remote/test_remote_factory.py
+-rw-r--r--   0        0        0     2475 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/remote/test_truss_remote.py
+-rw-r--r--   0        0        0      283 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     6060 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7513 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0     8326 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/control/control/test_server_integration.py
+-rw-r--r--   0        0        0     1560 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/core/server/common/test_truss_server.py
+-rw-r--r--   0        0        0      821 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2605 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/server/common/test_termination_handler_middleware.py
+-rw-r--r--   0        0        0     3131 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     7941 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/templates/server/test_schema.py
+-rw-r--r--   0        0        0     1952 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_build.py
+-rw-r--r--   0        0        0     9997 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    15051 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_docker.py
+-rw-r--r--   0        0        0    30398 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0    13995 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_model_schema.py
+-rw-r--r--   0        0        0     1483 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2024-04-03 21:50:07.387823 truss-0.9.9rc1/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    28421 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0     1358 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/tests/test_util.py
+-rw-r--r--   0        0        0     1865 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     1888 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/tests/test_workflows.py
+-rw-r--r--   0        0        0     7480 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/tests/util/test_path.py
+-rw-r--r--   0        0        0    23145 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/truss_config.py
+-rw-r--r--   0        0        0     2843 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    37089 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/truss_handle.py
+-rw-r--r--   0        0        0     5568 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/truss_spec.py
+-rw-r--r--   0        0        0     2729 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/types.py
+-rw-r--r--   0        0        0     3110 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/util/.truss_ignore
+-rw-r--r--   0        0        0      379 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/util/data_structures.py
+-rw-r--r--   0        0        0     2566 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/util/download.py
+-rw-r--r--   0        0        0       46 2024-04-04 23:08:16.722679 truss-0.9.9rc1/truss/util/errors.py
+-rw-r--r--   0        0        0      553 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/util/jinja.py
+-rw-r--r--   0        0        0     6183 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/util/path.py
+-rw-r--r--   0        0        0     2868 2024-04-03 21:50:07.391823 truss-0.9.9rc1/truss/validation.py
+-rw-r--r--   0        0        0     6990 1970-01-01 00:00:00.000000 truss-0.9.9rc1/PKG-INFO
```

### Comparing `truss-0.9.8/CODE_OF_CONDUCT.md` & `truss-0.9.9rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/CONTRIBUTING.md` & `truss-0.9.9rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/LICENSE` & `truss-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/README.md` & `truss-0.9.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/context_builder.Dockerfile` & `truss-0.9.9rc1/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/pyproject.toml` & `truss-0.9.9rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.9.8"
+version = "0.9.9rc1"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = [
```

### Comparing `truss-0.9.8/truss/blob/blob_backend_registry.py` & `truss-0.9.9rc1/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/blob/http_public_blob_backend.py` & `truss-0.9.9rc1/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/build.py` & `truss-0.9.9rc1/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/cli/cli.py` & `truss-0.9.9rc1/truss/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import inspect
 import json
 import logging
 import os
 import sys
+import time
 from functools import wraps
 from pathlib import Path
 from typing import Callable, Optional
 
 import rich
 import rich_click as click
 import truss
 from truss.cli.console import console
 from truss.cli.create import ask_name
 from truss.remote.baseten.core import (
+    ACTIVE_STATUS,
+    DEPLOYING_STATUSES,
     ModelId,
     ModelIdentifier,
     ModelName,
     ModelVersionId,
 )
 from truss.remote.baseten.service import BasetenService
 from truss.remote.remote_cli import inquire_model_name, inquire_remote_name
 from truss.remote.remote_factory import USER_TRUSSRC_PATH, RemoteFactory
 from truss.truss_config import Build, ModelServer
+from truss.util.errors import RemoteNetworkError
 
 logging.basicConfig(level=logging.INFO)
 
 
 click.rich_click.COMMAND_GROUPS = {
     "truss": [
         {
@@ -438,24 +442,41 @@
     type=str,
     required=False,
     help=(
         "Name of the deployment created by the push. Can only be "
         "used in combination with --publish or --promote."
     ),
 )
-@error_handling
+@click.option(
+    "--wait",
+    type=bool,
+    is_flag=True,
+    required=False,
+    default=False,
+    help="Wait for the deployment to complete before returning.",
+)
+@click.option(
+    "--timeout-seconds",
+    type=int,
+    required=False,
+    help="Maximum time to wait for deployment to complete in seconds. "
+    "Without specifying, the command will not complete until the deployment is complete.",
+)
+# @error_handling
 def push(
     target_directory: str,
     remote: str,
     model_name: str,
     publish: bool = False,
     trusted: bool = False,
     promote: bool = False,
     preserve_previous_production_deployment: bool = False,
     deployment_name: Optional[str] = None,
+    wait: bool = False,
+    timeout_seconds: Optional[int] = None,
 ) -> None:
     """
     Pushes a truss to a TrussRemote.
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
 
     """
@@ -487,15 +508,15 @@
     )  # type: ignore
 
     click.echo(f"✨ Model {model_name} was successfully pushed ✨")
 
     if service.is_draft:
         draft_model_text = """
 |---------------------------------------------------------------------------------------|
-| Your model has been deployed as a development model. Development models allow you to  |
+| Your model is deploying as a development model. Development models allow you to  |
 | iterate quickly during the deployment process.                                        |
 |                                                                                       |
 | When you are ready to publish your deployed model as a new deployment,                |
 | pass `--publish` to the `truss push` command. To monitor changes to your model and    |
 | rapidly iterate, run the `truss watch` command.                                       |
 |                                                                                       |
 |---------------------------------------------------------------------------------------|
@@ -514,14 +535,41 @@
     if promote:
         promotion_text = """Your Truss has been deployed as a production model. After it successfully deploys,
 it will become the next production deployment of your model."""
         console.print(promotion_text, style="green")
 
     logs_url = remote_provider.get_remote_logs_url(service)  # type: ignore[attr-defined]
     rich.print(f"🪵  View logs for your deployment at {logs_url}")
+    if wait:
+        start_time = time.time()
+        with console.status("[bold green]Deploying...") as status:
+            try:
+                # Poll for the deployment status until we have reached
+                # either ACTIVE, or a non-deploying status (in which case the deployment has failed).
+                for deployment_status in service.poll_deployment_status():
+                    if (
+                        timeout_seconds is not None
+                        and time.time() - start_time > timeout_seconds
+                    ):
+                        status.update("[bold red]Deployment timed out.")
+                        sys.exit(1)
+
+                    status.update(f"[bold green]{deployment_status}")
+
+                    if deployment_status == ACTIVE_STATUS:
+                        console.print("Deployment succeeded.", style="bold green")
+                        return
+
+                    if deployment_status not in DEPLOYING_STATUSES:
+                        console.print("Deployment succeeded.", style="bold green")
+                        sys.exit(1)
+
+            except RemoteNetworkError:
+                status.update("[bold red]Deployment failed -- could not reach remote.")
+                sys.exit(1)
 
 
 @truss_cli.command()
 def configure():
     # Read the original file content
     with open(USER_TRUSSRC_PATH, "r") as f:
         original_content = f.read()
```

### Comparing `truss-0.9.8/truss/config/trt_llm.py` & `truss-0.9.9rc1/truss/config/trt_llm.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/constants.py` & `truss-0.9.9rc1/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/image_builder/cache_warmer.py` & `truss-0.9.9rc1/truss/contexts/image_builder/cache_warmer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/image_builder/image_builder.py` & `truss-0.9.9rc1/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.9.9rc1/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/image_builder/util.py` & `truss-0.9.9rc1/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.9.9rc1/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/local_loader/load_model_local.py` & `truss-0.9.9rc1/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.9.9rc1/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/contexts/local_loader/utils.py` & `truss-0.9.9rc1/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/docker.py` & `truss-0.9.9rc1/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/errors.py` & `truss-0.9.9rc1/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/local/local_config.py` & `truss-0.9.9rc1/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/local/local_config_handler.py` & `truss-0.9.9rc1/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/model_inference.py` & `truss-0.9.9rc1/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/patch/calc_patch.py` & `truss-0.9.9rc1/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/patch/dir_signature.py` & `truss-0.9.9rc1/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/patch/hash.py` & `truss-0.9.9rc1/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/patch/local_truss_patch_applier.py` & `truss-0.9.9rc1/truss/patch/local_truss_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/patch/signature.py` & `truss-0.9.9rc1/truss/patch/signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/patch/truss_dir_patch_applier.py` & `truss-0.9.9rc1/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/patch/types.py` & `truss-0.9.9rc1/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/readme_generator.py` & `truss-0.9.9rc1/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/remote/baseten/api.py` & `truss-0.9.9rc1/truss/remote/baseten/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 
 
 class BasetenApi:
     """
     A client for the Baseten API.
 
     Args:
-        api_url: The URL of the Baseten API.
+        graphql_api_url: The URL of the Baseten GraphQL API.
+        rest_api_url: The URL of the Baseten REST API.
         auth_service: An AuthService instance.
     """
 
     class GraphQLErrorCodes(Enum):
         RESOURCE_NOT_FOUND = "RESOURCE_NOT_FOUND"
 
-    def __init__(self, api_url: str, auth_service: AuthService):
-        self._api_url = api_url
+    def __init__(
+        self, graphql_api_url: str, rest_api_url: str, auth_service: AuthService
+    ):
+        self._graphql_api_url = graphql_api_url
+        self._rest_api_url = rest_api_url
         self._auth_service = auth_service
         self._auth_token = self._auth_service.authenticate()
 
     def _post_graphql_query(self, query_string: str) -> dict:
         headers = self._auth_token.header()
         resp = requests.post(
-            self._api_url,
+            self._graphql_api_url,
             data={"query": query_string},
             headers=headers,
             timeout=120,
         )
 
         if not resp.ok:
             logger.error(f"GraphQL endpoint failed with error: {resp.content}")  # type: ignore
@@ -245,7 +249,19 @@
             needs_full_deploy
             error
         }}
         }}
         """
         resp = self._post_graphql_query(query_string)
         return resp["data"]["patch_draft_truss"]
+
+    def get_deployment(self, model_id: str, deployment_id: str) -> str:
+        headers = self._auth_token.header()
+        resp = requests.get(
+            f"{self._rest_api_url}/v1/models/{model_id}/deployments/{deployment_id}",
+            headers=headers,
+        )
+        if not resp.ok:
+            resp.raise_for_status()
+
+        deployment = resp.json()
+        return deployment
```

### Comparing `truss-0.9.8/truss/remote/baseten/auth.py` & `truss-0.9.9rc1/truss/remote/baseten/auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/remote/baseten/core.py` & `truss-0.9.9rc1/truss/remote/baseten/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from truss.remote.baseten.utils.transfer import multipart_upload_boto3
 from truss.truss_handle import TrussHandle
 from truss.util.path import load_trussignore_patterns
 
 logger = logging.getLogger(__name__)
 
 
+DEPLOYING_STATUSES = ["BUILDING", "DEPLOYING", "LOADING_MODEL", "UPDATING"]
+ACTIVE_STATUS = "ACTIVE"
+
+
 class ModelIdentifier:
     value: str
 
 
 class ModelName(ModelIdentifier):
     def __init__(self, name: str):
         self.value = name
```

### Comparing `truss-0.9.8/truss/remote/baseten/error.py` & `truss-0.9.9rc1/truss/remote/baseten/error.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/remote/baseten/remote.py` & `truss-0.9.9rc1/truss/remote/baseten/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,34 @@
 from truss.remote.baseten.utils.transfer import base64_encoded_json_str
 from truss.remote.truss_remote import TrussRemote, TrussService
 from truss.truss_config import ModelServer
 from truss.truss_handle import TrussHandle
 from truss.util.path import is_ignored, load_trussignore_patterns
 from watchfiles import watch
 
+API_URL_MAPPING = {
+    "https://app.baseten.co": "https://api.baseten.co",
+    "https://app.staging.baseten.co": "https://api.staging.baseten.co",
+    "https://app.dev.baseten.co": "https://api.staging.baseten.co",
+    # For local development, this is how we map URLs
+    "http://localhost:8000": "http://api.localhost:8000",
+}
+
 
 class BasetenRemote(TrussRemote):
     def __init__(self, remote_url: str, api_key: str, **kwargs):
         super().__init__(remote_url, **kwargs)
         self._auth_service = AuthService(api_key=api_key)
-        self._api = BasetenApi(f"{self._remote_url}/graphql/", self._auth_service)
+        self._api = BasetenApi(
+            f"{self._remote_url}/graphql/",
+            # Ensure we strip off trailing '/' to denormalize
+            # URLs.
+            API_URL_MAPPING[self._remote_url.strip("/")],
+            self._auth_service,
+        )
 
     def authenticate(self):
         return self._auth_service.validate()
 
     def push(  # type: ignore
         self,
         truss_handle: TrussHandle,
@@ -105,14 +119,15 @@
         return BasetenService(
             model_id=model_id,
             model_version_id=model_version_id,
             is_draft=not publish,
             api_key=self._auth_service.authenticate().value,
             service_url=f"{self._remote_url}/model_versions/{model_version_id}",
             truss_handle=truss_handle,
+            api=self._api,
         )
 
     @staticmethod
     def _get_matching_version(model_versions: List[dict], published: bool) -> dict:
         if not published:
             # Return the development model version.
             dev_version = get_dev_version_from_versions(model_versions)
@@ -188,14 +203,15 @@
 
         return BasetenService(
             model_id=model_id,
             model_version_id=model_version_id,
             is_draft=not published,
             api_key=self._auth_service.authenticate().value,
             service_url=f"{self._remote_url}{service_url_path}",
+            api=self._api,
         )
 
     def get_remote_logs_url(
         self,
         service: TrussService,
     ) -> str:
         return service.logs_url(self._remote_url)
```

### Comparing `truss-0.9.8/truss/remote/baseten/service.py` & `truss-0.9.9rc1/truss/remote/baseten/service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+import time
 from typing import Dict, Optional
 
+import requests
+from tenacity import retry, stop_after_delay, wait_fixed
+from truss.remote.baseten.api import BasetenApi
 from truss.remote.baseten.auth import AuthService
 from truss.remote.truss_remote import TrussService
 from truss.truss_handle import TrussHandle
+from truss.util.errors import RemoteNetworkError
 
 DEFAULT_STREAM_ENCODING = "utf-8"
 
 
 class BasetenService(TrussService):
     def __init__(
         self,
         model_id: str,
         model_version_id: str,
         is_draft: bool,
         api_key: str,
         service_url: str,
+        api: BasetenApi,
         truss_handle: Optional[TrussHandle] = None,
     ):
         super().__init__(is_draft=is_draft, service_url=service_url)
         self._model_id = model_id
         self._model_version_id = model_version_id
         self._auth_service = AuthService(api_key=api_key)
+        self._api = api
         self._truss_handle = truss_handle
 
     def is_live(self) -> bool:
         raise NotImplementedError
 
     def is_ready(self) -> bool:
         raise NotImplementedError
@@ -76,7 +83,23 @@
         return response.json()["model_output"]
 
     def authenticate(self) -> dict:
         return self._auth_service.authenticate().header()
 
     def logs_url(self, base_url: str) -> str:
         return f"{base_url}/models/{self._model_id}/logs/{self._model_version_id}"
+
+    @retry(stop=stop_after_delay(60), wait=wait_fixed(1))
+    def _fetch_deployment(self):
+        return self._api.get_deployment(self._model_id, self._model_version_id)
+
+    def poll_deployment_status(self):
+        """
+        Wait for the service to be deployed.
+        """
+        while True:
+            time.sleep(1)
+            try:
+                deployment = self._fetch_deployment()
+                yield deployment["status"]
+            except requests.exceptions.RequestException:
+                raise RemoteNetworkError("Could not reach backend.")
```

### Comparing `truss-0.9.8/truss/remote/baseten/utils/tar.py` & `truss-0.9.9rc1/truss/remote/baseten/utils/tar.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/remote/baseten/utils/transfer.py` & `truss-0.9.9rc1/truss/remote/baseten/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/remote/remote_cli.py` & `truss-0.9.9rc1/truss/remote/remote_cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/remote/remote_factory.py` & `truss-0.9.9rc1/truss/remote/remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/remote/truss_remote.py` & `truss-0.9.9rc1/truss/remote/truss_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,21 @@
     @abstractmethod
     def logs_url(self, base_url: str) -> str:
         """
         Get the URL for the service logs.
         """
         pass
 
+    @abstractmethod
+    def poll_deployment_status(self):
+        """
+        Poll for a deployment status.
+        """
+        pass
+
 
 class TrussRemote(ABC):
     """
     Define the abstract base class for a remote Truss service.
 
     A remote Truss service is a service that can push a TrussHandle to a remote location.
     The `push` and `authenticate` methods should be implemented in subclasses.
```

### Comparing `truss-0.9.8/truss/templates/README.md.jinja` & `truss-0.9.9rc1/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/base.Dockerfile.jinja` & `truss-0.9.9rc1/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/cache.Dockerfile.jinja` & `truss-0.9.9rc1/truss/templates/cache.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/application.py` & `truss-0.9.9rc1/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/endpoints.py` & `truss-0.9.9rc1/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/errors.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/helpers/types.py` & `truss-0.9.9rc1/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/control/control/server.py` & `truss-0.9.9rc1/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/custom/model/model.py` & `truss-0.9.9rc1/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/common/errors.py` & `truss-0.9.9rc1/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.9.9rc1/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/common/patches.py` & `truss-0.9.9rc1/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/common/retry.py` & `truss-0.9.9rc1/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/common/schema.py` & `truss-0.9.9rc1/truss/templates/server/common/schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/common/termination_handler_middleware.py` & `truss-0.9.9rc1/truss/templates/server/common/termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/common/truss_server.py` & `truss-0.9.9rc1/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/inference_server.py` & `truss-0.9.9rc1/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/server/model_wrapper.py` & `truss-0.9.9rc1/truss/templates/server/model_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,36 @@
 import time
 from collections.abc import Generator
 from contextlib import asynccontextmanager
 from enum import Enum
 from multiprocessing import Lock
 from pathlib import Path
 from threading import Thread
-from typing import Any, AsyncGenerator, Dict, Optional, Set, Union
+from typing import (
+    Any,
+    AsyncGenerator,
+    Callable,
+    Coroutine,
+    Dict,
+    NoReturn,
+    Optional,
+    Set,
+    TypeVar,
+    Union,
+)
 
 import pydantic
 from anyio import Semaphore, to_thread
 from common.patches import apply_patches
 from common.retry import retry
 from common.schema import TrussSchema
 from fastapi import HTTPException
 from pydantic import BaseModel
 from shared.secrets_resolver import SecretsResolver
+from typing_extensions import ParamSpec
 
 MODEL_BASENAME = "model"
 
 NUM_LOAD_RETRIES = int(os.environ.get("NUM_LOAD_RETRIES_TRUSS", "1"))
 STREAMING_RESPONSE_QUEUE_READ_TIMEOUT_SECS = 60
 DEFAULT_PREDICT_CONCURRENCY = 1
 
@@ -400,32 +412,42 @@
     return False
 
 
 def _elapsed_ms(since_micro_seconds: float) -> int:
     return int((time.perf_counter() - since_micro_seconds) * 1000)
 
 
-def _handle_exception():
+def _handle_exception(exception: Exception) -> NoReturn:
     # Note that logger.exception logs the stacktrace, such that the user can
     # debug this error from the logs.
-    logging.exception("Internal Server Error")
-    raise HTTPException(status_code=500, detail="Internal Server Error")
+    if isinstance(exception, HTTPException):
+        logging.exception("Model raised HTTPException")
+        raise exception
+    else:
+        logging.exception("Internal Server Error")
+        raise HTTPException(status_code=500, detail="Internal Server Error")
 
 
-def _intercept_exceptions_sync(func):
-    def inner(*args, **kwargs):
+_P = ParamSpec("_P")
+_R = TypeVar("_R")
+
+
+def _intercept_exceptions_sync(func: Callable[_P, _R]) -> Callable[_P, _R]:
+    def inner(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         try:
             return func(*args, **kwargs)
-        except Exception:
-            _handle_exception()
+        except Exception as e:
+            _handle_exception(e)
 
     return inner
 
 
-def _intercept_exceptions_async(func):
-    async def inner(*args, **kwargs):
+def _intercept_exceptions_async(
+    func: Callable[_P, Coroutine[Any, Any, _R]]
+) -> Callable[_P, Coroutine[Any, Any, _R]]:
+    async def inner(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         try:
             return await func(*args, **kwargs)
-        except Exception:
-            _handle_exception()
+        except Exception as e:
+            _handle_exception(e)
 
     return inner
```

### Comparing `truss-0.9.8/truss/templates/server.Dockerfile.jinja` & `truss-0.9.9rc1/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/shared/logging.py` & `truss-0.9.9rc1/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/shared/secrets_resolver.py` & `truss-0.9.9rc1/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/shared/serialization.py` & `truss-0.9.9rc1/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/shared/util.py` & `truss-0.9.9rc1/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/model/model.py` & `truss-0.9.9rc1/truss/templates/trtllm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/build_engine_utils.py` & `truss-0.9.9rc1/truss/templates/trtllm/packages/build_engine_utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/schema.py` & `truss-0.9.9rc1/truss/templates/trtllm/packages/schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt` & `truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py` & `truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt` & `truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py` & `truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt` & `truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt` & `truss-0.9.9rc1/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/triton_client.py` & `truss-0.9.9rc1/truss/templates/trtllm/packages/triton_client.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/templates/trtllm/packages/utils.py` & `truss-0.9.9rc1/truss/templates/trtllm/packages/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/auto-mpg.data` & `truss-0.9.9rc1/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/gcs_fix/model/model.py` & `truss-0.9.9rc1/truss/test_data/gcs_fix/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/happy.ipynb` & `truss-0.9.9rc1/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.9.9rc1/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/patch_ping_test_server/app.py` & `truss-0.9.9rc1/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/pima-indians-diabetes.csv` & `truss-0.9.9rc1/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/readme_int_example.md` & `truss-0.9.9rc1/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/readme_no_example.md` & `truss-0.9.9rc1/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/readme_str_example.md` & `truss-0.9.9rc1/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/server.Dockerfile` & `truss-0.9.9rc1/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_async_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_async_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_basic_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_basic_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_concurrency_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_concurrency_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_pyantic_v1/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_pyantic_v1/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_pyantic_v2/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_pyantic_v2/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_requirements_file_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_requirements_file_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_streaming_async_generator_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_streaming_async_generator_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_streaming_read_timeout/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_streaming_read_timeout/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_streaming_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_streaming_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_streaming_truss_with_error/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_streaming_truss_with_error/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/test_truss/model/model.py` & `truss-0.9.9rc1/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/test_data/workflow_text_to_num/workflow.py` & `truss-0.9.9rc1/truss/test_data/workflow_text_to_num/workflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/conftest.py` & `truss-0.9.9rc1/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.9.9rc1/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.9.9rc1/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.9.9rc1/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/helpers.py` & `truss-0.9.9rc1/truss/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/local/test_local_config_handler.py` & `truss-0.9.9rc1/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/patch/test_calc_patch.py` & `truss-0.9.9rc1/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/patch/test_dir_signature.py` & `truss-0.9.9rc1/truss/tests/patch/test_dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/patch/test_hash.py` & `truss-0.9.9rc1/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/patch/test_signature.py` & `truss-0.9.9rc1/truss/tests/patch/test_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.9.9rc1/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/remote/baseten/test_api.py` & `truss-0.9.9rc1/truss/tests/remote/baseten/test_api.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/remote/baseten/test_auth.py` & `truss-0.9.9rc1/truss/tests/remote/baseten/test_auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/remote/baseten/test_core.py` & `truss-0.9.9rc1/truss/tests/remote/baseten/test_core.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/remote/baseten/test_remote.py` & `truss-0.9.9rc1/truss/tests/remote/baseten/test_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/remote/test_remote_factory.py` & `truss-0.9.9rc1/truss/tests/remote/test_remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/remote/test_truss_remote.py` & `truss-0.9.9rc1/truss/tests/remote/test_truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.9.9rc1/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.9.9rc1/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/control/control/test_server.py` & `truss-0.9.9rc1/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/control/control/test_server_integration.py` & `truss-0.9.9rc1/truss/tests/templates/control/control/test_server_integration.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/core/server/common/test_truss_server.py` & `truss-0.9.9rc1/truss/tests/templates/core/server/common/test_truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/core/server/common/test_util.py` & `truss-0.9.9rc1/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.9.9rc1/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/server/common/test_retry.py` & `truss-0.9.9rc1/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/server/common/test_termination_handler_middleware.py` & `truss-0.9.9rc1/truss/tests/templates/server/common/test_termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.9.9rc1/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/templates/server/test_schema.py` & `truss-0.9.9rc1/truss/tests/templates/server/test_schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_build.py` & `truss-0.9.9rc1/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_config.py` & `truss-0.9.9rc1/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_context_builder_image.py` & `truss-0.9.9rc1/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_control_truss_patching.py` & `truss-0.9.9rc1/truss/tests/test_control_truss_patching.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_docker.py` & `truss-0.9.9rc1/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_model_inference.py` & `truss-0.9.9rc1/truss/tests/test_model_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,14 +724,52 @@
 
         assert_logs_contain_error(container.logs(), "ValueError: error")
 
         assert "Internal Server Error" in response.json()["error"]
 
 
 @pytest.mark.integration
+def test_truss_with_user_errors():
+    """Test that user-code raised `fastapi.HTTPExceptions` are passed through as is."""
+    model = """
+    import fastapi
+
+    class Model:
+        def predict(self, request):
+            raise fastapi.HTTPException(status_code=500, detail="My custom message.")
+    """
+
+    config = "model_name: error-truss"
+
+    with ensure_kill_all(), tempfile.TemporaryDirectory(dir=".") as tmp_work_dir:
+        truss_dir = Path(tmp_work_dir, "truss")
+
+        create_truss(truss_dir, config, textwrap.dedent(model))
+
+        tr = TrussHandle(truss_dir)
+        container = tr.docker_run(
+            local_port=8090, detach=True, wait_for_server_ready=True
+        )
+        truss_server_addr = "http://localhost:8090"
+        full_url = f"{truss_server_addr}/v1/models/model:predict"
+
+        response = requests.post(full_url, json={})
+        assert response.status_code == 500
+        assert "error" in response.json()
+
+        assert_logs_contain_error(
+            container.logs(),
+            "HTTPException: 500: My custom message.",
+            "Model raised HTTPException",
+        )
+
+        assert "My custom message." in response.json()["error"]
+
+
+@pytest.mark.integration
 def test_slow_truss():
     with ensure_kill_all():
         truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
         truss_dir = truss_root / "test_data" / "server_conformance_test_truss"
         tr = TrussHandle(truss_dir)
 
         _ = tr.docker_run(local_port=8090, detach=True, wait_for_server_ready=False)
```

### Comparing `truss-0.9.8/truss/tests/test_model_schema.py` & `truss-0.9.9rc1/truss/tests/test_model_schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.9.9rc1/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_truss_gatherer.py` & `truss-0.9.9rc1/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_truss_handle.py` & `truss-0.9.9rc1/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_util.py` & `truss-0.9.9rc1/truss/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_validation.py` & `truss-0.9.9rc1/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/tests/test_workflows.py` & `truss-0.9.9rc1/truss/tests/test_workflows.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,12 +47,15 @@
         response = requests.post(
             predict_url, json={"length": 30, "num_partitions": 3}, stream=True
         )
         print(response.content)
         assert response.status_code == 200
         assert response.json() == [6280, "erodfderodfderodfderodfderodfd", 123]
 
+        # Test with errors.
         response = requests.post(
             predict_url, json={"length": 300, "num_partitions": 3}, stream=True
         )
         print(response)
+        error = definitions.RemoteErrorDetail.parse_obj(response.json()["error"])
+        print(error.format())
         assert response.status_code == 500
```

### Comparing `truss-0.9.8/truss/tests/util/test_path.py` & `truss-0.9.9rc1/truss/tests/util/test_path.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/truss_config.py` & `truss-0.9.9rc1/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/truss_gatherer.py` & `truss-0.9.9rc1/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/truss_handle.py` & `truss-0.9.9rc1/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/truss_spec.py` & `truss-0.9.9rc1/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/types.py` & `truss-0.9.9rc1/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/util/.truss_ignore` & `truss-0.9.9rc1/truss/util/.truss_ignore`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/util/download.py` & `truss-0.9.9rc1/truss/util/download.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/util/gpu.py` & `truss-0.9.9rc1/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/util/path.py` & `truss-0.9.9rc1/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/truss/validation.py` & `truss-0.9.9rc1/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.8/PKG-INFO` & `truss-0.9.9rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.9.8
+Version: 0.9.9rc1
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
```

