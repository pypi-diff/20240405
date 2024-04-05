# Comparing `tmp/gradientai-1.8.1.tar.gz` & `tmp/gradientai-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradientai-1.8.1.tar", max compression
+gzip compressed data, was "gradientai-1.9.0.tar", max compression
```

## Comparing `gradientai-1.8.1.tar` & `gradientai-1.9.0.tar`

### file list

```diff
@@ -1,284 +1,339 @@
--rw-r--r--   0        0        0      384 2024-01-05 17:23:11.489991 gradientai-1.8.1/README.md
--rw-r--r--   0        0        0      873 2024-01-23 18:53:48.551772 gradientai-1.8.1/gradientai/__init__.py
--rw-r--r--   0        0        0     2237 2024-01-23 18:53:48.552274 gradientai-1.8.1/gradientai/__init__.pyi
--rw-r--r--   0        0        0     2686 2024-01-15 20:53:10.434985 gradientai-1.8.1/gradientai/_base_model.py
--rw-r--r--   0        0        0     3984 2023-12-12 23:07:24.497963 gradientai-1.8.1/gradientai/_embeddings_model.py
--rw-r--r--   0        0        0    12697 2024-03-28 19:25:07.833160 gradientai-1.8.1/gradientai/_gradient.py
--rw-r--r--   0        0        0     2333 2024-01-17 22:42:00.974311 gradientai-1.8.1/gradientai/_model.py
--rw-r--r--   0        0        0     3510 2023-11-01 18:32:45.222694 gradientai-1.8.1/gradientai/_model_adapter.py
--rw-r--r--   0        0        0     2439 2024-03-28 19:25:07.833447 gradientai-1.8.1/gradientai/_types.py
--rw-r--r--   0        0        0      730 2023-12-12 23:07:24.498331 gradientai-1.8.1/gradientai/helpers/asyncio_threads.py
--rw-r--r--   0        0        0     2155 2023-09-11 17:22:53.044122 gradientai-1.8.1/gradientai/helpers/env_manager.py
--rw-r--r--   0        0        0        0 2024-03-28 19:39:06.566008 gradientai-1.8.1/gradientai/openapi/__init__.py
--rw-r--r--   0        0        0    10079 2024-03-28 19:59:24.931201 gradientai-1.8.1/gradientai/openapi/client/__init__.py
--rw-r--r--   0        0        0      245 2024-03-28 19:59:24.931325 gradientai-1.8.1/gradientai/openapi/client/api/__init__.py
--rw-r--r--   0        0        0    44852 2024-03-28 19:39:06.452181 gradientai-1.8.1/gradientai/openapi/client/api/blocks_api.py
--rw-r--r--   0        0        0    15138 2024-03-28 19:39:06.503271 gradientai-1.8.1/gradientai/openapi/client/api/embeddings_api.py
--rw-r--r--   0        0        0    43721 2024-03-28 19:39:06.526340 gradientai-1.8.1/gradientai/openapi/client/api/models_api.py
--rw-r--r--   0        0        0    30160 2024-03-28 19:39:06.575272 gradientai-1.8.1/gradientai/openapi/client/api_client.py
--rw-r--r--   0        0        0      844 2024-03-28 19:39:06.578517 gradientai-1.8.1/gradientai/openapi/client/api_response.py
--rw-r--r--   0        0        0    14896 2024-03-28 19:39:06.550668 gradientai-1.8.1/gradientai/openapi/client/configuration.py
--rw-r--r--   0        0        0     1294 2024-03-28 19:39:05.669756 gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md
--rw-r--r--   0        0        0     1275 2024-03-28 19:39:05.718558 gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md
--rw-r--r--   0        0        0      989 2024-03-28 19:39:05.741426 gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentError.md
--rw-r--r--   0        0        0     1017 2024-03-28 19:39:05.756813 gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md
--rw-r--r--   0        0        0      935 2024-03-28 19:39:05.772197 gradientai-1.8.1/gradientai/openapi/client/docs/BaseModel.md
--rw-r--r--   0        0        0    17886 2024-03-28 19:39:06.495189 gradientai-1.8.1/gradientai/openapi/client/docs/BlocksApi.md
--rw-r--r--   0        0        0     2065 2024-03-28 19:39:05.787738 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelBodyParams.md
--rw-r--r--   0        0        0     1226 2024-03-28 19:39:05.796540 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md
--rw-r--r--   0        0        0     1153 2024-03-28 19:39:05.803225 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md
--rw-r--r--   0        0        0     1069 2024-03-28 19:39:05.814241 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelError.md
--rw-r--r--   0        0        0     1146 2024-03-28 19:39:05.824600 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md
--rw-r--r--   0        0        0     1161 2024-03-28 19:39:05.834803 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md
--rw-r--r--   0        0        0     1080 2024-03-28 19:39:05.843404 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md
--rw-r--r--   0        0        0     1224 2024-03-28 19:39:05.851102 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md
--rw-r--r--   0        0        0     1161 2024-03-28 19:39:05.858489 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md
--rw-r--r--   0        0        0     1067 2024-03-28 19:39:05.866654 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md
--rw-r--r--   0        0        0     1067 2024-03-28 19:39:05.876732 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md
--rw-r--r--   0        0        0     1067 2024-03-28 19:39:05.889161 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md
--rw-r--r--   0        0        0     1067 2024-03-28 19:39:05.901195 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md
--rw-r--r--   0        0        0     1067 2024-03-28 19:39:05.909436 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md
--rw-r--r--   0        0        0     1067 2024-03-28 19:39:05.918661 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md
--rw-r--r--   0        0        0     1067 2024-03-28 19:39:05.927692 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md
--rw-r--r--   0        0        0     1243 2024-03-28 19:39:05.936871 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md
--rw-r--r--   0        0        0     1394 2024-03-28 19:39:05.944594 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md
--rw-r--r--   0        0        0     1019 2024-03-28 19:39:05.951808 gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelSuccess.md
--rw-r--r--   0        0        0     1195 2024-03-28 19:39:05.957872 gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParams.md
--rw-r--r--   0        0        0     1622 2024-03-28 19:39:05.966226 gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md
--rw-r--r--   0        0        0     1565 2024-03-28 19:39:05.973544 gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md
--rw-r--r--   0        0        0     1550 2024-03-28 19:39:05.980787 gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md
--rw-r--r--   0        0        0     1219 2024-03-28 19:39:05.988942 gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md
--rw-r--r--   0        0        0      924 2024-03-28 19:39:05.998405 gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelError.md
--rw-r--r--   0        0        0      945 2024-03-28 19:39:06.006736 gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelSuccess.md
--rw-r--r--   0        0        0      924 2024-03-28 19:39:06.016873 gradientai-1.8.1/gradientai/openapi/client/docs/DeleteModelError.md
--rw-r--r--   0        0        0     5995 2024-03-28 19:39:06.517540 gradientai-1.8.1/gradientai/openapi/client/docs/EmbeddingsApi.md
--rw-r--r--   0        0        0     1218 2024-03-28 19:39:06.024993 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntityBodyParams.md
--rw-r--r--   0        0        0     1235 2024-03-28 19:39:06.033956 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md
--rw-r--r--   0        0        0      950 2024-03-28 19:39:06.041096 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntityError.md
--rw-r--r--   0        0        0     1052 2024-03-28 19:39:06.048016 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntitySuccess.md
--rw-r--r--   0        0        0     1105 2024-03-28 19:39:06.066755 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md
--rw-r--r--   0        0        0      911 2024-03-28 19:39:06.073798 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfError.md
--rw-r--r--   0        0        0     1050 2024-03-28 19:39:06.080599 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccess.md
--rw-r--r--   0        0        0     1462 2024-03-28 19:39:06.087400 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md
--rw-r--r--   0        0        0     1262 2024-03-28 19:39:06.094405 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md
--rw-r--r--   0        0        0     1380 2024-03-28 19:39:06.100957 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md
--rw-r--r--   0        0        0     1598 2024-03-28 19:39:06.108049 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md
--rw-r--r--   0        0        0     1646 2024-03-28 19:39:06.113156 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md
--rw-r--r--   0        0        0     1326 2024-03-28 19:39:06.119068 gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md
--rw-r--r--   0        0        0     1109 2024-03-28 19:39:06.124208 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParams.md
--rw-r--r--   0        0        0     1452 2024-03-28 19:39:06.130444 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md
--rw-r--r--   0        0        0     1496 2024-03-28 19:39:06.135217 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md
--rw-r--r--   0        0        0     1256 2024-03-28 19:39:06.140545 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md
--rw-r--r--   0        0        0     1562 2024-03-28 19:39:06.145803 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md
--rw-r--r--   0        0        0     1076 2024-03-28 19:39:06.152059 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelError.md
--rw-r--r--   0        0        0     1061 2024-03-28 19:39:06.157148 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md
--rw-r--r--   0        0        0     1074 2024-03-28 19:39:06.162838 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md
--rw-r--r--   0        0        0     1033 2024-03-28 19:39:06.167931 gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelSuccess.md
--rw-r--r--   0        0        0     1127 2024-03-28 19:39:06.173795 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md
--rw-r--r--   0        0        0     1177 2024-03-28 19:39:06.179644 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md
--rw-r--r--   0        0        0     1290 2024-03-28 19:39:06.186234 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md
--rw-r--r--   0        0        0     1290 2024-03-28 19:39:06.192537 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md
--rw-r--r--   0        0        0      963 2024-03-28 19:39:06.197234 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerError.md
--rw-r--r--   0        0        0     1097 2024-03-28 19:39:06.202717 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerSuccess.md
--rw-r--r--   0        0        0     1235 2024-03-28 19:39:06.207995 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md
--rw-r--r--   0        0        0     1359 2024-03-28 19:39:06.213608 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md
--rw-r--r--   0        0        0     1159 2024-03-28 19:39:06.219656 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md
--rw-r--r--   0        0        0     1229 2024-03-28 19:39:06.225513 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md
--rw-r--r--   0        0        0     1002 2024-03-28 19:39:06.230632 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingError.md
--rw-r--r--   0        0        0     1119 2024-03-28 19:39:06.235892 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md
--rw-r--r--   0        0        0     1273 2024-03-28 19:39:06.241063 gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md
--rw-r--r--   0        0        0      885 2024-03-28 19:39:06.248710 gradientai-1.8.1/gradientai/openapi/client/docs/GetModelError.md
--rw-r--r--   0        0        0     1034 2024-03-28 19:39:06.272839 gradientai-1.8.1/gradientai/openapi/client/docs/GetModelSuccess.md
--rw-r--r--   0        0        0      963 2024-03-28 19:39:06.282027 gradientai-1.8.1/gradientai/openapi/client/docs/ListEmbeddingsError.md
--rw-r--r--   0        0        0     1093 2024-03-28 19:39:06.289251 gradientai-1.8.1/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md
--rw-r--r--   0        0        0     1280 2024-03-28 19:39:06.296982 gradientai-1.8.1/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md
--rw-r--r--   0        0        0      911 2024-03-28 19:39:06.303675 gradientai-1.8.1/gradientai/openapi/client/docs/ListModelsError.md
--rw-r--r--   0        0        0     1002 2024-03-28 19:39:06.313353 gradientai-1.8.1/gradientai/openapi/client/docs/ListModelsSuccess.md
--rw-r--r--   0        0        0     1281 2024-03-28 19:39:06.321284 gradientai-1.8.1/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md
--rw-r--r--   0        0        0      988 2024-03-28 19:39:06.328369 gradientai-1.8.1/gradientai/openapi/client/docs/ModelAdapter.md
--rw-r--r--   0        0        0    17156 2024-03-28 19:39:06.534677 gradientai-1.8.1/gradientai/openapi/client/docs/ModelsApi.md
--rw-r--r--   0        0        0     1258 2024-03-28 19:39:06.334710 gradientai-1.8.1/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md
--rw-r--r--   0        0        0     1028 2024-03-28 19:39:06.340769 gradientai-1.8.1/gradientai/openapi/client/docs/PersonalizeDocumentError.md
--rw-r--r--   0        0        0     1068 2024-03-28 19:39:06.346481 gradientai-1.8.1/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md
--rw-r--r--   0        0        0     1347 2024-03-28 19:39:06.352201 gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md
--rw-r--r--   0        0        0     1286 2024-03-28 19:39:06.358858 gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md
--rw-r--r--   0        0        0     1002 2024-03-28 19:39:06.370626 gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentError.md
--rw-r--r--   0        0        0     1028 2024-03-28 19:39:06.382850 gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md
--rw-r--r--   0        0        0     5323 2024-03-28 19:39:06.569365 gradientai-1.8.1/gradientai/openapi/client/exceptions.py
--rw-r--r--   0        0        0     9262 2024-03-28 19:59:24.931487 gradientai-1.8.1/gradientai/openapi/client/models/__init__.py
--rw-r--r--   0        0        0     3617 2024-03-28 19:39:05.642985 gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_body_params.py
--rw-r--r--   0        0        0     3053 2024-03-28 19:39:05.689245 gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py
--rw-r--r--   0        0        0     2501 2024-03-28 19:39:05.732003 gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_error.py
--rw-r--r--   0        0        0     2799 2024-03-28 19:39:05.750143 gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_success.py
--rw-r--r--   0        0        0     3400 2024-03-28 19:39:05.763584 gradientai-1.8.1/gradientai/openapi/client/models/base_model.py
--rw-r--r--   0        0        0     6500 2024-03-28 19:39:05.782966 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_body_params.py
--rw-r--r--   0        0        0     3043 2024-03-28 19:39:05.791897 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_body_params_guidance.py
--rw-r--r--   0        0        0     2680 2024-03-28 19:39:05.799672 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_body_params_rag.py
--rw-r--r--   0        0        0    13624 2024-03-28 19:39:05.809114 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error.py
--rw-r--r--   0        0        0     3793 2024-03-28 19:39:05.818471 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of.py
--rw-r--r--   0        0        0     3887 2024-03-28 19:39:05.829522 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of1.py
--rw-r--r--   0        0        0     2885 2024-03-28 19:39:05.838866 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of10.py
--rw-r--r--   0        0        0     3347 2024-03-28 19:39:05.847292 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py
--rw-r--r--   0        0        0     3361 2024-03-28 19:39:05.854189 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of2.py
--rw-r--r--   0        0        0     2849 2024-03-28 19:39:05.862011 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of3.py
--rw-r--r--   0        0        0     2891 2024-03-28 19:39:05.870887 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of4.py
--rw-r--r--   0        0        0     2875 2024-03-28 19:39:05.882532 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of5.py
--rw-r--r--   0        0        0     2887 2024-03-28 19:39:05.895353 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of6.py
--rw-r--r--   0        0        0     2869 2024-03-28 19:39:05.905244 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of7.py
--rw-r--r--   0        0        0     2875 2024-03-28 19:39:05.912961 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of8.py
--rw-r--r--   0        0        0     2877 2024-03-28 19:39:05.923214 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of9.py
--rw-r--r--   0        0        0     3281 2024-03-28 19:39:05.932920 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of_payload.py
--rw-r--r--   0        0        0     2700 2024-03-28 19:39:05.940551 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py
--rw-r--r--   0        0        0     2665 2024-03-28 19:39:05.947938 gradientai-1.8.1/gradientai/openapi/client/models/complete_model_success.py
--rw-r--r--   0        0        0     3807 2024-03-28 19:39:05.954614 gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params.py
--rw-r--r--   0        0        0     4559 2024-03-28 19:39:05.961972 gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py
--rw-r--r--   0        0        0     3018 2024-03-28 19:39:05.969960 gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
--rw-r--r--   0        0        0     3165 2024-03-28 19:39:05.977033 gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py
--rw-r--r--   0        0        0     2836 2024-03-28 19:39:05.983516 gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_model.py
--rw-r--r--   0        0        0     2461 2024-03-28 19:39:05.993455 gradientai-1.8.1/gradientai/openapi/client/models/create_model_error.py
--rw-r--r--   0        0        0     2457 2024-03-28 19:39:06.002563 gradientai-1.8.1/gradientai/openapi/client/models/create_model_success.py
--rw-r--r--   0        0        0     2461 2024-03-28 19:39:06.009916 gradientai-1.8.1/gradientai/openapi/client/models/delete_model_error.py
--rw-r--r--   0        0        0     3456 2024-03-28 19:39:06.020954 gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_body_params.py
--rw-r--r--   0        0        0     3228 2024-03-28 19:39:06.029009 gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py
--rw-r--r--   0        0        0     2477 2024-03-28 19:39:06.037579 gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_error.py
--rw-r--r--   0        0        0     3136 2024-03-28 19:39:06.044362 gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_success.py
--rw-r--r--   0        0        0     5870 2024-03-28 19:39:06.052813 gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_success_entity_value.py
--rw-r--r--   0        0        0     2453 2024-03-28 19:39:06.070004 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_error.py
--rw-r--r--   0        0        0     3365 2024-03-28 19:39:06.076363 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success.py
--rw-r--r--   0        0        0     4761 2024-03-28 19:39:06.083698 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py
--rw-r--r--   0        0        0     2937 2024-03-28 19:39:06.091096 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py
--rw-r--r--   0        0        0     3397 2024-03-28 19:39:06.097230 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py
--rw-r--r--   0        0        0     3774 2024-03-28 19:39:06.104350 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
--rw-r--r--   0        0        0     3545 2024-03-28 19:39:06.110267 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
--rw-r--r--   0        0        0     3065 2024-03-28 19:39:06.116072 gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py
--rw-r--r--   0        0        0     3075 2024-03-28 19:39:06.121399 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params.py
--rw-r--r--   0        0        0     4023 2024-03-28 19:39:06.127327 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py
--rw-r--r--   0        0        0     3056 2024-03-28 19:39:06.132502 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
--rw-r--r--   0        0        0     5780 2024-03-28 19:39:06.138124 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py
--rw-r--r--   0        0        0     3137 2024-03-28 19:39:06.142837 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
--rw-r--r--   0        0        0    10150 2024-03-28 19:39:06.149201 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_error.py
--rw-r--r--   0        0        0     2881 2024-03-28 19:39:06.154420 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_error_one_of.py
--rw-r--r--   0        0        0     2851 2024-03-28 19:39:06.159465 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py
--rw-r--r--   0        0        0     2748 2024-03-28 19:39:06.165275 gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_success.py
--rw-r--r--   0        0        0     2993 2024-03-28 19:39:06.170445 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params.py
--rw-r--r--   0        0        0     6307 2024-03-28 19:39:06.176557 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params_source.py
--rw-r--r--   0        0        0     3023 2024-03-28 19:39:06.183086 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py
--rw-r--r--   0        0        0     2959 2024-03-28 19:39:06.188950 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py
--rw-r--r--   0        0        0     2485 2024-03-28 19:39:06.194675 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_error.py
--rw-r--r--   0        0        0     3047 2024-03-28 19:39:06.199431 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_success.py
--rw-r--r--   0        0        0     3197 2024-03-28 19:39:06.205106 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_success_rag_context.py
--rw-r--r--   0        0        0     2831 2024-03-28 19:39:06.210125 gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py
--rw-r--r--   0        0        0     3137 2024-03-28 19:39:06.216485 gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_body_params.py
--rw-r--r--   0        0        0     2629 2024-03-28 19:39:06.222293 gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py
--rw-r--r--   0        0        0     2509 2024-03-28 19:39:06.227975 gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_error.py
--rw-r--r--   0        0        0     3124 2024-03-28 19:39:06.232825 gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_success.py
--rw-r--r--   0        0        0     2802 2024-03-28 19:39:06.237975 gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py
--rw-r--r--   0        0        0     2437 2024-03-28 19:39:06.243804 gradientai-1.8.1/gradientai/openapi/client/models/get_model_error.py
--rw-r--r--   0        0        0     3226 2024-03-28 19:39:06.253359 gradientai-1.8.1/gradientai/openapi/client/models/get_model_success.py
--rw-r--r--   0        0        0     2485 2024-03-28 19:39:06.275987 gradientai-1.8.1/gradientai/openapi/client/models/list_embeddings_error.py
--rw-r--r--   0        0        0     3198 2024-03-28 19:39:06.285590 gradientai-1.8.1/gradientai/openapi/client/models/list_embeddings_success.py
--rw-r--r--   0        0        0     2877 2024-03-28 19:39:06.292445 gradientai-1.8.1/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py
--rw-r--r--   0        0        0     2453 2024-03-28 19:39:06.299864 gradientai-1.8.1/gradientai/openapi/client/models/list_models_error.py
--rw-r--r--   0        0        0     2988 2024-03-28 19:39:06.308732 gradientai-1.8.1/gradientai/openapi/client/models/list_models_success.py
--rw-r--r--   0        0        0     6222 2024-03-28 19:39:06.316989 gradientai-1.8.1/gradientai/openapi/client/models/list_models_success_models_inner.py
--rw-r--r--   0        0        0     3202 2024-03-28 19:39:06.324648 gradientai-1.8.1/gradientai/openapi/client/models/model_adapter.py
--rw-r--r--   0        0        0     2910 2024-03-28 19:39:06.331832 gradientai-1.8.1/gradientai/openapi/client/models/personalize_document_body_params.py
--rw-r--r--   0        0        0     2525 2024-03-28 19:39:06.337302 gradientai-1.8.1/gradientai/openapi/client/models/personalize_document_error.py
--rw-r--r--   0        0        0     2625 2024-03-28 19:39:06.343225 gradientai-1.8.1/gradientai/openapi/client/models/personalize_document_success.py
--rw-r--r--   0        0        0     4281 2024-03-28 19:39:06.348942 gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_body_params.py
--rw-r--r--   0        0        0     2771 2024-03-28 19:39:06.354323 gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py
--rw-r--r--   0        0        0     2509 2024-03-28 19:39:06.361523 gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_error.py
--rw-r--r--   0        0        0     2525 2024-03-28 19:39:06.375543 gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_success.py
--rw-r--r--   0        0        0    12904 2024-03-28 19:39:06.587599 gradientai-1.8.1/gradientai/openapi/client/rest.py
--rw-r--r--   0        0        0        0 2024-03-28 19:39:06.570853 gradientai-1.8.1/gradientai/openapi/client/test/__init__.py
--rw-r--r--   0        0        0     2004 2024-03-28 19:39:05.651797 gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py
--rw-r--r--   0        0        0     1960 2024-03-28 19:39:05.713840 gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py
--rw-r--r--   0        0        0     1655 2024-03-28 19:39:05.737092 gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_error.py
--rw-r--r--   0        0        0     1697 2024-03-28 19:39:05.753805 gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_success.py
--rw-r--r--   0        0        0     2039 2024-03-28 19:39:05.767838 gradientai-1.8.1/gradientai/openapi/client/test/test_base_model.py
--rw-r--r--   0        0        0     1639 2024-03-28 19:39:06.456532 gradientai-1.8.1/gradientai/openapi/client/test/test_blocks_api.py
--rw-r--r--   0        0        0     2280 2024-03-28 19:39:05.785404 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_body_params.py
--rw-r--r--   0        0        0     1930 2024-03-28 19:39:05.794659 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py
--rw-r--r--   0        0        0     1731 2024-03-28 19:39:05.801697 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_body_params_rag.py
--rw-r--r--   0        0        0     2177 2024-03-28 19:39:05.812181 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error.py
--rw-r--r--   0        0        0     2591 2024-03-28 19:39:05.821205 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of.py
--rw-r--r--   0        0        0     2257 2024-03-28 19:39:05.832709 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of1.py
--rw-r--r--   0        0        0     1802 2024-03-28 19:39:05.841471 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of10.py
--rw-r--r--   0        0        0     1812 2024-03-28 19:39:05.849442 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py
--rw-r--r--   0        0        0     2271 2024-03-28 19:39:05.856721 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of2.py
--rw-r--r--   0        0        0     1762 2024-03-28 19:39:05.864471 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of3.py
--rw-r--r--   0        0        0     1804 2024-03-28 19:39:05.873915 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of4.py
--rw-r--r--   0        0        0     1788 2024-03-28 19:39:05.886254 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of5.py
--rw-r--r--   0        0        0     1800 2024-03-28 19:39:05.898384 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of6.py
--rw-r--r--   0        0        0     1782 2024-03-28 19:39:05.907731 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of7.py
--rw-r--r--   0        0        0     1788 2024-03-28 19:39:05.915469 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of8.py
--rw-r--r--   0        0        0     1790 2024-03-28 19:39:05.926157 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of9.py
--rw-r--r--   0        0        0     2235 2024-03-28 19:39:05.935266 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py
--rw-r--r--   0        0        0     1999 2024-03-28 19:39:05.943076 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py
--rw-r--r--   0        0        0     1732 2024-03-28 19:39:05.950270 gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_success.py
--rw-r--r--   0        0        0     2659 2024-03-28 19:39:05.956399 gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params.py
--rw-r--r--   0        0        0     2349 2024-03-28 19:39:05.964529 gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py
--rw-r--r--   0        0        0     2121 2024-03-28 19:39:05.971870 gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
--rw-r--r--   0        0        0     2106 2024-03-28 19:39:05.978888 gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py
--rw-r--r--   0        0        0     1788 2024-03-28 19:39:05.987206 gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_model.py
--rw-r--r--   0        0        0     1595 2024-03-28 19:39:05.996366 gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_error.py
--rw-r--r--   0        0        0     1609 2024-03-28 19:39:06.004990 gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_success.py
--rw-r--r--   0        0        0     1595 2024-03-28 19:39:06.012375 gradientai-1.8.1/gradientai/openapi/client/test/test_delete_model_error.py
--rw-r--r--   0        0        0     1087 2024-03-28 19:39:06.509096 gradientai-1.8.1/gradientai/openapi/client/test/test_embeddings_api.py
--rw-r--r--   0        0        0     2242 2024-03-28 19:39:06.023336 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_body_params.py
--rw-r--r--   0        0        0     1857 2024-03-28 19:39:06.032017 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py
--rw-r--r--   0        0        0     1619 2024-03-28 19:39:06.039483 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_error.py
--rw-r--r--   0        0        0     1747 2024-03-28 19:39:06.046379 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_success.py
--rw-r--r--   0        0        0     1718 2024-03-28 19:39:06.055007 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py
--rw-r--r--   0        0        0     1583 2024-03-28 19:39:06.072129 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_error.py
--rw-r--r--   0        0        0     5829 2024-03-28 19:39:06.078560 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success.py
--rw-r--r--   0        0        0     5055 2024-03-28 19:39:06.085629 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py
--rw-r--r--   0        0        0     1938 2024-03-28 19:39:06.092963 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py
--rw-r--r--   0        0        0     3256 2024-03-28 19:39:06.099396 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py
--rw-r--r--   0        0        0     2800 2024-03-28 19:39:06.106469 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
--rw-r--r--   0        0        0     2291 2024-03-28 19:39:06.111813 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
--rw-r--r--   0        0        0     2066 2024-03-28 19:39:06.117765 gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py
--rw-r--r--   0        0        0     2583 2024-03-28 19:39:06.122917 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params.py
--rw-r--r--   0        0        0     2070 2024-03-28 19:39:06.129156 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py
--rw-r--r--   0        0        0     2047 2024-03-28 19:39:06.134020 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
--rw-r--r--   0        0        0     1844 2024-03-28 19:39:06.139509 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py
--rw-r--r--   0        0        0     2108 2024-03-28 19:39:06.144549 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
--rw-r--r--   0        0        0     2183 2024-03-28 19:39:06.150793 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_error.py
--rw-r--r--   0        0        0     1792 2024-03-28 19:39:06.156001 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py
--rw-r--r--   0        0        0     1766 2024-03-28 19:39:06.161598 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py
--rw-r--r--   0        0        0     1748 2024-03-28 19:39:06.166804 gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_success.py
--rw-r--r--   0        0        0     1758 2024-03-28 19:39:06.172465 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params.py
--rw-r--r--   0        0        0     1899 2024-03-28 19:39:06.178169 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params_source.py
--rw-r--r--   0        0        0     1904 2024-03-28 19:39:06.184849 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py
--rw-r--r--   0        0        0     1910 2024-03-28 19:39:06.191173 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py
--rw-r--r--   0        0        0     1631 2024-03-28 19:39:06.196085 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_error.py
--rw-r--r--   0        0        0     2101 2024-03-28 19:39:06.201332 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_success.py
--rw-r--r--   0        0        0     2299 2024-03-28 19:39:06.206773 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py
--rw-r--r--   0        0        0     2018 2024-03-28 19:39:06.212257 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py
--rw-r--r--   0        0        0     2123 2024-03-28 19:39:06.218328 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_body_params.py
--rw-r--r--   0        0        0     1861 2024-03-28 19:39:06.224247 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py
--rw-r--r--   0        0        0     1667 2024-03-28 19:39:06.229548 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_error.py
--rw-r--r--   0        0        0     2299 2024-03-28 19:39:06.234527 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_success.py
--rw-r--r--   0        0        0     2026 2024-03-28 19:39:06.239714 gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py
--rw-r--r--   0        0        0     1559 2024-03-28 19:39:06.246952 gradientai-1.8.1/gradientai/openapi/client/test/test_get_model_error.py
--rw-r--r--   0        0        0     2193 2024-03-28 19:39:06.269907 gradientai-1.8.1/gradientai/openapi/client/test/test_get_model_success.py
--rw-r--r--   0        0        0     1631 2024-03-28 19:39:06.278936 gradientai-1.8.1/gradientai/openapi/client/test/test_list_embeddings_error.py
--rw-r--r--   0        0        0     2101 2024-03-28 19:39:06.287720 gradientai-1.8.1/gradientai/openapi/client/test/test_list_embeddings_success.py
--rw-r--r--   0        0        0     1923 2024-03-28 19:39:06.295347 gradientai-1.8.1/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py
--rw-r--r--   0        0        0     1583 2024-03-28 19:39:06.302030 gradientai-1.8.1/gradientai/openapi/client/test/test_list_models_error.py
--rw-r--r--   0        0        0     1695 2024-03-28 19:39:06.311847 gradientai-1.8.1/gradientai/openapi/client/test/test_list_models_success.py
--rw-r--r--   0        0        0     2579 2024-03-28 19:39:06.318836 gradientai-1.8.1/gradientai/openapi/client/test/test_list_models_success_models_inner.py
--rw-r--r--   0        0        0     2155 2024-03-28 19:39:06.326847 gradientai-1.8.1/gradientai/openapi/client/test/test_model_adapter.py
--rw-r--r--   0        0        0     1568 2024-03-28 19:39:06.528677 gradientai-1.8.1/gradientai/openapi/client/test/test_models_api.py
--rw-r--r--   0        0        0     1844 2024-03-28 19:39:06.333368 gradientai-1.8.1/gradientai/openapi/client/test/test_personalize_document_body_params.py
--rw-r--r--   0        0        0     1691 2024-03-28 19:39:06.339339 gradientai-1.8.1/gradientai/openapi/client/test/test_personalize_document_error.py
--rw-r--r--   0        0        0     1743 2024-03-28 19:39:06.345157 gradientai-1.8.1/gradientai/openapi/client/test/test_personalize_document_success.py
--rw-r--r--   0        0        0     2044 2024-03-28 19:39:06.350779 gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_body_params.py
--rw-r--r--   0        0        0     1954 2024-03-28 19:39:06.357335 gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py
--rw-r--r--   0        0        0     1667 2024-03-28 19:39:06.363759 gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_error.py
--rw-r--r--   0        0        0     1691 2024-03-28 19:39:06.379074 gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_success.py
--rw-r--r--   0        0        0    19191 2024-03-28 19:59:24.931664 gradientai-1.8.1/gradientai/openapi/client_README.md
--rw-r--r--   0        0        0        0 2023-09-06 19:21:36.816287 gradientai-1.8.1/gradientai/py.typed
--rw-r--r--   0        0        0      210 2023-11-01 18:32:45.224496 gradientai-1.8.1/gradientai/pydantic_models/types.py
--rw-r--r--   0        0        0     1778 2024-03-28 19:35:29.902078 gradientai-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 gradientai-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      384 2024-01-02 22:48:19.948017 gradientai-1.9.0/README.md
+-rw-r--r--   0        0        0      873 2024-01-26 22:46:41.832392 gradientai-1.9.0/gradientai/__init__.py
+-rw-r--r--   0        0        0     2237 2024-01-26 22:46:41.832503 gradientai-1.9.0/gradientai/__init__.pyi
+-rw-r--r--   0        0        0     2686 2024-01-26 22:46:41.832628 gradientai-1.9.0/gradientai/_base_model.py
+-rw-r--r--   0        0        0     3984 2024-01-02 22:48:19.948502 gradientai-1.9.0/gradientai/_embeddings_model.py
+-rw-r--r--   0        0        0    16178 2024-04-03 23:04:21.105909 gradientai-1.9.0/gradientai/_gradient.py
+-rw-r--r--   0        0        0     2333 2024-04-03 00:11:07.185923 gradientai-1.9.0/gradientai/_model.py
+-rw-r--r--   0        0        0     3510 2023-10-24 19:44:32.688189 gradientai-1.9.0/gradientai/_model_adapter.py
+-rw-r--r--   0        0        0     1748 2024-04-03 23:04:21.106074 gradientai-1.9.0/gradientai/_rag.py
+-rw-r--r--   0        0        0     2497 2024-04-02 16:51:03.746721 gradientai-1.9.0/gradientai/_types.py
+-rw-r--r--   0        0        0      730 2024-01-02 22:48:19.948773 gradientai-1.9.0/gradientai/helpers/asyncio_threads.py
+-rw-r--r--   0        0        0     2155 2023-09-11 18:57:16.856296 gradientai-1.9.0/gradientai/helpers/env_manager.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:06:10.508888 gradientai-1.9.0/gradientai/openapi/__init__.py
+-rw-r--r--   0        0        0    11944 2024-04-02 23:02:40.025793 gradientai-1.9.0/gradientai/openapi/client/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-02 23:02:40.025926 gradientai-1.9.0/gradientai/openapi/client/api/__init__.py
+-rw-r--r--   0        0        0    59385 2024-04-02 21:06:10.436752 gradientai-1.9.0/gradientai/openapi/client/api/blocks_api.py
+-rw-r--r--   0        0        0    15138 2024-04-02 21:06:10.456255 gradientai-1.9.0/gradientai/openapi/client/api/embeddings_api.py
+-rw-r--r--   0        0        0     8147 2024-04-02 21:06:10.464141 gradientai-1.9.0/gradientai/openapi/client/api/files_api.py
+-rw-r--r--   0        0        0    43721 2024-04-02 21:06:10.473572 gradientai-1.9.0/gradientai/openapi/client/api/models_api.py
+-rw-r--r--   0        0        0    16242 2024-04-02 23:02:40.026264 gradientai-1.9.0/gradientai/openapi/client/api/rag_api.py
+-rw-r--r--   0        0        0    30160 2024-04-02 21:06:10.517186 gradientai-1.9.0/gradientai/openapi/client/api_client.py
+-rw-r--r--   0        0        0      844 2024-04-02 21:06:10.519343 gradientai-1.9.0/gradientai/openapi/client/api_response.py
+-rw-r--r--   0        0        0    14896 2024-04-02 21:06:10.495099 gradientai-1.9.0/gradientai/openapi/client/configuration.py
+-rw-r--r--   0        0        0     1259 2024-04-02 23:02:40.026440 gradientai-1.9.0/gradientai/openapi/client/docs/AddFilesToRagCollectionBodyParams.md
+-rw-r--r--   0        0        0     1101 2024-04-02 23:02:40.026527 gradientai-1.9.0/gradientai/openapi/client/docs/AddFilesToRagCollectionError.md
+-rw-r--r--   0        0        0     1294 2024-04-02 21:06:08.817381 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md
+-rw-r--r--   0        0        0     1275 2024-04-02 21:06:08.859982 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md
+-rw-r--r--   0        0        0      989 2024-04-02 21:06:08.888938 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentError.md
+-rw-r--r--   0        0        0     1017 2024-04-02 21:06:09.017017 gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md
+-rw-r--r--   0        0        0      935 2024-04-02 21:06:09.077859 gradientai-1.9.0/gradientai/openapi/client/docs/BaseModel.md
+-rw-r--r--   0        0        0    23913 2024-04-02 21:06:10.452912 gradientai-1.9.0/gradientai/openapi/client/docs/BlocksApi.md
+-rw-r--r--   0        0        0     2065 2024-04-02 21:06:09.106119 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParams.md
+-rw-r--r--   0        0        0     1226 2024-04-02 21:06:09.173646 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md
+-rw-r--r--   0        0        0     1153 2024-04-02 21:06:09.300783 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md
+-rw-r--r--   0        0        0     1069 2024-04-02 21:06:09.338931 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelError.md
+-rw-r--r--   0        0        0     1146 2024-04-02 21:06:09.380345 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md
+-rw-r--r--   0        0        0     1161 2024-04-02 21:06:09.414975 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md
+-rw-r--r--   0        0        0     1080 2024-04-02 21:06:09.450202 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md
+-rw-r--r--   0        0        0     1224 2024-04-02 21:06:09.525750 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md
+-rw-r--r--   0        0        0     1161 2024-04-02 21:06:09.547399 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.569264 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.585117 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.601035 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.613596 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.630346 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.652113 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md
+-rw-r--r--   0        0        0     1067 2024-04-02 21:06:09.675322 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md
+-rw-r--r--   0        0        0     1243 2024-04-02 21:06:09.694265 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md
+-rw-r--r--   0        0        0     1394 2024-04-02 21:06:09.713760 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md
+-rw-r--r--   0        0        0     1019 2024-04-02 21:06:09.728650 gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelSuccess.md
+-rw-r--r--   0        0        0     1172 2024-04-02 21:06:09.749173 gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionBodyParams.md
+-rw-r--r--   0        0        0     1100 2024-04-02 21:06:09.763865 gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionError.md
+-rw-r--r--   0        0        0     1135 2024-04-02 21:06:09.782221 gradientai-1.9.0/gradientai/openapi/client/docs/CreateAudioTranscriptionSuccess.md
+-rw-r--r--   0        0        0     1195 2024-04-02 21:06:09.799851 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParams.md
+-rw-r--r--   0        0        0     1622 2024-04-02 21:06:09.808092 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md
+-rw-r--r--   0        0        0     1565 2024-04-02 21:06:09.814804 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md
+-rw-r--r--   0        0        0     1550 2024-04-02 21:06:09.823247 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md
+-rw-r--r--   0        0        0     1219 2024-04-02 21:06:09.830872 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md
+-rw-r--r--   0        0        0      924 2024-04-02 21:06:09.838966 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelError.md
+-rw-r--r--   0        0        0      945 2024-04-02 21:06:09.847442 gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelSuccess.md
+-rw-r--r--   0        0        0     1254 2024-04-02 23:02:40.026608 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionBodyParams.md
+-rw-r--r--   0        0        0     1271 2024-04-02 23:02:40.026699 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionBodyParamsFilesInner.md
+-rw-r--r--   0        0        0     1035 2024-04-02 23:02:40.026778 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionError.md
+-rw-r--r--   0        0        0     1056 2024-04-02 23:02:40.026848 gradientai-1.9.0/gradientai/openapi/client/docs/CreateRagCollectionSuccess.md
+-rw-r--r--   0        0        0      924 2024-04-02 21:06:09.922306 gradientai-1.9.0/gradientai/openapi/client/docs/DeleteModelError.md
+-rw-r--r--   0        0        0     5995 2024-04-02 21:06:10.460915 gradientai-1.9.0/gradientai/openapi/client/docs/EmbeddingsApi.md
+-rw-r--r--   0        0        0     1218 2024-04-02 21:06:09.930543 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParams.md
+-rw-r--r--   0        0        0     1235 2024-04-02 21:06:09.942847 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md
+-rw-r--r--   0        0        0      950 2024-04-02 21:06:09.951498 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityError.md
+-rw-r--r--   0        0        0     1052 2024-04-02 21:06:09.958892 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccess.md
+-rw-r--r--   0        0        0     1105 2024-04-02 21:06:09.968200 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md
+-rw-r--r--   0        0        0      911 2024-04-02 21:06:09.974240 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfError.md
+-rw-r--r--   0        0        0     1050 2024-04-02 21:06:09.980697 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccess.md
+-rw-r--r--   0        0        0     1462 2024-04-02 21:06:09.989400 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md
+-rw-r--r--   0        0        0     1262 2024-04-02 21:06:09.999431 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md
+-rw-r--r--   0        0        0     1380 2024-04-02 21:06:10.006871 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md
+-rw-r--r--   0        0        0     1598 2024-04-02 21:06:10.015894 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md
+-rw-r--r--   0        0        0     1646 2024-04-02 21:06:10.022832 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md
+-rw-r--r--   0        0        0     1326 2024-04-02 21:06:10.029202 gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md
+-rw-r--r--   0        0        0     2801 2024-04-02 21:06:10.469329 gradientai-1.9.0/gradientai/openapi/client/docs/FilesApi.md
+-rw-r--r--   0        0        0     1109 2024-04-02 21:06:10.036440 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParams.md
+-rw-r--r--   0        0        0     1452 2024-04-02 21:06:10.042021 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md
+-rw-r--r--   0        0        0     1496 2024-04-02 21:06:10.048829 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md
+-rw-r--r--   0        0        0     1256 2024-04-02 21:06:10.057143 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md
+-rw-r--r--   0        0        0     1562 2024-04-02 21:06:10.064934 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md
+-rw-r--r--   0        0        0     1076 2024-04-02 21:06:10.072608 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelError.md
+-rw-r--r--   0        0        0     1061 2024-04-02 21:06:10.078529 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md
+-rw-r--r--   0        0        0     1074 2024-04-02 21:06:10.085792 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md
+-rw-r--r--   0        0        0     1033 2024-04-02 21:06:10.092123 gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelSuccess.md
+-rw-r--r--   0        0        0     1127 2024-04-02 21:06:10.101646 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md
+-rw-r--r--   0        0        0     1177 2024-04-02 21:06:10.134519 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md
+-rw-r--r--   0        0        0     1290 2024-04-02 21:06:10.146161 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md
+-rw-r--r--   0        0        0     1290 2024-04-02 21:06:10.154510 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md
+-rw-r--r--   0        0        0      963 2024-04-02 21:06:10.162634 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerError.md
+-rw-r--r--   0        0        0     1097 2024-04-02 21:06:10.169665 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccess.md
+-rw-r--r--   0        0        0     1235 2024-04-02 21:06:10.176849 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md
+-rw-r--r--   0        0        0     1359 2024-04-02 21:06:10.183918 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md
+-rw-r--r--   0        0        0     1159 2024-04-02 21:06:10.192220 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md
+-rw-r--r--   0        0        0     1229 2024-04-02 21:06:10.199299 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md
+-rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.209914 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingError.md
+-rw-r--r--   0        0        0     1119 2024-04-02 21:06:10.219023 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md
+-rw-r--r--   0        0        0     1273 2024-04-02 21:06:10.225005 gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md
+-rw-r--r--   0        0        0     1061 2024-04-02 21:06:10.230449 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionError.md
+-rw-r--r--   0        0        0     1197 2024-04-02 21:06:10.238093 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccess.md
+-rw-r--r--   0        0        0     1195 2024-04-02 21:06:10.243126 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf.md
+-rw-r--r--   0        0        0     1289 2024-04-02 21:06:10.248549 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1.md
+-rw-r--r--   0        0        0     1261 2024-04-02 21:06:10.254570 gradientai-1.9.0/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1Result.md
+-rw-r--r--   0        0        0      885 2024-04-02 21:06:10.260434 gradientai-1.9.0/gradientai/openapi/client/docs/GetModelError.md
+-rw-r--r--   0        0        0     1034 2024-04-02 21:06:10.266339 gradientai-1.9.0/gradientai/openapi/client/docs/GetModelSuccess.md
+-rw-r--r--   0        0        0      963 2024-04-02 21:06:10.273428 gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsError.md
+-rw-r--r--   0        0        0     1093 2024-04-02 21:06:10.278509 gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md
+-rw-r--r--   0        0        0     1280 2024-04-02 21:06:10.286179 gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md
+-rw-r--r--   0        0        0      911 2024-04-02 21:06:10.291565 gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsError.md
+-rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.297535 gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccess.md
+-rw-r--r--   0        0        0     1281 2024-04-02 21:06:10.303477 gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md
+-rw-r--r--   0        0        0      988 2024-04-02 21:06:10.309052 gradientai-1.9.0/gradientai/openapi/client/docs/ModelAdapter.md
+-rw-r--r--   0        0        0    17156 2024-04-02 21:06:10.478620 gradientai-1.9.0/gradientai/openapi/client/docs/ModelsApi.md
+-rw-r--r--   0        0        0     1258 2024-04-02 21:06:10.313692 gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md
+-rw-r--r--   0        0        0     1028 2024-04-02 21:06:10.319260 gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentError.md
+-rw-r--r--   0        0        0     1068 2024-04-02 21:06:10.325029 gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md
+-rw-r--r--   0        0        0     6299 2024-04-02 23:02:40.027022 gradientai-1.9.0/gradientai/openapi/client/docs/RAGApi.md
+-rw-r--r--   0        0        0     1347 2024-04-02 21:06:10.331891 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md
+-rw-r--r--   0        0        0     1286 2024-04-02 21:06:10.337363 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md
+-rw-r--r--   0        0        0     1002 2024-04-02 21:06:10.343168 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentError.md
+-rw-r--r--   0        0        0     1028 2024-04-02 21:06:10.348221 gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md
+-rw-r--r--   0        0        0      911 2024-04-02 21:06:10.356695 gradientai-1.9.0/gradientai/openapi/client/docs/UploadFileError.md
+-rw-r--r--   0        0        0      932 2024-04-02 21:06:10.363682 gradientai-1.9.0/gradientai/openapi/client/docs/UploadFileSuccess.md
+-rw-r--r--   0        0        0     5323 2024-04-02 21:06:10.512625 gradientai-1.9.0/gradientai/openapi/client/exceptions.py
+-rw-r--r--   0        0        0    11009 2024-04-02 23:02:40.027183 gradientai-1.9.0/gradientai/openapi/client/models/__init__.py
+-rw-r--r--   0        0        0     3166 2024-04-03 23:04:21.106342 gradientai-1.9.0/gradientai/openapi/client/models/add_files_to_rag_collection_body_params.py
+-rw-r--r--   0        0        0     2557 2024-04-02 23:02:40.027355 gradientai-1.9.0/gradientai/openapi/client/models/add_files_to_rag_collection_error.py
+-rw-r--r--   0        0        0     3617 2024-04-02 21:06:08.792526 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params.py
+-rw-r--r--   0        0        0     3053 2024-04-02 21:06:08.847811 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py
+-rw-r--r--   0        0        0     2501 2024-04-02 21:06:08.872357 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_error.py
+-rw-r--r--   0        0        0     2799 2024-04-02 21:06:08.904229 gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_success.py
+-rw-r--r--   0        0        0     3400 2024-04-02 21:06:09.034106 gradientai-1.9.0/gradientai/openapi/client/models/base_model.py
+-rw-r--r--   0        0        0     6500 2024-04-02 21:06:09.090984 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params.py
+-rw-r--r--   0        0        0     3043 2024-04-02 21:06:09.144530 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_guidance.py
+-rw-r--r--   0        0        0     2680 2024-04-02 21:06:09.246459 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_rag.py
+-rw-r--r--   0        0        0    13624 2024-04-02 21:06:09.326952 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error.py
+-rw-r--r--   0        0        0     3793 2024-04-02 21:06:09.357221 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of.py
+-rw-r--r--   0        0        0     3887 2024-04-02 21:06:09.397688 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1.py
+-rw-r--r--   0        0        0     2885 2024-04-02 21:06:09.433031 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of10.py
+-rw-r--r--   0        0        0     3347 2024-04-02 21:06:09.509206 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py
+-rw-r--r--   0        0        0     3361 2024-04-02 21:06:09.534327 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of2.py
+-rw-r--r--   0        0        0     2849 2024-04-02 21:06:09.557641 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of3.py
+-rw-r--r--   0        0        0     2891 2024-04-02 21:06:09.576512 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of4.py
+-rw-r--r--   0        0        0     2875 2024-04-02 21:06:09.591719 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of5.py
+-rw-r--r--   0        0        0     2887 2024-04-02 21:06:09.606721 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of6.py
+-rw-r--r--   0        0        0     2869 2024-04-02 21:06:09.620763 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of7.py
+-rw-r--r--   0        0        0     2875 2024-04-02 21:06:09.640394 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of8.py
+-rw-r--r--   0        0        0     2877 2024-04-02 21:06:09.666604 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of9.py
+-rw-r--r--   0        0        0     3281 2024-04-02 21:06:09.686784 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload.py
+-rw-r--r--   0        0        0     2700 2024-04-02 21:06:09.705656 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py
+-rw-r--r--   0        0        0     2665 2024-04-02 21:06:09.722372 gradientai-1.9.0/gradientai/openapi/client/models/complete_model_success.py
+-rw-r--r--   0        0        0     2619 2024-04-02 21:06:09.739180 gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_body_params.py
+-rw-r--r--   0        0        0     2565 2024-04-02 21:06:09.755475 gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_error.py
+-rw-r--r--   0        0        0     2640 2024-04-02 21:06:09.770734 gradientai-1.9.0/gradientai/openapi/client/models/create_audio_transcription_success.py
+-rw-r--r--   0        0        0     3807 2024-04-02 21:06:09.790028 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params.py
+-rw-r--r--   0        0        0     4559 2024-04-02 21:06:09.803767 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py
+-rw-r--r--   0        0        0     3018 2024-04-02 21:06:09.811376 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
+-rw-r--r--   0        0        0     3165 2024-04-02 21:06:09.819303 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py
+-rw-r--r--   0        0        0     2836 2024-04-02 21:06:09.826269 gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_model.py
+-rw-r--r--   0        0        0     2461 2024-04-02 21:06:09.834119 gradientai-1.9.0/gradientai/openapi/client/models/create_model_error.py
+-rw-r--r--   0        0        0     2457 2024-04-02 21:06:09.842823 gradientai-1.9.0/gradientai/openapi/client/models/create_model_success.py
+-rw-r--r--   0        0        0     3788 2024-04-02 23:02:40.027441 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_body_params.py
+-rw-r--r--   0        0        0     2727 2024-04-02 23:02:40.027522 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_body_params_files_inner.py
+-rw-r--r--   0        0        0     2525 2024-04-02 23:02:40.027595 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_error.py
+-rw-r--r--   0        0        0     2521 2024-04-02 23:02:40.027660 gradientai-1.9.0/gradientai/openapi/client/models/create_rag_collection_success.py
+-rw-r--r--   0        0        0     2461 2024-04-02 21:06:09.918218 gradientai-1.9.0/gradientai/openapi/client/models/delete_model_error.py
+-rw-r--r--   0        0        0     3456 2024-04-02 21:06:09.926059 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params.py
+-rw-r--r--   0        0        0     3228 2024-04-02 21:06:09.936371 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py
+-rw-r--r--   0        0        0     2477 2024-04-02 21:06:09.946388 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_error.py
+-rw-r--r--   0        0        0     3136 2024-04-02 21:06:09.955137 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success.py
+-rw-r--r--   0        0        0     5870 2024-04-02 21:06:09.964168 gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success_entity_value.py
+-rw-r--r--   0        0        0     2453 2024-04-02 21:06:09.971377 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_error.py
+-rw-r--r--   0        0        0     3365 2024-04-02 21:06:09.976832 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success.py
+-rw-r--r--   0        0        0     4761 2024-04-02 21:06:09.985105 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py
+-rw-r--r--   0        0        0     2937 2024-04-02 21:06:09.995158 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py
+-rw-r--r--   0        0        0     3397 2024-04-02 21:06:10.003745 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py
+-rw-r--r--   0        0        0     3774 2024-04-02 21:06:10.009350 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
+-rw-r--r--   0        0        0     3545 2024-04-02 21:06:10.019368 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
+-rw-r--r--   0        0        0     3065 2024-04-02 21:06:10.025975 gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py
+-rw-r--r--   0        0        0     3075 2024-04-02 21:06:10.032424 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params.py
+-rw-r--r--   0        0        0     4023 2024-04-02 21:06:10.039042 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py
+-rw-r--r--   0        0        0     3056 2024-04-02 21:06:10.044989 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
+-rw-r--r--   0        0        0     5780 2024-04-02 21:06:10.053458 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py
+-rw-r--r--   0        0        0     3137 2024-04-02 21:06:10.061882 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
+-rw-r--r--   0        0        0    10150 2024-04-02 21:06:10.068980 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error.py
+-rw-r--r--   0        0        0     2881 2024-04-02 21:06:10.075247 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of.py
+-rw-r--r--   0        0        0     2851 2024-04-02 21:06:10.081189 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py
+-rw-r--r--   0        0        0     2748 2024-04-02 21:06:10.088300 gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_success.py
+-rw-r--r--   0        0        0     2993 2024-04-02 21:06:10.098254 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params.py
+-rw-r--r--   0        0        0     6307 2024-04-02 21:06:10.105052 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source.py
+-rw-r--r--   0        0        0     3023 2024-04-02 21:06:10.138849 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py
+-rw-r--r--   0        0        0     2959 2024-04-02 21:06:10.149368 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py
+-rw-r--r--   0        0        0     2485 2024-04-02 21:06:10.157233 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_error.py
+-rw-r--r--   0        0        0     3047 2024-04-02 21:06:10.165942 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success.py
+-rw-r--r--   0        0        0     3197 2024-04-02 21:06:10.173414 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context.py
+-rw-r--r--   0        0        0     2831 2024-04-02 21:06:10.179649 gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py
+-rw-r--r--   0        0        0     3137 2024-04-02 21:06:10.188248 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params.py
+-rw-r--r--   0        0        0     2629 2024-04-02 21:06:10.194657 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py
+-rw-r--r--   0        0        0     2509 2024-04-02 21:06:10.205377 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_error.py
+-rw-r--r--   0        0        0     3124 2024-04-02 21:06:10.214647 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success.py
+-rw-r--r--   0        0        0     2802 2024-04-02 21:06:10.221585 gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py
+-rw-r--r--   0        0        0     2541 2024-04-02 21:06:10.227642 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_error.py
+-rw-r--r--   0        0        0     6225 2024-04-02 21:06:10.233896 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success.py
+-rw-r--r--   0        0        0     3230 2024-04-02 21:06:10.240370 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of.py
+-rw-r--r--   0        0        0     3331 2024-04-02 21:06:10.245238 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of1.py
+-rw-r--r--   0        0        0     2620 2024-04-02 21:06:10.251490 gradientai-1.9.0/gradientai/openapi/client/models/get_audio_transcription_success_one_of1_result.py
+-rw-r--r--   0        0        0     2437 2024-04-02 21:06:10.256772 gradientai-1.9.0/gradientai/openapi/client/models/get_model_error.py
+-rw-r--r--   0        0        0     3226 2024-04-02 21:06:10.262685 gradientai-1.9.0/gradientai/openapi/client/models/get_model_success.py
+-rw-r--r--   0        0        0     2485 2024-04-02 21:06:10.269520 gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_error.py
+-rw-r--r--   0        0        0     3198 2024-04-02 21:06:10.275832 gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success.py
+-rw-r--r--   0        0        0     2877 2024-04-02 21:06:10.281153 gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py
+-rw-r--r--   0        0        0     2453 2024-04-02 21:06:10.288818 gradientai-1.9.0/gradientai/openapi/client/models/list_models_error.py
+-rw-r--r--   0        0        0     2988 2024-04-02 21:06:10.294142 gradientai-1.9.0/gradientai/openapi/client/models/list_models_success.py
+-rw-r--r--   0        0        0     6222 2024-04-02 21:06:10.300547 gradientai-1.9.0/gradientai/openapi/client/models/list_models_success_models_inner.py
+-rw-r--r--   0        0        0     3202 2024-04-02 21:06:10.306093 gradientai-1.9.0/gradientai/openapi/client/models/model_adapter.py
+-rw-r--r--   0        0        0     2910 2024-04-02 21:06:10.311164 gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_body_params.py
+-rw-r--r--   0        0        0     2525 2024-04-02 21:06:10.316119 gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_error.py
+-rw-r--r--   0        0        0     2625 2024-04-02 21:06:10.322296 gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_success.py
+-rw-r--r--   0        0        0     4281 2024-04-02 21:06:10.327645 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params.py
+-rw-r--r--   0        0        0     2771 2024-04-02 21:06:10.334291 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py
+-rw-r--r--   0        0        0     2509 2024-04-02 21:06:10.339705 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_error.py
+-rw-r--r--   0        0        0     2525 2024-04-02 21:06:10.345591 gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_success.py
+-rw-r--r--   0        0        0     2453 2024-04-02 21:06:10.353564 gradientai-1.9.0/gradientai/openapi/client/models/upload_file_error.py
+-rw-r--r--   0        0        0     2449 2024-04-02 21:06:10.360525 gradientai-1.9.0/gradientai/openapi/client/models/upload_file_success.py
+-rw-r--r--   0        0        0    12904 2024-04-02 21:06:10.522227 gradientai-1.9.0/gradientai/openapi/client/rest.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:06:10.513888 gradientai-1.9.0/gradientai/openapi/client/test/__init__.py
+-rw-r--r--   0        0        0     2273 2024-04-02 23:02:40.027750 gradientai-1.9.0/gradientai/openapi/client/test/test_add_files_to_rag_collection_body_params.py
+-rw-r--r--   0        0        0     1745 2024-04-02 23:02:40.027813 gradientai-1.9.0/gradientai/openapi/client/test/test_add_files_to_rag_collection_error.py
+-rw-r--r--   0        0        0     2004 2024-04-02 21:06:08.808961 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py
+-rw-r--r--   0        0        0     1960 2024-04-02 21:06:08.854945 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py
+-rw-r--r--   0        0        0     1655 2024-04-02 21:06:08.881571 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_error.py
+-rw-r--r--   0        0        0     1697 2024-04-02 21:06:08.967099 gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_success.py
+-rw-r--r--   0        0        0     2039 2024-04-02 21:06:09.063993 gradientai-1.9.0/gradientai/openapi/client/test/test_base_model.py
+-rw-r--r--   0        0        0     1980 2024-04-02 21:06:10.439861 gradientai-1.9.0/gradientai/openapi/client/test/test_blocks_api.py
+-rw-r--r--   0        0        0     2280 2024-04-02 21:06:09.099603 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params.py
+-rw-r--r--   0        0        0     1930 2024-04-02 21:06:09.164507 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py
+-rw-r--r--   0        0        0     1731 2024-04-02 21:06:09.292954 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_rag.py
+-rw-r--r--   0        0        0     2177 2024-04-02 21:06:09.333291 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error.py
+-rw-r--r--   0        0        0     2591 2024-04-02 21:06:09.371930 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of.py
+-rw-r--r--   0        0        0     2257 2024-04-02 21:06:09.406401 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1.py
+-rw-r--r--   0        0        0     1802 2024-04-02 21:06:09.441943 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of10.py
+-rw-r--r--   0        0        0     1812 2024-04-02 21:06:09.518575 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py
+-rw-r--r--   0        0        0     2271 2024-04-02 21:06:09.542666 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of2.py
+-rw-r--r--   0        0        0     1762 2024-04-02 21:06:09.564892 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of3.py
+-rw-r--r--   0        0        0     1804 2024-04-02 21:06:09.581061 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of4.py
+-rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.598195 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of5.py
+-rw-r--r--   0        0        0     1800 2024-04-02 21:06:09.610916 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of6.py
+-rw-r--r--   0        0        0     1782 2024-04-02 21:06:09.625548 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of7.py
+-rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.648082 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of8.py
+-rw-r--r--   0        0        0     1790 2024-04-02 21:06:09.671711 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of9.py
+-rw-r--r--   0        0        0     2235 2024-04-02 21:06:09.691977 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py
+-rw-r--r--   0        0        0     1999 2024-04-02 21:06:09.710627 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py
+-rw-r--r--   0        0        0     1732 2024-04-02 21:06:09.725385 gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_success.py
+-rw-r--r--   0        0        0     1815 2024-04-02 21:06:09.747060 gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_body_params.py
+-rw-r--r--   0        0        0     1753 2024-04-02 21:06:09.758952 gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_error.py
+-rw-r--r--   0        0        0     1795 2024-04-02 21:06:09.778352 gradientai-1.9.0/gradientai/openapi/client/test/test_create_audio_transcription_success.py
+-rw-r--r--   0        0        0     2659 2024-04-02 21:06:09.796918 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params.py
+-rw-r--r--   0        0        0     2349 2024-04-02 21:06:09.806264 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py
+-rw-r--r--   0        0        0     2121 2024-04-02 21:06:09.813285 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py
+-rw-r--r--   0        0        0     2106 2024-04-02 21:06:09.821729 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py
+-rw-r--r--   0        0        0     1788 2024-04-02 21:06:09.828921 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_model.py
+-rw-r--r--   0        0        0     1595 2024-04-02 21:06:09.836385 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_error.py
+-rw-r--r--   0        0        0     1609 2024-04-02 21:06:09.845646 gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_success.py
+-rw-r--r--   0        0        0     2087 2024-04-02 23:02:40.027879 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_body_params.py
+-rw-r--r--   0        0        0     1926 2024-04-02 23:02:40.027954 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_body_params_files_inner.py
+-rw-r--r--   0        0        0     1693 2024-04-02 23:02:40.028029 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_error.py
+-rw-r--r--   0        0        0     1707 2024-04-02 23:02:40.028100 gradientai-1.9.0/gradientai/openapi/client/test/test_create_rag_collection_success.py
+-rw-r--r--   0        0        0     1595 2024-04-02 21:06:09.920600 gradientai-1.9.0/gradientai/openapi/client/test/test_delete_model_error.py
+-rw-r--r--   0        0        0     1087 2024-04-02 21:06:10.458193 gradientai-1.9.0/gradientai/openapi/client/test/test_embeddings_api.py
+-rw-r--r--   0        0        0     2242 2024-04-02 21:06:09.928651 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params.py
+-rw-r--r--   0        0        0     1857 2024-04-02 21:06:09.940584 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py
+-rw-r--r--   0        0        0     1619 2024-04-02 21:06:09.949460 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_error.py
+-rw-r--r--   0        0        0     1747 2024-04-02 21:06:09.957081 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success.py
+-rw-r--r--   0        0        0     1718 2024-04-02 21:06:09.966737 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py
+-rw-r--r--   0        0        0     1583 2024-04-02 21:06:09.973033 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_error.py
+-rw-r--r--   0        0        0     5829 2024-04-02 21:06:09.979063 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success.py
+-rw-r--r--   0        0        0     5055 2024-04-02 21:06:09.987342 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py
+-rw-r--r--   0        0        0     1938 2024-04-02 21:06:09.997669 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py
+-rw-r--r--   0        0        0     3256 2024-04-02 21:06:10.005551 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py
+-rw-r--r--   0        0        0     2800 2024-04-02 21:06:10.010890 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py
+-rw-r--r--   0        0        0     2291 2024-04-02 21:06:10.021591 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py
+-rw-r--r--   0        0        0     2066 2024-04-02 21:06:10.027698 gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py
+-rw-r--r--   0        0        0      876 2024-04-02 21:06:10.466006 gradientai-1.9.0/gradientai/openapi/client/test/test_files_api.py
+-rw-r--r--   0        0        0     2583 2024-04-02 21:06:10.034445 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params.py
+-rw-r--r--   0        0        0     2070 2024-04-02 21:06:10.040640 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py
+-rw-r--r--   0        0        0     2047 2024-04-02 21:06:10.047326 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py
+-rw-r--r--   0        0        0     1844 2024-04-02 21:06:10.055514 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py
+-rw-r--r--   0        0        0     2108 2024-04-02 21:06:10.063530 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py
+-rw-r--r--   0        0        0     2183 2024-04-02 21:06:10.071132 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error.py
+-rw-r--r--   0        0        0     1792 2024-04-02 21:06:10.077033 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py
+-rw-r--r--   0        0        0     1766 2024-04-02 21:06:10.084327 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py
+-rw-r--r--   0        0        0     1748 2024-04-02 21:06:10.090376 gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_success.py
+-rw-r--r--   0        0        0     1758 2024-04-02 21:06:10.100215 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params.py
+-rw-r--r--   0        0        0     1899 2024-04-02 21:06:10.125636 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source.py
+-rw-r--r--   0        0        0     1904 2024-04-02 21:06:10.144238 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py
+-rw-r--r--   0        0        0     1910 2024-04-02 21:06:10.152562 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py
+-rw-r--r--   0        0        0     1631 2024-04-02 21:06:10.159600 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_error.py
+-rw-r--r--   0        0        0     2101 2024-04-02 21:06:10.167754 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success.py
+-rw-r--r--   0        0        0     2299 2024-04-02 21:06:10.175433 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py
+-rw-r--r--   0        0        0     2018 2024-04-02 21:06:10.182073 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py
+-rw-r--r--   0        0        0     2123 2024-04-02 21:06:10.190615 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params.py
+-rw-r--r--   0        0        0     1861 2024-04-02 21:06:10.197672 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py
+-rw-r--r--   0        0        0     1667 2024-04-02 21:06:10.207994 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_error.py
+-rw-r--r--   0        0        0     2299 2024-04-02 21:06:10.217113 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success.py
+-rw-r--r--   0        0        0     2026 2024-04-02 21:06:10.223798 gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py
+-rw-r--r--   0        0        0     1717 2024-04-02 21:06:10.229190 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_error.py
+-rw-r--r--   0        0        0     2126 2024-04-02 21:06:10.236708 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success.py
+-rw-r--r--   0        0        0     1882 2024-04-02 21:06:10.241895 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of.py
+-rw-r--r--   0        0        0     2202 2024-04-02 21:06:10.246805 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1.py
+-rw-r--r--   0        0        0     1883 2024-04-02 21:06:10.253414 gradientai-1.9.0/gradientai/openapi/client/test/test_get_audio_transcription_success_one_of1_result.py
+-rw-r--r--   0        0        0     1559 2024-04-02 21:06:10.258844 gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_error.py
+-rw-r--r--   0        0        0     2193 2024-04-02 21:06:10.264578 gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_success.py
+-rw-r--r--   0        0        0     1631 2024-04-02 21:06:10.272082 gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_error.py
+-rw-r--r--   0        0        0     2101 2024-04-02 21:06:10.277361 gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success.py
+-rw-r--r--   0        0        0     1923 2024-04-02 21:06:10.284407 gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py
+-rw-r--r--   0        0        0     1583 2024-04-02 21:06:10.290426 gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_error.py
+-rw-r--r--   0        0        0     1695 2024-04-02 21:06:10.296286 gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success.py
+-rw-r--r--   0        0        0     2579 2024-04-02 21:06:10.302172 gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success_models_inner.py
+-rw-r--r--   0        0        0     2155 2024-04-02 21:06:10.307900 gradientai-1.9.0/gradientai/openapi/client/test/test_model_adapter.py
+-rw-r--r--   0        0        0     1568 2024-04-02 21:06:10.475138 gradientai-1.9.0/gradientai/openapi/client/test/test_models_api.py
+-rw-r--r--   0        0        0     1844 2024-04-02 21:06:10.312637 gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_body_params.py
+-rw-r--r--   0        0        0     1691 2024-04-02 21:06:10.317720 gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_error.py
+-rw-r--r--   0        0        0     1743 2024-04-02 21:06:10.323929 gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_success.py
+-rw-r--r--   0        0        0     1066 2024-04-02 23:02:40.028172 gradientai-1.9.0/gradientai/openapi/client/test/test_rag_api.py
+-rw-r--r--   0        0        0     2044 2024-04-02 21:06:10.329773 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params.py
+-rw-r--r--   0        0        0     1954 2024-04-02 21:06:10.336161 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py
+-rw-r--r--   0        0        0     1667 2024-04-02 21:06:10.341321 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_error.py
+-rw-r--r--   0        0        0     1691 2024-04-02 21:06:10.347050 gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_success.py
+-rw-r--r--   0        0        0     1583 2024-04-02 21:06:10.355366 gradientai-1.9.0/gradientai/openapi/client/test/test_upload_file_error.py
+-rw-r--r--   0        0        0     1597 2024-04-02 21:06:10.362354 gradientai-1.9.0/gradientai/openapi/client/test/test_upload_file_success.py
+-rw-r--r--   0        0        0    22901 2024-04-02 23:02:40.028355 gradientai-1.9.0/gradientai/openapi/client_README.md
+-rw-r--r--   0        0        0        0 2023-08-31 18:54:00.559055 gradientai-1.9.0/gradientai/py.typed
+-rw-r--r--   0        0        0      210 2023-10-24 19:44:32.690293 gradientai-1.9.0/gradientai/pydantic_models/types.py
+-rw-r--r--   0        0        0     1761 2024-04-05 00:24:39.981741 gradientai-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 gradientai-1.9.0/PKG-INFO
```

### Comparing `gradientai-1.8.1/gradientai/__init__.py` & `gradientai-1.9.0/gradientai/__init__.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/__init__.pyi` & `gradientai-1.9.0/gradientai/__init__.pyi`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/_base_model.py` & `gradientai-1.9.0/gradientai/_base_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/_embeddings_model.py` & `gradientai-1.9.0/gradientai/_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/_gradient.py` & `gradientai-1.9.0/gradientai/_gradient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,54 @@
+import os
+import time
 from types import TracebackType
 from typing import Any, List, Literal, Mapping, Optional, Type, overload
 
 from typing_extensions import Self, assert_never
 
 from gradientai._base_model import BaseModel, CapabilityFilterOption
 from gradientai._embeddings_model import EmbeddingsModel
-from gradientai._model import Model
+from gradientai._model import RAG, Model
 from gradientai._model_adapter import ModelAdapter
+from gradientai._rag import RAGCollection
 from gradientai._types import (
     AnalyzeSentimentParamsExample,
     AnalyzeSentimentResponse,
     AnswerParamsSource,
     AnswerResponse,
     ExtractParamsSchemaValue,
     ExtractPdfResponse,
     ExtractResponse,
     PersonalizeResponse,
     Sentiment,
     SummarizeParamsExample,
     SummarizeParamsLength,
     SummarizeResponse,
+    TranscribeAudioResponse,
 )
 from gradientai.helpers.env_manager import ENV_MANAGER
 from gradientai.openapi.client.api.blocks_api import BlocksApi
 from gradientai.openapi.client.api.embeddings_api import EmbeddingsApi
+from gradientai.openapi.client.api.files_api import FilesApi
 from gradientai.openapi.client.api.models_api import ModelsApi
+from gradientai.openapi.client.api.rag_api import RAGApi
 from gradientai.openapi.client.api_client import ApiClient
 from gradientai.openapi.client.configuration import Configuration
 from gradientai.openapi.client.models.analyze_sentiment_body_params import (
     AnalyzeSentimentBodyParams,
 )
+from gradientai.openapi.client.models.create_audio_transcription_body_params import (
+    CreateAudioTranscriptionBodyParams,
+)
+from gradientai.openapi.client.models.create_rag_collection_body_params import (
+    CreateRagCollectionBodyParams,
+)
+from gradientai.openapi.client.models.create_rag_collection_body_params_files_inner import (
+    CreateRagCollectionBodyParamsFilesInner,
+)
 from gradientai.openapi.client.models.extract_entity_body_params import (
     ExtractEntityBodyParams,
 )
 from gradientai.openapi.client.models.generate_answer_body_params import (
     GenerateAnswerBodyParams,
 )
 from gradientai.openapi.client.models.model_adapter import (
@@ -47,15 +62,17 @@
 )
 
 
 class Gradient:
     _api_client: ApiClient
     _blocks_api: BlocksApi
     _embeddings_api: EmbeddingsApi
+    _files_api: FilesApi
     _models_api: ModelsApi
+    _rag_api: RAGApi
     _workspace_id: str
 
     def __init__(
         self,
         *,
         access_token: Optional[str] = None,
         host: Optional[str] = None,
@@ -94,15 +111,17 @@
             Configuration(
                 access_token=access_token,
                 host=host,
             )
         )
         self._blocks_api = BlocksApi(self._api_client)
         self._embeddings_api = EmbeddingsApi(self._api_client)
+        self._files_api = FilesApi(self._api_client)
         self._models_api = ModelsApi(self._api_client)
+        self._rag_api = RAGApi(self._api_client)
         self._workspace_id = workspace_id
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
         self,
@@ -327,15 +346,15 @@
             key: value.actual_instance for key, value in result.entity.items()
         }
         return ExtractResponse(entity=entity)
 
     def extract_pdf(
         self,
         *,
-        filepath: str,
+        filepath: os.PathLike,
     ) -> ExtractPdfResponse:
         result = self._blocks_api.extract_pdf(
             x_gradient_workspace_id=self._workspace_id,
             file=filepath,
         )
 
         pages = [
@@ -381,7 +400,90 @@
         ]
 
         return ExtractPdfResponse(
             pages=pages,
             text=result.text,
             title=result.title,
         )
+
+    def transcribe_audio(
+        self,
+        *,
+        filepath: os.PathLike,
+    ) -> TranscribeAudioResponse:
+        file_result = self._files_api.upload_file(
+            file=filepath,
+            type="audioFile",
+            x_gradient_workspace_id=self._workspace_id,
+        )
+
+        create_transcription_result = self._blocks_api.create_audio_transcription(
+            create_audio_transcription_body_params=CreateAudioTranscriptionBodyParams(
+                file_id=file_result.id,
+            ),
+            x_gradient_workspace_id=self._workspace_id,
+        )
+
+        while True:
+            get_transcription_result = self._blocks_api.get_audio_transcription(
+                transcription_id=create_transcription_result.transcription_id,
+                x_gradient_workspace_id=self._workspace_id,
+            )
+
+            status = get_transcription_result.actual_instance.status
+            if (
+                status == "pending"
+                or status == "pendingCancellation"
+                or status == "running"
+            ):
+                time.sleep(1)
+                continue
+
+            if status == "cancelled" or status == "failed":
+                raise Exception("Unable to get transcription")
+
+            if status == "succeeded":
+                return TranscribeAudioResponse(
+                    text=get_transcription_result.actual_instance.result.text
+                )
+
+            raise Exception(f"Received unexpected status: {status}")
+
+    def create_rag_collection(
+        self,
+        *,
+        name: str,
+        slug: str,
+        filepaths: Optional[List[os.PathLike]] = None,
+    ) -> RAGCollection:
+        if filepaths is None:
+            filepaths = []
+
+        file_results = [
+            self._files_api.upload_file(
+                file=file_,
+                type="ragUserFile",
+                x_gradient_workspace_id=self._workspace_id,
+            )
+            for file_ in filepaths
+        ]
+
+        rag_result = self._rag_api.create_rag_collection(
+            x_gradient_workspace_id=self._workspace_id,
+            create_rag_collection_body_params=CreateRagCollectionBodyParams(
+                name=name,
+                slug=slug,
+                files=[
+                    CreateRagCollectionBodyParamsFilesInner(
+                        id=file_result.id, name=os.path.basename(file_path)
+                    )
+                    for (file_result, file_path) in zip(file_results, filepaths)
+                ],
+            ),
+        )
+
+        return RAGCollection(
+            id=rag_result.id,
+            files_api=self._files_api,
+            rag_api=self._rag_api,
+            workspace_id=self._workspace_id,
+        )
```

### Comparing `gradientai-1.8.1/gradientai/_model.py` & `gradientai-1.9.0/gradientai/_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/_model_adapter.py` & `gradientai-1.9.0/gradientai/_model_adapter.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/_types.py` & `gradientai-1.9.0/gradientai/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,7 +117,11 @@
     textBlocks: List[ExtractPdfResponseTextBlock]
 
 
 class ExtractPdfResponse(TypedDict):
     pages: List[ExtractPdfResponsePage]
     text: str
     title: Optional[str]
+
+
+class TranscribeAudioResponse(TypedDict):
+    text: str
```

### Comparing `gradientai-1.8.1/gradientai/helpers/asyncio_threads.py` & `gradientai-1.9.0/gradientai/helpers/asyncio_threads.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/helpers/env_manager.py` & `gradientai-1.9.0/gradientai/helpers/env_manager.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/__init__.py` & `gradientai-1.9.0/gradientai/openapi/client/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,26 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Gradient AI API
 
     Interface for interacting with Gradient AI.  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@gradient.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-# import apis into sdk package
-from gradientai.openapi.client.api.blocks_api import BlocksApi
-from gradientai.openapi.client.api.embeddings_api import EmbeddingsApi
-from gradientai.openapi.client.api.models_api import ModelsApi
-
-# import ApiClient
-from gradientai.openapi.client.api_response import ApiResponse
-from gradientai.openapi.client.api_client import ApiClient
-from gradientai.openapi.client.configuration import Configuration
-from gradientai.openapi.client.exceptions import OpenApiException
-from gradientai.openapi.client.exceptions import ApiTypeError
-from gradientai.openapi.client.exceptions import ApiValueError
-from gradientai.openapi.client.exceptions import ApiKeyError
-from gradientai.openapi.client.exceptions import ApiAttributeError
-from gradientai.openapi.client.exceptions import ApiException
-
-# import models into sdk package
+# import models into model package
+from gradientai.openapi.client.models.add_files_to_rag_collection_body_params import AddFilesToRagCollectionBodyParams
+from gradientai.openapi.client.models.add_files_to_rag_collection_error import AddFilesToRagCollectionError
 from gradientai.openapi.client.models.analyze_sentiment_body_params import AnalyzeSentimentBodyParams
 from gradientai.openapi.client.models.analyze_sentiment_body_params_examples_inner import AnalyzeSentimentBodyParamsExamplesInner
 from gradientai.openapi.client.models.analyze_sentiment_error import AnalyzeSentimentError
 from gradientai.openapi.client.models.analyze_sentiment_success import AnalyzeSentimentSuccess
 from gradientai.openapi.client.models.base_model import BaseModel
 from gradientai.openapi.client.models.complete_model_body_params import CompleteModelBodyParams
 from gradientai.openapi.client.models.complete_model_body_params_guidance import CompleteModelBodyParamsGuidance
@@ -52,21 +37,28 @@
 from gradientai.openapi.client.models.complete_model_error_one_of6 import CompleteModelErrorOneOf6
 from gradientai.openapi.client.models.complete_model_error_one_of7 import CompleteModelErrorOneOf7
 from gradientai.openapi.client.models.complete_model_error_one_of8 import CompleteModelErrorOneOf8
 from gradientai.openapi.client.models.complete_model_error_one_of9 import CompleteModelErrorOneOf9
 from gradientai.openapi.client.models.complete_model_error_one_of_payload import CompleteModelErrorOneOfPayload
 from gradientai.openapi.client.models.complete_model_error_one_of_payload_flagged_content_inner import CompleteModelErrorOneOfPayloadFlaggedContentInner
 from gradientai.openapi.client.models.complete_model_success import CompleteModelSuccess
+from gradientai.openapi.client.models.create_audio_transcription_body_params import CreateAudioTranscriptionBodyParams
+from gradientai.openapi.client.models.create_audio_transcription_error import CreateAudioTranscriptionError
+from gradientai.openapi.client.models.create_audio_transcription_success import CreateAudioTranscriptionSuccess
 from gradientai.openapi.client.models.create_model_body_params import CreateModelBodyParams
 from gradientai.openapi.client.models.create_model_body_params_initial_hyperparameters import CreateModelBodyParamsInitialHyperparameters
 from gradientai.openapi.client.models.create_model_body_params_initial_hyperparameters_lora_hyperparameters import CreateModelBodyParamsInitialHyperparametersLoraHyperparameters
 from gradientai.openapi.client.models.create_model_body_params_initial_hyperparameters_training_arguments import CreateModelBodyParamsInitialHyperparametersTrainingArguments
 from gradientai.openapi.client.models.create_model_body_params_model import CreateModelBodyParamsModel
 from gradientai.openapi.client.models.create_model_error import CreateModelError
 from gradientai.openapi.client.models.create_model_success import CreateModelSuccess
+from gradientai.openapi.client.models.create_rag_collection_body_params import CreateRagCollectionBodyParams
+from gradientai.openapi.client.models.create_rag_collection_body_params_files_inner import CreateRagCollectionBodyParamsFilesInner
+from gradientai.openapi.client.models.create_rag_collection_error import CreateRagCollectionError
+from gradientai.openapi.client.models.create_rag_collection_success import CreateRagCollectionSuccess
 from gradientai.openapi.client.models.delete_model_error import DeleteModelError
 from gradientai.openapi.client.models.extract_entity_body_params import ExtractEntityBodyParams
 from gradientai.openapi.client.models.extract_entity_body_params_schema_value import ExtractEntityBodyParamsSchemaValue
 from gradientai.openapi.client.models.extract_entity_error import ExtractEntityError
 from gradientai.openapi.client.models.extract_entity_success import ExtractEntitySuccess
 from gradientai.openapi.client.models.extract_entity_success_entity_value import ExtractEntitySuccessEntityValue
 from gradientai.openapi.client.models.extract_pdf_error import ExtractPdfError
@@ -95,14 +87,19 @@
 from gradientai.openapi.client.models.generate_answer_success_rag_context import GenerateAnswerSuccessRagContext
 from gradientai.openapi.client.models.generate_answer_success_rag_context_documents_inner import GenerateAnswerSuccessRagContextDocumentsInner
 from gradientai.openapi.client.models.generate_embedding_body_params import GenerateEmbeddingBodyParams
 from gradientai.openapi.client.models.generate_embedding_body_params_inputs_inner import GenerateEmbeddingBodyParamsInputsInner
 from gradientai.openapi.client.models.generate_embedding_error import GenerateEmbeddingError
 from gradientai.openapi.client.models.generate_embedding_success import GenerateEmbeddingSuccess
 from gradientai.openapi.client.models.generate_embedding_success_embeddings_inner import GenerateEmbeddingSuccessEmbeddingsInner
+from gradientai.openapi.client.models.get_audio_transcription_error import GetAudioTranscriptionError
+from gradientai.openapi.client.models.get_audio_transcription_success import GetAudioTranscriptionSuccess
+from gradientai.openapi.client.models.get_audio_transcription_success_one_of import GetAudioTranscriptionSuccessOneOf
+from gradientai.openapi.client.models.get_audio_transcription_success_one_of1 import GetAudioTranscriptionSuccessOneOf1
+from gradientai.openapi.client.models.get_audio_transcription_success_one_of1_result import GetAudioTranscriptionSuccessOneOf1Result
 from gradientai.openapi.client.models.get_model_error import GetModelError
 from gradientai.openapi.client.models.get_model_success import GetModelSuccess
 from gradientai.openapi.client.models.list_embeddings_error import ListEmbeddingsError
 from gradientai.openapi.client.models.list_embeddings_success import ListEmbeddingsSuccess
 from gradientai.openapi.client.models.list_embeddings_success_embeddings_models_inner import ListEmbeddingsSuccessEmbeddingsModelsInner
 from gradientai.openapi.client.models.list_models_error import ListModelsError
 from gradientai.openapi.client.models.list_models_success import ListModelsSuccess
@@ -111,7 +108,9 @@
 from gradientai.openapi.client.models.personalize_document_body_params import PersonalizeDocumentBodyParams
 from gradientai.openapi.client.models.personalize_document_error import PersonalizeDocumentError
 from gradientai.openapi.client.models.personalize_document_success import PersonalizeDocumentSuccess
 from gradientai.openapi.client.models.summarize_document_body_params import SummarizeDocumentBodyParams
 from gradientai.openapi.client.models.summarize_document_body_params_examples_inner import SummarizeDocumentBodyParamsExamplesInner
 from gradientai.openapi.client.models.summarize_document_error import SummarizeDocumentError
 from gradientai.openapi.client.models.summarize_document_success import SummarizeDocumentSuccess
+from gradientai.openapi.client.models.upload_file_error import UploadFileError
+from gradientai.openapi.client.models.upload_file_success import UploadFileSuccess
```

### Comparing `gradientai-1.8.1/gradientai/openapi/client/api/blocks_api.py` & `gradientai-1.9.0/gradientai/openapi/client/api/models_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,96 +16,97 @@
 import re  # noqa: F401
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBytes, StrictStr, constr
+from pydantic import StrictBool, StrictStr, constr
 
-from typing import Union
+from typing import Any, Dict, Optional
 
-from gradientai.openapi.client.models.analyze_sentiment_body_params import AnalyzeSentimentBodyParams
-from gradientai.openapi.client.models.analyze_sentiment_success import AnalyzeSentimentSuccess
-from gradientai.openapi.client.models.extract_entity_body_params import ExtractEntityBodyParams
-from gradientai.openapi.client.models.extract_entity_success import ExtractEntitySuccess
-from gradientai.openapi.client.models.extract_pdf_success import ExtractPdfSuccess
-from gradientai.openapi.client.models.generate_answer_body_params import GenerateAnswerBodyParams
-from gradientai.openapi.client.models.generate_answer_success import GenerateAnswerSuccess
-from gradientai.openapi.client.models.personalize_document_body_params import PersonalizeDocumentBodyParams
-from gradientai.openapi.client.models.personalize_document_success import PersonalizeDocumentSuccess
-from gradientai.openapi.client.models.summarize_document_body_params import SummarizeDocumentBodyParams
-from gradientai.openapi.client.models.summarize_document_success import SummarizeDocumentSuccess
+from gradientai.openapi.client.models.complete_model_body_params import CompleteModelBodyParams
+from gradientai.openapi.client.models.complete_model_success import CompleteModelSuccess
+from gradientai.openapi.client.models.create_model_body_params import CreateModelBodyParams
+from gradientai.openapi.client.models.create_model_success import CreateModelSuccess
+from gradientai.openapi.client.models.fine_tune_model_body_params import FineTuneModelBodyParams
+from gradientai.openapi.client.models.fine_tune_model_success import FineTuneModelSuccess
+from gradientai.openapi.client.models.get_model_success import GetModelSuccess
+from gradientai.openapi.client.models.list_models_success import ListModelsSuccess
 
 from gradientai.openapi.client.api_client import ApiClient
 from gradientai.openapi.client.api_response import ApiResponse
 from gradientai.openapi.client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class BlocksApi(object):
+class ModelsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def analyze_sentiment(self, x_gradient_workspace_id : constr(strict=True, min_length=1), analyze_sentiment_body_params : AnalyzeSentimentBodyParams, **kwargs) -> AnalyzeSentimentSuccess:  # noqa: E501
-        """Sentiment analysis  # noqa: E501
+    def complete_model(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), complete_model_body_params : CompleteModelBodyParams, **kwargs) -> CompleteModelSuccess:  # noqa: E501
+        """Complete model  # noqa: E501
 
-        Analyzes text to determine the emotional tone of the message.  # noqa: E501
+        Completes your fine-tuned model with the specified prompt string. The model will generate a completion.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.analyze_sentiment(x_gradient_workspace_id, analyze_sentiment_body_params, async_req=True)
+        >>> thread = api.complete_model(id, x_gradient_workspace_id, complete_model_body_params, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param analyze_sentiment_body_params: (required)
-        :type analyze_sentiment_body_params: AnalyzeSentimentBodyParams
+        :param complete_model_body_params: (required)
+        :type complete_model_body_params: CompleteModelBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AnalyzeSentimentSuccess
+        :rtype: CompleteModelSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the analyze_sentiment_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.analyze_sentiment_with_http_info(x_gradient_workspace_id, analyze_sentiment_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the complete_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.complete_model_with_http_info(id, x_gradient_workspace_id, complete_model_body_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def analyze_sentiment_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), analyze_sentiment_body_params : AnalyzeSentimentBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Sentiment analysis  # noqa: E501
+    def complete_model_with_http_info(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), complete_model_body_params : CompleteModelBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Complete model  # noqa: E501
 
-        Analyzes text to determine the emotional tone of the message.  # noqa: E501
+        Completes your fine-tuned model with the specified prompt string. The model will generate a completion.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.analyze_sentiment_with_http_info(x_gradient_workspace_id, analyze_sentiment_body_params, async_req=True)
+        >>> thread = api.complete_model_with_http_info(id, x_gradient_workspace_id, complete_model_body_params, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param analyze_sentiment_body_params: (required)
-        :type analyze_sentiment_body_params: AnalyzeSentimentBodyParams
+        :param complete_model_body_params: (required)
+        :type complete_model_body_params: CompleteModelBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -120,22 +121,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(AnalyzeSentimentSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(CompleteModelSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'id',
             'x_gradient_workspace_id',
-            'analyze_sentiment_body_params'
+            'complete_model_body_params'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -146,38 +148,41 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method analyze_sentiment" % _key
+                    " to method complete_model" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['analyze_sentiment_body_params'] is not None:
-            _body_params = _params['analyze_sentiment_body_params']
+        if _params['complete_model_body_params'] is not None:
+            _body_params = _params['complete_model_body_params']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -186,20 +191,20 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "AnalyzeSentimentSuccess",
-            '4XX': "AnalyzeSentimentError",
+            '200': "CompleteModelSuccess",
+            '4XX': "CompleteModelError",
         }
 
         return self.api_client.call_api(
-            '/blocks/analyze-sentiment', 'POST',
+            '/models/{id}/complete', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -208,59 +213,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def extract_entity(self, x_gradient_workspace_id : constr(strict=True, min_length=1), extract_entity_body_params : ExtractEntityBodyParams, **kwargs) -> ExtractEntitySuccess:  # noqa: E501
-        """Entity extraction  # noqa: E501
+    def create_model(self, x_gradient_workspace_id : constr(strict=True, min_length=1), create_model_body_params : CreateModelBodyParams, **kwargs) -> CreateModelSuccess:  # noqa: E501
+        """Create model  # noqa: E501
 
-        Extracts an entity from the document with the specified fields and types.  # noqa: E501
+        Creates a new instance of a model based on a specified model from the existing list.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.extract_entity(x_gradient_workspace_id, extract_entity_body_params, async_req=True)
+        >>> thread = api.create_model(x_gradient_workspace_id, create_model_body_params, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param extract_entity_body_params: (required)
-        :type extract_entity_body_params: ExtractEntityBodyParams
+        :param create_model_body_params: (required)
+        :type create_model_body_params: CreateModelBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ExtractEntitySuccess
+        :rtype: CreateModelSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the extract_entity_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.extract_entity_with_http_info(x_gradient_workspace_id, extract_entity_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the create_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.create_model_with_http_info(x_gradient_workspace_id, create_model_body_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def extract_entity_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), extract_entity_body_params : ExtractEntityBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Entity extraction  # noqa: E501
+    def create_model_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), create_model_body_params : CreateModelBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Create model  # noqa: E501
 
-        Extracts an entity from the document with the specified fields and types.  # noqa: E501
+        Creates a new instance of a model based on a specified model from the existing list.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.extract_entity_with_http_info(x_gradient_workspace_id, extract_entity_body_params, async_req=True)
+        >>> thread = api.create_model_with_http_info(x_gradient_workspace_id, create_model_body_params, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param extract_entity_body_params: (required)
-        :type extract_entity_body_params: ExtractEntityBodyParams
+        :param create_model_body_params: (required)
+        :type create_model_body_params: CreateModelBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -275,22 +280,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ExtractEntitySuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(CreateModelSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'x_gradient_workspace_id',
-            'extract_entity_body_params'
+            'create_model_body_params'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -301,15 +306,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method extract_entity" % _key
+                    " to method create_model" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -323,16 +328,16 @@
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['extract_entity_body_params'] is not None:
-            _body_params = _params['extract_entity_body_params']
+        if _params['create_model_body_params'] is not None:
+            _body_params = _params['create_model_body_params']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -341,20 +346,20 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "ExtractEntitySuccess",
-            '4XX': "ExtractEntityError",
+            '200': "CreateModelSuccess",
+            '4XX': "CreateModelError",
         }
 
         return self.api_client.call_api(
-            '/blocks/extract', 'POST',
+            '/models', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -363,59 +368,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def extract_pdf(self, x_gradient_workspace_id : constr(strict=True, min_length=1), file : Union[StrictBytes, StrictStr], **kwargs) -> ExtractPdfSuccess:  # noqa: E501
-        """PDF extraction  # noqa: E501
+    def delete_model(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> object:  # noqa: E501
+        """Delete model  # noqa: E501
 
-        Extracts content from the PDF.  # noqa: E501
+        Deletes the fine-tuned model.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.extract_pdf(x_gradient_workspace_id, file, async_req=True)
+        >>> thread = api.delete_model(id, x_gradient_workspace_id, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param file: (required)
-        :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ExtractPdfSuccess
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the extract_pdf_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.extract_pdf_with_http_info(x_gradient_workspace_id, file, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the delete_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.delete_model_with_http_info(id, x_gradient_workspace_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def extract_pdf_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), file : Union[StrictBytes, StrictStr], **kwargs) -> ApiResponse:  # noqa: E501
-        """PDF extraction  # noqa: E501
+    def delete_model_with_http_info(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> ApiResponse:  # noqa: E501
+        """Delete model  # noqa: E501
 
-        Extracts content from the PDF.  # noqa: E501
+        Deletes the fine-tuned model.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.extract_pdf_with_http_info(x_gradient_workspace_id, file, async_req=True)
+        >>> thread = api.delete_model_with_http_info(id, x_gradient_workspace_id, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param file: (required)
-        :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -430,22 +435,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ExtractPdfSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'x_gradient_workspace_id',
-            'file'
+            'id',
+            'x_gradient_workspace_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -456,60 +461,53 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method extract_pdf" % _key
+                    " to method delete_model" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
-        if _params['file']:
-            _files['file'] = _params['file']
-
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['multipart/form-data']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "ExtractPdfSuccess",
-            '4XX': "ExtractPdfError",
+            '200': "object",
+            '4XX': "DeleteModelError",
         }
 
         return self.api_client.call_api(
-            '/blocks/extract-pdf', 'POST',
+            '/models/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -518,59 +516,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def generate_answer(self, x_gradient_workspace_id : constr(strict=True, min_length=1), generate_answer_body_params : GenerateAnswerBodyParams, **kwargs) -> GenerateAnswerSuccess:  # noqa: E501
-        """Document question & answer  # noqa: E501
+    def fine_tune_model(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), fine_tune_model_body_params : FineTuneModelBodyParams, **kwargs) -> FineTuneModelSuccess:  # noqa: E501
+        """Fine-tune model  # noqa: E501
 
-        Answers questions using the provided context.  # noqa: E501
+        Fine-tunes the specified model with your data samples.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.generate_answer(x_gradient_workspace_id, generate_answer_body_params, async_req=True)
+        >>> thread = api.fine_tune_model(id, x_gradient_workspace_id, fine_tune_model_body_params, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param generate_answer_body_params: (required)
-        :type generate_answer_body_params: GenerateAnswerBodyParams
+        :param fine_tune_model_body_params: (required)
+        :type fine_tune_model_body_params: FineTuneModelBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GenerateAnswerSuccess
+        :rtype: FineTuneModelSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the generate_answer_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.generate_answer_with_http_info(x_gradient_workspace_id, generate_answer_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the fine_tune_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.fine_tune_model_with_http_info(id, x_gradient_workspace_id, fine_tune_model_body_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def generate_answer_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), generate_answer_body_params : GenerateAnswerBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Document question & answer  # noqa: E501
+    def fine_tune_model_with_http_info(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), fine_tune_model_body_params : FineTuneModelBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Fine-tune model  # noqa: E501
 
-        Answers questions using the provided context.  # noqa: E501
+        Fine-tunes the specified model with your data samples.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.generate_answer_with_http_info(x_gradient_workspace_id, generate_answer_body_params, async_req=True)
+        >>> thread = api.fine_tune_model_with_http_info(id, x_gradient_workspace_id, fine_tune_model_body_params, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param generate_answer_body_params: (required)
-        :type generate_answer_body_params: GenerateAnswerBodyParams
+        :param fine_tune_model_body_params: (required)
+        :type fine_tune_model_body_params: FineTuneModelBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -585,22 +587,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GenerateAnswerSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(FineTuneModelSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'id',
             'x_gradient_workspace_id',
-            'generate_answer_body_params'
+            'fine_tune_model_body_params'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -611,38 +614,41 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method generate_answer" % _key
+                    " to method fine_tune_model" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['generate_answer_body_params'] is not None:
-            _body_params = _params['generate_answer_body_params']
+        if _params['fine_tune_model_body_params'] is not None:
+            _body_params = _params['fine_tune_model_body_params']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -651,20 +657,20 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "GenerateAnswerSuccess",
-            '4XX': "GenerateAnswerError",
+            '200': "FineTuneModelSuccess",
+            '4XX': "FineTuneModelError",
         }
 
         return self.api_client.call_api(
-            '/blocks/answer', 'POST',
+            '/models/{id}/fine-tune', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -673,59 +679,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def personalize_document(self, x_gradient_workspace_id : constr(strict=True, min_length=1), personalize_document_body_params : PersonalizeDocumentBodyParams, **kwargs) -> PersonalizeDocumentSuccess:  # noqa: E501
-        """Document personalization  # noqa: E501
+    def get_model(self, id : constr(strict=True, max_length=50, min_length=50), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> GetModelSuccess:  # noqa: E501
+        """Describe model  # noqa: E501
 
-        Personalizes the document in a tone and style specific to the described target audience.  # noqa: E501
+        Describes the specified model, including the model ID, name, and base model ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.personalize_document(x_gradient_workspace_id, personalize_document_body_params, async_req=True)
+        >>> thread = api.get_model(id, x_gradient_workspace_id, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param personalize_document_body_params: (required)
-        :type personalize_document_body_params: PersonalizeDocumentBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PersonalizeDocumentSuccess
+        :rtype: GetModelSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the personalize_document_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.personalize_document_with_http_info(x_gradient_workspace_id, personalize_document_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the get_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.get_model_with_http_info(id, x_gradient_workspace_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def personalize_document_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), personalize_document_body_params : PersonalizeDocumentBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Document personalization  # noqa: E501
+    def get_model_with_http_info(self, id : constr(strict=True, max_length=50, min_length=50), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> ApiResponse:  # noqa: E501
+        """Describe model  # noqa: E501
 
-        Personalizes the document in a tone and style specific to the described target audience.  # noqa: E501
+        Describes the specified model, including the model ID, name, and base model ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.personalize_document_with_http_info(x_gradient_workspace_id, personalize_document_body_params, async_req=True)
+        >>> thread = api.get_model_with_http_info(id, x_gradient_workspace_id, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param personalize_document_body_params: (required)
-        :type personalize_document_body_params: PersonalizeDocumentBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -740,22 +746,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PersonalizeDocumentSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetModelSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'x_gradient_workspace_id',
-            'personalize_document_body_params'
+            'id',
+            'x_gradient_workspace_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -766,60 +772,53 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method personalize_document" % _key
+                    " to method get_model" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['personalize_document_body_params'] is not None:
-            _body_params = _params['personalize_document_body_params']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "PersonalizeDocumentSuccess",
-            '4XX': "PersonalizeDocumentError",
+            '200': "GetModelSuccess",
+            '4XX': "GetModelError",
         }
 
         return self.api_client.call_api(
-            '/blocks/personalize', 'POST',
+            '/models/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -828,59 +827,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def summarize_document(self, x_gradient_workspace_id : constr(strict=True, min_length=1), summarize_document_body_params : SummarizeDocumentBodyParams, **kwargs) -> SummarizeDocumentSuccess:  # noqa: E501
-        """Document summary  # noqa: E501
+    def list_models(self, x_gradient_workspace_id : constr(strict=True, min_length=1), capability : Optional[StrictStr] = None, only_base : Optional[StrictBool] = None, **kwargs) -> ListModelsSuccess:  # noqa: E501
+        """List available models  # noqa: E501
 
-        Generates a summary of the document using the provided guidance.  # noqa: E501
+        Lists the currently available models in the selected workspace and provides basic information, such as the model name, ID and whether it is a base or fine-tuned model.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.summarize_document(x_gradient_workspace_id, summarize_document_body_params, async_req=True)
+        >>> thread = api.list_models(x_gradient_workspace_id, capability, only_base, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param summarize_document_body_params: (required)
-        :type summarize_document_body_params: SummarizeDocumentBodyParams
+        :param capability:
+        :type capability: str
+        :param only_base:
+        :type only_base: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: SummarizeDocumentSuccess
+        :rtype: ListModelsSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the summarize_document_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.summarize_document_with_http_info(x_gradient_workspace_id, summarize_document_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the list_models_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.list_models_with_http_info(x_gradient_workspace_id, capability, only_base, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def summarize_document_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), summarize_document_body_params : SummarizeDocumentBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Document summary  # noqa: E501
+    def list_models_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), capability : Optional[StrictStr] = None, only_base : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """List available models  # noqa: E501
 
-        Generates a summary of the document using the provided guidance.  # noqa: E501
+        Lists the currently available models in the selected workspace and provides basic information, such as the model name, ID and whether it is a base or fine-tuned model.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.summarize_document_with_http_info(x_gradient_workspace_id, summarize_document_body_params, async_req=True)
+        >>> thread = api.list_models_with_http_info(x_gradient_workspace_id, capability, only_base, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param summarize_document_body_params: (required)
-        :type summarize_document_body_params: SummarizeDocumentBodyParams
+        :param capability:
+        :type capability: str
+        :param only_base:
+        :type only_base: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -895,22 +898,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(SummarizeDocumentSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(ListModelsSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'x_gradient_workspace_id',
-            'summarize_document_body_params'
+            'capability',
+            'only_base'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -921,60 +925,56 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method summarize_document" % _key
+                    " to method list_models" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('capability') is not None:  # noqa: E501
+            _query_params.append(('capability', _params['capability']))
+
+        if _params.get('only_base') is not None:  # noqa: E501
+            _query_params.append(('onlyBase', _params['only_base']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['summarize_document_body_params'] is not None:
-            _body_params = _params['summarize_document_body_params']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "SummarizeDocumentSuccess",
-            '4XX': "SummarizeDocumentError",
+            '200': "ListModelsSuccess",
+            '4XX': "ListModelsError",
         }
 
         return self.api_client.call_api(
-            '/blocks/summarize', 'POST',
+            '/models', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `gradientai-1.8.1/gradientai/openapi/client/api/embeddings_api.py` & `gradientai-1.9.0/gradientai/openapi/client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/api/models_api.py` & `gradientai-1.9.0/gradientai/openapi/client/api/blocks_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,97 +16,99 @@
 import re  # noqa: F401
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictStr, constr
+from pydantic import StrictBytes, StrictStr, constr
 
-from typing import Any, Dict, Optional
+from typing import Union
 
-from gradientai.openapi.client.models.complete_model_body_params import CompleteModelBodyParams
-from gradientai.openapi.client.models.complete_model_success import CompleteModelSuccess
-from gradientai.openapi.client.models.create_model_body_params import CreateModelBodyParams
-from gradientai.openapi.client.models.create_model_success import CreateModelSuccess
-from gradientai.openapi.client.models.fine_tune_model_body_params import FineTuneModelBodyParams
-from gradientai.openapi.client.models.fine_tune_model_success import FineTuneModelSuccess
-from gradientai.openapi.client.models.get_model_success import GetModelSuccess
-from gradientai.openapi.client.models.list_models_success import ListModelsSuccess
+from gradientai.openapi.client.models.analyze_sentiment_body_params import AnalyzeSentimentBodyParams
+from gradientai.openapi.client.models.analyze_sentiment_success import AnalyzeSentimentSuccess
+from gradientai.openapi.client.models.create_audio_transcription_body_params import CreateAudioTranscriptionBodyParams
+from gradientai.openapi.client.models.create_audio_transcription_success import CreateAudioTranscriptionSuccess
+from gradientai.openapi.client.models.extract_entity_body_params import ExtractEntityBodyParams
+from gradientai.openapi.client.models.extract_entity_success import ExtractEntitySuccess
+from gradientai.openapi.client.models.extract_pdf_success import ExtractPdfSuccess
+from gradientai.openapi.client.models.generate_answer_body_params import GenerateAnswerBodyParams
+from gradientai.openapi.client.models.generate_answer_success import GenerateAnswerSuccess
+from gradientai.openapi.client.models.get_audio_transcription_success import GetAudioTranscriptionSuccess
+from gradientai.openapi.client.models.personalize_document_body_params import PersonalizeDocumentBodyParams
+from gradientai.openapi.client.models.personalize_document_success import PersonalizeDocumentSuccess
+from gradientai.openapi.client.models.summarize_document_body_params import SummarizeDocumentBodyParams
+from gradientai.openapi.client.models.summarize_document_success import SummarizeDocumentSuccess
 
 from gradientai.openapi.client.api_client import ApiClient
 from gradientai.openapi.client.api_response import ApiResponse
 from gradientai.openapi.client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ModelsApi(object):
+class BlocksApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def complete_model(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), complete_model_body_params : CompleteModelBodyParams, **kwargs) -> CompleteModelSuccess:  # noqa: E501
-        """Complete model  # noqa: E501
+    def analyze_sentiment(self, x_gradient_workspace_id : constr(strict=True, min_length=1), analyze_sentiment_body_params : AnalyzeSentimentBodyParams, **kwargs) -> AnalyzeSentimentSuccess:  # noqa: E501
+        """Sentiment analysis  # noqa: E501
 
-        Completes your fine-tuned model with the specified prompt string. The model will generate a completion.  # noqa: E501
+        Analyzes text to determine the emotional tone of the message.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.complete_model(id, x_gradient_workspace_id, complete_model_body_params, async_req=True)
+        >>> thread = api.analyze_sentiment(x_gradient_workspace_id, analyze_sentiment_body_params, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param complete_model_body_params: (required)
-        :type complete_model_body_params: CompleteModelBodyParams
+        :param analyze_sentiment_body_params: (required)
+        :type analyze_sentiment_body_params: AnalyzeSentimentBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: CompleteModelSuccess
+        :rtype: AnalyzeSentimentSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the complete_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.complete_model_with_http_info(id, x_gradient_workspace_id, complete_model_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the analyze_sentiment_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.analyze_sentiment_with_http_info(x_gradient_workspace_id, analyze_sentiment_body_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def complete_model_with_http_info(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), complete_model_body_params : CompleteModelBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Complete model  # noqa: E501
+    def analyze_sentiment_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), analyze_sentiment_body_params : AnalyzeSentimentBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Sentiment analysis  # noqa: E501
 
-        Completes your fine-tuned model with the specified prompt string. The model will generate a completion.  # noqa: E501
+        Analyzes text to determine the emotional tone of the message.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.complete_model_with_http_info(id, x_gradient_workspace_id, complete_model_body_params, async_req=True)
+        >>> thread = api.analyze_sentiment_with_http_info(x_gradient_workspace_id, analyze_sentiment_body_params, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param complete_model_body_params: (required)
-        :type complete_model_body_params: CompleteModelBodyParams
+        :param analyze_sentiment_body_params: (required)
+        :type analyze_sentiment_body_params: AnalyzeSentimentBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -121,23 +123,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(CompleteModelSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(AnalyzeSentimentSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
             'x_gradient_workspace_id',
-            'complete_model_body_params'
+            'analyze_sentiment_body_params'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -148,41 +149,38 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method complete_model" % _key
+                    " to method analyze_sentiment" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['complete_model_body_params'] is not None:
-            _body_params = _params['complete_model_body_params']
+        if _params['analyze_sentiment_body_params'] is not None:
+            _body_params = _params['analyze_sentiment_body_params']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -191,20 +189,20 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "CompleteModelSuccess",
-            '4XX': "CompleteModelError",
+            '200': "AnalyzeSentimentSuccess",
+            '4XX': "AnalyzeSentimentError",
         }
 
         return self.api_client.call_api(
-            '/models/{id}/complete', 'POST',
+            '/blocks/analyze-sentiment', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -213,59 +211,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_model(self, x_gradient_workspace_id : constr(strict=True, min_length=1), create_model_body_params : CreateModelBodyParams, **kwargs) -> CreateModelSuccess:  # noqa: E501
-        """Create model  # noqa: E501
+    def create_audio_transcription(self, x_gradient_workspace_id : constr(strict=True, min_length=1), create_audio_transcription_body_params : CreateAudioTranscriptionBodyParams, **kwargs) -> CreateAudioTranscriptionSuccess:  # noqa: E501
+        """Create audio transcription  # noqa: E501
 
-        Creates a new instance of a model based on a specified model from the existing list.  # noqa: E501
+        Creates an audio transcription job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_model(x_gradient_workspace_id, create_model_body_params, async_req=True)
+        >>> thread = api.create_audio_transcription(x_gradient_workspace_id, create_audio_transcription_body_params, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param create_model_body_params: (required)
-        :type create_model_body_params: CreateModelBodyParams
+        :param create_audio_transcription_body_params: (required)
+        :type create_audio_transcription_body_params: CreateAudioTranscriptionBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: CreateModelSuccess
+        :rtype: CreateAudioTranscriptionSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the create_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.create_model_with_http_info(x_gradient_workspace_id, create_model_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the create_audio_transcription_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.create_audio_transcription_with_http_info(x_gradient_workspace_id, create_audio_transcription_body_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_model_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), create_model_body_params : CreateModelBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Create model  # noqa: E501
+    def create_audio_transcription_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), create_audio_transcription_body_params : CreateAudioTranscriptionBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Create audio transcription  # noqa: E501
 
-        Creates a new instance of a model based on a specified model from the existing list.  # noqa: E501
+        Creates an audio transcription job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_model_with_http_info(x_gradient_workspace_id, create_model_body_params, async_req=True)
+        >>> thread = api.create_audio_transcription_with_http_info(x_gradient_workspace_id, create_audio_transcription_body_params, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param create_model_body_params: (required)
-        :type create_model_body_params: CreateModelBodyParams
+        :param create_audio_transcription_body_params: (required)
+        :type create_audio_transcription_body_params: CreateAudioTranscriptionBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -280,22 +278,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(CreateModelSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(CreateAudioTranscriptionSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'x_gradient_workspace_id',
-            'create_model_body_params'
+            'create_audio_transcription_body_params'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -306,15 +304,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_model" % _key
+                    " to method create_audio_transcription" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -328,16 +326,16 @@
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['create_model_body_params'] is not None:
-            _body_params = _params['create_model_body_params']
+        if _params['create_audio_transcription_body_params'] is not None:
+            _body_params = _params['create_audio_transcription_body_params']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -346,20 +344,20 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "CreateModelSuccess",
-            '4XX': "CreateModelError",
+            '200': "CreateAudioTranscriptionSuccess",
+            '4XX': "CreateAudioTranscriptionError",
         }
 
         return self.api_client.call_api(
-            '/models', 'POST',
+            '/blocks/transcription', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -368,59 +366,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_model(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> object:  # noqa: E501
-        """Delete model  # noqa: E501
+    def extract_entity(self, x_gradient_workspace_id : constr(strict=True, min_length=1), extract_entity_body_params : ExtractEntityBodyParams, **kwargs) -> ExtractEntitySuccess:  # noqa: E501
+        """Entity extraction  # noqa: E501
 
-        Deletes the fine-tuned model.  # noqa: E501
+        Extracts an entity from the document with the specified fields and types.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_model(id, x_gradient_workspace_id, async_req=True)
+        >>> thread = api.extract_entity(x_gradient_workspace_id, extract_entity_body_params, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
+        :param extract_entity_body_params: (required)
+        :type extract_entity_body_params: ExtractEntityBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: object
+        :rtype: ExtractEntitySuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the delete_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.delete_model_with_http_info(id, x_gradient_workspace_id, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the extract_entity_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.extract_entity_with_http_info(x_gradient_workspace_id, extract_entity_body_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_model_with_http_info(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> ApiResponse:  # noqa: E501
-        """Delete model  # noqa: E501
+    def extract_entity_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), extract_entity_body_params : ExtractEntityBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Entity extraction  # noqa: E501
 
-        Deletes the fine-tuned model.  # noqa: E501
+        Extracts an entity from the document with the specified fields and types.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_model_with_http_info(id, x_gradient_workspace_id, async_req=True)
+        >>> thread = api.extract_entity_with_http_info(x_gradient_workspace_id, extract_entity_body_params, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
+        :param extract_entity_body_params: (required)
+        :type extract_entity_body_params: ExtractEntityBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -435,22 +433,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(ExtractEntitySuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'x_gradient_workspace_id'
+            'x_gradient_workspace_id',
+            'extract_entity_body_params'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -461,53 +459,60 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_model" % _key
+                    " to method extract_entity" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
+        if _params['extract_entity_body_params'] is not None:
+            _body_params = _params['extract_entity_body_params']
+
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "object",
-            '4XX': "DeleteModelError",
+            '200': "ExtractEntitySuccess",
+            '4XX': "ExtractEntityError",
         }
 
         return self.api_client.call_api(
-            '/models/{id}', 'DELETE',
+            '/blocks/extract', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -516,63 +521,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def fine_tune_model(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), fine_tune_model_body_params : FineTuneModelBodyParams, **kwargs) -> FineTuneModelSuccess:  # noqa: E501
-        """Fine-tune model  # noqa: E501
+    def extract_pdf(self, x_gradient_workspace_id : constr(strict=True, min_length=1), file : Union[StrictBytes, StrictStr], **kwargs) -> ExtractPdfSuccess:  # noqa: E501
+        """PDF extraction  # noqa: E501
 
-        Fine-tunes the specified model with your data samples.  # noqa: E501
+        Extracts content from the PDF.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.fine_tune_model(id, x_gradient_workspace_id, fine_tune_model_body_params, async_req=True)
+        >>> thread = api.extract_pdf(x_gradient_workspace_id, file, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param fine_tune_model_body_params: (required)
-        :type fine_tune_model_body_params: FineTuneModelBodyParams
+        :param file: (required)
+        :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: FineTuneModelSuccess
+        :rtype: ExtractPdfSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the fine_tune_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.fine_tune_model_with_http_info(id, x_gradient_workspace_id, fine_tune_model_body_params, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the extract_pdf_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.extract_pdf_with_http_info(x_gradient_workspace_id, file, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def fine_tune_model_with_http_info(self, id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), fine_tune_model_body_params : FineTuneModelBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
-        """Fine-tune model  # noqa: E501
+    def extract_pdf_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), file : Union[StrictBytes, StrictStr], **kwargs) -> ApiResponse:  # noqa: E501
+        """PDF extraction  # noqa: E501
 
-        Fine-tunes the specified model with your data samples.  # noqa: E501
+        Extracts content from the PDF.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.fine_tune_model_with_http_info(id, x_gradient_workspace_id, fine_tune_model_body_params, async_req=True)
+        >>> thread = api.extract_pdf_with_http_info(x_gradient_workspace_id, file, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param fine_tune_model_body_params: (required)
-        :type fine_tune_model_body_params: FineTuneModelBodyParams
+        :param file: (required)
+        :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -587,23 +588,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(FineTuneModelSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(ExtractPdfSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
             'x_gradient_workspace_id',
-            'fine_tune_model_body_params'
+            'file'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -614,41 +614,193 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method fine_tune_model" % _key
+                    " to method extract_pdf" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        if _params['x_gradient_workspace_id']:
+            _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        if _params['file']:
+            _files['file'] = _params['file']
+
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['multipart/form-data']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['AccessToken']  # noqa: E501
+
+        _response_types_map = {
+            '200': "ExtractPdfSuccess",
+            '4XX': "ExtractPdfError",
+        }
+
+        return self.api_client.call_api(
+            '/blocks/extract-pdf', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def generate_answer(self, x_gradient_workspace_id : constr(strict=True, min_length=1), generate_answer_body_params : GenerateAnswerBodyParams, **kwargs) -> GenerateAnswerSuccess:  # noqa: E501
+        """Document question & answer  # noqa: E501
+
+        Answers questions using the provided context.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.generate_answer(x_gradient_workspace_id, generate_answer_body_params, async_req=True)
+        >>> result = thread.get()
+
+        :param x_gradient_workspace_id: (required)
+        :type x_gradient_workspace_id: str
+        :param generate_answer_body_params: (required)
+        :type generate_answer_body_params: GenerateAnswerBodyParams
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenerateAnswerSuccess
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the generate_answer_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.generate_answer_with_http_info(x_gradient_workspace_id, generate_answer_body_params, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def generate_answer_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), generate_answer_body_params : GenerateAnswerBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Document question & answer  # noqa: E501
+
+        Answers questions using the provided context.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.generate_answer_with_http_info(x_gradient_workspace_id, generate_answer_body_params, async_req=True)
+        >>> result = thread.get()
+
+        :param x_gradient_workspace_id: (required)
+        :type x_gradient_workspace_id: str
+        :param generate_answer_body_params: (required)
+        :type generate_answer_body_params: GenerateAnswerBodyParams
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenerateAnswerSuccess, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'x_gradient_workspace_id',
+            'generate_answer_body_params'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method generate_answer" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['fine_tune_model_body_params'] is not None:
-            _body_params = _params['fine_tune_model_body_params']
+        if _params['generate_answer_body_params'] is not None:
+            _body_params = _params['generate_answer_body_params']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -657,20 +809,20 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "FineTuneModelSuccess",
-            '4XX': "FineTuneModelError",
+            '200': "GenerateAnswerSuccess",
+            '4XX': "GenerateAnswerError",
         }
 
         return self.api_client.call_api(
-            '/models/{id}/fine-tune', 'POST',
+            '/blocks/answer', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -679,57 +831,57 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_model(self, id : constr(strict=True, max_length=50, min_length=50), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> GetModelSuccess:  # noqa: E501
-        """Describe model  # noqa: E501
+    def get_audio_transcription(self, transcription_id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> GetAudioTranscriptionSuccess:  # noqa: E501
+        """Get audio transcription  # noqa: E501
 
-        Describes the specified model, including the model ID, name, and base model ID.  # noqa: E501
+        Gets the result of the audio transcription job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_model(id, x_gradient_workspace_id, async_req=True)
+        >>> thread = api.get_audio_transcription(transcription_id, x_gradient_workspace_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
+        :param transcription_id: (required)
+        :type transcription_id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetModelSuccess
+        :rtype: GetAudioTranscriptionSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the get_model_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_model_with_http_info(id, x_gradient_workspace_id, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the get_audio_transcription_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.get_audio_transcription_with_http_info(transcription_id, x_gradient_workspace_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_model_with_http_info(self, id : constr(strict=True, max_length=50, min_length=50), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> ApiResponse:  # noqa: E501
-        """Describe model  # noqa: E501
+    def get_audio_transcription_with_http_info(self, transcription_id : constr(strict=True, min_length=1), x_gradient_workspace_id : constr(strict=True, min_length=1), **kwargs) -> ApiResponse:  # noqa: E501
+        """Get audio transcription  # noqa: E501
 
-        Describes the specified model, including the model ID, name, and base model ID.  # noqa: E501
+        Gets the result of the audio transcription job.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_model_with_http_info(id, x_gradient_workspace_id, async_req=True)
+        >>> thread = api.get_audio_transcription_with_http_info(transcription_id, x_gradient_workspace_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
+        :param transcription_id: (required)
+        :type transcription_id: str
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
@@ -746,21 +898,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetModelSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetAudioTranscriptionSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
+            'transcription_id',
             'x_gradient_workspace_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -772,29 +924,29 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_model" % _key
+                    " to method get_audio_transcription" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
 
         # process the query parameters
         _query_params = []
+        if _params.get('transcription_id') is not None:  # noqa: E501
+            _query_params.append(('transcriptionId', _params['transcription_id']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
@@ -805,20 +957,20 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetModelSuccess",
-            '4XX': "GetModelError",
+            '200': "GetAudioTranscriptionSuccess",
+            '4XX': "GetAudioTranscriptionError",
         }
 
         return self.api_client.call_api(
-            '/models/{id}', 'GET',
+            '/blocks/transcription', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -827,63 +979,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_models(self, x_gradient_workspace_id : constr(strict=True, min_length=1), capability : Optional[StrictStr] = None, only_base : Optional[StrictBool] = None, **kwargs) -> ListModelsSuccess:  # noqa: E501
-        """List available models  # noqa: E501
+    def personalize_document(self, x_gradient_workspace_id : constr(strict=True, min_length=1), personalize_document_body_params : PersonalizeDocumentBodyParams, **kwargs) -> PersonalizeDocumentSuccess:  # noqa: E501
+        """Document personalization  # noqa: E501
 
-        Lists the currently available models in the selected workspace and provides basic information, such as the model name, ID and whether it is a base or fine-tuned model.  # noqa: E501
+        Personalizes the document in a tone and style specific to the described target audience.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_models(x_gradient_workspace_id, capability, only_base, async_req=True)
+        >>> thread = api.personalize_document(x_gradient_workspace_id, personalize_document_body_params, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param capability:
-        :type capability: str
-        :param only_base:
-        :type only_base: bool
+        :param personalize_document_body_params: (required)
+        :type personalize_document_body_params: PersonalizeDocumentBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ListModelsSuccess
+        :rtype: PersonalizeDocumentSuccess
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            raise ValueError("Error! Please call the list_models_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.list_models_with_http_info(x_gradient_workspace_id, capability, only_base, **kwargs)  # noqa: E501
+            raise ValueError("Error! Please call the personalize_document_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.personalize_document_with_http_info(x_gradient_workspace_id, personalize_document_body_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_models_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), capability : Optional[StrictStr] = None, only_base : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """List available models  # noqa: E501
+    def personalize_document_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), personalize_document_body_params : PersonalizeDocumentBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Document personalization  # noqa: E501
 
-        Lists the currently available models in the selected workspace and provides basic information, such as the model name, ID and whether it is a base or fine-tuned model.  # noqa: E501
+        Personalizes the document in a tone and style specific to the described target audience.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_models_with_http_info(x_gradient_workspace_id, capability, only_base, async_req=True)
+        >>> thread = api.personalize_document_with_http_info(x_gradient_workspace_id, personalize_document_body_params, async_req=True)
         >>> result = thread.get()
 
         :param x_gradient_workspace_id: (required)
         :type x_gradient_workspace_id: str
-        :param capability:
-        :type capability: str
-        :param only_base:
-        :type only_base: bool
+        :param personalize_document_body_params: (required)
+        :type personalize_document_body_params: PersonalizeDocumentBodyParams
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -898,23 +1046,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ListModelsSuccess, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PersonalizeDocumentSuccess, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'x_gradient_workspace_id',
-            'capability',
-            'only_base'
+            'personalize_document_body_params'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -925,56 +1072,215 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_models" % _key
+                    " to method personalize_document" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('capability') is not None:  # noqa: E501
-            _query_params.append(('capability', _params['capability']))
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        if _params['x_gradient_workspace_id']:
+            _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['personalize_document_body_params'] is not None:
+            _body_params = _params['personalize_document_body_params']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['AccessToken']  # noqa: E501
 
-        if _params.get('only_base') is not None:  # noqa: E501
-            _query_params.append(('onlyBase', _params['only_base']))
+        _response_types_map = {
+            '200': "PersonalizeDocumentSuccess",
+            '4XX': "PersonalizeDocumentError",
+        }
 
+        return self.api_client.call_api(
+            '/blocks/personalize', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def summarize_document(self, x_gradient_workspace_id : constr(strict=True, min_length=1), summarize_document_body_params : SummarizeDocumentBodyParams, **kwargs) -> SummarizeDocumentSuccess:  # noqa: E501
+        """Document summary  # noqa: E501
+
+        Generates a summary of the document using the provided guidance.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.summarize_document(x_gradient_workspace_id, summarize_document_body_params, async_req=True)
+        >>> result = thread.get()
+
+        :param x_gradient_workspace_id: (required)
+        :type x_gradient_workspace_id: str
+        :param summarize_document_body_params: (required)
+        :type summarize_document_body_params: SummarizeDocumentBodyParams
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: SummarizeDocumentSuccess
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the summarize_document_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.summarize_document_with_http_info(x_gradient_workspace_id, summarize_document_body_params, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def summarize_document_with_http_info(self, x_gradient_workspace_id : constr(strict=True, min_length=1), summarize_document_body_params : SummarizeDocumentBodyParams, **kwargs) -> ApiResponse:  # noqa: E501
+        """Document summary  # noqa: E501
+
+        Generates a summary of the document using the provided guidance.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.summarize_document_with_http_info(x_gradient_workspace_id, summarize_document_body_params, async_req=True)
+        >>> result = thread.get()
+
+        :param x_gradient_workspace_id: (required)
+        :type x_gradient_workspace_id: str
+        :param summarize_document_body_params: (required)
+        :type summarize_document_body_params: SummarizeDocumentBodyParams
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(SummarizeDocumentSuccess, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'x_gradient_workspace_id',
+            'summarize_document_body_params'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method summarize_document" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         if _params['x_gradient_workspace_id']:
             _header_params['x-gradient-workspace-id'] = _params['x_gradient_workspace_id']
 
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
+        if _params['summarize_document_body_params'] is not None:
+            _body_params = _params['summarize_document_body_params']
+
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['AccessToken']  # noqa: E501
 
         _response_types_map = {
-            '200': "ListModelsSuccess",
-            '4XX': "ListModelsError",
+            '200': "SummarizeDocumentSuccess",
+            '4XX': "SummarizeDocumentError",
         }
 
         return self.api_client.call_api(
-            '/models', 'GET',
+            '/blocks/summarize', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `gradientai-1.8.1/gradientai/openapi/client/api_client.py` & `gradientai-1.9.0/gradientai/openapi/client/api_client.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/api_response.py` & `gradientai-1.9.0/gradientai/openapi/client/api_response.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/configuration.py` & `gradientai-1.9.0/gradientai/openapi/client/configuration.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/BaseModel.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/BaseModel.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/BlocksApi.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ModelsApi.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# gradientai.openapi.client.BlocksApi
+# gradientai.openapi.client.ModelsApi
 
 All URIs are relative to *https://api.gradient.ai/api*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**analyze_sentiment**](BlocksApi.md#analyze_sentiment) | **POST** /blocks/analyze-sentiment | Sentiment analysis
-[**extract_entity**](BlocksApi.md#extract_entity) | **POST** /blocks/extract | Entity extraction
-[**extract_pdf**](BlocksApi.md#extract_pdf) | **POST** /blocks/extract-pdf | PDF extraction
-[**generate_answer**](BlocksApi.md#generate_answer) | **POST** /blocks/answer | Document question &amp; answer
-[**personalize_document**](BlocksApi.md#personalize_document) | **POST** /blocks/personalize | Document personalization
-[**summarize_document**](BlocksApi.md#summarize_document) | **POST** /blocks/summarize | Document summary
+[**complete_model**](ModelsApi.md#complete_model) | **POST** /models/{id}/complete | Complete model
+[**create_model**](ModelsApi.md#create_model) | **POST** /models | Create model
+[**delete_model**](ModelsApi.md#delete_model) | **DELETE** /models/{id} | Delete model
+[**fine_tune_model**](ModelsApi.md#fine_tune_model) | **POST** /models/{id}/fine-tune | Fine-tune model
+[**get_model**](ModelsApi.md#get_model) | **GET** /models/{id} | Describe model
+[**list_models**](ModelsApi.md#list_models) | **GET** /models | List available models
 
 
-# **analyze_sentiment**
-> AnalyzeSentimentSuccess analyze_sentiment(x_gradient_workspace_id, analyze_sentiment_body_params)
+# **complete_model**
+> CompleteModelSuccess complete_model(id, x_gradient_workspace_id, complete_model_body_params)
 
-Sentiment analysis
+Complete model
 
-Analyzes text to determine the emotional tone of the message.
+Completes your fine-tuned model with the specified prompt string. The model will generate a completion.
 
 ### Example
 
 * Bearer Authentication (AccessToken):
 ```python
 import time
 import os
 import gradientai.openapi.client
-from gradientai.openapi.client.models.analyze_sentiment_body_params import AnalyzeSentimentBodyParams
-from gradientai.openapi.client.models.analyze_sentiment_success import AnalyzeSentimentSuccess
+from gradientai.openapi.client.models.complete_model_body_params import CompleteModelBodyParams
+from gradientai.openapi.client.models.complete_model_success import CompleteModelSuccess
 from gradientai.openapi.client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.gradient.ai/api
 # See configuration.py for a list of all supported configuration parameters.
 configuration = gradientai.openapi.client.Configuration(
     host = "https://api.gradient.ai/api"
@@ -45,38 +45,40 @@
 configuration = gradientai.openapi.client.Configuration(
     access_token = os.environ["BEARER_TOKEN"]
 )
 
 # Enter a context with an instance of the API client
 with gradientai.openapi.client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = gradientai.openapi.client.BlocksApi(api_client)
+    api_instance = gradientai.openapi.client.ModelsApi(api_client)
+    id = 'id_example' # str | 
     x_gradient_workspace_id = 'x_gradient_workspace_id_example' # str | 
-    analyze_sentiment_body_params = gradientai.openapi.client.AnalyzeSentimentBodyParams() # AnalyzeSentimentBodyParams | 
+    complete_model_body_params = gradientai.openapi.client.CompleteModelBodyParams() # CompleteModelBodyParams | 
 
     try:
-        # Sentiment analysis
-        api_response = api_instance.analyze_sentiment(x_gradient_workspace_id, analyze_sentiment_body_params)
-        print("The response of BlocksApi->analyze_sentiment:\n")
+        # Complete model
+        api_response = api_instance.complete_model(id, x_gradient_workspace_id, complete_model_body_params)
+        print("The response of ModelsApi->complete_model:\n")
         pprint(api_response)
     except Exception as e:
-        print("Exception when calling BlocksApi->analyze_sentiment: %s\n" % e)
+        print("Exception when calling ModelsApi->complete_model: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
+ **id** | **str**|  | 
  **x_gradient_workspace_id** | **str**|  | 
- **analyze_sentiment_body_params** | [**AnalyzeSentimentBodyParams**](AnalyzeSentimentBodyParams.md)|  | 
+ **complete_model_body_params** | [**CompleteModelBodyParams**](CompleteModelBodyParams.md)|  | 
 
 ### Return type
 
-[**AnalyzeSentimentSuccess**](AnalyzeSentimentSuccess.md)
+[**CompleteModelSuccess**](CompleteModelSuccess.md)
 
 ### Authorization
 
 [AccessToken](../README.md#AccessToken)
 
 ### HTTP request headers
 
@@ -87,30 +89,30 @@
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Success |  -  |
 **4XX** | Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **extract_entity**
-> ExtractEntitySuccess extract_entity(x_gradient_workspace_id, extract_entity_body_params)
+# **create_model**
+> CreateModelSuccess create_model(x_gradient_workspace_id, create_model_body_params)
 
-Entity extraction
+Create model
 
-Extracts an entity from the document with the specified fields and types.
+Creates a new instance of a model based on a specified model from the existing list.
 
 ### Example
 
 * Bearer Authentication (AccessToken):
 ```python
 import time
 import os
 import gradientai.openapi.client
-from gradientai.openapi.client.models.extract_entity_body_params import ExtractEntityBodyParams
-from gradientai.openapi.client.models.extract_entity_success import ExtractEntitySuccess
+from gradientai.openapi.client.models.create_model_body_params import CreateModelBodyParams
+from gradientai.openapi.client.models.create_model_success import CreateModelSuccess
 from gradientai.openapi.client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.gradient.ai/api
 # See configuration.py for a list of all supported configuration parameters.
 configuration = gradientai.openapi.client.Configuration(
     host = "https://api.gradient.ai/api"
@@ -124,38 +126,38 @@
 configuration = gradientai.openapi.client.Configuration(
     access_token = os.environ["BEARER_TOKEN"]
 )
 
 # Enter a context with an instance of the API client
 with gradientai.openapi.client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = gradientai.openapi.client.BlocksApi(api_client)
+    api_instance = gradientai.openapi.client.ModelsApi(api_client)
     x_gradient_workspace_id = 'x_gradient_workspace_id_example' # str | 
-    extract_entity_body_params = gradientai.openapi.client.ExtractEntityBodyParams() # ExtractEntityBodyParams | 
+    create_model_body_params = gradientai.openapi.client.CreateModelBodyParams() # CreateModelBodyParams | 
 
     try:
-        # Entity extraction
-        api_response = api_instance.extract_entity(x_gradient_workspace_id, extract_entity_body_params)
-        print("The response of BlocksApi->extract_entity:\n")
+        # Create model
+        api_response = api_instance.create_model(x_gradient_workspace_id, create_model_body_params)
+        print("The response of ModelsApi->create_model:\n")
         pprint(api_response)
     except Exception as e:
-        print("Exception when calling BlocksApi->extract_entity: %s\n" % e)
+        print("Exception when calling ModelsApi->create_model: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **x_gradient_workspace_id** | **str**|  | 
- **extract_entity_body_params** | [**ExtractEntityBodyParams**](ExtractEntityBodyParams.md)|  | 
+ **create_model_body_params** | [**CreateModelBodyParams**](CreateModelBodyParams.md)|  | 
 
 ### Return type
 
-[**ExtractEntitySuccess**](ExtractEntitySuccess.md)
+[**CreateModelSuccess**](CreateModelSuccess.md)
 
 ### Authorization
 
 [AccessToken](../README.md#AccessToken)
 
 ### HTTP request headers
 
@@ -166,29 +168,28 @@
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Success |  -  |
 **4XX** | Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **extract_pdf**
-> ExtractPdfSuccess extract_pdf(x_gradient_workspace_id, file)
+# **delete_model**
+> object delete_model(id, x_gradient_workspace_id)
 
-PDF extraction
+Delete model
 
-Extracts content from the PDF.
+Deletes the fine-tuned model.
 
 ### Example
 
 * Bearer Authentication (AccessToken):
 ```python
 import time
 import os
 import gradientai.openapi.client
-from gradientai.openapi.client.models.extract_pdf_success import ExtractPdfSuccess
 from gradientai.openapi.client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.gradient.ai/api
 # See configuration.py for a list of all supported configuration parameters.
 configuration = gradientai.openapi.client.Configuration(
     host = "https://api.gradient.ai/api"
@@ -202,72 +203,72 @@
 configuration = gradientai.openapi.client.Configuration(
     access_token = os.environ["BEARER_TOKEN"]
 )
 
 # Enter a context with an instance of the API client
 with gradientai.openapi.client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = gradientai.openapi.client.BlocksApi(api_client)
+    api_instance = gradientai.openapi.client.ModelsApi(api_client)
+    id = 'id_example' # str | 
     x_gradient_workspace_id = 'x_gradient_workspace_id_example' # str | 
-    file = None # bytearray | 
 
     try:
-        # PDF extraction
-        api_response = api_instance.extract_pdf(x_gradient_workspace_id, file)
-        print("The response of BlocksApi->extract_pdf:\n")
+        # Delete model
+        api_response = api_instance.delete_model(id, x_gradient_workspace_id)
+        print("The response of ModelsApi->delete_model:\n")
         pprint(api_response)
     except Exception as e:
-        print("Exception when calling BlocksApi->extract_pdf: %s\n" % e)
+        print("Exception when calling ModelsApi->delete_model: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
+ **id** | **str**|  | 
  **x_gradient_workspace_id** | **str**|  | 
- **file** | **bytearray**|  | 
 
 ### Return type
 
-[**ExtractPdfSuccess**](ExtractPdfSuccess.md)
+**object**
 
 ### Authorization
 
 [AccessToken](../README.md#AccessToken)
 
 ### HTTP request headers
 
- - **Content-Type**: multipart/form-data
+ - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Success |  -  |
 **4XX** | Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **generate_answer**
-> GenerateAnswerSuccess generate_answer(x_gradient_workspace_id, generate_answer_body_params)
+# **fine_tune_model**
+> FineTuneModelSuccess fine_tune_model(id, x_gradient_workspace_id, fine_tune_model_body_params)
 
-Document question & answer
+Fine-tune model
 
-Answers questions using the provided context.
+Fine-tunes the specified model with your data samples.
 
 ### Example
 
 * Bearer Authentication (AccessToken):
 ```python
 import time
 import os
 import gradientai.openapi.client
-from gradientai.openapi.client.models.generate_answer_body_params import GenerateAnswerBodyParams
-from gradientai.openapi.client.models.generate_answer_success import GenerateAnswerSuccess
+from gradientai.openapi.client.models.fine_tune_model_body_params import FineTuneModelBodyParams
+from gradientai.openapi.client.models.fine_tune_model_success import FineTuneModelSuccess
 from gradientai.openapi.client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.gradient.ai/api
 # See configuration.py for a list of all supported configuration parameters.
 configuration = gradientai.openapi.client.Configuration(
     host = "https://api.gradient.ai/api"
@@ -281,38 +282,40 @@
 configuration = gradientai.openapi.client.Configuration(
     access_token = os.environ["BEARER_TOKEN"]
 )
 
 # Enter a context with an instance of the API client
 with gradientai.openapi.client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = gradientai.openapi.client.BlocksApi(api_client)
+    api_instance = gradientai.openapi.client.ModelsApi(api_client)
+    id = 'id_example' # str | 
     x_gradient_workspace_id = 'x_gradient_workspace_id_example' # str | 
-    generate_answer_body_params = gradientai.openapi.client.GenerateAnswerBodyParams() # GenerateAnswerBodyParams | 
+    fine_tune_model_body_params = gradientai.openapi.client.FineTuneModelBodyParams() # FineTuneModelBodyParams | 
 
     try:
-        # Document question & answer
-        api_response = api_instance.generate_answer(x_gradient_workspace_id, generate_answer_body_params)
-        print("The response of BlocksApi->generate_answer:\n")
+        # Fine-tune model
+        api_response = api_instance.fine_tune_model(id, x_gradient_workspace_id, fine_tune_model_body_params)
+        print("The response of ModelsApi->fine_tune_model:\n")
         pprint(api_response)
     except Exception as e:
-        print("Exception when calling BlocksApi->generate_answer: %s\n" % e)
+        print("Exception when calling ModelsApi->fine_tune_model: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
+ **id** | **str**|  | 
  **x_gradient_workspace_id** | **str**|  | 
- **generate_answer_body_params** | [**GenerateAnswerBodyParams**](GenerateAnswerBodyParams.md)|  | 
+ **fine_tune_model_body_params** | [**FineTuneModelBodyParams**](FineTuneModelBodyParams.md)|  | 
 
 ### Return type
 
-[**GenerateAnswerSuccess**](GenerateAnswerSuccess.md)
+[**FineTuneModelSuccess**](FineTuneModelSuccess.md)
 
 ### Authorization
 
 [AccessToken](../README.md#AccessToken)
 
 ### HTTP request headers
 
@@ -323,30 +326,29 @@
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Success |  -  |
 **4XX** | Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **personalize_document**
-> PersonalizeDocumentSuccess personalize_document(x_gradient_workspace_id, personalize_document_body_params)
+# **get_model**
+> GetModelSuccess get_model(id, x_gradient_workspace_id)
 
-Document personalization
+Describe model
 
-Personalizes the document in a tone and style specific to the described target audience.
+Describes the specified model, including the model ID, name, and base model ID.
 
 ### Example
 
 * Bearer Authentication (AccessToken):
 ```python
 import time
 import os
 import gradientai.openapi.client
-from gradientai.openapi.client.models.personalize_document_body_params import PersonalizeDocumentBodyParams
-from gradientai.openapi.client.models.personalize_document_success import PersonalizeDocumentSuccess
+from gradientai.openapi.client.models.get_model_success import GetModelSuccess
 from gradientai.openapi.client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.gradient.ai/api
 # See configuration.py for a list of all supported configuration parameters.
 configuration = gradientai.openapi.client.Configuration(
     host = "https://api.gradient.ai/api"
@@ -360,72 +362,71 @@
 configuration = gradientai.openapi.client.Configuration(
     access_token = os.environ["BEARER_TOKEN"]
 )
 
 # Enter a context with an instance of the API client
 with gradientai.openapi.client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = gradientai.openapi.client.BlocksApi(api_client)
+    api_instance = gradientai.openapi.client.ModelsApi(api_client)
+    id = 'id_example' # str | 
     x_gradient_workspace_id = 'x_gradient_workspace_id_example' # str | 
-    personalize_document_body_params = gradientai.openapi.client.PersonalizeDocumentBodyParams() # PersonalizeDocumentBodyParams | 
 
     try:
-        # Document personalization
-        api_response = api_instance.personalize_document(x_gradient_workspace_id, personalize_document_body_params)
-        print("The response of BlocksApi->personalize_document:\n")
+        # Describe model
+        api_response = api_instance.get_model(id, x_gradient_workspace_id)
+        print("The response of ModelsApi->get_model:\n")
         pprint(api_response)
     except Exception as e:
-        print("Exception when calling BlocksApi->personalize_document: %s\n" % e)
+        print("Exception when calling ModelsApi->get_model: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
+ **id** | **str**|  | 
  **x_gradient_workspace_id** | **str**|  | 
- **personalize_document_body_params** | [**PersonalizeDocumentBodyParams**](PersonalizeDocumentBodyParams.md)|  | 
 
 ### Return type
 
-[**PersonalizeDocumentSuccess**](PersonalizeDocumentSuccess.md)
+[**GetModelSuccess**](GetModelSuccess.md)
 
 ### Authorization
 
 [AccessToken](../README.md#AccessToken)
 
 ### HTTP request headers
 
- - **Content-Type**: application/json
+ - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Success |  -  |
 **4XX** | Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **summarize_document**
-> SummarizeDocumentSuccess summarize_document(x_gradient_workspace_id, summarize_document_body_params)
+# **list_models**
+> ListModelsSuccess list_models(x_gradient_workspace_id, capability=capability, only_base=only_base)
 
-Document summary
+List available models
 
-Generates a summary of the document using the provided guidance.
+Lists the currently available models in the selected workspace and provides basic information, such as the model name, ID and whether it is a base or fine-tuned model.
 
 ### Example
 
 * Bearer Authentication (AccessToken):
 ```python
 import time
 import os
 import gradientai.openapi.client
-from gradientai.openapi.client.models.summarize_document_body_params import SummarizeDocumentBodyParams
-from gradientai.openapi.client.models.summarize_document_success import SummarizeDocumentSuccess
+from gradientai.openapi.client.models.list_models_success import ListModelsSuccess
 from gradientai.openapi.client.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.gradient.ai/api
 # See configuration.py for a list of all supported configuration parameters.
 configuration = gradientai.openapi.client.Configuration(
     host = "https://api.gradient.ai/api"
@@ -439,46 +440,48 @@
 configuration = gradientai.openapi.client.Configuration(
     access_token = os.environ["BEARER_TOKEN"]
 )
 
 # Enter a context with an instance of the API client
 with gradientai.openapi.client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = gradientai.openapi.client.BlocksApi(api_client)
+    api_instance = gradientai.openapi.client.ModelsApi(api_client)
     x_gradient_workspace_id = 'x_gradient_workspace_id_example' # str | 
-    summarize_document_body_params = gradientai.openapi.client.SummarizeDocumentBodyParams() # SummarizeDocumentBodyParams | 
+    capability = 'fineTune' # str |  (optional) (default to 'fineTune')
+    only_base = False # bool |  (optional) (default to False)
 
     try:
-        # Document summary
-        api_response = api_instance.summarize_document(x_gradient_workspace_id, summarize_document_body_params)
-        print("The response of BlocksApi->summarize_document:\n")
+        # List available models
+        api_response = api_instance.list_models(x_gradient_workspace_id, capability=capability, only_base=only_base)
+        print("The response of ModelsApi->list_models:\n")
         pprint(api_response)
     except Exception as e:
-        print("Exception when calling BlocksApi->summarize_document: %s\n" % e)
+        print("Exception when calling ModelsApi->list_models: %s\n" % e)
 ```
 
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **x_gradient_workspace_id** | **str**|  | 
- **summarize_document_body_params** | [**SummarizeDocumentBodyParams**](SummarizeDocumentBodyParams.md)|  | 
+ **capability** | **str**|  | [optional] [default to &#39;fineTune&#39;]
+ **only_base** | **bool**|  | [optional] [default to False]
 
 ### Return type
 
-[**SummarizeDocumentSuccess**](SummarizeDocumentSuccess.md)
+[**ListModelsSuccess**](ListModelsSuccess.md)
 
 ### Authorization
 
 [AccessToken](../README.md#AccessToken)
 
 ### HTTP request headers
 
- - **Content-Type**: application/json
+ - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Success |  -  |
 **4XX** | Error |  -  |
```

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelBodyParamsRag.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf10.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf1Payload.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf2.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf3.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf4.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf5.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CompleteModelSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CompleteModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/CreateModelSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/CreateModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/DeleteModelError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/DeleteModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/EmbeddingsApi.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/EmbeddingsApi.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntityBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntityError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntityError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntitySuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerImagesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTablesInnerTableRowsInnerCellsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ExtractPdfSuccessPagesInnerTextBlocksInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerFineTuningParameters.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputs.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelBodyParamsSamplesInnerInputsAnyOfInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelErrorOneOf1.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/FineTuneModelSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/FineTuneModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSource.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerBodyParamsSourceOneOf1.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GetModelError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GetModelError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/GetModelSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/GetModelSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ListEmbeddingsError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ListModelsError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ListModelsSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ListModelsSuccessModelsInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/ModelAdapter.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/ModelAdapter.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/PersonalizeDocumentError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentError.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentError.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md` & `gradientai-1.9.0/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/exceptions.py` & `gradientai-1.9.0/gradientai/openapi/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/__init__.py` & `gradientai-1.9.0/gradientai/openapi/client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,45 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     Gradient AI API
 
     Interface for interacting with Gradient AI.  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@gradient.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-# import models into model package
+# import apis into sdk package
+from gradientai.openapi.client.api.blocks_api import BlocksApi
+from gradientai.openapi.client.api.embeddings_api import EmbeddingsApi
+from gradientai.openapi.client.api.files_api import FilesApi
+from gradientai.openapi.client.api.models_api import ModelsApi
+from gradientai.openapi.client.api.rag_api import RAGApi
+
+# import ApiClient
+from gradientai.openapi.client.api_response import ApiResponse
+from gradientai.openapi.client.api_client import ApiClient
+from gradientai.openapi.client.configuration import Configuration
+from gradientai.openapi.client.exceptions import OpenApiException
+from gradientai.openapi.client.exceptions import ApiTypeError
+from gradientai.openapi.client.exceptions import ApiValueError
+from gradientai.openapi.client.exceptions import ApiKeyError
+from gradientai.openapi.client.exceptions import ApiAttributeError
+from gradientai.openapi.client.exceptions import ApiException
+
+# import models into sdk package
+from gradientai.openapi.client.models.add_files_to_rag_collection_body_params import AddFilesToRagCollectionBodyParams
+from gradientai.openapi.client.models.add_files_to_rag_collection_error import AddFilesToRagCollectionError
 from gradientai.openapi.client.models.analyze_sentiment_body_params import AnalyzeSentimentBodyParams
 from gradientai.openapi.client.models.analyze_sentiment_body_params_examples_inner import AnalyzeSentimentBodyParamsExamplesInner
 from gradientai.openapi.client.models.analyze_sentiment_error import AnalyzeSentimentError
 from gradientai.openapi.client.models.analyze_sentiment_success import AnalyzeSentimentSuccess
 from gradientai.openapi.client.models.base_model import BaseModel
 from gradientai.openapi.client.models.complete_model_body_params import CompleteModelBodyParams
 from gradientai.openapi.client.models.complete_model_body_params_guidance import CompleteModelBodyParamsGuidance
@@ -35,21 +56,28 @@
 from gradientai.openapi.client.models.complete_model_error_one_of6 import CompleteModelErrorOneOf6
 from gradientai.openapi.client.models.complete_model_error_one_of7 import CompleteModelErrorOneOf7
 from gradientai.openapi.client.models.complete_model_error_one_of8 import CompleteModelErrorOneOf8
 from gradientai.openapi.client.models.complete_model_error_one_of9 import CompleteModelErrorOneOf9
 from gradientai.openapi.client.models.complete_model_error_one_of_payload import CompleteModelErrorOneOfPayload
 from gradientai.openapi.client.models.complete_model_error_one_of_payload_flagged_content_inner import CompleteModelErrorOneOfPayloadFlaggedContentInner
 from gradientai.openapi.client.models.complete_model_success import CompleteModelSuccess
+from gradientai.openapi.client.models.create_audio_transcription_body_params import CreateAudioTranscriptionBodyParams
+from gradientai.openapi.client.models.create_audio_transcription_error import CreateAudioTranscriptionError
+from gradientai.openapi.client.models.create_audio_transcription_success import CreateAudioTranscriptionSuccess
 from gradientai.openapi.client.models.create_model_body_params import CreateModelBodyParams
 from gradientai.openapi.client.models.create_model_body_params_initial_hyperparameters import CreateModelBodyParamsInitialHyperparameters
 from gradientai.openapi.client.models.create_model_body_params_initial_hyperparameters_lora_hyperparameters import CreateModelBodyParamsInitialHyperparametersLoraHyperparameters
 from gradientai.openapi.client.models.create_model_body_params_initial_hyperparameters_training_arguments import CreateModelBodyParamsInitialHyperparametersTrainingArguments
 from gradientai.openapi.client.models.create_model_body_params_model import CreateModelBodyParamsModel
 from gradientai.openapi.client.models.create_model_error import CreateModelError
 from gradientai.openapi.client.models.create_model_success import CreateModelSuccess
+from gradientai.openapi.client.models.create_rag_collection_body_params import CreateRagCollectionBodyParams
+from gradientai.openapi.client.models.create_rag_collection_body_params_files_inner import CreateRagCollectionBodyParamsFilesInner
+from gradientai.openapi.client.models.create_rag_collection_error import CreateRagCollectionError
+from gradientai.openapi.client.models.create_rag_collection_success import CreateRagCollectionSuccess
 from gradientai.openapi.client.models.delete_model_error import DeleteModelError
 from gradientai.openapi.client.models.extract_entity_body_params import ExtractEntityBodyParams
 from gradientai.openapi.client.models.extract_entity_body_params_schema_value import ExtractEntityBodyParamsSchemaValue
 from gradientai.openapi.client.models.extract_entity_error import ExtractEntityError
 from gradientai.openapi.client.models.extract_entity_success import ExtractEntitySuccess
 from gradientai.openapi.client.models.extract_entity_success_entity_value import ExtractEntitySuccessEntityValue
 from gradientai.openapi.client.models.extract_pdf_error import ExtractPdfError
@@ -78,14 +106,19 @@
 from gradientai.openapi.client.models.generate_answer_success_rag_context import GenerateAnswerSuccessRagContext
 from gradientai.openapi.client.models.generate_answer_success_rag_context_documents_inner import GenerateAnswerSuccessRagContextDocumentsInner
 from gradientai.openapi.client.models.generate_embedding_body_params import GenerateEmbeddingBodyParams
 from gradientai.openapi.client.models.generate_embedding_body_params_inputs_inner import GenerateEmbeddingBodyParamsInputsInner
 from gradientai.openapi.client.models.generate_embedding_error import GenerateEmbeddingError
 from gradientai.openapi.client.models.generate_embedding_success import GenerateEmbeddingSuccess
 from gradientai.openapi.client.models.generate_embedding_success_embeddings_inner import GenerateEmbeddingSuccessEmbeddingsInner
+from gradientai.openapi.client.models.get_audio_transcription_error import GetAudioTranscriptionError
+from gradientai.openapi.client.models.get_audio_transcription_success import GetAudioTranscriptionSuccess
+from gradientai.openapi.client.models.get_audio_transcription_success_one_of import GetAudioTranscriptionSuccessOneOf
+from gradientai.openapi.client.models.get_audio_transcription_success_one_of1 import GetAudioTranscriptionSuccessOneOf1
+from gradientai.openapi.client.models.get_audio_transcription_success_one_of1_result import GetAudioTranscriptionSuccessOneOf1Result
 from gradientai.openapi.client.models.get_model_error import GetModelError
 from gradientai.openapi.client.models.get_model_success import GetModelSuccess
 from gradientai.openapi.client.models.list_embeddings_error import ListEmbeddingsError
 from gradientai.openapi.client.models.list_embeddings_success import ListEmbeddingsSuccess
 from gradientai.openapi.client.models.list_embeddings_success_embeddings_models_inner import ListEmbeddingsSuccessEmbeddingsModelsInner
 from gradientai.openapi.client.models.list_models_error import ListModelsError
 from gradientai.openapi.client.models.list_models_success import ListModelsSuccess
@@ -94,7 +127,9 @@
 from gradientai.openapi.client.models.personalize_document_body_params import PersonalizeDocumentBodyParams
 from gradientai.openapi.client.models.personalize_document_error import PersonalizeDocumentError
 from gradientai.openapi.client.models.personalize_document_success import PersonalizeDocumentSuccess
 from gradientai.openapi.client.models.summarize_document_body_params import SummarizeDocumentBodyParams
 from gradientai.openapi.client.models.summarize_document_body_params_examples_inner import SummarizeDocumentBodyParamsExamplesInner
 from gradientai.openapi.client.models.summarize_document_error import SummarizeDocumentError
 from gradientai.openapi.client.models.summarize_document_success import SummarizeDocumentSuccess
+from gradientai.openapi.client.models.upload_file_error import UploadFileError
+from gradientai.openapi.client.models.upload_file_success import UploadFileSuccess
```

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/analyze_sentiment_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/analyze_sentiment_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/base_model.py` & `gradientai-1.9.0/gradientai/openapi/client/models/base_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_body_params_guidance.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_guidance.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_body_params_rag.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_body_params_rag.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of1.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of10.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of10.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of1_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of2.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of2.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of3.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of3.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of4.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of4.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of5.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of5.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of6.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of6.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of7.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of7.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of8.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of8.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of9.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of9.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of_payload.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_error_one_of_payload_flagged_content_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/complete_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/complete_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py` & `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py` & `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_lora_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py` & `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_initial_hyperparameters_training_arguments.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/create_model_body_params_model.py` & `gradientai-1.9.0/gradientai/openapi/client/models/create_model_body_params_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/create_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/create_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/create_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/create_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/delete_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/delete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_body_params_schema_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_entity_success_entity_value.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_entity_success_entity_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_images_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/extract_pdf_success_pages_inner_text_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_error_one_of.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/fine_tune_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/fine_tune_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params_source.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_body_params_source_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_success_rag_context.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_answer_success_rag_context_documents_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_body_params_inputs_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/generate_embedding_success_embeddings_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/get_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/get_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/get_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/get_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/list_embeddings_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/list_embeddings_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/list_embeddings_success_embeddings_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/list_models_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/list_models_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/list_models_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/list_models_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/list_models_success_models_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/list_models_success_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/model_adapter.py` & `gradientai-1.9.0/gradientai/openapi/client/models/model_adapter.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/personalize_document_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/personalize_document_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/personalize_document_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/personalize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_error.py` & `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/models/summarize_document_success.py` & `gradientai-1.9.0/gradientai/openapi/client/models/summarize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/rest.py` & `gradientai-1.9.0/gradientai/openapi/client/rest.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_analyze_sentiment_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_analyze_sentiment_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_base_model.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_base_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_blocks_api.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_models_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,65 +12,65 @@
     Do not edit the class manually.
 """
 
 
 import unittest
 
 import gradientai.openapi.client
-from gradientai.openapi.client.api.blocks_api import BlocksApi  # noqa: E501
+from gradientai.openapi.client.api.models_api import ModelsApi  # noqa: E501
 from gradientai.openapi.client.rest import ApiException
 
 
-class TestBlocksApi(unittest.TestCase):
-    """BlocksApi unit test stubs"""
+class TestModelsApi(unittest.TestCase):
+    """ModelsApi unit test stubs"""
 
     def setUp(self):
-        self.api = gradientai.openapi.client.api.blocks_api.BlocksApi()  # noqa: E501
+        self.api = gradientai.openapi.client.api.models_api.ModelsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_analyze_sentiment(self):
-        """Test case for analyze_sentiment
+    def test_complete_model(self):
+        """Test case for complete_model
 
-        Sentiment analysis  # noqa: E501
+        Complete model  # noqa: E501
         """
         pass
 
-    def test_extract_entity(self):
-        """Test case for extract_entity
+    def test_create_model(self):
+        """Test case for create_model
 
-        Entity extraction  # noqa: E501
+        Create model  # noqa: E501
         """
         pass
 
-    def test_extract_pdf(self):
-        """Test case for extract_pdf
+    def test_delete_model(self):
+        """Test case for delete_model
 
-        PDF extraction  # noqa: E501
+        Delete model  # noqa: E501
         """
         pass
 
-    def test_generate_answer(self):
-        """Test case for generate_answer
+    def test_fine_tune_model(self):
+        """Test case for fine_tune_model
 
-        Document question & answer  # noqa: E501
+        Fine-tune model  # noqa: E501
         """
         pass
 
-    def test_personalize_document(self):
-        """Test case for personalize_document
+    def test_get_model(self):
+        """Test case for get_model
 
-        Document personalization  # noqa: E501
+        Describe model  # noqa: E501
         """
         pass
 
-    def test_summarize_document(self):
-        """Test case for summarize_document
+    def test_list_models(self):
+        """Test case for list_models
 
-        Document summary  # noqa: E501
+        List available models  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_guidance.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_body_params_rag.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_body_params_rag.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of1.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of10.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of10.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of1_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of2.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of2.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of3.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of3.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of4.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of4.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of5.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of5.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of6.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of6.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of7.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of7.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of8.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of8.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of9.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of9.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_error_one_of_payload_flagged_content_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_complete_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_complete_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_lora_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_initial_hyperparameters_training_arguments.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_body_params_model.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_body_params_model.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_create_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_create_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_delete_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_delete_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_embeddings_api.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_embeddings_api.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_body_params_schema_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_entity_success_entity_value.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_images_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_tables_inner_table_rows_inner_cells_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_extract_pdf_success_pages_inner_text_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_fine_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_body_params_samples_inner_inputs_any_of_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_error_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_fine_tune_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_fine_tune_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params_source.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_body_params_source_one_of1.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_answer_success_rag_context_documents_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_body_params_inputs_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_generate_embedding_success_embeddings_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_get_model_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_get_model_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_get_model_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_list_embeddings_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_list_embeddings_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_list_embeddings_success_embeddings_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_list_models_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_list_models_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_list_models_success_models_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_list_models_success_models_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_model_adapter.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_model_adapter.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_models_api.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_blocks_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,65 +12,79 @@
     Do not edit the class manually.
 """
 
 
 import unittest
 
 import gradientai.openapi.client
-from gradientai.openapi.client.api.models_api import ModelsApi  # noqa: E501
+from gradientai.openapi.client.api.blocks_api import BlocksApi  # noqa: E501
 from gradientai.openapi.client.rest import ApiException
 
 
-class TestModelsApi(unittest.TestCase):
-    """ModelsApi unit test stubs"""
+class TestBlocksApi(unittest.TestCase):
+    """BlocksApi unit test stubs"""
 
     def setUp(self):
-        self.api = gradientai.openapi.client.api.models_api.ModelsApi()  # noqa: E501
+        self.api = gradientai.openapi.client.api.blocks_api.BlocksApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_complete_model(self):
-        """Test case for complete_model
+    def test_analyze_sentiment(self):
+        """Test case for analyze_sentiment
 
-        Complete model  # noqa: E501
+        Sentiment analysis  # noqa: E501
         """
         pass
 
-    def test_create_model(self):
-        """Test case for create_model
+    def test_create_audio_transcription(self):
+        """Test case for create_audio_transcription
 
-        Create model  # noqa: E501
+        Create audio transcription  # noqa: E501
         """
         pass
 
-    def test_delete_model(self):
-        """Test case for delete_model
+    def test_extract_entity(self):
+        """Test case for extract_entity
 
-        Delete model  # noqa: E501
+        Entity extraction  # noqa: E501
         """
         pass
 
-    def test_fine_tune_model(self):
-        """Test case for fine_tune_model
+    def test_extract_pdf(self):
+        """Test case for extract_pdf
 
-        Fine-tune model  # noqa: E501
+        PDF extraction  # noqa: E501
         """
         pass
 
-    def test_get_model(self):
-        """Test case for get_model
+    def test_generate_answer(self):
+        """Test case for generate_answer
 
-        Describe model  # noqa: E501
+        Document question & answer  # noqa: E501
         """
         pass
 
-    def test_list_models(self):
-        """Test case for list_models
+    def test_get_audio_transcription(self):
+        """Test case for get_audio_transcription
 
-        List available models  # noqa: E501
+        Get audio transcription  # noqa: E501
+        """
+        pass
+
+    def test_personalize_document(self):
+        """Test case for personalize_document
+
+        Document personalization  # noqa: E501
+        """
+        pass
+
+    def test_summarize_document(self):
+        """Test case for summarize_document
+
+        Document summary  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_personalize_document_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_personalize_document_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_personalize_document_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_personalize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_body_params.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_body_params_examples_inner.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_error.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_error.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client/test/test_summarize_document_success.py` & `gradientai-1.9.0/gradientai/openapi/client/test/test_summarize_document_success.py`

 * *Files identical despite different names*

### Comparing `gradientai-1.8.1/gradientai/openapi/client_README.md` & `gradientai-1.9.0/gradientai/openapi/client_README.md`

 * *Files 16% similar despite different names*

```diff
@@ -70,31 +70,38 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *BlocksApi* | [**analyze_sentiment**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#analyze_sentiment) | **POST** /blocks/analyze-sentiment | Sentiment analysis
+*BlocksApi* | [**create_audio_transcription**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#create_audio_transcription) | **POST** /blocks/transcription | Create audio transcription
 *BlocksApi* | [**extract_entity**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#extract_entity) | **POST** /blocks/extract | Entity extraction
 *BlocksApi* | [**extract_pdf**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#extract_pdf) | **POST** /blocks/extract-pdf | PDF extraction
 *BlocksApi* | [**generate_answer**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#generate_answer) | **POST** /blocks/answer | Document question &amp; answer
+*BlocksApi* | [**get_audio_transcription**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#get_audio_transcription) | **GET** /blocks/transcription | Get audio transcription
 *BlocksApi* | [**personalize_document**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#personalize_document) | **POST** /blocks/personalize | Document personalization
 *BlocksApi* | [**summarize_document**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BlocksApi.md#summarize_document) | **POST** /blocks/summarize | Document summary
 *EmbeddingsApi* | [**generate_embedding**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/EmbeddingsApi.md#generate_embedding) | **POST** /embeddings/{slug} | Generate embeddings
 *EmbeddingsApi* | [**list_embeddings**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/EmbeddingsApi.md#list_embeddings) | **GET** /embeddings | List available embeddings models
+*FilesApi* | [**upload_file**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/FilesApi.md#upload_file) | **POST** /files | File upload
 *ModelsApi* | [**complete_model**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ModelsApi.md#complete_model) | **POST** /models/{id}/complete | Complete model
 *ModelsApi* | [**create_model**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ModelsApi.md#create_model) | **POST** /models | Create model
 *ModelsApi* | [**delete_model**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ModelsApi.md#delete_model) | **DELETE** /models/{id} | Delete model
 *ModelsApi* | [**fine_tune_model**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ModelsApi.md#fine_tune_model) | **POST** /models/{id}/fine-tune | Fine-tune model
 *ModelsApi* | [**get_model**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ModelsApi.md#get_model) | **GET** /models/{id} | Describe model
 *ModelsApi* | [**list_models**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ModelsApi.md#list_models) | **GET** /models | List available models
+*RAGApi* | [**add_files_to_rag_collection**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/RAGApi.md#add_files_to_rag_collection) | **POST** /rag-collections/{id}/files | Add files to RAG collection
+*RAGApi* | [**create_rag_collection**](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/RAGApi.md#create_rag_collection) | **POST** /rag-collections | RAG collections
 
 
 ## Documentation For Models
 
+ - [AddFilesToRagCollectionBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/AddFilesToRagCollectionBodyParams.md)
+ - [AddFilesToRagCollectionError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/AddFilesToRagCollectionError.md)
  - [AnalyzeSentimentBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/AnalyzeSentimentBodyParams.md)
  - [AnalyzeSentimentBodyParamsExamplesInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/AnalyzeSentimentBodyParamsExamplesInner.md)
  - [AnalyzeSentimentError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/AnalyzeSentimentError.md)
  - [AnalyzeSentimentSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/AnalyzeSentimentSuccess.md)
  - [BaseModel](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/BaseModel.md)
  - [CompleteModelBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelBodyParams.md)
  - [CompleteModelBodyParamsGuidance](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelBodyParamsGuidance.md)
@@ -111,21 +118,28 @@
  - [CompleteModelErrorOneOf6](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelErrorOneOf6.md)
  - [CompleteModelErrorOneOf7](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelErrorOneOf7.md)
  - [CompleteModelErrorOneOf8](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelErrorOneOf8.md)
  - [CompleteModelErrorOneOf9](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelErrorOneOf9.md)
  - [CompleteModelErrorOneOfPayload](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayload.md)
  - [CompleteModelErrorOneOfPayloadFlaggedContentInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelErrorOneOfPayloadFlaggedContentInner.md)
  - [CompleteModelSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CompleteModelSuccess.md)
+ - [CreateAudioTranscriptionBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateAudioTranscriptionBodyParams.md)
+ - [CreateAudioTranscriptionError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateAudioTranscriptionError.md)
+ - [CreateAudioTranscriptionSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateAudioTranscriptionSuccess.md)
  - [CreateModelBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateModelBodyParams.md)
  - [CreateModelBodyParamsInitialHyperparameters](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparameters.md)
  - [CreateModelBodyParamsInitialHyperparametersLoraHyperparameters](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersLoraHyperparameters.md)
  - [CreateModelBodyParamsInitialHyperparametersTrainingArguments](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateModelBodyParamsInitialHyperparametersTrainingArguments.md)
  - [CreateModelBodyParamsModel](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateModelBodyParamsModel.md)
  - [CreateModelError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateModelError.md)
  - [CreateModelSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateModelSuccess.md)
+ - [CreateRagCollectionBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateRagCollectionBodyParams.md)
+ - [CreateRagCollectionBodyParamsFilesInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateRagCollectionBodyParamsFilesInner.md)
+ - [CreateRagCollectionError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateRagCollectionError.md)
+ - [CreateRagCollectionSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/CreateRagCollectionSuccess.md)
  - [DeleteModelError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/DeleteModelError.md)
  - [ExtractEntityBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ExtractEntityBodyParams.md)
  - [ExtractEntityBodyParamsSchemaValue](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ExtractEntityBodyParamsSchemaValue.md)
  - [ExtractEntityError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ExtractEntityError.md)
  - [ExtractEntitySuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ExtractEntitySuccess.md)
  - [ExtractEntitySuccessEntityValue](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ExtractEntitySuccessEntityValue.md)
  - [ExtractPdfError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ExtractPdfError.md)
@@ -154,14 +168,19 @@
  - [GenerateAnswerSuccessRagContext](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContext.md)
  - [GenerateAnswerSuccessRagContextDocumentsInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GenerateAnswerSuccessRagContextDocumentsInner.md)
  - [GenerateEmbeddingBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GenerateEmbeddingBodyParams.md)
  - [GenerateEmbeddingBodyParamsInputsInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GenerateEmbeddingBodyParamsInputsInner.md)
  - [GenerateEmbeddingError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GenerateEmbeddingError.md)
  - [GenerateEmbeddingSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GenerateEmbeddingSuccess.md)
  - [GenerateEmbeddingSuccessEmbeddingsInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GenerateEmbeddingSuccessEmbeddingsInner.md)
+ - [GetAudioTranscriptionError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GetAudioTranscriptionError.md)
+ - [GetAudioTranscriptionSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GetAudioTranscriptionSuccess.md)
+ - [GetAudioTranscriptionSuccessOneOf](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf.md)
+ - [GetAudioTranscriptionSuccessOneOf1](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1.md)
+ - [GetAudioTranscriptionSuccessOneOf1Result](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GetAudioTranscriptionSuccessOneOf1Result.md)
  - [GetModelError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GetModelError.md)
  - [GetModelSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/GetModelSuccess.md)
  - [ListEmbeddingsError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ListEmbeddingsError.md)
  - [ListEmbeddingsSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ListEmbeddingsSuccess.md)
  - [ListEmbeddingsSuccessEmbeddingsModelsInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ListEmbeddingsSuccessEmbeddingsModelsInner.md)
  - [ListModelsError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ListModelsError.md)
  - [ListModelsSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/ListModelsSuccess.md)
@@ -170,14 +189,16 @@
  - [PersonalizeDocumentBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/PersonalizeDocumentBodyParams.md)
  - [PersonalizeDocumentError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/PersonalizeDocumentError.md)
  - [PersonalizeDocumentSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/PersonalizeDocumentSuccess.md)
  - [SummarizeDocumentBodyParams](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/SummarizeDocumentBodyParams.md)
  - [SummarizeDocumentBodyParamsExamplesInner](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/SummarizeDocumentBodyParamsExamplesInner.md)
  - [SummarizeDocumentError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/SummarizeDocumentError.md)
  - [SummarizeDocumentSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/SummarizeDocumentSuccess.md)
+ - [UploadFileError](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/UploadFileError.md)
+ - [UploadFileSuccess](https://github.com/Preemo-Inc/gradientai-python-sdk/blob/main/gradientai/openapi/client/docs/UploadFileSuccess.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
 Authentication schemes defined for the API:
```

### Comparing `gradientai-1.8.1/pyproject.toml` & `gradientai-1.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
-name = "gradientai"
-version = "1.8.1"
-description = "Gradient AI API"
 authors = ["Gradient AI Support <support@gradient.ai>"]
+description = "Gradient AI API"
+keywords = [
+  "Gradient AI API",
+  "ai",
+  "artificial intelligence",
+  "fine-tuning",
+  "large language model",
+  "llm",
+  "gradient",
+  "gradient ai",
+]
 license = "MIT"
+name = "gradientai"
 readme = "README.md"
 repository = "https://github.com/Preemo-Inc/gradientai-python-sdk"
-keywords = [
-    "Gradient AI API",
-    "ai",
-    "artificial intelligence",
-    "fine-tuning",
-    "large language model",
-    "llm",
-    "gradient",
-    "gradient ai"
-  ]
+version = "1.9.0"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 pydantic = "^1.10.5, <2"
 python = "^3.8.1"
 python-dateutil = ">=2.8.2"
 urllib3 = ">= 1.25.3"
 
 [tool.poetry.dev-dependencies]
+Flake8-pyproject = "1.2.3"
 autoflake = "2.0.1"
 black = "22.3.0"
 build = "0.10.0"
 flake8 = "6.0.0"
-Flake8-pyproject = "1.2.3"
 isort = "5.10.1"
 mypy = "1.3.0"
 pep8-naming = "0.13.0"
 pytest = "7.2.1"
 python-dotenv = "1.0.0"
 twine = "4.0.2"
 
@@ -73,19 +73,19 @@
   "W",
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
-plugins = ["pydantic.mypy"]
 check_untyped_defs = true
 disallow_any_unimported = true
 disallow_untyped_defs = true
 no_implicit_optional = true
+plugins = ["pydantic.mypy"]
 show_error_codes = true
 warn_return_any = true
 warn_unused_ignores = true
 
 [build-system]
-requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
```

### Comparing `gradientai-1.8.1/PKG-INFO` & `gradientai-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradientai
-Version: 1.8.1
+Version: 1.9.0
 Summary: Gradient AI API
 Home-page: https://github.com/Preemo-Inc/gradientai-python-sdk
 License: MIT
 Keywords: Gradient AI API,ai,artificial intelligence,fine-tuning,large language model,llm,gradient,gradient ai
 Author: Gradient AI Support
 Author-email: support@gradient.ai
 Requires-Python: >=3.8.1,<4.0.0
```

