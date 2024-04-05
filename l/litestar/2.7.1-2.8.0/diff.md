# Comparing `tmp/litestar-2.7.1.tar.gz` & `tmp/litestar-2.8.0.tar.gz`

## Comparing `litestar-2.7.1.tar` & `litestar-2.8.0.tar`

### file list

```diff
@@ -1,706 +1,713 @@
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 litestar-2.7.1/Makefile
--rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 litestar-2.7.1/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/__main__.py
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_multipart.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_parsers.py
--rw-r--r--   0        0        0    38972 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/app.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/background_tasks.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/concurrency.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/constants.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/controller.py
--rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/data_extractors.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/di.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/enums.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/file_system.py
--rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/pagination.py
--rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/py.typed
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/router.py
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/status_codes.py
--rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/typing.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/utils.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    16651 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_layers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/datastructures.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/plugin.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/responses.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    25017 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/plugins/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/plugins/dataclass.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/plugins/pagination.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/plugins/struct.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/schema_generation/plugins/typed_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_signature/__init__.py
--rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_signature/model.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_signature/types.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/_signature/utils.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/__init__.py
--rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/asyncpg.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/psycopg.py
--rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/cli/__init__.py
--rw-r--r--   0        0        0    20700 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/cli/_utils.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12280 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/config/app.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/config/compression.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/config/csrf.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/connection/__init__.py
--rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/connection/base.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/connection/request.py
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/connection/websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/__init__.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/jinja.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/mako.py
--rw-r--r--   0        0        0     7519 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/minijinja.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/minijnja.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/piccolo.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/attrs/__init__.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/attrs/attrs_schema_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/prometheus/config.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/prometheus/controller.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/prometheus/middleware.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/pydantic/config.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/pydantic/pydantic_di_plugin.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/pydantic/pydantic_dto_factory.py
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/pydantic/pydantic_init_plugin.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/pydantic/pydantic_schema_plugin.py
--rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/pydantic/utils.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/repository/testing.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    18908 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/state.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/datastructures/url.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/__init__.py
--rw-r--r--   0        0        0    33732 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/_backend.py
--rw-r--r--   0        0        0    22848 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/_codegen_backend.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/_types.py
--rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/base_dto.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/config.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/data_structures.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/dataclass_dto.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/field.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/msgspec_dto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/dto/types.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/events/__init__.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/events/emitter.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/events/listener.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/exceptions/dto_exceptions.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    23613 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    28825 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    65669 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    18859 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/logging/_utils.py
--rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/logging/picologging.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/base.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/csrf.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10827 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/response_cache.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/compression/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/compression/brotli_facade.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/compression/facade.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/compression/gzip_facade.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/compression/middleware.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/config.py
--rw-r--r--   0        0        0    22855 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/controller.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/plugins/__init__.py
--rw-r--r--   0        0        0    10955 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/plugins/base.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/plugins/core.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/plugins/sqlalchemy.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/plugins/structlog.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/_exceptions.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/_filters.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/exceptions.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/filters.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/handlers.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/abc/__init__.py
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/abc/_async.py
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/abc/_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/testing/__init__.py
--rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/response/__init__.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/response/base.py
--rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/response/file.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/response/redirect.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/response/sse.py
--rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/response/streaming.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/response/template.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/routes/base.py
--rw-r--r--   0        0        0    12878 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/routes/http.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/__init__.py
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/base.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/jwt/__init__.py
--rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/jwt/auth.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/jwt/middleware.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/jwt/token.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/serialization/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/serialization/msgspec_hooks.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/static_files/base.py
--rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/static_files/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/stores/base.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/stores/file.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/stores/memory.py
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/stores/redis.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/template/__init__.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/template/base.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/template/config.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/__init__.py
--rw-r--r--   0        0        0    30991 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/transport.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/__init__.py
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/composite_types.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/empty.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/file_types.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/protocols.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/types/serialization.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/compat.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/deprecation.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/empty.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/helpers.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/module_loader.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/path.py
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/predicates.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/sequence.py
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/signature.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/sync.py
--rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/typing.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/warnings.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/scope/__init__.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 litestar-2.7.1/litestar/utils/scope/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/__init__.py
--rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/conftest.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/docker-compose.yml
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/docker_service_fixtures.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/helpers.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/__init__.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_advanced_alchemy.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_exception_handlers.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_option_requests.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_pydantic.py
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_response_caching.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_router_registration.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_starlette_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/test_dependency_validation.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/test_injection_of_classes.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/test_inter_dependencies.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/test_request_local_caching.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_life_cycle_hooks/__init__.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_life_cycle_hooks/test_after_request.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_life_cycle_hooks/test_after_response.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_life_cycle_hooks/test_before_request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/conftest.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/test_asset_url_path.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/test_path_mounting.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/test_path_resolution.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/test_route_indexing.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/test_route_reverse.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/e2e/test_routing/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/__init__.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/conftest.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_cache_control_headers.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_exceptions.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_hello_world.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_lifecycle_hooks.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_openapi.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_request_data.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_routing.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_signature_namespace.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_startup_and_shutdown.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_static_files.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_stores.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_todo_app.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_using_session_auth.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_hooks/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_hooks/test_application_after_exception_hook.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_hooks/test_application_before_send.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_hooks/test_lifespan_manager.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_hooks/test_on_app_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_state/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_state/test_passing_initial_state.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_state/test_using_application_state.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_state/test_using_custom_state.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_application_state/test_using_immutable_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/__init__.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/test_piccolo_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/test_sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dependency_injection/test_dependency_validation_error.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dto/__init__.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dto/test_example_apps.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_dto/test_tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_middleware/__init__.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_middleware/test_abstract_middleware.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_middleware/test_call_order.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_middleware/test_session_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_pagination/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_pagination/test_using_classic_pagination.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_pagination/test_using_cursor_pagination.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_pagination/test_using_offset_pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_parameters/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_parameters/test_header_and_cookies_parameters.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_parameters/test_layered_parameters.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_parameters/test_path_parameters.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_parameters/test_query_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_plugins/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_plugins/test_di_plugin.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_plugins/test_example_apps.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/test_background_tasks.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/test_custom_responses.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/test_json_suffix_responses.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/test_response_cookies.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/test_response_headers.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/test_returning_responses.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_responses/test_sse_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_security/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_templating/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_templating/test_engine_instance.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_templating/test_returning_templates.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/examples/test_templating/test_template_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/conftest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/piccolo_conf.py
--rw-r--r--   0        0        0    14723 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_app.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_asgi_router.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_background_tasks.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_concurrency.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_controller.py
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_data_extractors.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_deprecations.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_di.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_events.py
--rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_exceptions.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_file_system.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_guards.py
--rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_pagination.py
--rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_params.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_parsers.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_request_class_resolution.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response_class_resolution.py
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_stores.py
--rw-r--r--   0        0        0    16804 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_typing.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_websocket_class_resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_channels/__init__.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_channels/conftest.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_channels/test_backends.py
--rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_channels/test_plugin.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_channels/test_subscriber.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_channels/util.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/__init__.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/conftest.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/test_cli.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/test_cli_plugin.py
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/test_core_commands.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/test_env_resolution.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/test_schema_commands.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/test_session_commands.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_cli/test_ssl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_connection/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_connection/test_base.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_connection/test_connection_caching.py
--rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_connection/test_request.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_connection/test_websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/conftest.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_minijinja.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_msgspec.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_opentelemetry.py
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_prometheus.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_repository.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_attrs/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_htmx/__init__.py
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_htmx/test_htmx_request.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_htmx/test_htmx_response.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/tables.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/conftest.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/models.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_dto.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_integration.py
--rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_openapi.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/__init_.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/test_cookie.py
--rw-r--r--   0        0        0    13358 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/test_headers.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/test_multi_dicts.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/test_response_header.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/test_state.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/test_upload_file.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_datastructures/test_url.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/__init__.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/conftest.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_config.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_integration.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_interface.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/__init__.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_base_dto.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_dataclass_dto.py
--rw-r--r--   0        0        0    30290 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_integration.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/conftest.py
--rw-r--r--   0        0        0    16209 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/test_backends.py
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_asgi_handlers/__init__.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_base_handlers/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_base_handlers/test_opt.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_base_handlers/test_resolution.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_base_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_defaults.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_delete.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_head.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_media_type.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_sync.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0    14434 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/__init__.py
--rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/flower.jpeg
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_cleanup_group.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_cookie_params.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_defaults.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_dependency_batches.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_generator_dependencies.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_header_params.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_json_data.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_layered_params.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_msgpack_data.py
--rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_multipart_data.py
--rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_path_params.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_query_params.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_url_encoded_data.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_kwargs/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_logging/__init__.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_logging/test_logging_config.py
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_logging/test_structlog_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/__init__.py
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_allowed_hosts_middleware.py
--rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_base_authentication_middleware.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_base_middleware.py
--rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_compression_middleware.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_cors_middleware.py
--rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_csrf_middleware.py
--rw-r--r--   0        0        0    14751 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_exception_handler_middleware.py
--rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_middleware_handling.py
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_session/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_session/conftest.py
--rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_session/test_client_side_backend.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_session/test_integration.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_session/test_middleware.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_middleware/test_session/test_server_side_backend.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/__init__.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/conftest.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_constrained_fields.py
--rw-r--r--   0        0        0    14482 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_controller.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_datastructures.py
--rw-r--r--   0        0        0    16325 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_integration.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_parameters.py
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_path_item.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_request_body.py
--rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_responses.py
--rw-r--r--   0        0        0    20596 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_schema.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_security_schemes.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_spec_generation.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_tags.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_typescript_converter/__init__.py
--rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_typescript_converter/test_converter.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_plugins/__init__.py
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_plugins/test_base.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_plugins/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_repository/__init__.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_repository/models_bigint.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_repository/models_uuid.py
--rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_repository/test_generic_mock_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/__init__.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_base_response.py
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_file_response.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_redirect_response.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_response_cookies.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_response_headers.py
--rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_response_to_asgi_response.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_serialization.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_sse.py
--rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_streaming_response.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_type_decoders.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_response/test_type_encoders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_security/__init__.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_security/test_security.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_security/test_session_auth.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_security/test_jwt/test_auth.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_security/test_jwt/test_integration.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_security/test_jwt/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_signature/__init__.py
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_signature/test_parsing.py
--rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_signature/test_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_static_files/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_static_files/conftest.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_static_files/test_create_static_router.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_static_files/test_file_serving_resolution.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_static_files/test_html_mode.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_static_files/test_static_files_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_template/__init__.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_template/test_built_in.py
--rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_template/test_builtin_functions.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_template/test_config.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_template/test_context.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_template/test_csrf_token.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_template/test_template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_testing/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_testing/test_lifespan_handler.py
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_testing/test_request_factory.py
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_testing/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_types/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_types/test_protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_compat.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_dataclass.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_deprecation.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_helpers.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_module_loader.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_path.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_predicates.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_scope.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_sequence.py
--rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_signature.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_sync.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_typing.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.7.1/tests/unit/test_utils/test_version.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.7.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 litestar-2.7.1/LICENSE
--rw-r--r--   0        0        0    91774 2020-02-02 00:00:00.000000 litestar-2.7.1/README.md
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 litestar-2.7.1/pyproject.toml
--rw-r--r--   0        0        0    96685 2020-02-02 00:00:00.000000 litestar-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 litestar-2.8.0/Makefile
+-rw-r--r--   0        0        0    19851 2020-02-02 00:00:00.000000 litestar-2.8.0/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/__main__.py
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_multipart.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_parsers.py
+-rw-r--r--   0        0        0    39616 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/app.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/background_tasks.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/concurrency.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/constants.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/controller.py
+-rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/data_extractors.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/di.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/enums.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/file_system.py
+-rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/pagination.py
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/py.typed
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/router.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/status_codes.py
+-rw-r--r--   0        0        0    25972 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/typing.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    16651 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_layers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/datastructures.py
+-rw-r--r--   0        0        0    10647 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/plugin.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    25613 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/dataclass.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/pagination.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/struct.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/typed_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/model.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/types.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/utils.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/__init__.py
+-rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/asyncpg.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/psycopg.py
+-rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    20230 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/_utils.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/app.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/compression.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/csrf.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/base.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/request.py
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/mako.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/minijinja.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/minijnja.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/piccolo.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/attrs/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/attrs/attrs_schema_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/config.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_di_plugin.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_dto_factory.py
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_init_plugin.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_schema_plugin.py
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/utils.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/testing.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17475 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/url.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/__init__.py
+-rw-r--r--   0        0        0    33807 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/_backend.py
+-rw-r--r--   0        0        0    22848 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/_codegen_backend.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/_types.py
+-rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/base_dto.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/config.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/data_structures.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/dataclass_dto.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/field.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/msgspec_dto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/types.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/events/emitter.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/events/listener.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/dto_exceptions.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    29363 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    65669 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/picologging.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/base.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/response_cache.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/brotli_facade.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/facade.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/gzip_facade.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/middleware.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/config.py
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/plugins.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/__init__.py
+-rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/base.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/core.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/flash.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/sqlalchemy.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/structlog.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/_exceptions.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/_filters.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/exceptions.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/filters.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/handlers.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/abc/__init__.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/abc/_async.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/abc/_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/testing/__init__.py
+-rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/__init__.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/base.py
+-rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/file.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/sse.py
+-rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/streaming.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/template.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/base.py
+-rw-r--r--   0        0        0    12878 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/http.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/base.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/__init__.py
+-rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/auth.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/middleware.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/token.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/serialization/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/serialization/msgspec_hooks.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/static_files/base.py
+-rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/static_files/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/base.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/file.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/memory.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/template/__init__.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/template/base.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/__init__.py
+-rw-r--r--   0        0        0    31457 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/empty.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/file_types.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/serialization.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/empty.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/helpers.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/module_loader.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/path.py
+-rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/predicates.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/signature.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/sync.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/warnings.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/scope/__init__.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/scope/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/__init__.py
+-rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/conftest.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/docker-compose.yml
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/docker_service_fixtures.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/helpers.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/__init__.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_advanced_alchemy.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_exception_handlers.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_option_requests.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_pydantic.py
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_response_caching.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_router_registration.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_starlette_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_dependency_validation.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_classes.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_inter_dependencies.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_request_local_caching.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/__init__.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_request.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_response.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_before_request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/conftest.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_asset_url_path.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_path_mounting.py
+-rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_path_resolution.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_route_indexing.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_route_reverse.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/__init__.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/conftest.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_cache_control_headers.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_exceptions.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_hello_world.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_lifecycle_hooks.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_request_data.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_routing.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_signature_namespace.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_startup_and_shutdown.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_static_files.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_stores.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_todo_app.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_using_session_auth.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_application_after_exception_hook.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_application_before_send.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_lifespan_manager.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_on_app_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_passing_initial_state.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_using_application_state.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_using_custom_state.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_using_immutable_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_piccolo_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_validation_error.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dto/__init__.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dto/test_example_apps.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dto/test_tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/__init__.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_abstract_middleware.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_call_order.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_session_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_openapi/__init__.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_openapi/test_openapi.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_openapi/test_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/test_using_classic_pagination.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/test_using_cursor_pagination.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/test_using_offset_pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_header_and_cookies_parameters.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_layered_parameters.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_path_parameters.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_query_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/test_di_plugin.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/test_example_apps.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_background_tasks.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_custom_responses.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_json_suffix_responses.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_response_cookies.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_response_headers.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_returning_responses.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_sse_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/test_engine_instance.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/test_returning_templates.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/test_template_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/piccolo_conf.py
+-rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_app.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_asgi_router.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_background_tasks.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_concurrency.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_controller.py
+-rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_data_extractors.py
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_deprecations.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_di.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_events.py
+-rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_exceptions.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_file_system.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_guards.py
+-rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_pagination.py
+-rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_params.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_parsers.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_request_class_resolution.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response_class_resolution.py
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_stores.py
+-rw-r--r--   0        0        0    17322 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_typing.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_websocket_class_resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/__init__.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/conftest.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/test_backends.py
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/test_plugin.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/test_subscriber.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/util.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/__init__.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/conftest.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_cli.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_cli_plugin.py
+-rw-r--r--   0        0        0    23147 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_core_commands.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_env_resolution.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_schema_commands.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_session_commands.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_ssl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_base.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_connection_caching.py
+-rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_request.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/conftest.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_minijinja.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_msgspec.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_opentelemetry.py
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_prometheus.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_repository.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_htmx/__init__.py
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_request.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_response.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/tables.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/conftest.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/models.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_dto.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
+-rw-r--r--   0        0        0    11001 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_integration.py
+-rw-r--r--   0        0        0    29005 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_openapi.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/__init_.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_cookie.py
+-rw-r--r--   0        0        0    13358 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_headers.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_multi_dicts.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_response_header.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_state.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_upload_file.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_url.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/__init__.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/conftest.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_config.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_integration.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_interface.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/__init__.py
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_base_dto.py
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_dataclass_dto.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_field.py
+-rw-r--r--   0        0        0    30290 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_integration.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/conftest.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_backends.py
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/__init__.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_opt.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_resolution.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_defaults.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_delete.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_head.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_media_type.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_sync.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/__init__.py
+-rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/flower.jpeg
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_cleanup_group.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_cookie_params.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_defaults.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_dependency_batches.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_generator_dependencies.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_header_params.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_json_data.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_layered_params.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_msgpack_data.py
+-rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_multipart_data.py
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_path_params.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_query_params.py
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_url_encoded_data.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_logging/__init__.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_logging/test_logging_config.py
+-rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_logging/test_structlog_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/__init__.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_allowed_hosts_middleware.py
+-rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_base_authentication_middleware.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_base_middleware.py
+-rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_compression_middleware.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_cors_middleware.py
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_csrf_middleware.py
+-rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_exception_handler_middleware.py
+-rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_middleware_handling.py
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/conftest.py
+-rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_client_side_backend.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_integration.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_middleware.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_server_side_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/__init__.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/conftest.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_constrained_fields.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_datastructures.py
+-rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_endpoints.py
+-rw-r--r--   0        0        0    19008 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_integration.py
+-rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_parameters.py
+-rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_path_item.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_render_plugins.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_request_body.py
+-rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_responses.py
+-rw-r--r--   0        0        0    22306 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_schema.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_security_schemes.py
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_spec_generation.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_tags.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/__init__.py
+-rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_converter.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/__init__.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/test_base.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/test_flash.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/__init__.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/models_bigint.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/models_uuid.py
+-rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/test_generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/__init__.py
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_base_response.py
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_file_response.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_redirect_response.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_response_cookies.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_response_headers.py
+-rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_response_to_asgi_response.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_serialization.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_sse.py
+-rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_streaming_response.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_type_decoders.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_type_encoders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/__init__.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_security.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_session_auth.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/test_auth.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/test_integration.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_signature/__init__.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_signature/test_parsing.py
+-rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_signature/test_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/conftest.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_create_static_router.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_file_serving_resolution.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_html_mode.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_static_files_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/__init__.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_built_in.py
+-rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_builtin_functions.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_config.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_context.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_csrf_token.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/test_lifespan_handler.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/test_request_factory.py
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_types/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_types/test_protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_compat.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_dataclass.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_deprecation.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_helpers.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_module_loader.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_path.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_predicates.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_scope.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_sequence.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_signature.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_sync.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_typing.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_version.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 litestar-2.8.0/LICENSE
+-rw-r--r--   0        0        0    92575 2020-02-02 00:00:00.000000 litestar-2.8.0/README.md
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 litestar-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    97593 2020-02-02 00:00:00.000000 litestar-2.8.0/PKG-INFO
```

### Comparing `litestar-2.7.1/Makefile` & `litestar-2.8.0/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -98,16 +98,22 @@
 
 .PHONY: pre-commit
 pre-commit: 										## Runs pre-commit hooks; includes ruff formatting and linting, codespell
 	@echo "=> Running pre-commit process"
 	@$(PDM) run pre-commit run --all-files
 	@echo "=> Pre-commit complete"
 
+.PHONY: slots-check
+slots-check: 										## Check for slots usage in classes
+	@echo "=> Checking for slots usage in classes"
+	@$(PDM) run slotscheck litestar
+	@echo "=> Slots check complete"
+
 .PHONY: lint
-lint: pre-commit type-check 						## Run all linting
+lint: pre-commit type-check slots-check				## Run all linting
 
 .PHONY: coverage
 coverage:  											## Run the tests and generate coverage report
 	@echo "=> Running tests with coverage"
 	@$(PDM) run pytest tests --cov -n auto
 	@$(PDM) run coverage html
 	@$(PDM) run coverage xml
```

### Comparing `litestar-2.7.1/docs/PYPI_README.md` & `litestar-2.8.0/docs/PYPI_README.md`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 - [OpenAPI 3.1 schema generation](#openapi)
 - [Life Cycle Hooks](#request-life-cycle-hooks)
 - [Route Guards based Authorization](#route-guards)
 - Support for `dataclasses`, `TypedDict`, [pydantic version 1 and version 2](https://docs.pydantic.dev/latest/),
   [msgspec](https://github.com/jcrist/msgspec) and [attrs](https://www.attrs.org/en/stable/)
 - Layered parameter declaration
 - [Automatic API documentation with](#redoc-swagger-ui-and-stoplight-elements-api-documentation):
+  - [Scalar](https://github.com/scalar/scalar/)
   - [RapiDoc](https://github.com/rapi-doc/RapiDoc)
   - [Redoc](https://github.com/Redocly/redoc)
   - [Stoplight Elements](https://github.com/stoplightio/elements)
   - [Swagger-UI](https://swagger.io/tools/swagger-ui/)
 - [Trio](https://trio.readthedocs.io/en/stable/) support (built-in, via [AnyIO](https://anyio.readthedocs.io/))
 - Ultra-fast validation, serialization and deserialization using [msgspec](https://github.com/jcrist/msgspec)
 - SQLAlchemy integration
@@ -121,18 +122,18 @@
 
 <a href="https://github.com/scalar/scalar/?utm_source=litestar&utm_medium=website&utm_campaign=main-badge" target="_blank" title="Scalar.com - Document, Discover and Test APIs with Scalar."><img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/sponsors/scalar.svg" width="180" alt="Scalar.com"></a>
 <a href="https://telemetrysports.com/" title="Telemetry Sports - Changing the way data influences the sports experience"><img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/sponsors/telemetry-sports/unofficial-telemetry-whitebg.svg" width="150" alt="Telemetry Sports"></a>
 <a href="https://www.stok.kr/" title="Stok - Stack Up Your Assets!"><img src="https://avatars.githubusercontent.com/u/144093421?s=400&v=4" width="150" alt="Stok"></a>
 
 <a href="https://docs.litestar.dev/dev/#sponsors" class="external-link" target="_blank">Check out our sponsors in the docs</a>
 
-If you would like to support the work that we do please consider [becoming a sponsor][sponsor-github]
-on [GitHub][sponsor-github] or [Open Collective][sponsor-oc].
+If you would like to support the work that we do please consider [becoming a sponsor][sponsor-polar]
+via [Polar.sh][sponsor-polar] (preferred), [GitHub][sponsor-github] or [Open Collective][sponsor-oc].
 
-We also participate in pledge-based sponsorship with [Polar][sponsor-polar].
+Also, exclusively with [Polar][sponsor-polar], you can engage in pledge-based sponsorships.
 
 [sponsor-github]: https://github.com/sponsors/litestar-org
 [sponsor-oc]: https://opencollective.com/litestar
 [sponsor-polar]: https://polar.sh/litestar-org
 
 ## Features
```

### Comparing `litestar-2.7.1/litestar/__init__.py` & `litestar-2.8.0/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_multipart.py` & `litestar-2.8.0/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_parsers.py` & `litestar-2.8.0/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/app.py` & `litestar-2.8.0/litestar/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import inspect
 import logging
 import os
+import warnings
 from contextlib import (
     AbstractAsyncContextManager,
     AsyncExitStack,
     asynccontextmanager,
     suppress,
 )
 from datetime import date, datetime, time, timedelta
@@ -16,20 +17,21 @@
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Iterable, Mapping, Sequence, TypedDict, cast
 
 from litestar._asgi import ASGIRouter
 from litestar._asgi.utils import get_route_handlers, wrap_in_exception_handler
 from litestar._openapi.plugin import OpenAPIPlugin
 from litestar._openapi.schema_generation import openapi_schema_plugins
 from litestar.config.allowed_hosts import AllowedHostsConfig
-from litestar.config.app import AppConfig
+from litestar.config.app import AppConfig, ExperimentalFeatures
 from litestar.config.response_cache import ResponseCacheConfig
 from litestar.connection import Request, WebSocket
 from litestar.datastructures.state import State
 from litestar.events.emitter import BaseEventEmitterBackend, SimpleEventEmitter
 from litestar.exceptions import (
+    LitestarWarning,
     MissingDependencyException,
     NoRouteMatchFoundException,
 )
 from litestar.logging.config import LoggingConfig, get_logger_placeholder
 from litestar.middleware.cors import CORSMiddleware
 from litestar.openapi.config import OpenAPIConfig
 from litestar.plugins import (
@@ -51,15 +53,14 @@
 from litestar.utils.dataclass import extract_dataclass_items
 from litestar.utils.predicates import is_async_callable
 from litestar.utils.warnings import warn_pdb_on_exception
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-    from litestar.config.app import ExperimentalFeatures
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.datastructures import CacheControlHeader, ETag
     from litestar.dto import AbstractDTO
     from litestar.events.listener import EventListener
     from litestar.logging.config import BaseLoggingConfig
@@ -146,29 +147,25 @@
         "asgi_router",
         "before_send",
         "compression_config",
         "cors_config",
         "csrf_config",
         "event_emitter",
         "get_logger",
-        "include_in_schema",
         "logger",
         "logging_config",
         "multipart_form_part_limit",
         "on_shutdown",
         "on_startup",
         "openapi_config",
-        "request_class",
         "response_cache_config",
         "route_map",
-        "signature_namespace",
         "state",
         "stores",
         "template_engine",
-        "websocket_class",
         "pdb_on_exception",
         "experimental_features",
     )
 
     def __init__(
         self,
         route_handlers: Sequence[ControllerRouterHandler] | None = None,
@@ -197,14 +194,15 @@
         multipart_form_part_limit: int = 1000,
         on_app_init: Sequence[OnAppInitHandler] | None = None,
         on_shutdown: Sequence[LifespanHook] | None = None,
         on_startup: Sequence[LifespanHook] | None = None,
         openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
         opt: Mapping[str, Any] | None = None,
         parameters: ParametersMap | None = None,
+        path: str | None = None,
         plugins: Sequence[PluginProtocol] | None = None,
         request_class: type[Request] | None = None,
         response_cache_config: ResponseCacheConfig | None = None,
         response_class: type[Response] | None = None,
         response_cookies: ResponseCookies | None = None,
         response_headers: ResponseHeaders | None = None,
         return_dto: type[AbstractDTO] | None | EmptyType = Empty,
@@ -276,14 +274,18 @@
                 application startup.
             openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
             opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <litestar.connection.request.Request>` or
                 :class:`ASGI Scope <.types.Scope>`.
             parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
                 paths.
+            path: A path fragment that is prefixed to all route handlers, controllers and routers associated
+                with the application instance.
+
+                .. versionadded:: 2.8.0
             pdb_on_exception: Drop into the PDB when an exception occurs.
             plugins: Sequence of plugins.
             request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
             response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
                 response.
             response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
             response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
@@ -349,14 +351,15 @@
             logging_config=logging_config,
             middleware=list(middleware or []),
             multipart_form_part_limit=multipart_form_part_limit,
             on_shutdown=list(on_shutdown or []),
             on_startup=list(on_startup or []),
             openapi_config=openapi_config,
             opt=dict(opt or {}),
+            path=path or "",
             parameters=parameters or {},
             pdb_on_exception=pdb_on_exception,
             plugins=self._get_default_plugins(list(plugins or [])),
             request_class=request_class,
             response_cache_config=response_cache_config or ResponseCacheConfig(),
             response_class=response_class,
             response_cookies=response_cookies or [],
@@ -392,14 +395,24 @@
             config.stores if isinstance(config.stores, StoreRegistry) else StoreRegistry(config.stores)
         )
         self._lifespan_managers = config.lifespan
         for store in self.stores._stores.values():
             self._lifespan_managers.append(store)
         self._server_lifespan_managers = [p.server_lifespan for p in config.plugins or [] if isinstance(p, CLIPlugin)]
         self.experimental_features = frozenset(config.experimental_features or [])
+        if ExperimentalFeatures.DTO_CODEGEN in self.experimental_features:
+            warnings.warn(
+                "Use of redundant experimental feature flag DTO_CODEGEN. "
+                "DTO codegen backend is enabled by default since Litestar 2.8. The "
+                "DTO_CODEGEN feature flag can be safely removed from the configuration "
+                "and will be removed in version 3.0.",
+                category=LitestarWarning,
+                stacklevel=2,
+            )
+
         self.get_logger: GetLogger = get_logger_placeholder
         self.logger: Logger | None = None
         self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
         self.asgi_router = ASGIRouter(app=self)
 
         self.after_exception = [ensure_async_callable(h) for h in config.after_exception]
         self.allowed_hosts = cast("AllowedHostsConfig | None", config.allowed_hosts)
@@ -444,15 +457,15 @@
             dto=config.dto,
             etag=config.etag,
             exception_handlers=config.exception_handlers,
             guards=config.guards,
             middleware=config.middleware,
             opt=config.opt,
             parameters=config.parameters,
-            path="",
+            path=config.path,
             request_class=self.request_class,
             response_class=config.response_class,
             response_cookies=config.response_cookies,
             response_headers=config.response_headers,
             return_dto=config.return_dto,
             # route handlers are registered below
             route_handlers=[],
@@ -860,15 +873,15 @@
 
     def update_openapi_schema(self) -> None:
         """Update the OpenAPI schema to reflect the route handlers registered on the app.
 
         Returns:
             None
         """
-        self.plugins.get(OpenAPIPlugin)._build_openapi_schema()
+        self.plugins.get(OpenAPIPlugin)._build_openapi()
 
     def emit(self, event_id: str, *args: Any, **kwargs: Any) -> None:
         """Emit an event to all attached listeners.
 
         Args:
             event_id: The ID of the event to emit, e.g ``my_event``.
             args: args to pass to the listener(s).
```

### Comparing `litestar-2.7.1/litestar/background_tasks.py` & `litestar-2.8.0/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/concurrency.py` & `litestar-2.8.0/litestar/concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/constants.py` & `litestar-2.8.0/litestar/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+from __future__ import annotations
+
 from dataclasses import MISSING
 from inspect import Signature
 from typing import Any, Final
+from uuid import uuid4
 
 from msgspec import UnsetType
 
 from litestar.enums import MediaType
 from litestar.types import Empty
 from litestar.utils.deprecation import warn_deprecation
 
 DEFAULT_ALLOWED_CORS_HEADERS: Final = {"Accept", "Accept-Language", "Content-Language", "Content-Type"}
 DEFAULT_CHUNK_SIZE: Final = 1024 * 128  # 128KB
 HTTP_DISCONNECT: Final = "http.disconnect"
 HTTP_RESPONSE_BODY: Final = "http.response.body"
 HTTP_RESPONSE_START: Final = "http.response.start"
 ONE_MEGABYTE: Final = 1024 * 1024
+OPENAPI_JSON_HANDLER_NAME: Final = f"{uuid4().hex}_litestar_openapi_json"
 OPENAPI_NOT_INITIALIZED: Final = "Litestar has not been instantiated with OpenAPIConfig"
 REDIRECT_STATUS_CODES: Final = {301, 302, 303, 307, 308}
 REDIRECT_ALLOWED_MEDIA_TYPES: Final = {MediaType.TEXT, MediaType.HTML, MediaType.JSON}
 RESERVED_KWARGS: Final = {"state", "headers", "cookies", "request", "socket", "data", "query", "scope", "body"}
 SKIP_VALIDATION_NAMES: Final = {"request", "socket", "scope", "receive", "send"}
 UNDEFINED_SENTINELS: Final = {Signature.empty, Empty, Ellipsis, MISSING, UnsetType}
 WEBSOCKET_CLOSE: Final = "websocket.close"
 WEBSOCKET_DISCONNECT: Final = "websocket.disconnect"
 
-
 # deprecated constants
 _SCOPE_STATE_CSRF_TOKEN_KEY = "csrf_token"  # noqa: S105  # possible hardcoded password
 _SCOPE_STATE_DEPENDENCY_CACHE: Final = "dependency_cache"
 _SCOPE_STATE_NAMESPACE: Final = "__litestar__"
 _SCOPE_STATE_RESPONSE_COMPRESSED: Final = "response_compressed"
 _SCOPE_STATE_DO_CACHE: Final = "do_cache"
 _SCOPE_STATE_IS_CACHED: Final = "is_cached"
```

### Comparing `litestar-2.7.1/litestar/controller.py` & `litestar-2.8.0/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/data_extractors.py` & `litestar-2.8.0/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/di.py` & `litestar-2.8.0/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/enums.py` & `litestar-2.8.0/litestar/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     DELETE = "DELETE"
     GET = "GET"
     HEAD = "HEAD"
     OPTIONS = "OPTIONS"
     PATCH = "PATCH"
     POST = "POST"
     PUT = "PUT"
+    TRACE = "TRACE"
 
 
 class MediaType(str, Enum):
     """An Enum for ``Content-Type`` header values."""
 
     JSON = "application/json"
     MESSAGEPACK = "application/x-msgpack"
```

### Comparing `litestar-2.7.1/litestar/file_system.py` & `litestar-2.8.0/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/pagination.py` & `litestar-2.8.0/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/params.py` & `litestar-2.8.0/litestar/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,21 @@
     """Constrict a string value to be upper case."""
     format: str | None = field(default=None)
     """Specify the format to which a string value should be converted."""
     enum: Sequence[Any] | None = field(default=None)
     """A sequence of valid values."""
     read_only: bool | None = field(default=None)
     """A boolean flag dictating whether this parameter is read only."""
+    schema_extra: dict[str, Any] | None = field(default=None)
+    """Extensions to the generated schema.
+
+    If set, will overwrite the matching fields in the generated schema.
+
+    .. versionadded:: 2.8.0
+    """
 
     @property
     def is_constrained(self) -> bool:
         """Return True if any of the constraints are set."""
         return any(
             attr if attr and attr is not Empty else False  # type: ignore[comparison-overlap]
             for attr in (
@@ -183,14 +190,15 @@
     min_items: int | None = None,
     min_length: int | None = None,
     multiple_of: float | None = None,
     pattern: str | None = None,
     query: str | None = None,
     required: bool | None = None,
     title: str | None = None,
+    schema_extra: dict[str, Any] | None = None,
 ) -> Any:
     """Create an extended parameter kwarg definition.
 
     Args:
         annotation: `Empty` by default.
         const: A boolean flag dictating whether this parameter is a constant. If True, the value passed to the parameter
             must equal its default value. This also causes the OpenAPI const field
@@ -223,14 +231,18 @@
             Equivalent to multipleOf in the OpenAPI specification.
         pattern: A string representing a regex against which the given string will be matched.
             Equivalent to pattern in the OpenAPI specification.
         query: The query parameter key for this parameter.
         required: A boolean flag dictating whether this parameter is required.
             If set to False, None values will be allowed. Defaults to True.
         title: String value used in the title section of the OpenAPI schema for the given parameter.
+        schema_extra: Extensions to the generated schema. If set, will overwrite the matching fields in the generated
+            schema.
+
+            .. versionadded:: 2.8.0
     """
     return ParameterKwarg(
         annotation=annotation,
         header=header,
         cookie=cookie,
         query=query,
         examples=examples,
@@ -247,14 +259,15 @@
         le=le,
         multiple_of=multiple_of,
         min_items=min_items,
         max_items=max_items,
         min_length=min_length,
         max_length=max_length,
         pattern=pattern,
+        schema_extra=schema_extra,
     )
 
 
 @dataclass(frozen=True)
 class BodyKwarg(KwargDefinition):
     """Data container representing a request body."""
 
@@ -290,14 +303,15 @@
     media_type: str | RequestEncodingType = RequestEncodingType.JSON,
     min_items: int | None = None,
     min_length: int | None = None,
     multipart_form_part_limit: int | None = None,
     multiple_of: float | None = None,
     pattern: str | None = None,
     title: str | None = None,
+    schema_extra: dict[str, Any] | None = None,
 ) -> Any:
     """Create an extended request body kwarg definition.
 
     Args:
         const: A boolean flag dictating whether this parameter is a constant. If True, the value passed to the parameter
             must equal its default value. This also causes the OpenAPI const field to be
             populated with the default value.
@@ -327,14 +341,18 @@
         multipart_form_part_limit: The maximal number of allowed parts in a multipart/formdata request.
             This limit is intended to protect from DoS attacks.
         multiple_of: Constrict value to a multiple of a given float or int.
             Equivalent to multipleOf in the OpenAPI specification.
         pattern: A string representing a regex against which the given string will be matched.
             Equivalent to pattern in the OpenAPI specification.
         title: String value used in the title section of the OpenAPI schema for the given parameter.
+        schema_extra: Extensions to the generated schema. If set, will overwrite the matching fields in the generated
+            schema.
+
+            .. versionadded:: 2.8.0
     """
     return BodyKwarg(
         media_type=media_type,
         examples=examples,
         external_docs=external_docs,
         content_encoding=content_encoding,
         default=default,
@@ -348,14 +366,15 @@
         multiple_of=multiple_of,
         min_items=min_items,
         max_items=max_items,
         min_length=min_length,
         max_length=max_length,
         pattern=pattern,
         multipart_form_part_limit=multipart_form_part_limit,
+        schema_extra=schema_extra,
     )
 
 
 @dataclass(frozen=True)
 class DependencyKwarg:
     """Data container representing a dependency."""
```

### Comparing `litestar-2.7.1/litestar/router.py` & `litestar-2.8.0/litestar/router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/status_codes.py` & `litestar-2.8.0/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/typing.py` & `litestar-2.8.0/litestar/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from collections import abc, deque
 from copy import deepcopy
 from dataclasses import dataclass, is_dataclass, replace
 from inspect import Parameter, Signature
 from typing import (
     Any,
     AnyStr,
@@ -17,15 +18,15 @@
     TypeVar,
     cast,
 )
 
 from msgspec import UnsetType
 from typing_extensions import NotRequired, Required, Self, get_args, get_origin, get_type_hints, is_typeddict
 
-from litestar.exceptions import ImproperlyConfiguredException
+from litestar.exceptions import ImproperlyConfiguredException, LitestarWarning
 from litestar.openapi.spec import Example
 from litestar.params import BodyKwarg, DependencyKwarg, KwargDefinition, ParameterKwarg
 from litestar.types import Empty
 from litestar.types.builtin_types import NoneType, UnionTypes
 from litestar.utils.predicates import (
     is_annotated_type,
     is_any,
@@ -92,15 +93,15 @@
     extra = {
         **cast("dict[str, Any]", extra or getattr(value, "extra", None) or {}),
         **(getattr(value, "json_schema_extra", None) or {}),
     }
     example_list: list[Any] | None
     if example := extra.pop("example", None):
         example_list = [Example(value=example)]
-    elif examples := getattr(value, "examples", None):
+    elif examples := (extra.pop("examples", None) or getattr(value, "examples", None)):
         example_list = [Example(value=example) for example in cast("list[str]", examples)]
     else:
         example_list = None
 
     return {
         k: v
         for k, v in {
@@ -508,20 +509,39 @@
 
         args = () if origin is abc.Callable else get_args(unwrapped)
 
         if not kwargs.get("kwarg_definition"):
             if isinstance(kwargs.get("default"), (KwargDefinition, DependencyKwarg)):
                 kwargs["kwarg_definition"] = kwargs.pop("default")
             elif any(isinstance(v, (KwargDefinition, DependencyKwarg)) for v in metadata):
-                kwargs["kwarg_definition"] = next(  # pragma: no cover
+                kwarg_definition = kwargs["kwarg_definition"] = next(  # pragma: no cover
                     # see https://github.com/nedbat/coveragepy/issues/475
                     v
                     for v in metadata
                     if isinstance(v, (KwargDefinition, DependencyKwarg))
                 )
+                if kwarg_definition.default is not Empty:
+                    warnings.warn(
+                        f"Deprecated default value specification for annotation '{annotation}'. Setting defaults "
+                        f"inside 'typing.Annotated' is discouraged and support for this will be removed in a future "
+                        f"version. Defaults should be set with regular parameter default values. Use "
+                        "'param: Annotated[<type>, Parameter(...)] = <default>' instead of "
+                        "'param: Annotated[<type>, Parameter(..., default=<default>)].",
+                        category=DeprecationWarning,
+                        stacklevel=2,
+                    )
+                    if "default" in kwargs and kwarg_definition.default != kwargs["default"]:
+                        warnings.warn(
+                            f"Ambiguous default values for annotation '{annotation}'. The default value "
+                            f"'{kwarg_definition.default!r}' set inside the parameter annotation differs from the "
+                            f"parameter default value '{kwargs['default']!r}'",
+                            category=LitestarWarning,
+                            stacklevel=2,
+                        )
+
                 metadata = tuple(v for v in metadata if not isinstance(v, (KwargDefinition, DependencyKwarg)))
             elif (extra := kwargs.get("extra", {})) and "kwarg_definition" in extra:
                 kwargs["kwarg_definition"] = extra.pop("kwarg_definition")
             else:
                 kwargs["kwarg_definition"], kwargs["extra"] = cls._extract_metadata(
                     annotation=annotation,
                     name=kwargs.get("name", ""),
```

### Comparing `litestar-2.7.1/litestar/_asgi/asgi_router.py` & `litestar-2.8.0/litestar/_asgi/asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_asgi/utils.py` & `litestar-2.8.0/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.8.0/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.8.0/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_asgi/routing_trie/types.py` & `litestar-2.8.0/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_asgi/routing_trie/validate.py` & `litestar-2.8.0/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_kwargs/cleanup.py` & `litestar-2.8.0/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_kwargs/dependencies.py` & `litestar-2.8.0/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_kwargs/extractors.py` & `litestar-2.8.0/litestar/_kwargs/extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_kwargs/kwargs_model.py` & `litestar-2.8.0/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_kwargs/parameter_definition.py` & `litestar-2.8.0/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_layers/utils.py` & `litestar-2.8.0/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/datastructures.py` & `litestar-2.8.0/litestar/_openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/parameters.py` & `litestar-2.8.0/litestar/_openapi/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,30 +92,30 @@
         """
         self.context = context
         self.schema_creator = SchemaCreator.from_openapi_context(self.context, prefer_alias=True)
         self.route_handler = route_handler
         self.parameters = ParameterCollection(route_handler)
         self.dependency_providers = route_handler.resolve_dependencies()
         self.layered_parameters = route_handler.resolve_layered_parameters()
-        self.path_parameters_names = {p.name for p in path_parameters}
+        self.path_parameters: dict[str, PathParameterDefinition] = {p.name: p for p in path_parameters}
 
     def create_parameter(self, field_definition: FieldDefinition, parameter_name: str) -> Parameter:
         """Create an OpenAPI Parameter instance for a field definition.
 
         Args:
             field_definition: The field definition.
             parameter_name: The name of the parameter.
         """
 
         result: Schema | Reference | None = None
         kwarg_definition = (
             field_definition.kwarg_definition if isinstance(field_definition.kwarg_definition, ParameterKwarg) else None
         )
 
-        if parameter_name in self.path_parameters_names:
+        if parameter_name in self.path_parameters:
             param_in = ParamType.PATH
             is_required = True
             result = self.schema_creator.for_field_definition(field_definition)
         elif kwarg_definition and kwarg_definition.header:
             parameter_name = kwarg_definition.header
             param_in = ParamType.HEADER
             is_required = field_definition.is_required
@@ -211,14 +211,25 @@
 
         for field_name, field_definition in intersection_fields:
             self.parameters.add(self.get_layered_parameter(field_name=field_name, field_definition=field_definition))
 
     def create_parameters_for_handler(self) -> list[Parameter]:
         """Create a list of path/query/header Parameter models for the given PathHandler."""
         handler_fields = self.route_handler.parsed_fn_signature.parameters
+        # not all path parameters have to be consumed by the handler. Because even not
+        # consumed path parameters must still be specified, we create stub parameters
+        # for the unconsumed ones so a correct OpenAPI schema can be generated
+        params_not_consumed_by_handler = set(self.path_parameters) - handler_fields.keys()
+        handler_fields.update(
+            {
+                param_name: FieldDefinition.from_kwarg(self.path_parameters[param_name].type, name=param_name)
+                for param_name in params_not_consumed_by_handler
+            }
+        )
+
         self.create_parameters_for_field_definitions(handler_fields)
         return self.parameters.list()
 
 
 def create_parameters_for_handler(
     context: OpenAPIContext,
     route_handler: BaseRouteHandler,
```

### Comparing `litestar-2.7.1/litestar/_openapi/request_body.py` & `litestar-2.8.0/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/responses.py` & `litestar-2.8.0/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/utils.py` & `litestar-2.8.0/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/examples.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/schema.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     _type_or_first_not_none_inner_type,
     get_json_schema_formatted_examples,
 )
 from litestar.datastructures import UploadFile
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema, SchemaDataContainer
-from litestar.params import BodyKwarg, ParameterKwarg
+from litestar.params import BodyKwarg, KwargDefinition, ParameterKwarg
 from litestar.plugins import OpenAPISchemaPlugin
 from litestar.types import Empty
 from litestar.types.builtin_types import NoneType
 from litestar.typing import FieldDefinition
 from litestar.utils.helpers import get_name
 from litestar.utils.predicates import (
     is_class_and_subclass,
@@ -565,14 +565,25 @@
                     # by this point, we have already set the `exclusive_minimum` and/or `exclusive_maximum` fields
                     # to floating point timestamp values on the schema object. However, the original `date` objects
                     # that define those constraints on `KwargDefinition` are still `date` objects. We don't want to
                     # overwrite them here.
                     if getattr(schema, schema_key, None) is None:
                         setattr(schema, schema_key, value)
 
+            if isinstance(field.kwarg_definition, KwargDefinition) and (extra := field.kwarg_definition.schema_extra):
+                for schema_key, value in extra.items():
+                    if not hasattr(schema, schema_key):
+                        raise ValueError(
+                            f"`schema_extra` declares key `{schema_key}` which does not exist in `Schema` object"
+                        )
+                    setattr(schema, schema_key, value)
+
+        if schema.default is None and field.default is not Empty:
+            schema.default = field.default
+
         if not schema.examples and self.generate_examples:
             from litestar._openapi.schema_generation.examples import create_examples_for_field
 
             schema.examples = get_json_schema_formatted_examples(create_examples_for_field(field))
 
         if schema.title and schema.type == OpenAPIType.OBJECT:
             key = _get_normalized_schema_key(field.annotation)
```

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/utils.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/plugins/__init__.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/plugins/dataclass.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/dataclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
+import dataclasses
 from dataclasses import MISSING, fields
 from typing import TYPE_CHECKING
 
 from litestar.plugins import OpenAPISchemaPlugin
+from litestar.types import Empty
 from litestar.typing import FieldDefinition
 from litestar.utils.predicates import is_optional_union
 
 if TYPE_CHECKING:
     from litestar._openapi.schema_generation import SchemaCreator
     from litestar.openapi.spec import Schema
 
@@ -27,10 +29,15 @@
                 if (
                     field.default is MISSING
                     and field.default_factory is MISSING
                     and not is_optional_union(type_hints[field.name])
                 )
             ),
             property_fields={
-                field.name: FieldDefinition.from_kwarg(type_hints[field.name], field.name) for field in dataclass_fields
+                field.name: FieldDefinition.from_kwarg(
+                    annotation=type_hints[field.name],
+                    name=field.name,
+                    default=field.default if field.default is not dataclasses.MISSING else Empty,
+                )
+                for field in dataclass_fields
             },
         )
```

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/plugins/pagination.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/plugins/struct.py` & `litestar-2.8.0/litestar/dto/dataclass_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from dataclasses import MISSING, fields, replace
+from typing import TYPE_CHECKING, Generic, TypeVar
 
-from msgspec import Struct
-from msgspec.structs import fields
-
-from litestar.plugins import OpenAPISchemaPlugin
+from litestar.dto.base_dto import AbstractDTO
+from litestar.dto.data_structures import DTOFieldDefinition
+from litestar.dto.field import extract_dto_field
+from litestar.params import DependencyKwarg, KwargDefinition
 from litestar.types.empty import Empty
-from litestar.typing import FieldDefinition
-from litestar.utils.predicates import is_optional_union
 
 if TYPE_CHECKING:
-    from msgspec.structs import FieldInfo
+    from typing import Collection, Generator
+
+    from litestar.types.protocols import DataclassProtocol
+    from litestar.typing import FieldDefinition
 
-    from litestar._openapi.schema_generation import SchemaCreator
-    from litestar.openapi.spec import Schema
 
+__all__ = ("DataclassDTO", "T")
 
-class StructSchemaPlugin(OpenAPISchemaPlugin):
-    def is_plugin_supported_field(self, field_definition: FieldDefinition) -> bool:
-        return not field_definition.is_union and field_definition.is_subclass_of(Struct)
-
-    def to_openapi_schema(self, field_definition: FieldDefinition, schema_creator: SchemaCreator) -> Schema:
-        def is_field_required(field: FieldInfo) -> bool:
-            return field.required or field.default_factory is Empty
-
-        type_hints = field_definition.get_type_hints(include_extras=True, resolve_generics=True)
-        struct_fields = fields(field_definition.type_)
-
-        return schema_creator.create_component_schema(
-            field_definition,
-            required=sorted(
-                [
-                    field.encode_name
-                    for field in struct_fields
-                    if is_field_required(field=field) and not is_optional_union(type_hints[field.name])
-                ]
-            ),
-            property_fields={
-                field.encode_name: FieldDefinition.from_kwarg(type_hints[field.name], field.encode_name)
-                for field in struct_fields
-            },
-        )
+T = TypeVar("T", bound="DataclassProtocol | Collection[DataclassProtocol]")
+AnyDataclass = TypeVar("AnyDataclass", bound="DataclassProtocol")
+
+
+class DataclassDTO(AbstractDTO[T], Generic[T]):
+    """Support for domain modelling with dataclasses."""
+
+    @classmethod
+    def generate_field_definitions(
+        cls, model_type: type[DataclassProtocol]
+    ) -> Generator[DTOFieldDefinition, None, None]:
+        dc_fields = {f.name: f for f in fields(model_type)}
+        for key, field_definition in cls.get_model_type_hints(model_type).items():
+            if not (dc_field := dc_fields.get(key)):
+                continue
+
+            default = dc_field.default if dc_field.default is not MISSING else Empty
+            default_factory = dc_field.default_factory if dc_field.default_factory is not MISSING else None
+            field_defintion = replace(
+                DTOFieldDefinition.from_field_definition(
+                    field_definition=field_definition,
+                    default_factory=default_factory,
+                    dto_field=extract_dto_field(field_definition, dc_field.metadata),
+                    model_name=model_type.__name__,
+                ),
+                name=key,
+                default=default,
+            )
+
+            yield (
+                replace(field_defintion, default=Empty, kwarg_definition=default)
+                if isinstance(default, (KwargDefinition, DependencyKwarg))
+                else field_defintion
+            )
+
+    @classmethod
+    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
+        return hasattr(field_definition.annotation, "__dataclass_fields__")
```

### Comparing `litestar-2.7.1/litestar/_openapi/schema_generation/plugins/typed_dict.py` & `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/typed_dict.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.8.0/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.8.0/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_openapi/typescript_converter/types.py` & `litestar-2.8.0/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_signature/model.py` & `litestar-2.8.0/litestar/_signature/model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/_signature/utils.py` & `litestar-2.8.0/litestar/_signature/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/channels/plugin.py` & `litestar-2.8.0/litestar/channels/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/channels/subscriber.py` & `litestar-2.8.0/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/channels/backends/asyncpg.py` & `litestar-2.8.0/litestar/channels/backends/asyncpg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/channels/backends/base.py` & `litestar-2.8.0/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/channels/backends/memory.py` & `litestar-2.8.0/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/channels/backends/psycopg.py` & `litestar-2.8.0/litestar/channels/backends/psycopg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/channels/backends/redis.py` & `litestar-2.8.0/litestar/channels/backends/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/cli/__init__.py` & `litestar-2.8.0/litestar/cli/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     from rich_click.cli import patch as rich_click_patch
 
     rich_click_patch()
     click.rich_click.USE_RICH_MARKUP = True
     click.rich_click.USE_MARKDOWN = False
     click.rich_click.SHOW_ARGUMENTS = True
     click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
-    click.rich_click.SHOW_ARGUMENTS = True
-    click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
     click.rich_click.STYLE_ERRORS_SUGGESTION = "magenta italic"
     click.rich_click.ERRORS_SUGGESTION = ""
     click.rich_click.ERRORS_EPILOGUE = ""
     click.rich_click.MAX_WIDTH = 80
     click.rich_click.SHOW_METAVARS_COLUMN = True
     click.rich_click.APPEND_METAVARS_HELP = True
```

### Comparing `litestar-2.7.1/litestar/cli/_utils.py` & `litestar-2.8.0/litestar/cli/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,30 +70,19 @@
 
 
 @dataclass
 class LitestarEnv:
     """Information about the current Litestar environment variables."""
 
     app_path: str
-    debug: bool
     app: Litestar
     cwd: Path
     host: str | None = None
     port: int | None = None
-    fd: int | None = None
-    uds: str | None = None
-    reload: bool | None = None
-    reload_dirs: tuple[str, ...] | None = None
-    reload_include: tuple[str, ...] | None = None
-    reload_exclude: tuple[str, ...] | None = None
-    web_concurrency: int | None = None
     is_app_factory: bool = False
-    certfile_path: str | None = None
-    keyfile_path: str | None = None
-    create_self_signed_cert: bool = False
 
     @classmethod
     def from_env(cls, app_path: str | None, app_dir: Path | None = None) -> LitestarEnv:
         """Load environment variables.
 
         If ``python-dotenv`` is installed, use it to populate environment first
         """
@@ -103,48 +92,34 @@
             sys.path.append(cwd_str_path)
 
         with contextlib.suppress(ImportError):
             import dotenv
 
             dotenv.load_dotenv()
         app_path = app_path or getenv("LITESTAR_APP")
+        app_name = getenv("LITESTAR_APP_NAME") or "Litestar"
+        quiet_console = getenv("LITESTAR_QUIET_CONSOLE") or False
         if app_path and getenv("LITESTAR_APP") is None:
             os.environ["LITESTAR_APP"] = app_path
         if app_path:
-            console.print(f"Using Litestar app from env: [bright_blue]{app_path!r}")
+            if not quiet_console and isatty():
+                console.print(f"Using {app_name} app from env: [bright_blue]{app_path!r}")
             loaded_app = _load_app_from_path(app_path)
         else:
             loaded_app = _autodiscover_app(cwd)
 
         port = getenv("LITESTAR_PORT")
-        web_concurrency = getenv("WEB_CONCURRENCY")
-        uds = getenv("LITESTAR_UNIX_DOMAIN_SOCKET")
-        fd = getenv("LITESTAR_FILE_DESCRIPTOR")
-        reload_dirs = tuple(s.strip() for s in getenv("LITESTAR_RELOAD_DIRS", "").split(",") if s) or None
-        reload_include = tuple(s.strip() for s in getenv("LITESTAR_RELOAD_INCLUDES", "").split(",") if s) or None
-        reload_exclude = tuple(s.strip() for s in getenv("LITESTAR_RELOAD_EXCLUDES", "").split(",") if s) or None
 
         return cls(
             app_path=loaded_app.app_path,
             app=loaded_app.app,
-            debug=_bool_from_env("LITESTAR_DEBUG"),
             host=getenv("LITESTAR_HOST"),
             port=int(port) if port else None,
-            uds=uds,
-            fd=int(fd) if fd else None,
-            reload=_bool_from_env("LITESTAR_RELOAD"),
-            reload_dirs=reload_dirs,
-            reload_include=reload_include,
-            reload_exclude=reload_exclude,
-            web_concurrency=int(web_concurrency) if web_concurrency else None,
             is_app_factory=loaded_app.is_factory,
             cwd=cwd,
-            certfile_path=getenv("LITESTAR_SSL_CERT_PATH"),
-            keyfile_path=getenv("LITESTAR_SSL_KEY_PATH"),
-            create_self_signed_cert=_bool_from_env("LITESTAR_CREATE_SELF_SIGNED_CERT"),
         )
 
 
 @dataclass
 class LoadedApp:
     """Information about a loaded Litestar app."""
 
@@ -324,49 +299,54 @@
         if path.exists() or path.with_suffix(".py").exists():
             yield path
         if arbitrary and path.is_dir():
             yield from _arbitrary_autodiscovery_paths(path)
 
 
 def _autodiscover_app(cwd: Path) -> LoadedApp:
+    app_name = getenv("LITESTAR_APP_NAME") or "Litestar"
+    quiet_console = getenv("LITESTAR_QUIET_CONSOLE") or False
     for file_path in _autodiscovery_paths(cwd):
         import_path = _path_to_dotted_path(file_path.relative_to(cwd))
         module = importlib.import_module(import_path)
 
         for attr, value in chain(
             [("app", getattr(module, "app", None)), ("application", getattr(module, "application", None))],
             module.__dict__.items(),
         ):
             if isinstance(value, Litestar):
                 app_string = f"{import_path}:{attr}"
                 os.environ["LITESTAR_APP"] = app_string
-                console.print(f"Using Litestar app from [bright_blue]{app_string}")
+                if not quiet_console and isatty():
+                    console.print(f"Using {app_name} app from [bright_blue]{app_string}")
                 return LoadedApp(app=value, app_path=app_string, is_factory=False)
 
         if hasattr(module, "create_app"):
             app_string = f"{import_path}:create_app"
             os.environ["LITESTAR_APP"] = app_string
-            console.print(f"Using Litestar factory [bright_blue]{app_string}")
+            if not quiet_console and isatty():
+                console.print(f"Using {app_name} factory from [bright_blue]{app_string}")
             return LoadedApp(app=module.create_app(), app_path=app_string, is_factory=True)
 
         for attr, value in module.__dict__.items():
             if not callable(value):
                 continue
             return_annotation = (
                 get_type_hints(value, include_extras=True).get("return") if hasattr(value, "__annotations__") else None
             )
             if not return_annotation:
                 continue
             if return_annotation in ("Litestar", Litestar):
                 app_string = f"{import_path}:{attr}"
                 os.environ["LITESTAR_APP"] = app_string
-                console.print(f"Using Litestar factory [bright_blue]{app_string}")
+                if not quiet_console and sys.stdout.isatty():
+                    console.print(f"Using {app_name} factory from [bright_blue]{app_string}")
                 return LoadedApp(app=value(), app_path=f"{app_string}", is_factory=True)
 
-    raise LitestarCLIException("Could not find a Litestar app or factory")
+    raise LitestarCLIException(f"Could not find {app_name} instance or factory")
 
 
 def _format_is_enabled(value: Any) -> str:
     """Return a coloured string `"Enabled" if ``value`` is truthy, else "Disabled"."""
     return "[green]Enabled[/]" if value else "[red]Disabled[/]"
 
 
@@ -385,15 +365,20 @@
     if app.allowed_hosts:
         allowed_hosts = app.allowed_hosts
 
         table.add_row("Allowed hosts", ", ".join(allowed_hosts.allowed_hosts))
 
     openapi_enabled = _format_is_enabled(app.openapi_config)
     if app.openapi_config:
-        openapi_enabled += f" path=[yellow]{app.openapi_config.openapi_controller.path}"
+        path = (
+            app.openapi_config.openapi_controller.path
+            if app.openapi_config.openapi_controller
+            else app.openapi_config.path or "/schema"
+        )
+        openapi_enabled += f" path=[yellow]{path}"
     table.add_row("OpenAPI", openapi_enabled)
 
     table.add_row("Compression", app.compression_config.backend if app.compression_config else "[red]Disabled")
 
     if app.template_engine:
         table.add_row("Template engine", type(app.template_engine).__name__)
 
@@ -554,9 +539,21 @@
 
     return regex_routes
 
 
 def remove_default_schema_routes(
     routes: list[HTTPRoute | ASGIRoute | WebSocketRoute], openapi_config: OpenAPIConfig
 ) -> list[HTTPRoute | ASGIRoute | WebSocketRoute]:
-    schema_path = openapi_config.openapi_controller.path
+    schema_path = (
+        (openapi_config.path or "/schema")
+        if openapi_config.openapi_controller is None
+        else openapi_config.openapi_controller.path
+    )
     return remove_routes_with_patterns(routes, (schema_path,))
+
+
+def isatty() -> bool:
+    """Detect if a terminal is TTY enabled.
+
+    This is a convenience wrapper around the built in system methods.  This allows for easier testing of TTY/non-TTY modes.
+    """
+    return sys.stdout.isatty()
```

### Comparing `litestar-2.7.1/litestar/cli/main.py` & `litestar-2.8.0/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/cli/commands/core.py` & `litestar-2.8.0/litestar/cli/commands/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from litestar.app import DEFAULT_OPENAPI_CONFIG
 from litestar.cli._utils import (
     UVICORN_INSTALLED,
     LitestarEnv,
     console,
     create_ssl_files,
+    isatty,
     remove_default_schema_routes,
     remove_routes_with_patterns,
     show_app_info,
     validate_ssl_file_paths,
 )
 from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.utils.helpers import unwrap_partial
@@ -99,14 +100,23 @@
         process_args["ssl-keyfile"] = keyfile_path
     subprocess.run(
         [sys.executable, "-m", "uvicorn", env.app_path, *_convert_uvicorn_args(process_args)],  # noqa: S603
         check=True,
     )
 
 
+class CommaSplittedPath(click.Path):
+    """A Click Path that splits the input string by commas.
+
+    .. versionadded:: 2.8.0
+    """
+
+    envvar_list_splitter = ","
+
+
 @command(name="version")
 @option("-s", "--short", help="Exclude release level and serial information", is_flag=True, default=False)
 def version_command(short: bool) -> None:
     """Show the currently installed Litestar version."""
     from litestar import __version__
 
     click.echo(__version__.formatted(short=short))
@@ -116,51 +126,79 @@
 def info_command(app: Litestar) -> None:
     """Show information about the detected Litestar app."""
 
     show_app_info(app)
 
 
 @command(name="run")
-@option("-r", "--reload", help="Reload server on changes", default=False, is_flag=True)
-@option("-R", "--reload-dir", help="Directories to watch for file changes", multiple=True)
+@option("-r", "--reload", help="Reload server on changes", default=False, is_flag=True, envvar="LITESTAR_RELOAD")
+@option(
+    "-R",
+    "--reload-dir",
+    help="Directories to watch for file changes",
+    type=CommaSplittedPath(),
+    multiple=True,
+    envvar="LITESTAR_RELOAD_DIRS",
+)
 @option(
-    "-I", "--reload-include", help="Glob patterns for files to include when watching for file changes", multiple=True
+    "-I",
+    "--reload-include",
+    help="Glob patterns for files to include when watching for file changes",
+    type=CommaSplittedPath(),
+    multiple=True,
+    envvar="LITESTAR_RELOAD_INCLUDES",
 )
 @option(
-    "-E", "--reload-exclude", help="Glob patterns for files to exclude when watching for file changes", multiple=True
+    "-E",
+    "--reload-exclude",
+    help="Glob patterns for files to exclude when watching for file changes",
+    type=CommaSplittedPath(),
+    multiple=True,
+    envvar="LITESTAR_RELOAD_EXCLUDES",
 )
-@option("-p", "--port", help="Serve under this port", type=int, default=8000, show_default=True)
+@option("-p", "--port", help="Serve under this port", type=int, default=8000, show_default=True, envvar="LITESTAR_PORT")
 @option(
     "-W",
     "--wc",
     "--web-concurrency",
     help="The number of HTTP workers to launch",
     type=click.IntRange(min=1, max=multiprocessing.cpu_count() + 1),
     show_default=True,
     default=1,
+    envvar=["LITESTAR_WEB_CONCURRENCY", "WEB_CONCURRENCY"],
 )
-@option("-H", "--host", help="Server under this host", default="127.0.0.1", show_default=True)
+@option("-H", "--host", help="Server under this host", default="127.0.0.1", show_default=True, envvar="LITESTAR_HOST")
 @option(
     "-F",
     "--fd",
     "--file-descriptor",
     help="Bind to a socket from this file descriptor.",
     type=int,
     default=None,
     show_default=True,
+    envvar="LITESTAR_FILE_DESCRIPTOR",
 )
-@option("-U", "--uds", "--unix-domain-socket", help="Bind to a UNIX domain socket.", default=None, show_default=True)
-@option("-d", "--debug", help="Run app in debug mode", is_flag=True)
-@option("-P", "--pdb", "--use-pdb", help="Drop into PDB on an exception", is_flag=True)
-@option("--ssl-certfile", help="Location of the SSL cert file", default=None)
-@option("--ssl-keyfile", help="Location of the SSL key file", default=None)
+@option(
+    "-U",
+    "--uds",
+    "--unix-domain-socket",
+    help="Bind to a UNIX domain socket.",
+    default=None,
+    show_default=True,
+    envvar="LITESTAR_UNIX_DOMAIN_SOCKET",
+)
+@option("-d", "--debug", help="Run app in debug mode", is_flag=True, envvar="LITESTAR_DEBUG")
+@option("-P", "--pdb", "--use-pdb", help="Drop into PDB on an exception", is_flag=True, envvar="LITESTAR_PDB")
+@option("--ssl-certfile", help="Location of the SSL cert file", default=None, envvar="LITESTAR_SSL_CERT_PATH")
+@option("--ssl-keyfile", help="Location of the SSL key file", default=None, envvar="LITESTAR_SSL_KEY_PATH")
 @option(
     "--create-self-signed-cert",
     help="If certificate and key are not found at specified locations, create a self-signed certificate and a key",
     is_flag=True,
+    envvar="LITESTAR_CREATE_SELF_SIGNED_CERT",
 )
 def run_command(
     reload: bool,
     port: int,
     wc: int,
     host: str,
     fd: int | None,
@@ -185,15 +223,15 @@
     """
 
     if debug:
         os.environ["LITESTAR_DEBUG"] = "1"
 
     if pdb:
         os.environ["LITESTAR_PDB"] = "1"
-
+    quiet_console = os.getenv("LITESTAR_QUIET_CONSOLE") or False
     if not UVICORN_INSTALLED:
         console.print(
             r"uvicorn is not installed. Please install the standard group, litestar\[standard], to use this command."
         )
         sys.exit(1)
 
     if callable(ctx.obj):
@@ -203,38 +241,26 @@
             ctx.obj.app.debug = True
         if pdb:
             ctx.obj.app.pdb_on_exception = True
 
     env: LitestarEnv = ctx.obj
     app = env.app
 
-    reload_dirs = env.reload_dirs or reload_dir
-    reload_include = env.reload_include or reload_include
-    reload_exclude = env.reload_exclude or reload_exclude
-
-    host = env.host or host
-    port = env.port if env.port is not None else port
-    fd = env.fd if env.fd is not None else fd
-    uds = env.uds or uds
-    reload = env.reload or reload or bool(reload_dirs) or bool(reload_include) or bool(reload_exclude)
-    workers = env.web_concurrency or wc
-
-    ssl_certfile = ssl_certfile or env.certfile_path
-    ssl_keyfile = ssl_keyfile or env.keyfile_path
-    create_self_signed_cert = create_self_signed_cert or env.create_self_signed_cert
+    reload = reload or bool(reload_dir) or bool(reload_include) or bool(reload_exclude)
+    workers = wc
 
     certfile_path, keyfile_path = (
         create_ssl_files(ssl_certfile, ssl_keyfile, host)
         if create_self_signed_cert
         else validate_ssl_file_paths(ssl_certfile, ssl_keyfile)
     )
 
-    console.rule("[yellow]Starting server process", align="left")
-
-    show_app_info(app)
+    if not quiet_console and isatty():
+        console.rule("[yellow]Starting server process", align="left")
+        show_app_info(app)
     with _server_lifespan(app):
         if workers == 1 and not reload:
             import uvicorn
 
             # A guard statement at the beginning of this function prevents uvicorn from being unbound
             # See "reportUnboundVariable in:
             # https://microsoft.github.io/pyright/#/configuration?id=type-check-diagnostics-settings
@@ -259,15 +285,15 @@
 
             _run_uvicorn_in_subprocess(
                 env=env,
                 host=host,
                 port=port,
                 workers=workers,
                 reload=reload,
-                reload_dirs=reload_dirs,
+                reload_dirs=reload_dir,
                 reload_include=reload_include,
                 reload_exclude=reload_exclude,
                 fd=fd,
                 uds=uds,
                 certfile_path=certfile_path,
                 keyfile_path=keyfile_path,
             )
```

### Comparing `litestar-2.7.1/litestar/cli/commands/schema.py` & `litestar-2.8.0/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/cli/commands/sessions.py` & `litestar-2.8.0/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/config/allowed_hosts.py` & `litestar-2.8.0/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/config/app.py` & `litestar-2.8.0/litestar/config/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,20 @@
     """A string keyed dictionary of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
     wherever you have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <litestar.types.Scope>`.
 
     Can be overridden by routers and router handlers.
     """
     parameters: ParametersMap = field(default_factory=dict)
     """A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application paths."""
+    path: str = field(default="")
+    """A base path that prefixed to all route handlers, controllers and routers associated with the
+    application instance.
+
+    .. versionadded:: 2.8.0
+    """
     pdb_on_exception: bool = field(default=False)
     """Drop into the PDB on an exception"""
     plugins: list[PluginProtocol] = field(default_factory=list)
     """List of :class:`SerializationPluginProtocol <.plugins.SerializationPluginProtocol>`."""
     request_class: type[Request] | None = field(default=None)
     """An optional subclass of :class:`Request <.connection.Request>` to use for http connections."""
     response_class: type[Response] | None = field(default=None)
```

### Comparing `litestar-2.7.1/litestar/config/compression.py` & `litestar-2.8.0/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/config/cors.py` & `litestar-2.8.0/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/config/csrf.py` & `litestar-2.8.0/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/config/response_cache.py` & `litestar-2.8.0/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/connection/__init__.py` & `litestar-2.8.0/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/connection/base.py` & `litestar-2.8.0/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/connection/request.py` & `litestar-2.8.0/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/connection/websocket.py` & `litestar-2.8.0/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/jinja.py` & `litestar-2.8.0/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/mako.py` & `litestar-2.8.0/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/minijinja.py` & `litestar-2.8.0/litestar/contrib/minijinja.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,25 +155,33 @@
 
         Raises:
             TemplateNotFoundException: if no template is found.
         """
         return MiniJinjaTemplate(self.engine, template_name)
 
     def register_template_callable(
-        self, key: str, template_callable: TemplateCallableType[StateProtocol, P, T]
+        self,
+        key: str,
+        template_callable: TemplateCallableType[StateProtocol, P, T],
     ) -> None:
         """Register a callable on the template engine.
 
         Args:
             key: The callable key, i.e. the value to use inside the template to call the callable.
             template_callable: A callable to register.
 
         Returns:
             None
         """
+
+        def is_decorated(func: Callable) -> bool:
+            return hasattr(func, "__wrapped__") or func.__name__ not in globals()
+
+        if not is_decorated(template_callable):
+            template_callable = _transform_state(template_callable)  # type: ignore[arg-type] # pragma: no cover
         self.engine.add_global(key, pass_state(template_callable))
 
     def render_string(self, template_string: str, context: Mapping[str, Any]) -> str:
         """Render a template from a string with the given context.
 
         Args:
             template_string: The template string to render.
```

### Comparing `litestar-2.7.1/litestar/contrib/piccolo.py` & `litestar-2.8.0/litestar/contrib/piccolo.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/htmx/_utils.py` & `litestar-2.8.0/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/htmx/request.py` & `litestar-2.8.0/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/htmx/response.py` & `litestar-2.8.0/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/htmx/types.py` & `litestar-2.8.0/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/jwt/__init__.py` & `litestar-2.8.0/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.8.0/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/opentelemetry/config.py` & `litestar-2.8.0/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.8.0/litestar/contrib/opentelemetry/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     from litestar.contrib.opentelemetry import OpenTelemetryConfig
     from litestar.types import ASGIApp, Receive, Scope, Send
 
 
 class OpenTelemetryInstrumentationMiddleware(AbstractMiddleware):
     """OpenTelemetry Middleware."""
 
-    __slots__ = ("open_telemetry_middleware",)
-
     def __init__(self, app: ASGIApp, config: OpenTelemetryConfig) -> None:
         """Middleware that adds OpenTelemetry instrumentation to the application.
 
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of :class:`OpenTelemetryConfig <.contrib.opentelemetry.OpenTelemetryConfig>`
         """
```

### Comparing `litestar-2.7.1/litestar/contrib/prometheus/config.py` & `litestar-2.8.0/litestar/contrib/prometheus/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/prometheus/controller.py` & `litestar-2.8.0/litestar/contrib/prometheus/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/prometheus/middleware.py` & `litestar-2.8.0/litestar/contrib/prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/pydantic/__init__.py` & `litestar-2.8.0/litestar/contrib/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/pydantic/pydantic_di_plugin.py` & `litestar-2.8.0/litestar/contrib/pydantic/pydantic_di_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/pydantic/pydantic_dto_factory.py` & `litestar-2.8.0/litestar/contrib/pydantic/pydantic_dto_factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from dataclasses import replace
-from typing import TYPE_CHECKING, Collection, Generic, TypeVar
+from typing import TYPE_CHECKING, Any, Collection, Generic, TypeVar
+from warnings import warn
 
-from typing_extensions import TypeAlias, override
+from typing_extensions import Annotated, TypeAlias, override
 
 from litestar.contrib.pydantic.utils import is_pydantic_undefined
 from litestar.dto.base_dto import AbstractDTO
 from litestar.dto.data_structures import DTOFieldDefinition
-from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
+from litestar.dto.field import DTO_FIELD_META_KEY, extract_dto_field
 from litestar.exceptions import MissingDependencyException, ValidationException
 from litestar.types.empty import Empty
+from litestar.typing import FieldDefinition
 
 if TYPE_CHECKING:
-    from typing import Any, Generator
-
-    from litestar.typing import FieldDefinition
+    from typing import Generator
 
 try:
     import pydantic as _  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("pydantic") from e
 
 
@@ -42,31 +42,59 @@
 
 
 T = TypeVar("T", bound="ModelType | Collection[ModelType]")
 
 
 __all__ = ("PydanticDTO",)
 
+_down_types = {
+    pydantic_v2.JsonValue: Any,
+    pydantic_v1.EmailStr: str,
+    pydantic_v2.EmailStr: str,
+    pydantic_v1.IPvAnyAddress: str,
+    pydantic_v2.IPvAnyAddress: str,
+    pydantic_v1.IPvAnyInterface: str,
+    pydantic_v2.IPvAnyInterface: str,
+    pydantic_v1.IPvAnyNetwork: str,
+    pydantic_v2.IPvAnyNetwork: str,
+}
+
+
+def convert_validation_error(validation_error: ValidationErrorV1 | ValidationErrorV2) -> list[dict[str, Any]]:
+    error_list = validation_error.errors()
+    for error in error_list:
+        if isinstance(exception := error.get("ctx", {}).get("error"), Exception):
+            error["ctx"]["error"] = type(exception).__name__
+    return error_list  # type: ignore[return-value]
+
+
+def downtype_for_data_transfer(field_definition: FieldDefinition) -> FieldDefinition:
+    if sub := _down_types.get(field_definition.annotation):
+        return FieldDefinition.from_kwarg(
+            annotation=Annotated[sub, field_definition.metadata], name=field_definition.name
+        )
+    return field_definition
+
 
 class PydanticDTO(AbstractDTO[T], Generic[T]):
     """Support for domain modelling with Pydantic."""
 
     @override
     def decode_builtins(self, value: dict[str, Any]) -> Any:
         try:
             return super().decode_builtins(value)
         except (ValidationErrorV2, ValidationErrorV1) as ex:
-            raise ValidationException(extra=ex.errors()) from ex
+            raise ValidationException(extra=convert_validation_error(ex)) from ex
 
     @override
     def decode_bytes(self, value: bytes) -> Any:
         try:
             return super().decode_bytes(value)
         except (ValidationErrorV2, ValidationErrorV1) as ex:
-            raise ValidationException(extra=ex.errors()) from ex
+            raise ValidationException(extra=convert_validation_error(ex)) from ex
 
     @classmethod
     def generate_field_definitions(
         cls, model_type: type[pydantic_v1.BaseModel | pydantic_v2.BaseModel]
     ) -> Generator[DTOFieldDefinition, None, None]:
         model_field_definitions = cls.get_model_type_hints(model_type)
 
@@ -76,16 +104,30 @@
         except AttributeError:
             model_fields = {
                 k: model_field.field_info
                 for k, model_field in model_type.__fields__.items()  # type: ignore[union-attr]
             }
 
         for field_name, field_info in model_fields.items():
-            field_definition = model_field_definitions[field_name]
-            dto_field = (field_definition.extra or {}).pop(DTO_FIELD_META_KEY, DTOField())
+            field_definition = downtype_for_data_transfer(model_field_definitions[field_name])
+            dto_field = extract_dto_field(field_definition, field_definition.extra)
+
+            try:
+                extra = field_info.extra  # type: ignore[union-attr]
+            except AttributeError:
+                extra = field_info.json_schema_extra  # type: ignore[union-attr]
+
+            if extra is not None and extra.pop(DTO_FIELD_META_KEY, None):
+                warn(
+                    message="Declaring 'DTOField' via Pydantic's 'Field.extra' is deprecated. "
+                    "Use 'Annotated', e.g., 'Annotated[str, DTOField(mark='read-only')]' instead. "
+                    "Support for 'DTOField' in 'Field.extra' will be removed in v3.",
+                    category=DeprecationWarning,
+                    stacklevel=2,
+                )
 
             if not is_pydantic_undefined(field_info.default):
                 default = field_info.default
             elif field_definition.is_optional:
                 default = None
             else:
                 default = Empty
```

### Comparing `litestar-2.7.1/litestar/contrib/pydantic/pydantic_init_plugin.py` & `litestar-2.8.0/litestar/contrib/pydantic/pydantic_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/pydantic/pydantic_schema_plugin.py` & `litestar-2.8.0/litestar/contrib/pydantic/pydantic_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/pydantic/utils.py` & `litestar-2.8.0/litestar/contrib/pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/repository/__init__.py` & `litestar-2.8.0/litestar/contrib/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/repository/exceptions.py` & `litestar-2.8.0/litestar/contrib/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/repository/filters.py` & `litestar-2.8.0/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/repository/handlers.py` & `litestar-2.8.0/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/repository/testing.py` & `litestar-2.8.0/litestar/contrib/repository/testing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/repository/abc/__init__.py` & `litestar-2.8.0/litestar/contrib/repository/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/sqlalchemy/base.py` & `litestar-2.8.0/litestar/contrib/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/compat.py` & `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/datastructures/__init__.py` & `litestar-2.8.0/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/datastructures/cookie.py` & `litestar-2.8.0/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/datastructures/headers.py` & `litestar-2.8.0/litestar/datastructures/headers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from abc import ABC, abstractmethod
 from contextlib import suppress
 from copy import copy
-from dataclasses import dataclass
+from dataclasses import dataclass, fields
 from typing import (
     TYPE_CHECKING,
+    AbstractSet,
     Any,
     ClassVar,
     Dict,
     Iterable,
     Iterator,
     List,
     Mapping,
@@ -16,23 +17,21 @@
     Optional,
     Pattern,
     Tuple,
     Union,
     cast,
 )
 
+import msgspec
 from multidict import CIMultiDict, CIMultiDictProxy, MultiMapping
-from typing_extensions import get_type_hints
 
 from litestar._multipart import parse_content_header
 from litestar.datastructures.multi_dicts import MultiMixin
-from litestar.dto.base_dto import AbstractDTO
 from litestar.exceptions import ImproperlyConfiguredException, ValidationException
 from litestar.types.empty import Empty
-from litestar.typing import FieldDefinition
 from litestar.utils.dataclass import simple_asdict
 from litestar.utils.scope.state import ScopeState
 
 if TYPE_CHECKING:
     from litestar.types.asgi_types import (
         HeaderScope,
         Message,
@@ -299,15 +298,15 @@
     must_understand: Optional[bool] = None
     """Accessor for the ``must-understand`` directive."""
     immutable: Optional[bool] = None
     """Accessor for the ``immutable`` directive."""
     stale_while_revalidate: Optional[int] = None
     """Accessor for the ``stale-while-revalidate`` directive."""
 
-    _field_definitions: ClassVar[Optional[Dict[str, FieldDefinition]]] = None
+    _field_names: ClassVar[AbstractSet[str]]
 
     def _get_header_value(self) -> str:
         """Get the header value as string."""
 
         cc_items = [
             key.replace("_", "-") if isinstance(value, bool) else f"{key.replace('_', '-')}={value}"
             for key, value in simple_asdict(self, exclude_none=True, exclude={"documentation_only"}).items()
@@ -321,80 +320,55 @@
         Args:
             header_value: the header value as string
 
         Returns:
             An instance of ``CacheControlHeader``
         """
 
-        cc_items = [v.strip() for v in header_value.split(",")]
         kwargs: Dict[str, Any] = {}
-        field_definitions = cls._get_field_definitions()
-        for cc_item in cc_items:
-            key_value = cc_item.split("=")
-            key_value[0] = key_value[0].replace("-", "_")
-            if len(key_value) == 1:
-                kwargs[key_value[0]] = True
-            elif len(key_value) == 2:
-                key, value = key_value
-                if key not in field_definitions:
-                    raise ImproperlyConfiguredException("Invalid cache-control header")
-                kwargs[key] = cls._convert_to_type(value, field_definition=field_definitions[key])
+        field_names = cls._get_field_names()
+        for cc_item in (stripped for v in header_value.split(",") if (stripped := v.strip())):
+            key, *value = cc_item.split("=", maxsplit=1)
+            key = key.replace("-", "_")
+            if key not in field_names:
+                raise ImproperlyConfiguredException("Invalid cache-control header")
+            if not value:
+                kwargs[key] = True
             else:
-                raise ImproperlyConfiguredException("Invalid cache-control header value")
+                (kwargs[key],) = value
 
         try:
-            return CacheControlHeader(**kwargs)
-        except TypeError as exc:
+            return msgspec.convert(kwargs, CacheControlHeader, strict=False)
+        except msgspec.ValidationError as exc:
             raise ImproperlyConfiguredException from exc
 
     @classmethod
     def prevent_storing(cls) -> "CacheControlHeader":
         """Create a ``cache-control`` header with the ``no-store`` directive which indicates that any caches of any kind
         (private or shared) should not store this response.
         """
 
         return cls(no_store=True)
 
     @classmethod
-    def _get_field_definitions(cls) -> Dict[str, FieldDefinition]:
+    def _get_field_names(cls) -> AbstractSet[str]:
         """Get the type annotations for the ``CacheControlHeader`` class properties.
 
         This is needed due to the conversion from pydantic models to dataclasses. Dataclasses do not support
         automatic conversion of types like pydantic models do.
 
         Returns:
             A dictionary of type annotations
 
         """
-
-        if cls._field_definitions is None:
-            cls._field_definitions = {}
-            for key, value in get_type_hints(cls, include_extras=True).items():
-                definition = FieldDefinition.from_kwarg(annotation=value, name=key)
-                # resolve_model_type so that field_definition.raw has the real raw type e.g. <class 'bool'>
-                cls._field_definitions[key] = AbstractDTO.resolve_model_type(definition)
-        return cls._field_definitions
-
-    @classmethod
-    def _convert_to_type(cls, value: str, field_definition: FieldDefinition) -> Any:
-        """Convert the value to the expected type.
-
-        Args:
-            value: the value of the cache-control directive
-            field_definition: the field definition for the value to convert
-
-        Returns:
-            The value converted to the expected type
-        """
-        # bool values shouldn't be initiated since they should have been caught earlier in the from_header method and
-        # set with a value of True
-        expected_type = field_definition.raw
-        if expected_type is bool:
-            raise ImproperlyConfiguredException("Invalid cache-control header value")
-        return expected_type(value)
+        try:
+            names = cls._field_names
+        except AttributeError:
+            names = cls._field_names = {f.name for f in fields(cls)}
+        return names
 
 
 @dataclass
 class ETag(Header):
     """An ``etag`` header."""
 
     HEADER_NAME: ClassVar[str] = "etag"
```

### Comparing `litestar-2.7.1/litestar/datastructures/multi_dicts.py` & `litestar-2.8.0/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/datastructures/response_header.py` & `litestar-2.8.0/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/datastructures/state.py` & `litestar-2.8.0/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/datastructures/upload_file.py` & `litestar-2.8.0/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/datastructures/url.py` & `litestar-2.8.0/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/dto/_backend.py` & `litestar-2.8.0/litestar/dto/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,14 +402,16 @@
 
         transfer_model: NestedFieldInfo | None = None
 
         if self.dto_factory.detect_nested_field(field_definition):
             if nested_depth == self.dto_factory.config.max_nested_depth:
                 raise RecursionError
 
+            unique_name = f"{unique_name}{field_definition.raw.__name__}"
+
             nested_field_definitions = self.parse_model(
                 model_type=field_definition.annotation,
                 exclude=exclude,
                 include=include,
                 rename_fields=rename_fields,
                 nested_depth=nested_depth + 1,
             )
```

### Comparing `litestar-2.7.1/litestar/dto/_codegen_backend.py` & `litestar-2.8.0/litestar/dto/_codegen_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/dto/_types.py` & `litestar-2.8.0/litestar/dto/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,14 @@
     key_type: CompositeType | SimpleType
     value_type: CompositeType | SimpleType
 
 
 @dataclass(frozen=True)
 class TransferDTOFieldDefinition(DTOFieldDefinition):
     __slots__ = (
-        "default_factory",
-        "dto_field",
-        "model_name",
         "is_excluded",
         "is_partial",
         "serialization_name",
         "transfer_type",
         "unique_name",
     )
```

### Comparing `litestar-2.7.1/litestar/dto/base_dto.py` & `litestar-2.8.0/litestar/dto/base_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,17 +174,15 @@
                     model_type_field_definition, field_definition, wrapper_attribute_name = resolved_generic_result
                 else:
                     raise InvalidAnnotationException(
                         f"DTO narrowed with '{cls.model_type}', handler type is '{field_definition.annotation}'"
                     )
 
             if backend_cls is None:
-                backend_cls = DTOCodegenBackend if cls.config.experimental_codegen_backend else DTOBackend
-            elif backend_cls is DTOCodegenBackend and cls.config.experimental_codegen_backend is False:
-                backend_cls = DTOBackend
+                backend_cls = DTOCodegenBackend if cls.config.experimental_codegen_backend is not False else DTOBackend
 
             backend_context[key] = backend_cls(  # type: ignore[literal-required]
                 dto_factory=cls,
                 field_definition=field_definition,
                 model_type=model_type_field_definition.annotation,
                 wrapper_attribute_name=wrapper_attribute_name,
                 is_data_field=field_definition.name == "data",
```

### Comparing `litestar-2.7.1/litestar/dto/config.py` & `litestar-2.8.0/litestar/dto/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/dto/data_structures.py` & `litestar-2.8.0/litestar/dto/data_structures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/dto/dataclass_dto.py` & `litestar-2.8.0/litestar/dto/msgspec_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 from __future__ import annotations
 
-from dataclasses import MISSING, fields, replace
+from dataclasses import replace
 from typing import TYPE_CHECKING, Generic, TypeVar
 
+from msgspec import NODEFAULT, Struct, structs
+
 from litestar.dto.base_dto import AbstractDTO
 from litestar.dto.data_structures import DTOFieldDefinition
-from litestar.dto.field import DTO_FIELD_META_KEY, DTOField
-from litestar.params import DependencyKwarg, KwargDefinition
+from litestar.dto.field import DTO_FIELD_META_KEY, extract_dto_field
 from litestar.types.empty import Empty
 
 if TYPE_CHECKING:
-    from typing import Collection, Generator
+    from typing import Any, Collection, Generator
 
-    from litestar.types.protocols import DataclassProtocol
     from litestar.typing import FieldDefinition
 
 
-__all__ = ("DataclassDTO", "T")
+__all__ = ("MsgspecDTO",)
 
-T = TypeVar("T", bound="DataclassProtocol | Collection[DataclassProtocol]")
-AnyDataclass = TypeVar("AnyDataclass", bound="DataclassProtocol")
+T = TypeVar("T", bound="Struct | Collection[Struct]")
 
 
-class DataclassDTO(AbstractDTO[T], Generic[T]):
-    """Support for domain modelling with dataclasses."""
+class MsgspecDTO(AbstractDTO[T], Generic[T]):
+    """Support for domain modelling with Msgspec."""
 
     @classmethod
-    def generate_field_definitions(
-        cls, model_type: type[DataclassProtocol]
-    ) -> Generator[DTOFieldDefinition, None, None]:
-        dc_fields = {f.name: f for f in fields(model_type)}
+    def generate_field_definitions(cls, model_type: type[Struct]) -> Generator[DTOFieldDefinition, None, None]:
+        msgspec_fields = {f.name: f for f in structs.fields(model_type)}
+
+        def default_or_empty(value: Any) -> Any:
+            return Empty if value is NODEFAULT else value
+
+        def default_or_none(value: Any) -> Any:
+            return None if value is NODEFAULT else value
+
         for key, field_definition in cls.get_model_type_hints(model_type).items():
-            if not (dc_field := dc_fields.get(key)):
-                continue
+            msgspec_field = msgspec_fields[key]
+            dto_field = extract_dto_field(field_definition, field_definition.extra)
+            field_definition.extra.pop(DTO_FIELD_META_KEY, None)
 
-            default = dc_field.default if dc_field.default is not MISSING else Empty
-            default_factory = dc_field.default_factory if dc_field.default_factory is not MISSING else None
-            field_defintion = replace(
+            yield replace(
                 DTOFieldDefinition.from_field_definition(
                     field_definition=field_definition,
-                    default_factory=default_factory,
-                    dto_field=dc_field.metadata.get(DTO_FIELD_META_KEY, DTOField()),
+                    dto_field=dto_field,
                     model_name=model_type.__name__,
+                    default_factory=default_or_none(msgspec_field.default_factory),
                 ),
+                default=default_or_empty(msgspec_field.default),
                 name=key,
-                default=default,
-            )
-
-            yield (
-                replace(field_defintion, default=Empty, kwarg_definition=default)
-                if isinstance(default, (KwargDefinition, DependencyKwarg))
-                else field_defintion
             )
 
     @classmethod
     def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
-        return hasattr(field_definition.annotation, "__dataclass_fields__")
+        return field_definition.is_subclass_of(Struct)
```

### Comparing `litestar-2.7.1/litestar/events/emitter.py` & `litestar-2.8.0/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/events/listener.py` & `litestar-2.8.0/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/exceptions/__init__.py` & `litestar-2.8.0/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/exceptions/base_exceptions.py` & `litestar-2.8.0/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/exceptions/http_exceptions.py` & `litestar-2.8.0/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/exceptions/websocket_exceptions.py` & `litestar-2.8.0/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/handlers/__init__.py` & `litestar-2.8.0/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/handlers/asgi_handlers.py` & `litestar-2.8.0/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/handlers/base.py` & `litestar-2.8.0/litestar/handlers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from copy import copy
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Mapping, Sequence, cast
 
 from litestar._signature import SignatureModel
-from litestar.config.app import ExperimentalFeatures
 from litestar.di import Provide
 from litestar.dto import DTOData
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.plugins import DIPlugin, PluginRegistry
 from litestar.serialization import default_deserializer, default_serializer
 from litestar.types import (
     Dependencies,
@@ -28,15 +27,14 @@
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from litestar.app import Litestar
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
     from litestar.dto import AbstractDTO
-    from litestar.dto._backend import DTOBackend
     from litestar.params import ParameterKwarg
     from litestar.router import Router
     from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
     from litestar.types.empty import EmptyType
 
 __all__ = ("BaseRouteHandler",)
 
@@ -438,21 +436,14 @@
             ns: dict[str, Any] = {}
             for layer in self.ownership_layers:
                 ns.update(layer.signature_namespace)
 
             self._resolved_signature_namespace = ns
         return cast("dict[str, Any]", self._resolved_signature_namespace)
 
-    def _get_dto_backend_cls(self) -> type[DTOBackend] | None:
-        if ExperimentalFeatures.DTO_CODEGEN in self.app.experimental_features:
-            from litestar.dto._codegen_backend import DTOCodegenBackend
-
-            return DTOCodegenBackend
-        return None
-
     def resolve_data_dto(self) -> type[AbstractDTO] | None:
         """Resolve the data_dto by starting from the route handler and moving up.
         If a handler is found it is returned, otherwise None is set.
         This method is memoized so the computation occurs only once.
 
         Returns:
             An optional :class:`DTO type <.dto.base_dto.AbstractDTO>`
@@ -474,15 +465,14 @@
             else:
                 data_dto = None
 
             if self.parsed_data_field and data_dto:
                 data_dto.create_for_field_definition(
                     field_definition=self.parsed_data_field,
                     handler_id=self.handler_id,
-                    backend_cls=self._get_dto_backend_cls(),
                 )
 
             self._resolved_data_dto = data_dto
 
         return self._resolved_data_dto
 
     def resolve_return_dto(self) -> type[AbstractDTO] | None:
@@ -508,15 +498,14 @@
             else:
                 return_dto = self.resolve_data_dto()
 
             if return_dto and return_dto.is_supported_model_type_field(self.parsed_return_field):
                 return_dto.create_for_field_definition(
                     field_definition=self.parsed_return_field,
                     handler_id=self.handler_id,
-                    backend_cls=self._get_dto_backend_cls(),
                 )
                 self._resolved_return_dto = return_dto
             else:
                 self._resolved_return_dto = None
 
         return self._resolved_return_dto
```

### Comparing `litestar-2.7.1/litestar/handlers/http_handlers/_utils.py` & `litestar-2.8.0/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/handlers/http_handlers/base.py` & `litestar-2.8.0/litestar/handlers/http_handlers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     """
 
     __slots__ = (
         "_resolved_after_response",
         "_resolved_before_request",
         "_response_handler_mapping",
         "_resolved_include_in_schema",
+        "_resolved_response_class",
+        "_resolved_request_class",
         "_resolved_tags",
         "_resolved_security",
         "after_request",
         "after_response",
         "background",
         "before_request",
         "cache",
@@ -286,14 +288,16 @@
         self.security = security
         self.responses = responses
         # memoized attributes, defaulted to Empty
         self._resolved_after_response: AsyncAnyCallable | None | EmptyType = Empty
         self._resolved_before_request: AsyncAnyCallable | None | EmptyType = Empty
         self._response_handler_mapping: ResponseHandlerMap = {"default_handler": Empty, "response_type_handler": Empty}
         self._resolved_include_in_schema: bool | EmptyType = Empty
+        self._resolved_response_class: type[Response] | EmptyType = Empty
+        self._resolved_request_class: type[Request] | EmptyType = Empty
         self._resolved_security: list[SecurityRequirement] | EmptyType = Empty
         self._resolved_tags: list[str] | EmptyType = Empty
 
     def __call__(self, fn: AnyCallable) -> HTTPRouteHandler:
         """Replace a function with itself."""
         if not is_async_callable(fn):
             if self.sync_to_thread is None:
@@ -308,31 +312,38 @@
         """Return the closest custom Request class in the owner graph or the default Request class.
 
         This method is memoized so the computation occurs only once.
 
         Returns:
             The default :class:`Request <.connection.Request>` class for the route handler.
         """
-        return next(
-            (layer.request_class for layer in reversed(self.ownership_layers) if layer.request_class is not None),
-            Request,
-        )
+
+        if self._resolved_request_class is Empty:
+            self._resolved_request_class = next(
+                (layer.request_class for layer in reversed(self.ownership_layers) if layer.request_class is not None),
+                Request,
+            )
+
+        return cast("type[Request]", self._resolved_request_class)
 
     def resolve_response_class(self) -> type[Response]:
         """Return the closest custom Response class in the owner graph or the default Response class.
 
         This method is memoized so the computation occurs only once.
 
         Returns:
             The default :class:`Response <.response.Response>` class for the route handler.
         """
-        return next(
-            (layer.response_class for layer in reversed(self.ownership_layers) if layer.response_class is not None),
-            Response,
-        )
+        if self._resolved_response_class is Empty:
+            self._resolved_response_class = next(
+                (layer.response_class for layer in reversed(self.ownership_layers) if layer.response_class is not None),
+                Response,
+            )
+
+        return cast("type[Response]", self._resolved_response_class)
 
     def resolve_response_headers(self) -> frozenset[ResponseHeader]:
         """Return all header parameters in the scope of the handler function.
 
         Returns:
             A dictionary mapping keys to :class:`ResponseHeader <.datastructures.ResponseHeader>` instances.
         """
```

### Comparing `litestar-2.7.1/litestar/handlers/http_handlers/decorators.py` & `litestar-2.8.0/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.8.0/litestar/handlers/websocket_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.8.0/litestar/handlers/websocket_handlers/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,19 +58,18 @@
     returned
     """
 
     __slots__ = {
         "connection_accept_handler": "Callback to accept a WebSocket connection. By default, calls WebSocket.accept",
         "on_accept": "Callback invoked after a WebSocket connection has been accepted",
         "on_disconnect": "Callback invoked after a WebSocket connection has been closed",
-        "weboscket_class": "WebSocket class",
         "_connection_lifespan": None,
-        "_handle_receive": None,
-        "_handle_send": None,
+        "_receive_handler": None,
         "_receive_mode": None,
+        "_send_handler": None,
         "_send_mode": None,
     }
 
     @overload
     def __init__(
         self,
         path: str | list[str] | None = None,
```

### Comparing `litestar-2.7.1/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.8.0/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 class WebsocketRouteHandler(BaseRouteHandler):
     """Websocket route handler decorator.
 
     Use this decorator to decorate websocket handler functions.
     """
 
+    __slots__ = ("websocket_class",)
+
     def __init__(
         self,
         path: str | list[str] | None = None,
         *,
         dependencies: Dependencies | None = None,
         exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
         guards: list[Guard] | None = None,
```

### Comparing `litestar-2.7.1/litestar/logging/_utils.py` & `litestar-2.8.0/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/logging/config.py` & `litestar-2.8.0/litestar/logging/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,14 @@
     from structlog.types import BindableLogger, Processor, WrappedLogger
     from structlog.typing import EventDict
 
     from litestar.types import Logger, Scope
     from litestar.types.callable_types import ExceptionLoggingHandler, GetLogger
 
 
-try:
-    from structlog.types import BindableLogger, Processor, WrappedLogger
-except ImportError:
-    BindableLogger = Any  # type: ignore[assignment, misc]
-    Processor = Any  # type: ignore[misc]
-    WrappedLogger = Any  # type: ignore[misc]
-
-
 default_handlers: dict[str, dict[str, Any]] = {
     "console": {
         "class": "logging.StreamHandler",
         "level": "DEBUG",
         "formatter": "standard",
     },
     "queue_listener": {
```

### Comparing `litestar-2.7.1/litestar/logging/picologging.py` & `litestar-2.8.0/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/logging/standard.py` & `litestar-2.8.0/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/_utils.py` & `litestar-2.8.0/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/allowed_hosts.py` & `litestar-2.8.0/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/authentication.py` & `litestar-2.8.0/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/base.py` & `litestar-2.8.0/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/cors.py` & `litestar-2.8.0/litestar/middleware/cors.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     from litestar.config.cors import CORSConfig
     from litestar.types import ASGIApp, Message, Receive, Scope, Send
 
 
 class CORSMiddleware(AbstractMiddleware):
     """CORS Middleware."""
 
-    __slots__ = ("config",)
-
     def __init__(self, app: ASGIApp, config: CORSConfig) -> None:
         """Middleware that adds CORS validation to the application.
 
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of :class:`CORSConfig <litestar.config.cors.CORSConfig>`
         """
```

### Comparing `litestar-2.7.1/litestar/middleware/csrf.py` & `litestar-2.8.0/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/logging.py` & `litestar-2.8.0/litestar/middleware/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     BindableLogger = object  # type: ignore[assignment, misc]
     structlog_installed = False
 
 
 class LoggingMiddleware(AbstractMiddleware):
     """Logging middleware."""
 
-    __slots__ = ("config", "logger", "request_extractor", "response_extractor", "is_struct_logger")
-
     logger: Logger
 
     def __init__(self, app: ASGIApp, config: LoggingMiddlewareConfig) -> None:
         """Initialize ``LoggingMiddleware``.
 
         Args:
             app: The ``next`` ASGI app to call.
```

### Comparing `litestar-2.7.1/litestar/middleware/rate_limit.py` & `litestar-2.8.0/litestar/middleware/rate_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,14 @@
     history: list[int]
     reset: int
 
 
 class RateLimitMiddleware(AbstractMiddleware):
     """Rate-limiting middleware."""
 
-    __slots__ = ("app", "check_throttle_handler", "max_requests", "unit", "request_quota", "config")
-
     def __init__(self, app: ASGIApp, config: RateLimitConfig) -> None:
         """Initialize ``RateLimitMiddleware``.
 
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of RateLimitConfig.
         """
```

### Comparing `litestar-2.7.1/litestar/middleware/response_cache.py` & `litestar-2.8.0/litestar/middleware/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/compression/brotli_facade.py` & `litestar-2.8.0/litestar/middleware/compression/brotli_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/compression/facade.py` & `litestar-2.8.0/litestar/middleware/compression/facade.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     from litestar.config.compression import CompressionConfig
     from litestar.enums import CompressionEncoding
 
 
 class CompressionFacade(Protocol):
     """A unified facade offering a uniform interface for different compression libraries."""
 
+    __slots__ = ()
+
     encoding: ClassVar[str]
     """The encoding of the compression."""
 
     def __init__(
         self, buffer: BytesIO, compression_encoding: CompressionEncoding | str, config: CompressionConfig
     ) -> None:
         """Initialize ``CompressionFacade``.
```

### Comparing `litestar-2.7.1/litestar/middleware/compression/gzip_facade.py` & `litestar-2.8.0/litestar/middleware/compression/gzip_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/compression/middleware.py` & `litestar-2.8.0/litestar/middleware/compression/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.8.0/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/exceptions/middleware.py` & `litestar-2.8.0/litestar/middleware/exceptions/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import TYPE_CHECKING, Any, Type, cast
 
 from litestar.datastructures import Headers
 from litestar.enums import MediaType, ScopeType
 from litestar.exceptions import HTTPException, LitestarException, WebSocketException
 from litestar.middleware.cors import CORSMiddleware
 from litestar.middleware.exceptions._debug_response import _get_type_encoders_for_request, create_debug_response
-from litestar.serialization import encode_json
+from litestar.serialization import encode_json, get_serializer
 from litestar.status_codes import HTTP_500_INTERNAL_SERVER_ERROR
 from litestar.utils.deprecation import warn_deprecation
 
 __all__ = ("ExceptionHandlerMiddleware", "ExceptionResponseContent", "create_exception_response")
 
 
 if TYPE_CHECKING:
@@ -93,24 +93,25 @@
 
         Returns:
             A response instance.
         """
         from litestar.response import Response
 
         content: Any = {k: v for k, v in asdict(self).items() if k not in ("headers", "media_type") and v is not None}
+        type_encoders = _get_type_encoders_for_request(request) if request is not None else None
 
         if self.media_type != MediaType.JSON:
-            content = encode_json(content)
+            content = encode_json(content, get_serializer(type_encoders))
 
         return Response(
             content=content,
             headers=self.headers,
             status_code=self.status_code,
             media_type=self.media_type,
-            type_encoders=_get_type_encoders_for_request(request) if request is not None else None,
+            type_encoders=type_encoders,
         )
 
 
 def _starlette_exception_handler(request: Request[Any, Any, Any], exc: StarletteHTTPException) -> Response:
     return create_exception_response(
         request=request,
         exc=HTTPException(
```

### Comparing `litestar-2.7.1/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.8.0/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.8.0/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/session/base.py` & `litestar-2.8.0/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/session/client_side.py` & `litestar-2.8.0/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/middleware/session/server_side.py` & `litestar-2.8.0/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/controller.py` & `litestar-2.8.0/litestar/openapi/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from __future__ import annotations
 
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Callable, Final, Literal
+from typing import TYPE_CHECKING, Any, Callable, Literal
 
-from yaml import dump as dump_yaml
-
-from litestar.constants import OPENAPI_NOT_INITIALIZED
+from litestar.constants import OPENAPI_JSON_HANDLER_NAME, OPENAPI_NOT_INITIALIZED
 from litestar.controller import Controller
 from litestar.enums import MediaType, OpenAPIMediaType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers import get
+from litestar.openapi.config import _DEFAULT_SCHEMA_SITE
 from litestar.response.base import ASGIResponse
 from litestar.serialization import encode_json
 from litestar.serialization.msgspec_hooks import decode_json
 from litestar.status_codes import HTTP_404_NOT_FOUND
 
 __all__ = ("OpenAPIController",)
 
 
 if TYPE_CHECKING:
     from litestar.connection.request import Request
     from litestar.openapi.spec.open_api import OpenAPI
 
-_OPENAPI_JSON_ROUTER_NAME: Final = "__litestar_openapi_json"
-
 
 class OpenAPIController(Controller):
     """Controller for OpenAPI endpoints."""
 
     path: str = "/schema"
     """Base path for the OpenAPI documentation endpoints."""
     style: str = "body { margin: 0; padding: 0 }"
@@ -114,19 +111,21 @@
 
         asgi_root_path = set(filter(None, request.scope.get("root_path", "").split("/")))
         full_request_path = set(filter(None, request.url.path.split("/")))
         request_path = full_request_path.difference(asgi_root_path)
         root_path = set(filter(None, self.path.split("/")))
 
         config = request.app.openapi_config
+        enabled_endpoints = config.enabled_endpoints or set()
+        root_schema_site = config.root_schema_site or _DEFAULT_SCHEMA_SITE
 
-        if request_path == root_path and config.root_schema_site in config.enabled_endpoints:
+        if request_path == root_path and root_schema_site in enabled_endpoints:
             return True
 
-        return bool(request_path & config.enabled_endpoints)
+        return bool(request_path & enabled_endpoints)
 
     @property
     def favicon(self) -> str:
         """Return favicon ``<link>`` tag, if applicable.
 
         Returns:
             A ``<link>`` tag if ``self.favicon_url`` is not empty, otherwise returns a placeholder meta tag.
@@ -161,28 +160,30 @@
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A Response instance with the YAML object rendered into a string.
         """
+        from yaml import dump as dump_yaml
+
         if self.should_serve_endpoint(request):
             if not self._dumped_json_schema:
                 schema_json = decode_json(self._get_schema_as_json(request))
                 schema_yaml = dump_yaml(schema_json, default_flow_style=False)
                 self._dumped_yaml_schema = schema_yaml.encode("utf-8")
             return ASGIResponse(body=self._dumped_yaml_schema, media_type=OpenAPIMediaType.OPENAPI_YAML)
         return ASGIResponse(body=b"", status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(
         path="/openapi.json",
         media_type=OpenAPIMediaType.OPENAPI_JSON,
         include_in_schema=False,
         sync_to_thread=False,
-        name=_OPENAPI_JSON_ROUTER_NAME,
+        name=OPENAPI_JSON_HANDLER_NAME,
     )
     def retrieve_schema_json(self, request: Request[Any, Any, Any]) -> ASGIResponse:
         """Return the OpenAPI schema as JSON with an ``application/vnd.oai.openapi+json`` Content-Type header.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
@@ -214,15 +215,15 @@
         Raises:
             ImproperlyConfiguredException: If the application ``openapi_config`` attribute is ``None``.
         """
         config = request.app.openapi_config
         if not config:  # pragma: no cover
             raise ImproperlyConfiguredException(OPENAPI_NOT_INITIALIZED)
 
-        render_method = self.render_methods_map[config.root_schema_site]
+        render_method = self.render_methods_map[config.root_schema_site or _DEFAULT_SCHEMA_SITE]
 
         if self.should_serve_endpoint(request):
             return ASGIResponse(body=render_method(request), media_type=MediaType.HTML)
         return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/swagger", include_in_schema=False, sync_to_thread=False)
     def swagger_ui(self, request: Request[Any, Any, Any]) -> ASGIResponse:
@@ -464,15 +465,15 @@
             <style>{self.style}</style>
           </head>
         """
 
         body = f"""
           <body>
             <elements-api
-                apiDescriptionUrl="{request.app.route_reverse(_OPENAPI_JSON_ROUTER_NAME)}"
+                apiDescriptionUrl="{request.app.route_reverse(OPENAPI_JSON_HANDLER_NAME)}"
                 router="hash"
                 layout="sidebar"
             />
           </body>
         """
 
         return f"""
@@ -495,15 +496,15 @@
             <script src="{self.rapidoc_js_url}" crossorigin></script>
             <style>{self.style}</style>
           </head>
         """
 
         body = f"""
           <body>
-            <rapi-doc spec-url="{request.app.route_reverse(_OPENAPI_JSON_ROUTER_NAME)}" />
+            <rapi-doc spec-url="{request.app.route_reverse(OPENAPI_JSON_HANDLER_NAME)}" />
           </body>
         """
 
         return f"""
         <!DOCTYPE html>
             <html>
                 {head}
```

### Comparing `litestar-2.7.1/litestar/openapi/datastructures.py` & `litestar-2.8.0/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/__init__.py` & `litestar-2.8.0/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/base.py` & `litestar-2.8.0/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/callback.py` & `litestar-2.8.0/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/components.py` & `litestar-2.8.0/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/contact.py` & `litestar-2.8.0/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/discriminator.py` & `litestar-2.8.0/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/encoding.py` & `litestar-2.8.0/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/enums.py` & `litestar-2.8.0/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/example.py` & `litestar-2.8.0/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/external_documentation.py` & `litestar-2.8.0/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/header.py` & `litestar-2.8.0/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/info.py` & `litestar-2.8.0/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/license.py` & `litestar-2.8.0/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/link.py` & `litestar-2.8.0/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/media_type.py` & `litestar-2.8.0/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/oauth_flow.py` & `litestar-2.8.0/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/oauth_flows.py` & `litestar-2.8.0/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/open_api.py` & `litestar-2.8.0/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/operation.py` & `litestar-2.8.0/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/parameter.py` & `litestar-2.8.0/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/path_item.py` & `litestar-2.8.0/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/paths.py` & `litestar-2.8.0/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/reference.py` & `litestar-2.8.0/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/request_body.py` & `litestar-2.8.0/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/response.py` & `litestar-2.8.0/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/responses.py` & `litestar-2.8.0/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/schema.py` & `litestar-2.8.0/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/security_requirement.py` & `litestar-2.8.0/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/security_scheme.py` & `litestar-2.8.0/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/server.py` & `litestar-2.8.0/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/server_variable.py` & `litestar-2.8.0/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/tag.py` & `litestar-2.8.0/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/openapi/spec/xml.py` & `litestar-2.8.0/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/plugins/base.py` & `litestar-2.8.0/litestar/plugins/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,16 @@
         """
         raise NotImplementedError()
 
 
 class OpenAPISchemaPlugin(OpenAPISchemaPluginProtocol):
     """Plugin to extend the support of OpenAPI schema generation for non-library types."""
 
+    __slots__ = ()
+
     @staticmethod
     def is_plugin_supported_type(value: Any) -> bool:
         """Given a value of indeterminate type, determine if this value is supported by the plugin.
 
         This is called by the default implementation of :meth:`is_plugin_supported_field` for
         backwards compatibility. User's should prefer to override that method instead.
```

### Comparing `litestar-2.7.1/litestar/plugins/core.py` & `litestar-2.8.0/litestar/plugins/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/plugins/sqlalchemy.py` & `litestar-2.8.0/litestar/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/plugins/structlog.py` & `litestar-2.8.0/litestar/plugins/structlog.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/repository/_filters.py` & `litestar-2.8.0/litestar/repository/_filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/repository/filters.py` & `litestar-2.8.0/litestar/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/repository/handlers.py` & `litestar-2.8.0/litestar/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/repository/abc/_async.py` & `litestar-2.8.0/litestar/repository/abc/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/repository/abc/_sync.py` & `litestar-2.8.0/litestar/repository/abc/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/repository/testing/generic_mock_repository.py` & `litestar-2.8.0/litestar/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/response/base.py` & `litestar-2.8.0/litestar/response/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/response/file.py` & `litestar-2.8.0/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/response/redirect.py` & `litestar-2.8.0/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/response/sse.py` & `litestar-2.8.0/litestar/response/sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/response/streaming.py` & `litestar-2.8.0/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/response/template.py` & `litestar-2.8.0/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/routes/asgi.py` & `litestar-2.8.0/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/routes/base.py` & `litestar-2.8.0/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/routes/http.py` & `litestar-2.8.0/litestar/routes/http.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/routes/websocket.py` & `litestar-2.8.0/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/security/base.py` & `litestar-2.8.0/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/security/jwt/__init__.py` & `litestar-2.8.0/litestar/security/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/security/jwt/auth.py` & `litestar-2.8.0/litestar/security/jwt/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/security/jwt/middleware.py` & `litestar-2.8.0/litestar/security/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/security/jwt/token.py` & `litestar-2.8.0/litestar/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/security/session_auth/auth.py` & `litestar-2.8.0/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/security/session_auth/middleware.py` & `litestar-2.8.0/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/serialization/msgspec_hooks.py` & `litestar-2.8.0/litestar/serialization/msgspec_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/static_files/base.py` & `litestar-2.8.0/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/static_files/config.py` & `litestar-2.8.0/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/stores/base.py` & `litestar-2.8.0/litestar/stores/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 __all__ = ("Store", "NamespacedStore", "StorageObject")
 
 
 class Store(ABC):
     """Thread and process safe asynchronous key/value store."""
 
+    __slots__ = ()
+
     @abstractmethod
     async def set(self, key: str, value: str | bytes, expires_in: int | timedelta | None = None) -> None:
         """Set a value.
 
         Args:
             key: Key to associate the value with
             value: Value to store
@@ -93,14 +95,16 @@
 class NamespacedStore(Store):
     """A subclass of :class:`Store`, offering hierarchical namespacing.
 
     Bulk actions on a parent namespace should affect all child namespaces, whereas other operations on all namespaces
     should be isolated.
     """
 
+    __slots__ = ("namespace",)
+
     @abstractmethod
     def with_namespace(self, namespace: str) -> Self:
         """Return a new instance of :class:`NamespacedStore`, which exists in a child namespace of the current namespace.
         Bulk actions on the parent namespace should affect all child namespaces, whereas other operations on all
         namespaces should be isolated.
         """
```

### Comparing `litestar-2.7.1/litestar/stores/file.py` & `litestar-2.8.0/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/stores/memory.py` & `litestar-2.8.0/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/stores/redis.py` & `litestar-2.8.0/litestar/stores/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 if TYPE_CHECKING:
     from types import TracebackType
 
 
 class RedisStore(NamespacedStore):
     """Redis based, thread and process safe asynchronous key/value store."""
 
-    __slots__ = ("_redis",)
+    __slots__ = (
+        "_delete_all_script",
+        "_get_and_renew_script",
+        "_redis",
+        "handle_client_shutdown",
+    )
 
     def __init__(
         self, redis: Redis, namespace: str | None | EmptyType = Empty, handle_client_shutdown: bool = False
     ) -> None:
         """Initialize :class:`RedisStore`
 
         Args:
```

### Comparing `litestar-2.7.1/litestar/stores/registry.py` & `litestar-2.8.0/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/template/base.py` & `litestar-2.8.0/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/template/config.py` & `litestar-2.8.0/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/__init__.py` & `litestar-2.8.0/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/helpers.py` & `litestar-2.8.0/litestar/testing/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     multipart_form_part_limit: int = 1000,
     on_app_init: Sequence[OnAppInitHandler] | None = None,
     on_shutdown: Sequence[LifespanHook] | None = None,
     on_startup: Sequence[LifespanHook] | None = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
+    path: str | None = None,
     plugins: Sequence[PluginProtocol] | None = None,
     lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
     raise_server_exceptions: bool = True,
     pdb_on_exception: bool | None = None,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: type[Response] | None = None,
@@ -197,14 +198,18 @@
             application startup.
         openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
         opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
             wherever you have access to :class:`Request <litestar.connection.request.Request>` or
             :class:`ASGI Scope <.types.Scope>`.
         parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
             paths.
+        path: A path fragment that is prefixed to all route handlers, controllers and routers associated
+            with the application instance.
+
+            .. versionadded:: 2.8.0
         pdb_on_exception: Drop into the PDB when an exception occurs.
         plugins: Sequence of plugins.
         request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
         response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
             response.
         response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
         response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
@@ -269,14 +274,15 @@
         multipart_form_part_limit=multipart_form_part_limit,
         on_app_init=on_app_init,
         on_shutdown=on_shutdown,
         on_startup=on_startup,
         openapi_config=openapi_config,
         opt=opt,
         parameters=parameters,
+        path=path,
         pdb_on_exception=pdb_on_exception,
         plugins=plugins,
         request_class=request_class,
         response_cache_config=response_cache_config,
         response_class=response_class,
         response_cookies=response_cookies,
         response_headers=response_headers,
@@ -339,14 +345,15 @@
     on_app_init: Sequence[OnAppInitHandler] | None = None,
     on_shutdown: Sequence[LifespanHook] | None = None,
     on_startup: Sequence[LifespanHook] | None = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
     pdb_on_exception: bool | None = None,
+    path: str | None = None,
     plugins: Sequence[PluginProtocol] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: type[Response] | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: ResponseHeaders | None = None,
@@ -452,14 +459,18 @@
             application startup.
         openapi_config: Defaults to :attr:`DEFAULT_OPENAPI_CONFIG`
         opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
             wherever you have access to :class:`Request <litestar.connection.request.Request>` or
             :class:`ASGI Scope <.types.Scope>`.
         parameters: A mapping of :class:`Parameter <.params.Parameter>` definitions available to all application
             paths.
+        path: A path fragment that is prefixed to all route handlers, controllers and routers associated
+            with the application instance.
+
+            .. versionadded:: 2.8.0
         pdb_on_exception: Drop into the PDB when an exception occurs.
         plugins: Sequence of plugins.
         request_class: An optional subclass of :class:`Request <.connection.Request>` to use for http connections.
         response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the app's default
             response.
         response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>`.
         response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
@@ -523,14 +534,15 @@
         multipart_form_part_limit=multipart_form_part_limit,
         on_app_init=on_app_init,
         on_shutdown=on_shutdown,
         on_startup=on_startup,
         openapi_config=openapi_config,
         opt=opt,
         parameters=parameters,
+        path=path,
         pdb_on_exception=pdb_on_exception,
         plugins=plugins,
         request_class=request_class,
         response_cache_config=response_cache_config,
         response_class=response_class,
         response_cookies=response_cookies,
         response_headers=response_headers,
```

### Comparing `litestar-2.7.1/litestar/testing/life_span_handler.py` & `litestar-2.8.0/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/request_factory.py` & `litestar-2.8.0/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/transport.py` & `litestar-2.8.0/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/websocket_test_session.py` & `litestar-2.8.0/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/client/__init__.py` & `litestar-2.8.0/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/client/async_client.py` & `litestar-2.8.0/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/client/base.py` & `litestar-2.8.0/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/testing/client/sync_client.py` & `litestar-2.8.0/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/__init__.py` & `litestar-2.8.0/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/asgi_types.py` & `litestar-2.8.0/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/builtin_types.py` & `litestar-2.8.0/litestar/types/builtin_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/callable_types.py` & `litestar-2.8.0/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/composite_types.py` & `litestar-2.8.0/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/file_types.py` & `litestar-2.8.0/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/helper_types.py` & `litestar-2.8.0/litestar/types/helper_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/internal_types.py` & `litestar-2.8.0/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/protocols.py` & `litestar-2.8.0/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/types/serialization.py` & `litestar-2.8.0/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/__init__.py` & `litestar-2.8.0/litestar/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from .helpers import get_enum_string_value, get_name, unique_name_for_scope, url_quote
 from .path import join_paths, normalize_path
 from .predicates import (
     _is_sync_or_async_generator,
     is_annotated_type,
     is_any,
     is_async_callable,
-    is_attrs_class,
     is_class_and_subclass,
     is_class_var,
     is_dataclass_class,
     is_dataclass_instance,
     is_generic,
     is_mapping,
     is_non_string_iterable,
@@ -40,15 +39,14 @@
     "get_enum_string_value",
     "get_name",
     "get_origin_or_inner_type",
     "get_serializer_from_scope",
     "is_annotated_type",
     "is_any",
     "is_async_callable",
-    "is_attrs_class",
     "is_class_and_subclass",
     "is_class_var",
     "is_dataclass_class",
     "is_dataclass_instance",
     "is_generic",
     "is_mapping",
     "is_non_string_iterable",
```

### Comparing `litestar-2.7.1/litestar/utils/compat.py` & `litestar-2.8.0/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/dataclass.py` & `litestar-2.8.0/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/deprecation.py` & `litestar-2.8.0/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/empty.py` & `litestar-2.8.0/litestar/utils/empty.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/helpers.py` & `litestar-2.8.0/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/module_loader.py` & `litestar-2.8.0/litestar/utils/module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/path.py` & `litestar-2.8.0/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/predicates.py` & `litestar-2.8.0/litestar/utils/predicates.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,34 +30,28 @@
     ParamSpec,
     TypeGuard,
     _AnnotatedAlias,
     get_args,
 )
 
 from litestar.constants import UNDEFINED_SENTINELS
-from litestar.types import Empty
 from litestar.types.builtin_types import NoneType, UnionTypes
 from litestar.utils.deprecation import warn_deprecation
 from litestar.utils.helpers import unwrap_partial
 from litestar.utils.typing import get_origin_or_inner_type
 
 if TYPE_CHECKING:
     from litestar.types.callable_types import AnyGenerator
     from litestar.types.protocols import DataclassProtocol
 
-try:
-    import attrs
-except ImportError:
-    attrs = Empty  # type: ignore[assignment]
 
 __all__ = (
     "is_annotated_type",
     "is_any",
     "is_async_callable",
-    "is_attrs_class",
     "is_class_and_subclass",
     "is_class_var",
     "is_dataclass_class",
     "is_dataclass_instance",
     "is_generic",
     "is_mapping",
     "is_non_string_iterable",
@@ -258,26 +252,14 @@
     """
     origin = get_origin_or_inner_type(annotation)
     return origin is Optional or (
         get_origin_or_inner_type(annotation) in UnionTypes and NoneType in get_args(annotation)
     )
 
 
-def is_attrs_class(annotation: Any) -> TypeGuard[type[attrs.AttrsInstance]]:  # pyright: ignore
-    """Given a type annotation determine if the annotation is a class that includes an attrs attribute.
-
-    Args:
-        annotation: A type.
-
-    Returns:
-        A typeguard determining whether the type is an attrs class.
-    """
-    return attrs.has(annotation) if attrs is not Empty else False  # type: ignore[comparison-overlap]
-
-
 def is_class_var(annotation: Any) -> bool:
     """Check if the given annotation is a ClassVar.
 
     Args:
         annotation: A type annotation
 
     Returns:
```

### Comparing `litestar-2.7.1/litestar/utils/sequence.py` & `litestar-2.8.0/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/signature.py` & `litestar-2.8.0/litestar/utils/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from typing_extensions import Annotated, Self, get_args, get_origin, get_type_hints
 
 from litestar import connection, datastructures, types
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Empty
 from litestar.typing import FieldDefinition
-from litestar.utils.typing import unwrap_annotation
+from litestar.utils.typing import expand_type_var_in_type_hint, unwrap_annotation
 
 if TYPE_CHECKING:
     from typing import Sequence
 
     from litestar.types import AnyCallable
 
 if sys.version_info < (3, 11):
@@ -208,16 +208,17 @@
             signature_namespace: mapping of names to types for forward reference resolution
 
         Returns:
             ParsedSignature
         """
         signature = Signature.from_callable(fn)
         fn_type_hints = get_fn_type_hints(fn, namespace=signature_namespace)
+        expanded_type_hints = expand_type_var_in_type_hint(fn_type_hints, signature_namespace)
 
-        return cls.from_signature(signature, fn_type_hints)
+        return cls.from_signature(signature, expanded_type_hints)
 
     @classmethod
     def from_signature(cls, signature: Signature, fn_type_hints: dict[str, type]) -> Self:
         """Parse an :class:`inspect.Signature` instance.
 
         Args:
             signature: An :class:`inspect.Signature` instance.
```

### Comparing `litestar-2.7.1/litestar/utils/sync.py` & `litestar-2.8.0/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/typing.py` & `litestar-2.8.0/litestar/utils/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,14 +258,29 @@
             type_hints = get_type_hints(origin, globalns=globalns, localns=localns, include_extras=include_extras)
         # the __parameters__ is only available on the origin itself and not the annotation
         typevar_map = dict(zip(origin.__parameters__, get_args(annotation)))
 
     return {n: _substitute_typevars(type_, typevar_map) for n, type_ in type_hints.items()}
 
 
+def expand_type_var_in_type_hint(type_hint: dict[str, Any], namespace: dict[str, Any] | None) -> dict[str, Any]:
+    """Expand TypeVar for any parameters in type_hint
+
+    Args:
+        type_hint: mapping of parameter to type obtained from calling `get_type_hints` or `get_fn_type_hints`
+        namespace: mapping of TypeVar to concrete type
+
+    Returns:
+        type_hint with any TypeVar parameter expanded
+    """
+    if namespace:
+        return {name: _substitute_typevars(hint, namespace) for name, hint in type_hint.items()}
+    return type_hint
+
+
 def _substitute_typevars(obj: Any, typevar_map: Mapping[Any, Any]) -> Any:
     if params := getattr(obj, "__parameters__", None):
         args = tuple(_substitute_typevars(typevar_map.get(p, p), typevar_map) for p in params)
         return obj[args]
 
     if isinstance(obj, TypeVar):
         # If there's a mapped type for the TypeVar already, then it should be returned instead
```

### Comparing `litestar-2.7.1/litestar/utils/version.py` & `litestar-2.8.0/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/warnings.py` & `litestar-2.8.0/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/scope/__init__.py` & `litestar-2.8.0/litestar/utils/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/litestar/utils/scope/state.py` & `litestar-2.8.0/litestar/utils/scope/state.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         "base_url",
         "body",
         "content_type",
         "cookies",
         "csrf_token",
         "dependency_cache",
         "do_cache",
+        "flash_messages",
         "form",
         "headers",
         "is_cached",
         "json",
         "log_context",
         "msgpack",
         "parsed_query",
@@ -52,14 +53,15 @@
         self.body = Empty
         self.content_type = Empty
         self.cookies = Empty
         self.csrf_token = Empty
         self.dependency_cache = Empty
         self.do_cache = Empty
         self.form = Empty
+        self.flash_messages = []
         self.headers = Empty
         self.is_cached = Empty
         self.json = Empty
         self.log_context: dict[str, Any] = {}
         self.msgpack = Empty
         self.parsed_query = Empty
         self.response_compressed = Empty
@@ -72,14 +74,15 @@
     body: bytes | EmptyType
     content_type: tuple[str, dict[str, str]] | EmptyType
     cookies: dict[str, str] | EmptyType
     csrf_token: str | EmptyType
     dependency_cache: dict[str, Any] | EmptyType
     do_cache: bool | EmptyType
     form: dict[str, str | list[str]] | EmptyType
+    flash_messages: list[dict[str, str]]
     headers: Headers | EmptyType
     is_cached: bool | EmptyType
     json: Any | EmptyType
     log_context: dict[str, Any]
     msgpack: Any | EmptyType
     parsed_query: tuple[tuple[str, str], ...] | EmptyType
     response_compressed: bool | EmptyType
```

### Comparing `litestar-2.7.1/tests/conftest.py` & `litestar-2.8.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 from datetime import datetime
 from os import urandom
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Generator, TypeVar, Union, cast
 from unittest.mock import AsyncMock, MagicMock
 
 import pytest
-from pytest_lazyfixture import lazy_fixture
+from pytest_lazy_fixtures import lf
 from redis.asyncio import Redis as AsyncRedis
 from redis.client import Redis
 from time_machine import travel
 
 from litestar.logging import LoggingConfig
 from litestar.logging.config import default_handlers as logging_default_handlers
 from litestar.middleware.session import SessionMiddleware
 from litestar.middleware.session.base import BaseSessionBackend
 from litestar.middleware.session.client_side import ClientSideSessionBackend, CookieBackendConfig
 from litestar.middleware.session.server_side import ServerSideSessionBackend, ServerSideSessionConfig
+from litestar.openapi.config import OpenAPIConfig
 from litestar.stores.base import Store
 from litestar.stores.file import FileStore
 from litestar.stores.memory import MemoryStore
 from litestar.stores.redis import RedisStore
 from litestar.testing import RequestFactory
 
 if TYPE_CHECKING:
@@ -105,16 +106,16 @@
 @pytest.fixture()
 def cookie_session_backend(cookie_session_backend_config: CookieBackendConfig) -> ClientSideSessionBackend:
     return ClientSideSessionBackend(config=cookie_session_backend_config)
 
 
 @pytest.fixture(
     params=[
-        pytest.param(lazy_fixture("cookie_session_backend_config"), id="cookie"),
-        pytest.param(lazy_fixture("server_side_session_config"), id="server-side"),
+        pytest.param(lf("cookie_session_backend_config"), id="cookie"),
+        pytest.param(lf("server_side_session_config"), id="server-side"),
     ]
 )
 def session_backend_config(request: pytest.FixtureRequest) -> ServerSideSessionConfig | CookieBackendConfig:
     return cast("Union[ServerSideSessionConfig, CookieBackendConfig]", request.param)
 
 
 @pytest.fixture()
@@ -311,7 +312,12 @@
     Redis(host=docker_ip, port=6397).flushall()
     client: AsyncRedis = AsyncRedis(host=docker_ip, port=6397)
     yield client
     try:
         await client.aclose()  # type: ignore[attr-defined]
     except RuntimeError:
         pass
+
+
+@pytest.fixture(autouse=True)
+def _patch_openapi_config(monkeypatch: pytest.MonkeyPatch) -> None:
+    monkeypatch.setattr("litestar.app.DEFAULT_OPENAPI_CONFIG", OpenAPIConfig(title="Litestar API", version="1.0.0"))
```

### Comparing `litestar-2.7.1/tests/docker_service_fixtures.py` & `litestar-2.8.0/tests/docker_service_fixtures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/helpers.py` & `litestar-2.8.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/models.py` & `litestar-2.8.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_advanced_alchemy.py` & `litestar-2.8.0/tests/e2e/test_advanced_alchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_exception_handlers.py` & `litestar-2.8.0/tests/e2e/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_option_requests.py` & `litestar-2.8.0/tests/e2e/test_option_requests.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_pydantic.py` & `litestar-2.8.0/tests/e2e/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_response_caching.py` & `litestar-2.8.0/tests/e2e/test_response_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_router_registration.py` & `litestar-2.8.0/tests/e2e/test_router_registration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_starlette_responses.py` & `litestar-2.8.0/tests/e2e/test_starlette_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_dependency_injection/test_dependency_validation.py` & `litestar-2.8.0/tests/e2e/test_dependency_injection/test_dependency_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py` & `litestar-2.8.0/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_dependency_injection/test_injection_of_classes.py` & `litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_classes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py` & `litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_dependency_injection/test_inter_dependencies.py` & `litestar-2.8.0/tests/e2e/test_dependency_injection/test_inter_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_dependency_injection/test_request_local_caching.py` & `litestar-2.8.0/tests/e2e/test_dependency_injection/test_request_local_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py` & `litestar-2.8.0/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_life_cycle_hooks/test_after_request.py` & `litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_life_cycle_hooks/test_after_response.py` & `litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_life_cycle_hooks/test_before_request.py` & `litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_before_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_routing/conftest.py` & `litestar-2.8.0/tests/e2e/test_routing/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_routing/test_asset_url_path.py` & `litestar-2.8.0/tests/e2e/test_routing/test_asset_url_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_routing/test_path_mounting.py` & `litestar-2.8.0/tests/e2e/test_routing/test_path_mounting.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_routing/test_path_resolution.py` & `litestar-2.8.0/tests/e2e/test_routing/test_path_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_routing/test_route_indexing.py` & `litestar-2.8.0/tests/e2e/test_routing/test_route_indexing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_routing/test_route_reverse.py` & `litestar-2.8.0/tests/e2e/test_routing/test_route_reverse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/e2e/test_routing/test_validations.py` & `litestar-2.8.0/tests/e2e/test_routing/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_cache_control_headers.py` & `litestar-2.8.0/tests/examples/test_cache_control_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_exceptions.py` & `litestar-2.8.0/tests/examples/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_lifecycle_hooks.py` & `litestar-2.8.0/tests/examples/test_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_openapi.py` & `litestar-2.8.0/tests/examples/test_openapi/test_openapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,15 @@
                         "type": "object",
                         "required": ["id"],
                         "title": "IdContainer",
                     }
                 }
             },
         }
+
+
+def test_customize_path() -> None:
+    from docs.examples.openapi.customize_path import app
+
+    with TestClient(app=app) as client:
+        resp = client.get("/docs/openapi.json")
+        assert resp.status_code == 200
```

### Comparing `litestar-2.7.1/tests/examples/test_request_data.py` & `litestar-2.8.0/tests/examples/test_request_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_routing.py` & `litestar-2.8.0/tests/examples/test_routing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_startup_and_shutdown.py` & `litestar-2.8.0/tests/examples/test_startup_and_shutdown.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_static_files.py` & `litestar-2.8.0/tests/examples/test_static_files.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_stores.py` & `litestar-2.8.0/tests/examples/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_todo_app.py` & `litestar-2.8.0/tests/examples/test_todo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_using_session_auth.py` & `litestar-2.8.0/tests/examples/test_using_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_application_hooks/test_application_after_exception_hook.py` & `litestar-2.8.0/tests/examples/test_application_hooks/test_application_after_exception_hook.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_application_hooks/test_lifespan_manager.py` & `litestar-2.8.0/tests/examples/test_application_hooks/test_lifespan_manager.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_application_state/test_using_application_state.py` & `litestar-2.8.0/tests/examples/test_application_state/test_using_application_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_contrib/test_piccolo_orm.py` & `litestar-2.8.0/tests/examples/test_contrib/test_piccolo_orm.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py` & `litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py` & `litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py` & `litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py` & `litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_dto/test_example_apps.py` & `litestar-2.8.0/tests/examples/test_dto/test_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_dto/test_tutorial.py` & `litestar-2.8.0/tests/examples/test_dto/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_middleware/test_abstract_middleware.py` & `litestar-2.8.0/tests/examples/test_middleware/test_abstract_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_middleware/test_logging_middleware.py` & `litestar-2.8.0/tests/examples/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_middleware/test_session_middleware.py` & `litestar-2.8.0/tests/examples/test_middleware/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_pagination/test_using_classic_pagination.py` & `litestar-2.8.0/tests/examples/test_pagination/test_using_classic_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_pagination/test_using_cursor_pagination.py` & `litestar-2.8.0/tests/examples/test_pagination/test_using_cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_pagination/test_using_offset_pagination.py` & `litestar-2.8.0/tests/examples/test_pagination/test_using_offset_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_parameters/test_header_and_cookies_parameters.py` & `litestar-2.8.0/tests/examples/test_parameters/test_header_and_cookies_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_parameters/test_layered_parameters.py` & `litestar-2.8.0/tests/examples/test_parameters/test_layered_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_parameters/test_path_parameters.py` & `litestar-2.8.0/tests/examples/test_parameters/test_path_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_parameters/test_query_parameters.py` & `litestar-2.8.0/tests/examples/test_parameters/test_query_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py` & `litestar-2.8.0/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_responses/test_background_tasks.py` & `litestar-2.8.0/tests/examples/test_responses/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_responses/test_response_cookies.py` & `litestar-2.8.0/tests/examples/test_responses/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_responses/test_response_headers.py` & `litestar-2.8.0/tests/examples/test_responses/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_responses/test_sse_responses.py` & `litestar-2.8.0/tests/examples/test_responses/test_sse_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_security/test_jwt/test_using_jwt_auth.py` & `litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py` & `litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py` & `litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_templating/test_engine_instance.py` & `litestar-2.8.0/tests/examples/test_templating/test_engine_instance.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_templating/test_returning_templates.py` & `litestar-2.8.0/tests/examples/test_templating/test_returning_templates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/examples/test_templating/test_template_functions.py` & `litestar-2.8.0/tests/examples/test_templating/test_template_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/conftest.py` & `litestar-2.8.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_app.py` & `litestar-2.8.0/tests/unit/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from unittest.mock import MagicMock, Mock, PropertyMock
 
 import pytest
 from click import Group
 from pytest import MonkeyPatch
 
 from litestar import Litestar, MediaType, Request, Response, get
-from litestar.config.app import AppConfig
+from litestar.config.app import AppConfig, ExperimentalFeatures
 from litestar.config.response_cache import ResponseCacheConfig
 from litestar.contrib.sqlalchemy.plugins import SQLAlchemySerializationPlugin
 from litestar.datastructures import MutableScopeHeaders, State
 from litestar.events.emitter import SimpleEventEmitter
 from litestar.exceptions import (
     ImproperlyConfiguredException,
     InternalServerException,
@@ -441,7 +441,21 @@
         assert counter["value"] == 0
 
     assert counter["value"] == 4
     assert events[0] == "ctx_2"
     assert events[1] == "ctx_1"
     assert events[2] == "hook_a"
     assert events[3] == "hook_b"
+
+
+def test_use_dto_codegen_feature_flag_warns() -> None:
+    with pytest.warns(LitestarWarning, match="Use of redundant experimental feature flag DTO_CODEGEN"):
+        Litestar(experimental_features=[ExperimentalFeatures.DTO_CODEGEN])
+
+
+def test_using_custom_path_parameter() -> None:
+    @get()
+    def my_route_handler() -> None: ...
+
+    with create_test_client(my_route_handler, path="/abc") as client:
+        response = client.get("/abc")
+        assert response.status_code == HTTP_200_OK
```

### Comparing `litestar-2.7.1/tests/unit/test_asgi_router.py` & `litestar-2.8.0/tests/unit/test_asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_background_tasks.py` & `litestar-2.8.0/tests/unit/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_concurrency.py` & `litestar-2.8.0/tests/unit/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_controller.py` & `litestar-2.8.0/tests/unit/test_controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_data_extractors.py` & `litestar-2.8.0/tests/unit/test_data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_di.py` & `litestar-2.8.0/tests/unit/test_di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_events.py` & `litestar-2.8.0/tests/unit/test_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 from unittest.mock import MagicMock
 
 import pytest
-from pytest_lazyfixture import lazy_fixture
+from pytest_lazy_fixtures import lf
 
 from litestar import Litestar, Request, get
 from litestar.events.emitter import SimpleEventEmitter
 from litestar.events.listener import EventListener, listener
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.status_codes import HTTP_200_OK
 from litestar.testing import create_test_client
@@ -32,15 +32,15 @@
     @listener("test_event")
     async def listener_fn(*args: Any, **kwargs: Any) -> None:
         mock(*args, **kwargs)
 
     return listener_fn
 
 
-@pytest.mark.parametrize("event_listener", [lazy_fixture("sync_listener"), lazy_fixture("async_listener")])
+@pytest.mark.parametrize("event_listener", [lf("sync_listener"), lf("async_listener")])
 def test_event_listener(mock: MagicMock, event_listener: EventListener, anyio_backend: AnyIOBackend) -> None:
     @get("/")
     def route_handler(request: Request[Any, Any, Any]) -> None:
         request.app.emit("test_event", "positional", keyword="keyword-value")
 
     with create_test_client(
         route_handlers=[route_handler], listeners=[event_listener], backend=anyio_backend
```

### Comparing `litestar-2.7.1/tests/unit/test_exceptions.py` & `litestar-2.8.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_file_system.py` & `litestar-2.8.0/tests/unit/test_file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_guards.py` & `litestar-2.8.0/tests/unit/test_guards.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_pagination.py` & `litestar-2.8.0/tests/unit/test_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_params.py` & `litestar-2.8.0/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_parsers.py` & `litestar-2.8.0/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_request_class_resolution.py` & `litestar-2.8.0/tests/unit/test_request_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response_class_resolution.py` & `litestar-2.8.0/tests/unit/test_response_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_stores.py` & `litestar-2.8.0/tests/unit/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_typing.py` & `litestar-2.8.0/tests/unit/test_typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from typing import Any, ForwardRef, Generic, List, Optional, Tuple, TypeVar, Union
 
 import annotated_types
 import msgspec
 import pytest
 from typing_extensions import Annotated, NotRequired, Required, TypedDict, get_type_hints
 
-from litestar.params import DependencyKwarg, KwargDefinition, ParameterKwarg
+from litestar.exceptions import LitestarWarning
+from litestar.params import DependencyKwarg, KwargDefinition, Parameter, ParameterKwarg
 from litestar.typing import FieldDefinition, _unpack_predicate
 
 from .test_utils.test_signature import T, _check_field_definition, field_definition_int, test_type_hints
 
 
 @pytest.mark.parametrize(
     ("annotation", "expected"),
@@ -446,7 +447,17 @@
         (annotated_types.IsAscii.__metadata__[0], {"pattern": "[[:ascii:]]"}),  # pyright: ignore
         (annotated_types.IsDigits.__metadata__[0], {"pattern": "[[:digit:]]"}),  # pyright: ignore
         (object(), {}),
     ],
 )
 def test_unpack_predicate(predicate: Any, expected_meta: dict[str, Any]) -> None:
     assert _unpack_predicate(predicate) == expected_meta
+
+
+def test_warn_ambiguous_default_values() -> None:
+    with pytest.warns(LitestarWarning, match="Ambiguous default values"):
+        FieldDefinition.from_annotation(Annotated[int, Parameter(default=1)], default=2)
+
+
+def test_warn_defaults_inside_parameter_definition() -> None:
+    with pytest.warns(DeprecationWarning, match="Deprecated default value specification"):
+        FieldDefinition.from_annotation(Annotated[int, Parameter(default=1)], default=1)
```

### Comparing `litestar-2.7.1/tests/unit/test_websocket_class_resolution.py` & `litestar-2.8.0/tests/unit/test_websocket_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_channels/conftest.py` & `litestar-2.8.0/tests/unit/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_channels/test_backends.py` & `litestar-2.8.0/tests/unit/test_channels/test_backends.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_channels/test_plugin.py` & `litestar-2.8.0/tests/unit/test_channels/test_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_channels/test_subscriber.py` & `litestar-2.8.0/tests/unit/test_channels/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_cli/__init__.py` & `litestar-2.8.0/tests/unit/test_cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,20 +74,17 @@
 
 def create_app() -> Litestar:
     return Litestar(route_handlers=[], plugins=[StartupPrintPlugin()])
 
 """
 APP_FILE_CONTENT_ROUTES_EXAMPLE = """
 from litestar import Litestar, get
-from litestar.openapi import OpenAPIConfig, OpenAPIController
+from litestar.openapi import OpenAPIConfig
 from typing import Dict
 
-class CustomOpenAPIController(OpenAPIController):
-    path = "/api-docs"
-
 
 @get("/")
 def hello_world() -> Dict[str, str]:
     return {"hello": "world"}
 
 
 @get("/foo")
@@ -101,12 +98,13 @@
 
 
 
 app = Litestar(
     openapi_config=OpenAPIConfig(
         title="test_app",
         version="0",
-        openapi_controller=CustomOpenAPIController),
+        path="/api-docs",
+    ),
     route_handlers=[hello_world, foo, long_api]
 )
 
 """
```

### Comparing `litestar-2.7.1/tests/unit/test_cli/conftest.py` & `litestar-2.8.0/tests/unit/test_cli/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_cli/test_cli.py` & `litestar-2.8.0/tests/unit/test_cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_cli/test_cli_plugin.py` & `litestar-2.8.0/tests/unit/test_cli/test_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_cli/test_core_commands.py` & `litestar-2.8.0/tests/unit/test_cli/test_core_commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import io
 import os
 import re
 import sys
 from pathlib import Path
-from typing import Callable, Generator, List, Optional, Tuple
+from typing import Callable, Generator, List, Literal, Optional, Tuple, Union
 from unittest.mock import MagicMock
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from click.testing import CliRunner
 from pytest_mock import MockerFixture
+from rich.console import Console
 
 from litestar import __version__ as litestar_version
-from litestar.cli._utils import remove_default_schema_routes, remove_routes_with_patterns
+from litestar.cli import _utils
+from litestar.cli.commands import core
 from litestar.cli.main import litestar_group as cli_command
 from litestar.exceptions import LitestarWarning
 
 from . import (
     APP_FACTORY_FILE_CONTENT_SERVER_LIFESPAN_PLUGIN,
     APP_FILE_CONTENT_ROUTES_EXAMPLE,
     CREATE_APP_FILE_CONTENT,
@@ -51,16 +54,19 @@
         (False, None, None, ["*.py"], None),
         (False, None, ["*.yml", "*.rst"], None, None),
         (None, None, None, None, 2),
         (True, None, None, None, 2),
         (False, None, None, None, 2),
     ],
 )
+@pytest.mark.parametrize("tty_enabled", [True, False])
+@pytest.mark.parametrize("quiet_console", [True, False])
 def test_run_command(
     mock_show_app_info: MagicMock,
+    mocker: MockerFixture,
     runner: CliRunner,
     monkeypatch: MonkeyPatch,
     reload: Optional[bool],
     port: Optional[int],
     host: Optional[str],
     fd: Optional[int],
     uds: Optional[str],
@@ -68,18 +74,25 @@
     app_dir: Optional[str],
     reload_dir: Optional[List[str]],
     reload_include: Optional[List[str]],
     reload_exclude: Optional[List[str]],
     custom_app_file: Optional[Path],
     create_app_file: CreateAppFileFixture,
     set_in_env: bool,
+    tty_enabled: bool,
+    quiet_console: bool,
     mock_subprocess_run: MagicMock,
     mock_uvicorn_run: MagicMock,
     tmp_project_dir: Path,
 ) -> None:
+    monkeypatch.delenv("LITESTAR_QUIET_CONSOLE", raising=False)
+    if quiet_console:
+        monkeypatch.setenv("LITESTAR_QUIET_CONSOLE", "true")
+    mocker.patch.object(core, "isatty", return_value=tty_enabled)
+    mocker.patch.object(_utils, "isatty", return_value=tty_enabled)
     args = []
     if custom_app_file:
         args.extend(["--app", f"{custom_app_file.stem}:app"])
     if app_dir is not None:
         args.extend(["--app-dir", str(Path(tmp_project_dir / app_dir))])
     args.extend(["run"])
 
@@ -111,26 +124,26 @@
         if set_in_env:
             monkeypatch.setenv("LITESTAR_UNIX_DOMAIN_SOCKET", uds)
         else:
             args.extend(["--uds", uds])
     else:
         uds = None
 
-    if fd:
+    if fd is not None:
         if set_in_env:
             monkeypatch.setenv("LITESTAR_FILE_DESCRIPTOR", str(fd))
         else:
             args.extend(["--fd", str(fd)])
     else:
         fd = None
 
     if web_concurrency is None:
         web_concurrency = 1
     elif set_in_env:
-        monkeypatch.setenv("WEB_CONCURRENCY", str(web_concurrency))
+        monkeypatch.setenv("LITESTAR_WEB_CONCURRENCY", str(web_concurrency))
     else:
         args.extend(["--web-concurrency", str(web_concurrency)])
 
     if reload_dir is not None:
         if set_in_env:
             monkeypatch.setenv("LITESTAR_RELOAD_DIRS", ",".join(reload_dir))
         else:
@@ -145,15 +158,14 @@
     if reload_exclude is not None:
         if set_in_env:
             monkeypatch.setenv("LITESTAR_RELOAD_EXCLUDES", ",".join(reload_exclude))
         else:
             args.extend([f"--reload-exclude={s}" for s in reload_exclude])
 
     path = create_app_file(custom_app_file or "app.py", directory=app_dir)
-
     result = runner.invoke(cli_command, args)
 
     assert result.exception is None
     assert result.exit_code == 0
 
     if reload or reload_dir or reload_include or reload_exclude or web_concurrency > 1:
         expected_args = [
@@ -189,17 +201,22 @@
             uds=uds,
             fd=fd,
             factory=False,
             ssl_certfile=None,
             ssl_keyfile=None,
         )
 
-    mock_show_app_info.assert_called_once()
+    if tty_enabled and not quiet_console:
+        mock_show_app_info.assert_called_once()
+    else:
+        mock_show_app_info.assert_not_called()
 
 
+@pytest.mark.parametrize("quiet_console", [True, False])
+@pytest.mark.parametrize("tty_enabled", [True, False])
 @pytest.mark.parametrize(
     "file_name,file_content,factory_name",
     [
         ("_create_app.py", CREATE_APP_FILE_CONTENT, "create_app"),
         ("_generic_app_factory.py", GENERIC_APP_FACTORY_FILE_CONTENT, "any_name"),
         ("_generic_app_factory_string_ann.py", GENERIC_APP_FACTORY_FILE_CONTENT_STRING_ANNOTATION, "any_name"),
     ],
@@ -208,38 +225,63 @@
 def test_run_command_with_autodiscover_app_factory(
     runner: CliRunner,
     mock_uvicorn_run: MagicMock,
     file_name: str,
     file_content: str,
     factory_name: str,
     patch_autodiscovery_paths: Callable[[List[str]], None],
+    tty_enabled: bool,
+    quiet_console: bool,
     create_app_file: CreateAppFileFixture,
+    mocker: MockerFixture,
+    monkeypatch: MonkeyPatch,
 ) -> None:
+    monkeypatch.delenv("LITESTAR_QUIET_CONSOLE", raising=False)
+    if quiet_console:
+        monkeypatch.setenv("LITESTAR_QUIET_CONSOLE", "true")
+    mocker.patch.object(core, "isatty", return_value=tty_enabled)
+    mocker.patch.object(_utils, "isatty", return_value=tty_enabled)
     patch_autodiscovery_paths([file_name])
     path = create_app_file(file_name, content=file_content)
     result = runner.invoke(cli_command, "run")
-
     assert result.exception is None
     assert result.exit_code == 0
 
     mock_uvicorn_run.assert_called_once_with(
         app=f"{path.stem}:{factory_name}",
         host="127.0.0.1",
         port=8000,
         factory=True,
         uds=None,
         fd=None,
         ssl_certfile=None,
         ssl_keyfile=None,
     )
+    if tty_enabled and not quiet_console:
+        assert len(result.output) > 0
+    else:
+        assert len(result.output) == 0
 
 
+@pytest.mark.parametrize("quiet_console", [True, False])
+@pytest.mark.parametrize("tty_enabled", [True, False])
 def test_run_command_with_app_factory(
-    runner: CliRunner, mock_uvicorn_run: MagicMock, create_app_file: CreateAppFileFixture
+    runner: CliRunner,
+    mock_uvicorn_run: MagicMock,
+    create_app_file: CreateAppFileFixture,
+    tty_enabled: bool,
+    quiet_console: bool,
+    mocker: MockerFixture,
+    monkeypatch: MonkeyPatch,
 ) -> None:
+    monkeypatch.delenv("LITESTAR_QUIET_CONSOLE", raising=False)
+    if quiet_console:
+        monkeypatch.setenv("LITESTAR_QUIET_CONSOLE", "true")
+    mocker.patch.object(core, "isatty", return_value=tty_enabled)
+    mocker.patch.object(_utils, "isatty", return_value=tty_enabled)
     path = create_app_file("_create_app_with_path.py", content=CREATE_APP_FILE_CONTENT)
     app_path = f"{path.stem}:create_app"
     result = runner.invoke(cli_command, ["--app", app_path, "run"])
 
     assert result.exception is None
     assert result.exit_code == 0
 
@@ -249,14 +291,127 @@
         port=8000,
         factory=True,
         uds=None,
         fd=None,
         ssl_certfile=None,
         ssl_keyfile=None,
     )
+    if tty_enabled and not quiet_console:
+        assert len(result.output) > 0
+    else:
+        assert len(result.output) == 0
+
+
+@pytest.mark.parametrize(
+    "cli, env, expected",
+    (
+        (
+            ("--reload", True),
+            ("LITESTAR_RELOAD", False),
+            "--reload",
+        ),
+        (
+            ("--reload-dir", [".", "../somewhere_else"]),
+            ("LITESTAR_RELOAD_DIRS", ["../somewhere_else3", "../somewhere_else2"]),
+            ["--reload-dir=.", "--reload-dir=../somewhere_else"],
+        ),
+        (
+            ("--reload-include", ["*.rst", "*.yml"]),
+            ("LITESTAR_RELOAD_INCLUDES", ["*.rst2", "*.yml2"]),
+            ["--reload-include=*.rst", "--reload-include=*.yml"],
+        ),
+        (
+            ("--reload-exclude", ["*.rst", "*.yml"]),
+            ("LITESTAR_RELOAD_EXCLUDES", ["*.rst2", "*.yml2"]),
+            ["--reload-exclude=*.rst", "--reload-exclude=*.yml"],
+        ),
+        (
+            ("--wc", 2),
+            ("LITESTAR_WEB_CONCURRENCY", 4),
+            "--workers=2",
+        ),
+        (
+            ("--fd", 0),
+            ("LITESTAR_FILE_DESCRIPTOR", 1),
+            "--fd=0",
+        ),
+        (
+            ("--uds", "/run/uvicorn/litestar_test.sock"),
+            ("LITESTAR_UNIX_DOMAIN_SOCKET", "/run/uvicorn/litestar_test2.sock"),
+            "--uds=/run/uvicorn/litestar_test.sock",
+        ),
+        (
+            ("-d", True),
+            ("LITESTAR_DEBUG", False),
+            ("LITESTAR_DEBUG", "1"),
+        ),
+        (
+            ("--pdb", True),
+            ("LITESTAR_PDB", False),
+            ("LITESTAR_PDB", "1"),
+        ),
+    ),
+)
+def test_run_command_arguments_precedence(
+    cli: Tuple[str, Union[Literal[True], List[str], str]],
+    env: Tuple[str, Union[Literal[True], List[str], str]],
+    expected: str,
+    runner: CliRunner,
+    monkeypatch: MonkeyPatch,
+    mock_subprocess_run: MagicMock,
+    tmp_project_dir: Path,
+    create_app_file: CreateAppFileFixture,
+    mock_uvicorn_run: MagicMock,
+) -> None:
+    args = []
+    args.extend(["--app", f"{Path('my_app.py').stem}:app"])
+    args.extend(["--app-dir", str(Path(tmp_project_dir / "custom_subfolder"))])
+    args.extend(["run"])
+    create_app_file("my_app.py", directory="custom_subfolder")
+
+    env_name, env_value = env
+    cli_name, cli_value = cli
+
+    if env_name:
+        if isinstance(env_value, list):
+            monkeypatch.setenv(env_name, "".join(env_value))
+        else:
+            monkeypatch.setenv(env_name, env_value)  # type: ignore[arg-type] # pyright: ignore (reportGeneralTypeIssues)
+
+    if cli_name:
+        if cli_value is True:
+            args.append(cli_name)
+        elif isinstance(cli_value, list):
+            for value in cli_value:
+                args.extend([cli_name, value])
+        else:
+            args.extend([cli_name, cli_value])
+
+    result = runner.invoke(cli_command, args)
+
+    assert result.exception is None
+    assert result.exit_code == 0
+
+    if cli_name in ["--fd", "--uds"]:
+        mock_subprocess_run.assert_not_called()
+        if isinstance(expected, list):  # type: ignore[unreachable]
+            assert all(_ in mock_uvicorn_run.call_args_list[0].args[0] for _ in expected)  # type: ignore[unreachable]
+        else:
+            assert mock_uvicorn_run.call_args_list[0].kwargs.get(cli_name.strip("--")) == cli_value
+
+    elif cli_name in ["-d", "--pdb"]:
+        assert os.environ.get(expected[0]) == expected[1]
+
+    else:
+        mock_subprocess_run.assert_called_once()
+
+        if isinstance(expected, list):  # type: ignore[unreachable]
+            assert all(_ in mock_subprocess_run.call_args_list[0].args[0] for _ in expected)  # type: ignore[unreachable]
+        else:
+            assert expected in mock_subprocess_run.call_args_list[0].args[0]
 
 
 @pytest.fixture()
 def unset_env() -> Generator[None, None, None]:
     initial_env = {**os.environ}
     yield
     for key in os.environ.keys() - initial_env.keys():
@@ -275,14 +430,79 @@
     result = runner.invoke(cli_command, ["--app", app_path, "run", "--debug"])
 
     assert result.exit_code == 0
     assert os.getenv("LITESTAR_DEBUG") == "1"
 
 
 @pytest.mark.usefixtures("mock_uvicorn_run", "unset_env")
+def test_run_command_quiet_console(
+    app_file: Path,
+    mocker: MockerFixture,
+    runner: CliRunner,
+    monkeypatch: MonkeyPatch,
+    create_app_file: CreateAppFileFixture,
+) -> None:
+    mocker.patch.object(core, "isatty", return_value=True)
+    mocker.patch.object(_utils, "isatty", return_value=True)
+    console = Console(file=io.StringIO(), force_interactive=True)
+    monkeypatch.setattr(_utils, "console", console)
+
+    path = create_app_file("_create_app_with_path.py", content=CREATE_APP_FILE_CONTENT)
+    app_path = f"{path.stem}:create_app"
+    monkeypatch.delenv("LITESTAR_QUIET_CONSOLE", raising=False)
+    result = runner.invoke(cli_command, ["--app", app_path, "run"])
+    assert result.exit_code == 0
+    normal_output = console.file.getvalue()  # type: ignore[attr-defined]
+    assert "Using Litestar app from env:" in normal_output
+    assert "Starting server process" in result.stdout
+    del result
+    console = Console(file=io.StringIO(), force_interactive=True)
+    monkeypatch.setattr(_utils, "console", console)
+    monkeypatch.setenv("LITESTAR_QUIET_CONSOLE", "1")
+    assert os.getenv("LITESTAR_QUIET_CONSOLE") == "1"
+    result = runner.invoke(cli_command, ["--app", app_path, "run"])
+    assert result.exit_code == 0
+    quiet_output = console.file.getvalue()  # type: ignore[attr-defined]
+    assert "Starting server process" not in result.stdout
+    assert "Using Litestar app from env:" not in quiet_output
+    console.clear()
+
+
+@pytest.mark.usefixtures("mock_uvicorn_run", "unset_env")
+def test_run_command_custom_app_name(
+    app_file: Path,
+    runner: CliRunner,
+    monkeypatch: MonkeyPatch,
+    create_app_file: CreateAppFileFixture,
+    mocker: MockerFixture,
+) -> None:
+    mocker.patch.object(core, "isatty", return_value=True)
+    mocker.patch.object(_utils, "isatty", return_value=True)
+
+    console = Console(file=io.StringIO(), force_interactive=True)
+    monkeypatch.setattr(_utils, "console", console)
+
+    path = create_app_file("_create_app_with_path.py", content=CREATE_APP_FILE_CONTENT)
+    app_path = f"{path.stem}:create_app"
+    monkeypatch.delenv("LITESTAR_APP_NAME", raising=False)
+    result = runner.invoke(cli_command, ["--app", app_path, "run"])
+    assert result.exit_code == 0
+    _output = console.file.getvalue()  # type: ignore[attr-defined]
+    assert "Using Litestar app from env:" in _output
+    console = Console(file=io.StringIO(), force_interactive=True)
+    monkeypatch.setattr(_utils, "console", console)
+    monkeypatch.setenv("LITESTAR_APP_NAME", "My Stuff")
+    assert os.getenv("LITESTAR_APP_NAME") == "My Stuff"
+    result = runner.invoke(cli_command, ["--app", app_path, "run"])
+    assert result.exit_code == 0
+    _output = console.file.getvalue()  # type: ignore[attr-defined]
+    assert "Using My Stuff app from env:" in _output
+
+
+@pytest.mark.usefixtures("mock_uvicorn_run", "unset_env")
 def test_run_command_pdb(
     app_file: Path,
     runner: CliRunner,
     monkeypatch: MonkeyPatch,
     create_app_file: CreateAppFileFixture,
 ) -> None:
     monkeypatch.delenv("LITESTAR_PDB", raising=False)
@@ -346,29 +566,29 @@
         ssl_keyfile=None,
     )
 
 
 @pytest.mark.parametrize(
     "app_content, schema_enabled, exclude_pattern_list, expected_result_routes_count",
     [
-        pytest.param(APP_FILE_CONTENT_ROUTES_EXAMPLE, False, (), 3, id="schema-enabled_no-exclude"),
+        pytest.param(APP_FILE_CONTENT_ROUTES_EXAMPLE, False, (), 3, id="schema-disabled_no-exclude"),
         pytest.param(
             APP_FILE_CONTENT_ROUTES_EXAMPLE,
             False,
             ("/foo", "/destroy/.*", "/java", "/haskell"),
             2,
-            id="schema-enabled_exclude",
+            id="schema-disabled_exclude",
         ),
-        pytest.param(APP_FILE_CONTENT_ROUTES_EXAMPLE, True, (), 12, id="schema-disabled_no-exclude"),
+        pytest.param(APP_FILE_CONTENT_ROUTES_EXAMPLE, True, (), 13, id="schema-enabled_no-exclude"),
         pytest.param(
             APP_FILE_CONTENT_ROUTES_EXAMPLE,
             True,
             ("/foo", "/destroy/.*", "/java", "/haskell"),
-            11,
-            id="schema-disabled_exclude",
+            12,
+            id="schema-enabled_exclude",
         ),
     ],
 )
 @pytest.mark.xdist_group("cli_autodiscovery")
 def test_routes_command_options(
     runner: CliRunner,
     app_content: str,
@@ -421,15 +641,15 @@
         http_route = MagicMock()
         http_route.path = route
         http_routes.append(http_route)
 
     api_config = MagicMock()
     api_config.openapi_controller.path = "/schema"
 
-    results = remove_default_schema_routes(http_routes, api_config)  # type: ignore[arg-type]
+    results = _utils.remove_default_schema_routes(http_routes, api_config)  # type: ignore[arg-type]
     assert len(results) == 3
     for result in results:
         words = re.split(r"(^\/[a-z]+)", result.path)
         assert "/schema" not in words
 
 
 def test_remove_routes_with_patterns() -> None:
@@ -437,12 +657,12 @@
     http_routes = []
     for route in routes:
         http_route = MagicMock()
         http_route.path = route
         http_routes.append(http_route)
 
     patterns = ("/destroy", "/pizza", "[]")
-    results = remove_routes_with_patterns(http_routes, patterns)  # type: ignore[arg-type]
+    results = _utils.remove_routes_with_patterns(http_routes, patterns)  # type: ignore[arg-type]
     paths = [route.path for route in results]
     assert len(paths) == 2
     for route in ["/", "/foo"]:
         assert route in paths
```

### Comparing `litestar-2.7.1/tests/unit/test_cli/test_env_resolution.py` & `litestar-2.8.0/tests/unit/test_cli/test_env_resolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,21 @@
 from pathlib import Path
-from typing import Optional
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from click import ClickException
 
 from litestar import Litestar
 from litestar.cli._utils import LitestarEnv, _path_to_dotted_path
 
 from .conftest import CreateAppFileFixture
 
 pytestmark = pytest.mark.xdist_group("cli_autodiscovery")
 
 
-@pytest.mark.parametrize("env_name,attr_name", [("LITESTAR_DEBUG", "debug"), ("LITESTAR_RELOAD", "reload")])
-@pytest.mark.parametrize(
-    "env_value,expected_value",
-    [("true", True), ("True", True), ("1", True), ("0", False), (None, False)],
-)
-def test_litestar_env_from_env_booleans(
-    monkeypatch: MonkeyPatch,
-    app_file: Path,
-    attr_name: str,
-    env_name: str,
-    env_value: Optional[str],
-    expected_value: bool,
-) -> None:
-    monkeypatch.delenv(env_name, raising=False)
-    if env_value is not None:
-        monkeypatch.setenv(env_name, env_value)
-
-    env = LitestarEnv.from_env(f"{app_file.stem}:app")
-
-    assert getattr(env, attr_name) is expected_value
-    assert isinstance(env.app, Litestar)
-
-
 def test_litestar_env_from_env_port(monkeypatch: MonkeyPatch, app_file: Path) -> None:
     env = LitestarEnv.from_env(f"{app_file.stem}:app")
     assert env.port is None
 
     monkeypatch.setenv("LITESTAR_PORT", "7000")
     env = LitestarEnv.from_env(f"{app_file.stem}:app")
     assert env.port == 7000
```

### Comparing `litestar-2.7.1/tests/unit/test_cli/test_schema_commands.py` & `litestar-2.8.0/tests/unit/test_cli/test_schema_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_cli/test_session_commands.py` & `litestar-2.8.0/tests/unit/test_cli/test_session_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_cli/test_ssl.py` & `litestar-2.8.0/tests/unit/test_cli/test_ssl.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_connection/test_base.py` & `litestar-2.8.0/tests/unit/test_connection/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_connection/test_connection_caching.py` & `litestar-2.8.0/tests/unit/test_connection/test_connection_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_connection/test_request.py` & `litestar-2.8.0/tests/unit/test_connection/test_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_connection/test_websocket.py` & `litestar-2.8.0/tests/unit/test_connection/test_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/conftest.py` & `litestar-2.8.0/tests/unit/test_contrib/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_minijinja.py` & `litestar-2.8.0/tests/unit/test_contrib/test_minijinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_msgspec.py` & `litestar-2.8.0/tests/unit/test_contrib/test_msgspec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from msgspec import Meta, Struct, field
 from typing_extensions import Annotated
 
-from litestar.dto import MsgspecDTO, dto_field
+from litestar.dto import DTOField, MsgspecDTO, dto_field
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.typing import FieldDefinition
 
 if TYPE_CHECKING:
     from typing import Callable
 
 
@@ -34,7 +34,21 @@
         a: int
 
     class NotStruct:
         pass
 
     assert MsgspecDTO.detect_nested_field(FieldDefinition.from_annotation(TestStruct)) is True
     assert MsgspecDTO.detect_nested_field(FieldDefinition.from_annotation(NotStruct)) is False
+
+
+ReadOnlyInt = Annotated[int, DTOField("read-only")]
+
+
+def test_msgspec_dto_annotated_dto_field() -> None:
+    class Model(Struct):
+        a: Annotated[int, DTOField("read-only")]
+        b: ReadOnlyInt
+
+    dto_type = MsgspecDTO[Model]
+    fields = list(dto_type.generate_field_definitions(Model))
+    assert fields[0].dto_field == DTOField("read-only")
+    assert fields[1].dto_field == DTOField("read-only")
```

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_opentelemetry.py` & `litestar-2.8.0/tests/unit/test_contrib/test_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_prometheus.py` & `litestar-2.8.0/tests/unit/test_contrib/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_repository.py` & `litestar-2.8.0/tests/unit/test_contrib/test_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_sqlalchemy.py` & `litestar-2.8.0/tests/unit/test_contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py` & `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_schema_plugin.py` & `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py` & `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_attrs/test_signature.py` & `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_htmx/test_htmx_request.py` & `litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_htmx/test_htmx_response.py` & `litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/endpoints.py` & `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/endpoints.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py` & `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/tables.py` & `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/tables.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py` & `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/conftest.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/models.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_dto.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_openapi.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,14 +549,34 @@
 
     assert isinstance(value, Schema)
     assert value.description == "description"
     assert value.title == "title"
     assert value.examples == ["example"]
 
 
+def test_create_schema_for_field_v2__examples() -> None:
+    class Model(pydantic_v2.BaseModel):
+        value: str = pydantic_v2.Field(
+            title="title", description="description", max_length=16, json_schema_extra={"examples": ["example"]}
+        )
+
+    schema = get_schema_for_field_definition(
+        FieldDefinition.from_kwarg(name="Model", annotation=Model), plugins=[PydanticSchemaPlugin()]
+    )
+
+    assert schema.properties
+
+    value = schema.properties["value"]
+
+    assert isinstance(value, Schema)
+    assert value.description == "description"
+    assert value.title == "title"
+    assert value.examples == ["example"]
+
+
 @pytest.mark.parametrize("with_future_annotations", [True, False])
 def test_create_schema_for_pydantic_model_with_annotated_model_attribute(
     with_future_annotations: bool, create_module: "Callable[[str], ModuleType]", pydantic_version: PydanticVersion
 ) -> None:
     """Test that a model with an annotated attribute is correctly handled."""
     module = create_module(
         f"""
```

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import pydantic as pydantic_v2
+import pytest
 from pydantic import v1 as pydantic_v1
 from typing_extensions import Annotated
 
 from litestar.contrib.pydantic import PydanticDTO
-from litestar.dto import dto_field
+from litestar.dto import DTOField, dto_field
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.typing import FieldDefinition
 
+from . import PydanticVersion
+
 if TYPE_CHECKING:
     from typing import Callable
 
 
 def test_field_definition_generation_v1(
     int_factory: Callable[[], int],
     expected_field_defs: list[DTOFieldDefinition],
 ) -> None:
     class TestModel(pydantic_v1.BaseModel):
         a: int
-        b: Annotated[int, pydantic_v1.Field(**dto_field("read-only"))]  # pyright: ignore
+        b: Annotated[int, DTOField("read-only")]
         c: Annotated[int, pydantic_v1.Field(gt=1)]
         d: int = pydantic_v1.Field(default=1)
         e: int = pydantic_v1.Field(default_factory=int_factory)
 
     field_defs = list(PydanticDTO.generate_field_definitions(TestModel))
     assert field_defs[0].model_name == "TestModel"
     for field_def, exp in zip(field_defs, expected_field_defs):
@@ -34,15 +37,15 @@
 
 def test_field_definition_generation_v2(
     int_factory: Callable[[], int],
     expected_field_defs: list[DTOFieldDefinition],
 ) -> None:
     class TestModel(pydantic_v2.BaseModel):
         a: int
-        b: Annotated[int, pydantic_v2.Field(**dto_field("read-only"))]  # pyright: ignore
+        b: Annotated[int, DTOField("read-only")]
         c: Annotated[int, pydantic_v2.Field(gt=1)]
         d: int = pydantic_v2.Field(default=1)
         e: int = pydantic_v2.Field(default_factory=int_factory)
 
     field_defs = list(PydanticDTO.generate_field_definitions(TestModel))
     assert field_defs[0].model_name == "TestModel"
     for field_def, exp in zip(field_defs, expected_field_defs):
@@ -54,7 +57,37 @@
         a: int
 
     class NotModel:
         pass
 
     assert PydanticDTO.detect_nested_field(FieldDefinition.from_annotation(TestModel)) is True
     assert PydanticDTO.detect_nested_field(FieldDefinition.from_annotation(NotModel)) is False
+
+
+ReadOnlyInt = Annotated[int, DTOField("read-only")]
+
+
+def test_pydantic_dto_annotated_dto_field(base_model: type[pydantic_v1.BaseModel | pydantic_v2.BaseModel]) -> None:
+    class Model(base_model):  # type: ignore[misc, valid-type]
+        a: Annotated[int, DTOField("read-only")]
+        b: ReadOnlyInt
+
+    dto_type = PydanticDTO[Model]
+    fields = list(dto_type.generate_field_definitions(Model))
+    assert fields[0].dto_field == DTOField("read-only")
+    assert fields[1].dto_field == DTOField("read-only")
+
+
+def test_dto_field_via_pydantic_field_extra_deprecation(
+    pydantic_version: PydanticVersion,
+) -> None:
+    if pydantic_version == "v1":
+
+        class Model(pydantic_v1.BaseModel):  # pyright: ignore
+            a: int = pydantic_v1.Field(**dto_field("read-only"))  # type: ignore[arg-type, misc]
+    else:
+
+        class Model(pydantic_v2.BaseModel):  # type: ignore[no-redef]
+            a: int = pydantic_v2.Field(**dto_field("read-only"))  # type: ignore[arg-type, pydantic-field]
+
+    with pytest.warns(DeprecationWarning):
+        next(PydanticDTO.generate_field_definitions(Model))
```

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_contrib/test_pydantic/test_utils.py` & `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_datastructures/test_cookie.py` & `litestar-2.8.0/tests/unit/test_datastructures/test_cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_datastructures/test_headers.py` & `litestar-2.8.0/tests/unit/test_datastructures/test_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_datastructures/test_multi_dicts.py` & `litestar-2.8.0/tests/unit/test_datastructures/test_multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_datastructures/test_state.py` & `litestar-2.8.0/tests/unit/test_datastructures/test_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_datastructures/test_upload_file.py` & `litestar-2.8.0/tests/unit/test_datastructures/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_datastructures/test_url.py` & `litestar-2.8.0/tests/unit/test_datastructures/test_url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_dto/conftest.py` & `litestar-2.8.0/tests/unit/test_dto/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_integration.py` & `litestar-2.8.0/tests/unit/test_dto/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,7 +149,20 @@
     Litestar(
         route_handlers=[handler],
         experimental_features=[ExperimentalFeatures.DTO_CODEGEN],
     )
 
     backend = handler.resolve_data_dto()._dto_backends[handler.handler_id]["data_backend"]  # type: ignore[union-attr]
     assert isinstance(backend, DTOBackend)
+
+
+def test_use_codegen_backend_by_default(ModelDataDTO: type[AbstractDTO]) -> None:
+    ModelDataDTO.config = DTOConfig()
+
+    @post(dto=ModelDataDTO, signature_types=[Model])
+    def handler(data: Model) -> Model:
+        return data
+
+    Litestar(route_handlers=[handler])
+
+    backend = handler.resolve_data_dto()._dto_backends[handler.handler_id]["data_backend"]  # type: ignore[union-attr]
+    assert isinstance(backend, DTOBackend)
```

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_factory/test_base_dto.py` & `litestar-2.8.0/tests/unit/test_dto/test_factory/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_factory/test_dataclass_dto.py` & `litestar-2.8.0/tests/unit/test_dto/test_factory/test_dataclass_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import sys
 from dataclasses import dataclass, field, replace
 from typing import ClassVar, List
 from unittest.mock import ANY
 
 import pytest
+from typing_extensions import Annotated
 
 from litestar.dto import DataclassDTO, DTOField
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.typing import FieldDefinition
 
 
 @dataclass
@@ -117,7 +118,24 @@
     for field_def, exp in zip(dto_type.generate_field_definitions(Model), expected):
         assert field_def == exp
 
 
 def test_dataclass_detect_nested(dto_type: type[DataclassDTO[Model]]) -> None:
     assert dto_type.detect_nested_field(FieldDefinition.from_annotation(Model)) is True
     assert dto_type.detect_nested_field(FieldDefinition.from_annotation(int)) is False
+
+
+ReadOnlyInt = Annotated[int, DTOField("read-only")]
+
+
+def test_dataclass_dto_annotated_dto_field() -> None:
+    Annotated[int, DTOField("read-only")]
+
+    @dataclass
+    class Model:
+        a: Annotated[int, DTOField("read-only")]
+        b: ReadOnlyInt
+
+    dto_type = DataclassDTO[Model]
+    fields = list(dto_type.generate_field_definitions(Model))
+    assert fields[0].dto_field == DTOField("read-only")
+    assert fields[1].dto_field == DTOField("read-only")
```

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_factory/test_integration.py` & `litestar-2.8.0/tests/unit/test_dto/test_factory/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_factory/test_utils.py` & `litestar-2.8.0/tests/unit/test_dto/test_factory/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/test_backends.py` & `litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,26 +192,28 @@
         handler_id=app.get_handler_index_by_name("test")["handler"].handler_id,  # type: ignore[index]
         field_definition=FieldDefinition.from_annotation(DC),
         schema_creator=creator,
     )
     schemas = creator.schema_registry.generate_components_schemas()
     assert isinstance(ref, Reference)
     schema = schemas[ref.value]
+    assert schema.title == "HandlerDCResponseBody"
     assert schema.properties is not None
     a, b, c = schema.properties["a"], schema.properties["b"], schema.properties["c"]
     assert isinstance(a, Schema)
     assert a.type == "integer"
     assert isinstance(b, Schema)
     assert b.type == "string"
     assert isinstance(c, Schema)
     assert c.type == "array"
     assert isinstance(c.items, Schema)
     assert c.items.type == "integer"
     assert isinstance(nested := schema.properties["nested"], Reference)  # noqa: RUF018
     nested_schema = schemas[nested.value]
+    assert nested_schema.title == "HandlerDCNestedDCResponseBody"
     assert nested_schema.properties is not None
     nested_a, nested_b = nested_schema.properties["a"], nested_schema.properties["b"]
     assert isinstance(nested_a, Schema)
     assert nested_a.type == "integer"
     assert isinstance(nested_b, Schema)
     assert nested_b.type == "string"
```

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py` & `litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_dto/test_factory/test_backends/test_utils.py` & `litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py` & `litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py` & `litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_asgi_handlers/test_validations.py` & `litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_base_handlers/test_opt.py` & `litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_opt.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_base_handlers/test_resolution.py` & `litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_base_handlers/test_validations.py` & `litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_defaults.py` & `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_head.py` & `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_head.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py` & `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_media_type.py` & `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py` & `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_sync.py` & `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_http_handlers/test_validations.py` & `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py` & `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py` & `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py` & `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py` & `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from contextlib import asynccontextmanager
 from dataclasses import dataclass, field
 from typing import Any, AsyncGenerator, Dict, List, Optional, Type, Union, cast
 from unittest.mock import AsyncMock, MagicMock
 
 import pytest
-from pytest_lazyfixture import lazy_fixture
+from pytest_lazy_fixtures import lf
 
 from litestar import Controller, Litestar, Request, WebSocket
 from litestar.datastructures import State
 from litestar.di import Provide
 from litestar.dto import DataclassDTO, dto_field
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.websocket_handlers import WebsocketListener, websocket_listener
@@ -43,17 +43,17 @@
 
     return websocket_listener("/")(listener)
 
 
 @pytest.mark.parametrize(
     "listener",
     [
-        lazy_fixture("sync_listener_callable"),
-        lazy_fixture("async_listener_callable"),
-        lazy_fixture("listener_class"),
+        lf("sync_listener_callable"),
+        lf("async_listener_callable"),
+        lf("listener_class"),
     ],
 )
 def test_basic_listener(mock: MagicMock, listener: Union[websocket_listener, Type[WebsocketListener]]) -> None:
     client = create_test_client([listener])
     with client.websocket_connect("/") as ws:
         ws.send_text("foo")
         assert ws.receive_text() == "foo"
```

### Comparing `litestar-2.7.1/tests/unit/test_handlers/test_websocket_handlers/test_validations.py` & `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/flower.jpeg` & `litestar-2.8.0/tests/unit/test_kwargs/flower.jpeg`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_cleanup_group.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_cleanup_group.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_cookie_params.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_cookie_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_defaults.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_dependency_batches.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_dependency_batches.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_generator_dependencies.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_generator_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_header_params.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_header_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_json_data.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_json_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_layered_params.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_layered_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_msgpack_data.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_msgpack_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_multipart_data.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_multipart_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_path_params.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_path_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_query_params.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_query_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_reserved_kwargs_injection.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_reserved_kwargs_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_url_encoded_data.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_url_encoded_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_kwargs/test_validations.py` & `litestar-2.8.0/tests/unit/test_kwargs/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_logging/test_logging_config.py` & `litestar-2.8.0/tests/unit/test_logging/test_logging_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_logging/test_structlog_config.py` & `litestar-2.8.0/tests/unit/test_logging/test_structlog_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_allowed_hosts_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_allowed_hosts_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_base_authentication_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_base_authentication_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_base_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_base_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_compression_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_compression_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_cors_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_cors_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_csrf_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_csrf_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_exception_handler_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_exception_handler_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 from _pytest.capture import CaptureFixture
 from pytest_mock import MockerFixture
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from structlog.testing import capture_logs
 
-from litestar import Litestar, Request, Response, get
+from litestar import Litestar, MediaType, Request, Response, get
 from litestar.exceptions import HTTPException, InternalServerException, ValidationException
 from litestar.logging.config import LoggingConfig, StructLoggingConfig
 from litestar.middleware.exceptions import ExceptionHandlerMiddleware
 from litestar.middleware.exceptions._debug_response import get_symbol_name
 from litestar.middleware.exceptions.middleware import _starlette_exception_handler, get_exception_handler
 from litestar.status_codes import HTTP_400_BAD_REQUEST, HTTP_500_INTERNAL_SERVER_ERROR
 from litestar.testing import TestClient, create_test_client
@@ -367,22 +367,24 @@
         exc = e
 
     if exc is not None and exc.__traceback__ is not None:
         frame = getinnerframes(exc.__traceback__, 2)[-1]
         assert get_symbol_name(frame) == "Test.method"
 
 
-def test_serialize_custom_types() -> None:
+@pytest.mark.parametrize("media_type", list(MediaType))
+def test_serialize_custom_types(media_type: MediaType) -> None:
     # ensure type encoders are passed down to the created response so custom types that
     # might end up as part of a ValidationException are handled properly
     # https://github.com/litestar-org/litestar/issues/2867
+    # https://github.com/litestar-org/litestar/issues/3192
     class Foo:
         def __init__(self, value: str) -> None:
             self.value = value
 
-    @get()
+    @get(media_type=media_type)
     def handler() -> None:
         raise ValidationException(extra={"foo": Foo("bar")})
 
     with create_test_client([handler], type_encoders={Foo: lambda f: f.value}) as client:
         res = client.get("/")
         assert res.json()["extra"] == {"foo": "bar"}
```

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_logging_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_middleware_handling.py` & `litestar-2.8.0/tests/unit/test_middleware/test_middleware_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_rate_limit_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_rate_limit_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_session/conftest.py` & `litestar-2.8.0/tests/unit/test_middleware/test_session/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_session/test_client_side_backend.py` & `litestar-2.8.0/tests/unit/test_middleware/test_session/test_client_side_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_session/test_integration.py` & `litestar-2.8.0/tests/unit/test_middleware/test_session/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_session/test_middleware.py` & `litestar-2.8.0/tests/unit/test_middleware/test_session/test_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_middleware/test_session/test_server_side_backend.py` & `litestar-2.8.0/tests/unit/test_middleware/test_session/test_server_side_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_openapi/conftest.py` & `litestar-2.8.0/tests/unit/test_openapi/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 from typing import Any, Dict, List, Optional, Type, Union
 
 import pytest
 
 from litestar import Controller, MediaType, delete, get, patch, post, put
 from litestar.datastructures import ResponseHeader, State
 from litestar.dto import DataclassDTO, DTOConfig, DTOData
+from litestar.openapi.controller import OpenAPIController
 from litestar.openapi.spec.example import Example
 from litestar.params import Parameter
 from tests.models import DataclassPerson, DataclassPersonFactory, DataclassPet
 from tests.unit.test_openapi.utils import Gender, PetException
 
 
 class PartialDataclassPersonDTO(DataclassDTO[DataclassPerson]):
     config = DTOConfig(partial=True)
 
 
 def create_person_controller() -> Type[Controller]:
     class PersonController(Controller):
         path = "/{service_id:int}/person"
 
-        @get()
+        @get(sync_to_thread=False)
         def get_persons(
             self,
             # expected to be ignored
             headers: Any,
             request: Any,
             state: State,
             query: Dict[str, Any],
@@ -49,79 +50,87 @@
             # header parameter
             secret_header: str = Parameter(header="secret"),
             # cookie parameter
             cookie_value: int = Parameter(cookie="value"),
         ) -> List[DataclassPerson]:
             return []
 
-        @post(media_type=MediaType.TEXT)
+        @post(media_type=MediaType.TEXT, sync_to_thread=False)
         def create_person(
             self, data: DataclassPerson, secret_header: str = Parameter(header="secret")
         ) -> DataclassPerson:
             return data
 
-        @post(path="/bulk", dto=PartialDataclassPersonDTO)
+        @post(path="/bulk", dto=PartialDataclassPersonDTO, sync_to_thread=False)
         def bulk_create_person(
             self, data: DTOData[List[DataclassPerson]], secret_header: str = Parameter(header="secret")
         ) -> List[DataclassPerson]:
             return []
 
-        @put(path="/bulk")
+        @put(path="/bulk", sync_to_thread=False)
         def bulk_update_person(
             self, data: List[DataclassPerson], secret_header: str = Parameter(header="secret")
         ) -> List[DataclassPerson]:
             return []
 
-        @patch(path="/bulk", dto=PartialDataclassPersonDTO)
+        @patch(path="/bulk", dto=PartialDataclassPersonDTO, sync_to_thread=False)
         def bulk_partial_update_person(
             self, data: DTOData[List[DataclassPerson]], secret_header: str = Parameter(header="secret")
         ) -> List[DataclassPerson]:
             return []
 
-        @get(path="/{person_id:str}")
+        @get(path="/{person_id:str}", sync_to_thread=False)
         def get_person_by_id(self, person_id: str) -> DataclassPerson:
             """Description in docstring."""
             return DataclassPersonFactory.build(id=person_id)
 
-        @patch(path="/{person_id:str}", description="Description in decorator", dto=PartialDataclassPersonDTO)
+        @patch(
+            path="/{person_id:str}",
+            description="Description in decorator",
+            dto=PartialDataclassPersonDTO,
+            sync_to_thread=False,
+        )
         def partial_update_person(self, person_id: str, data: DTOData[DataclassPerson]) -> DataclassPerson:
             """Description in docstring."""
             return DataclassPersonFactory.build(id=person_id)
 
-        @put(path="/{person_id:str}")
+        @put(path="/{person_id:str}", sync_to_thread=False)
         def update_person(self, person_id: str, data: DataclassPerson) -> DataclassPerson:
             """Multiline docstring example.
 
             Line 3.
             """
             return data
 
-        @delete(path="/{person_id:str}")
+        @delete(path="/{person_id:str}", sync_to_thread=False)
         def delete_person(self, person_id: str) -> None:
             return None
 
-        @get(path="/dataclass")
+        @get(path="/dataclass", sync_to_thread=False)
         def get_person_dataclass(self) -> DataclassPerson:
             return DataclassPerson(
                 first_name="Moishe", last_name="zuchmir", id="1", optional=None, complex={}, pets=None
             )
 
     return PersonController
 
 
 def create_pet_controller() -> Type[Controller]:
     class PetController(Controller):
         path = "/pet"
 
-        @get()
+        @get(sync_to_thread=False)
         def pets(self) -> List[DataclassPet]:
             return []
 
         @get(
-            path="/owner-or-pet", response_headers=[ResponseHeader(name="x-my-tag", value="123")], raises=[PetException]
+            path="/owner-or-pet",
+            response_headers=[ResponseHeader(name="x-my-tag", value="123")],
+            raises=[PetException],
+            sync_to_thread=False,
         )
         def get_pets_or_owners(self) -> List[Union[DataclassPerson, DataclassPet]]:
             return []
 
     return PetController
 
 
@@ -131,7 +140,12 @@
     return create_person_controller()
 
 
 @pytest.fixture
 @pytest.mark.usefixtures("disable_warn_implicit_sync_to_thread")
 def pet_controller() -> Type[Controller]:
     return create_pet_controller()
+
+
+@pytest.fixture(params=[OpenAPIController, None])
+def openapi_controller(request: pytest.FixtureRequest) -> Optional[Type[OpenAPIController]]:
+    return request.param  # type: ignore[no-any-return]
```

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_datastructures.py` & `litestar-2.8.0/tests/unit/test_openapi/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_integration.py` & `litestar-2.8.0/tests/unit/test_openapi/test_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 from __future__ import annotations
 
+import dataclasses
 from dataclasses import dataclass
 from types import ModuleType
 from typing import Callable, Generic, Optional, TypeVar, cast
 
 import msgspec
 import pytest
 import yaml
 from typing_extensions import Annotated
 
 from litestar import Controller, Litestar, delete, get, patch, post
 from litestar._openapi.plugin import OpenAPIPlugin
-from litestar.app import DEFAULT_OPENAPI_CONFIG
 from litestar.enums import MediaType, OpenAPIMediaType, ParamType
 from litestar.openapi import OpenAPIConfig, OpenAPIController
 from litestar.openapi.spec import Parameter as OpenAPIParameter
 from litestar.params import Parameter
 from litestar.serialization.msgspec_hooks import decode_json, encode_json, get_serializer
 from litestar.status_codes import HTTP_200_OK, HTTP_404_NOT_FOUND
 from litestar.testing import create_test_client
 
 CREATE_EXAMPLES_VALUES = (True, False)
 
 
-@pytest.mark.parametrize("create_examples", CREATE_EXAMPLES_VALUES)
+@pytest.fixture(params=[True, False])
+def create_examples(request: pytest.FixtureRequest) -> bool:
+    return request.param  # type: ignore[no-any-return]
+
+
 @pytest.mark.parametrize("schema_path", ["/schema/openapi.yaml", "/schema/openapi.yml"])
 def test_openapi(
-    person_controller: type[Controller], pet_controller: type[Controller], create_examples: bool, schema_path: str
+    person_controller: type[Controller],
+    pet_controller: type[Controller],
+    create_examples: bool,
+    schema_path: str,
+    openapi_controller: type[OpenAPIController] | None,
 ) -> None:
-    openapi_config = OpenAPIConfig("Example API", "1.0.0", create_examples=create_examples)
+    openapi_config = OpenAPIConfig(
+        "Example API", "1.0.0", create_examples=create_examples, openapi_controller=openapi_controller
+    )
     with create_test_client([person_controller, pet_controller], openapi_config=openapi_config) as client:
         assert client.app.openapi_schema
         openapi_schema = client.app.openapi_schema
         assert openapi_schema.paths
         response = client.get(schema_path)
         assert response.status_code == HTTP_200_OK
         assert response.headers["content-type"] == OpenAPIMediaType.OPENAPI_YAML.value
         assert client.app.openapi_schema
         serializer = get_serializer(client.app.type_encoders)
         schema_json = decode_json(encode_json(openapi_schema.to_schema(), serializer))
         assert response.content.decode("utf-8") == yaml.dump(schema_json)
 
 
-@pytest.mark.parametrize("create_examples", CREATE_EXAMPLES_VALUES)
 def test_openapi_json(
-    person_controller: type[Controller], pet_controller: type[Controller], create_examples: bool
+    person_controller: type[Controller],
+    pet_controller: type[Controller],
+    create_examples: bool,
+    openapi_controller: type[OpenAPIController] | None,
 ) -> None:
-    openapi_config = OpenAPIConfig("Example API", "1.0.0", create_examples=create_examples)
+    openapi_config = OpenAPIConfig(
+        "Example API", "1.0.0", create_examples=create_examples, openapi_controller=openapi_controller
+    )
     with create_test_client([person_controller, pet_controller], openapi_config=openapi_config) as client:
         assert client.app.openapi_schema
         openapi_schema = client.app.openapi_schema
         assert openapi_schema.paths
         response = client.get("/schema/openapi.json")
         assert response.status_code == HTTP_200_OK
         assert response.headers["content-type"] == OpenAPIMediaType.OPENAPI_JSON.value
@@ -59,54 +73,68 @@
         assert response.content == encode_json(openapi_schema.to_schema(), serializer)
 
 
 @pytest.mark.parametrize(
     "endpoint, schema_path", [("openapi.yaml", "/schema/openapi.yaml"), ("openapi.yml", "/schema/openapi.yml")]
 )
 def test_openapi_yaml_not_allowed(
-    endpoint: str, schema_path: str, person_controller: type[Controller], pet_controller: type[Controller]
+    endpoint: str,
+    schema_path: str,
+    person_controller: type[Controller],
+    pet_controller: type[Controller],
+    openapi_controller: type[OpenAPIController] | None,
 ) -> None:
-    openapi_config = DEFAULT_OPENAPI_CONFIG
-    openapi_config.enabled_endpoints.discard(endpoint)
+    openapi_config = OpenAPIConfig(
+        "Example API", "1.0.0", enabled_endpoints=set(), openapi_controller=openapi_controller
+    )
 
     with create_test_client([person_controller, pet_controller], openapi_config=openapi_config) as client:
         assert client.app.openapi_schema
         openapi_schema = client.app.openapi_schema
         assert openapi_schema.paths
         response = client.get(schema_path)
         assert response.status_code == HTTP_404_NOT_FOUND
 
 
 def test_openapi_json_not_allowed(person_controller: type[Controller], pet_controller: type[Controller]) -> None:
-    openapi_config = DEFAULT_OPENAPI_CONFIG
-    openapi_config.enabled_endpoints.discard("openapi.json")
+    # only tested with the OpenAPIController, b/c new router based approach always serves `openapi.json`.
+    openapi_config = OpenAPIConfig(
+        "Example API",
+        "1.0.0",
+        enabled_endpoints=set(),
+        openapi_controller=OpenAPIController,
+    )
 
     with create_test_client([person_controller, pet_controller], openapi_config=openapi_config) as client:
         assert client.app.openapi_schema
         openapi_schema = client.app.openapi_schema
         assert openapi_schema.paths
         response = client.get("/schema/openapi.json")
         assert response.status_code == HTTP_404_NOT_FOUND
 
 
-def test_openapi_custom_path() -> None:
-    openapi_config = OpenAPIConfig(title="my title", version="1.0.0", path="/custom_schema_path")
+def test_openapi_custom_path(openapi_controller: type[OpenAPIController] | None) -> None:
+    openapi_config = OpenAPIConfig(
+        title="my title", version="1.0.0", path="/custom_schema_path", openapi_controller=openapi_controller
+    )
     with create_test_client([], openapi_config=openapi_config) as client:
         response = client.get("/schema")
         assert response.status_code == HTTP_404_NOT_FOUND
 
         response = client.get("/custom_schema_path")
         assert response.status_code == HTTP_200_OK
 
         response = client.get("/custom_schema_path/openapi.json")
         assert response.status_code == HTTP_200_OK
 
 
-def test_openapi_normalizes_custom_path() -> None:
-    openapi_config = OpenAPIConfig(title="my title", version="1.0.0", path="custom_schema_path")
+def test_openapi_normalizes_custom_path(openapi_controller: type[OpenAPIController] | None) -> None:
+    openapi_config = OpenAPIConfig(
+        title="my title", version="1.0.0", path="custom_schema_path", openapi_controller=openapi_controller
+    )
     with create_test_client([], openapi_config=openapi_config) as client:
         response = client.get("/custom_schema_path/openapi.json")
         assert response.status_code == HTTP_200_OK
 
         response = client.get("/custom_schema_path/openapi.json")
         assert response.status_code == HTTP_200_OK
 
@@ -141,16 +169,15 @@
         response = client.get("/override_docs_path/openapi.json")
         assert response.status_code == HTTP_200_OK
 
         response = client.get("/override_docs_path/openapi.json")
         assert response.status_code == HTTP_200_OK
 
 
-@pytest.mark.parametrize("create_examples", CREATE_EXAMPLES_VALUES)
-def test_msgspec_schema_generation(create_examples: bool) -> None:
+def test_msgspec_schema_generation(create_examples: bool, openapi_controller: type[OpenAPIController] | None) -> None:
     class Lookup(msgspec.Struct):
         id: Annotated[
             str,
             msgspec.Meta(
                 min_length=12,
                 max_length=16,
                 description="A unique identifier",
@@ -164,14 +191,15 @@
 
     with create_test_client(
         route_handlers=[example_route],
         openapi_config=OpenAPIConfig(
             title="Example API",
             version="1.0.0",
             create_examples=create_examples,
+            openapi_controller=openapi_controller,
         ),
         signature_types=[Lookup],
     ) as client:
         response = client.get("/schema/openapi.json")
         assert response.status_code == HTTP_200_OK
         assert response.json()["components"]["schemas"]["test_msgspec_schema_generation.Lookup"]["properties"][
             "id"
@@ -180,25 +208,65 @@
             "examples": ["e4eaaaf2-d142-11e1-b3e4-080027620cdd"],
             "maxLength": 16,
             "minLength": 12,
             "type": "string",
         }
 
 
-def test_schema_for_optional_path_parameter() -> None:
+def test_dataclass_field_default() -> None:
+    # https://github.com/litestar-org/litestar/issues/3201
+    @dataclass
+    class SomeModel:
+        field_a: str = "default_a"
+        field_b: str = dataclasses.field(default="default_b")
+        field_c: str = dataclasses.field(default_factory=lambda: "default_c")
+
+    @get("/")
+    async def handler() -> SomeModel:
+        return SomeModel()
+
+    app = Litestar(route_handlers=[handler], signature_types=[SomeModel])
+    schema = app.openapi_schema.components.schemas["test_dataclass_field_default.SomeModel"]
+    assert schema
+    assert schema.properties["field_a"].default == "default_a"  # type: ignore[union-attr, index]
+    assert schema.properties["field_b"].default == "default_b"  # type: ignore[union-attr, index]
+    assert schema.properties["field_c"].default is None  # type: ignore[union-attr, index]
+
+
+def test_struct_field_default() -> None:
+    # https://github.com/litestar-org/litestar/issues/3201
+    class SomeModel(msgspec.Struct, kw_only=True):
+        field_a: str = "default_a"
+        field_b: str = msgspec.field(default="default_b")
+        field_c: str = msgspec.field(default_factory=lambda: "default_c")
+
+    @get("/")
+    async def handler() -> SomeModel:
+        return SomeModel()
+
+    app = Litestar(route_handlers=[handler], signature_types=[SomeModel])
+    schema = app.openapi_schema.components.schemas["test_struct_field_default.SomeModel"]
+    assert schema
+    assert schema.properties["field_a"].default == "default_a"  # type: ignore[union-attr, index]
+    assert schema.properties["field_b"].default == "default_b"  # type: ignore[union-attr, index]
+    assert schema.properties["field_c"].default is None  # type: ignore[union-attr, index]
+
+
+def test_schema_for_optional_path_parameter(openapi_controller: type[OpenAPIController] | None) -> None:
     @get(path=["/", "/{test_message:str}"], media_type=MediaType.TEXT, sync_to_thread=False)
     def handler(test_message: Optional[str]) -> str:  # noqa: UP007
         return test_message or "no message"
 
     with create_test_client(
         route_handlers=[handler],
         openapi_config=OpenAPIConfig(
             title="Example API",
             version="1.0.0",
             create_examples=True,
+            openapi_controller=openapi_controller,
         ),
     ) as client:
         response = client.get("/schema/openapi.json")
         assert response.status_code == HTTP_200_OK
         assert "parameters" not in response.json()["paths"]["/"]["get"]  # type[ignore]
         parameter = response.json()["paths"]["/{test_message}"]["get"]["parameters"][0]  # type[ignore]
         assert parameter
@@ -210,28 +278,29 @@
 
 
 @dataclass
 class Foo(Generic[T]):
     foo: T
 
 
-def test_with_generic_class() -> None:
+def test_with_generic_class(openapi_controller: type[OpenAPIController] | None) -> None:
     @get("/foo-str", sync_to_thread=False)
     def handler_foo_str() -> Foo[str]:
         return Foo("")
 
     @get("/foo-int", sync_to_thread=False)
     def handler_foo_int() -> Foo[int]:
         return Foo(1)
 
     with create_test_client(
         route_handlers=[handler_foo_str, handler_foo_int],
         openapi_config=OpenAPIConfig(
             title="Example API",
             version="1.0.0",
+            openapi_controller=openapi_controller,
         ),
     ) as client:
         response = client.get("/schema/openapi.json")
         assert response.status_code == HTTP_200_OK
         assert response.json() == {
             "info": {"title": "Example API", "version": "1.0.0"},
             "openapi": "3.1.0",
```

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_parameters.py` & `litestar-2.8.0/tests/unit/test_openapi/test_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Optional, Type, cast
+from typing import TYPE_CHECKING, Any, List, Optional, Type, cast
 from uuid import UUID
 
 import pytest
 from typing_extensions import Annotated
 
 from litestar import Controller, Litestar, Router, get
 from litestar._openapi.datastructures import OpenAPIContext
@@ -320,14 +320,54 @@
     ) as client:
         response = client.get("/schema/openapi.json")
         assert response.json()["paths"]["/"]["get"]["parameters"][0]["examples"] == {
             "text-example-1": {"summary": "example summary", "value": "example value"}
         }
 
 
+def test_parameter_schema_extra() -> None:
+    @get()
+    async def handler(
+        query1: Annotated[
+            str,
+            Parameter(
+                schema_extra={
+                    "schema_not": Schema(
+                        any_of=[
+                            Schema(type=OpenAPIType.STRING, pattern=r"^somePrefix:.*$"),
+                            Schema(type=OpenAPIType.STRING, enum=["denied", "values"]),
+                        ]
+                    ),
+                }
+            ),
+        ],
+    ) -> Any:
+        return query1
+
+    @get()
+    async def error_handler(query1: Annotated[str, Parameter(schema_extra={"invalid": "dummy"})]) -> Any:
+        return query1
+
+    # Success
+    app = Litestar([handler])
+    schema = app.openapi_schema.to_schema()
+    assert schema["paths"]["/"]["get"]["parameters"][0]["schema"]["not"] == {
+        "anyOf": [
+            {"type": "string", "pattern": r"^somePrefix:.*$"},
+            {"type": "string", "enum": ["denied", "values"]},
+        ]
+    }
+
+    # Attempt to pass invalid key
+    app = Litestar([error_handler])
+    with pytest.raises(ValueError) as e:
+        app.openapi_schema
+    assert str(e.value).startswith("`schema_extra` declares key")
+
+
 def test_uuid_path_description_generation() -> None:
     # https://github.com/litestar-org/litestar/issues/2967
     @get("str/{id:str}")
     async def str_path(id: Annotated[str, Parameter(description="String ID")]) -> str:
         return id
 
     @get("uuid/{id:uuid}")
```

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_path_item.py` & `litestar-2.8.0/tests/unit/test_openapi/test_path_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
+import dataclasses
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Callable, cast
+from unittest.mock import MagicMock
 
 import pytest
 from typing_extensions import TypeAlias
 
-from litestar import Controller, Litestar, Request, Router, delete, get
+from litestar import Controller, HttpMethod, Litestar, Request, Router, delete, get
 from litestar._openapi.datastructures import OpenAPIContext
-from litestar._openapi.path_item import PathItemFactory
+from litestar._openapi.path_item import PathItemFactory, merge_path_item_operations
 from litestar._openapi.utils import default_operation_id_creator
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.http_handlers import HTTPRouteHandler
 from litestar.openapi.config import OpenAPIConfig
-from litestar.openapi.spec import Operation
+from litestar.openapi.spec import Operation, PathItem
 from litestar.utils import find_index
 
 if TYPE_CHECKING:
     from litestar.routes import HTTPRoute
 
 
 @pytest.fixture()
@@ -211,7 +213,34 @@
     app = Litestar(route_handlers=[handler_1, handler_2])
     index = find_index(app.routes, lambda x: x.path_format == "/")
     route_with_multiple_methods = cast("HTTPRoute", app.routes[index])
     factory = create_factory(route_with_multiple_methods)
     schema = factory.create_path_item()
     assert schema.get
     assert schema.delete is None
+
+
+@pytest.mark.parametrize("method", HttpMethod)
+def test_merge_path_item_operations_operation_set_on_both_raises(method: HttpMethod) -> None:
+    with pytest.raises(ValueError, match="Cannot merge operation"):
+        merge_path_item_operations(
+            PathItem(**{method.value.lower(): MagicMock()}),
+            PathItem(**{method.value.lower(): MagicMock()}),
+            for_path="/",
+        )
+
+
+@pytest.mark.parametrize(
+    "attr",
+    [
+        f.name
+        for f in dataclasses.fields(PathItem)
+        if f.name.upper()
+        not in [
+            *HttpMethod,
+            "TRACE",  # remove once https://github.com/litestar-org/litestar/pull/3294 is merged
+        ]
+    ],
+)
+def test_merge_path_item_operation_differing_values_raises(attr: str) -> None:
+    with pytest.raises(ImproperlyConfiguredException, match="Conflicting OpenAPI path configuration for '/'"):
+        merge_path_item_operations(PathItem(), PathItem(**{attr: MagicMock()}), for_path="/")
```

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_request_body.py` & `litestar-2.8.0/tests/unit/test_openapi/test_request_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Type
 from unittest.mock import ANY, MagicMock
 
 import pytest
+from typing_extensions import Annotated
 
-from litestar import Controller, Litestar, post
+from litestar import Controller, Litestar, get, post
 from litestar._openapi.datastructures import OpenAPIContext
 from litestar._openapi.request_body import create_request_body
 from litestar.datastructures.upload_file import UploadFile
 from litestar.dto import AbstractDTO
 from litestar.enums import RequestEncodingType
 from litestar.handlers import BaseRouteHandler
 from litestar.openapi.config import OpenAPIConfig
@@ -52,14 +53,39 @@
         for route_handler, _ in route.route_handler_map.values():  # type: ignore[union-attr]
             handler_fields = route_handler.parsed_fn_signature.parameters
             if "data" in handler_fields:
                 request_body = create_request(route_handler, handler_fields["data"])
                 assert request_body
 
 
+def test_request_body_schema_extra() -> None:
+    @dataclass
+    class RequestBody:
+        foo: str
+
+    @get()
+    async def handler(
+        body1: Annotated[
+            RequestBody,
+            Body(
+                title="Default title",
+                schema_extra={
+                    "title": "Overridden title",
+                },
+            ),
+        ],
+    ) -> Any:
+        return body1
+
+    app = Litestar([handler])
+    schema = app.openapi_schema.to_schema()
+    resp = next(iter(schema["components"]["schemas"].values()))
+    assert resp["title"] == "Overridden title"
+
+
 def test_upload_single_file_schema_generation() -> None:
     @post(path="/file-upload")
     async def handle_file_upload(
         data: UploadFile = Body(media_type=RequestEncodingType.MULTI_PART),
     ) -> None:
         return None
```

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_responses.py` & `litestar-2.8.0/tests/unit/test_openapi/test_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_schema.py` & `litestar-2.8.0/tests/unit/test_openapi/test_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 
 import annotated_types
 import msgspec
 import pytest
 from msgspec import Struct
 from typing_extensions import Annotated, TypeAlias
 
-from litestar import Controller, MediaType, get
+from litestar import Controller, MediaType, get, post
 from litestar._openapi.schema_generation.plugins import openapi_schema_plugins
 from litestar._openapi.schema_generation.schema import (
     KWARG_DEFINITION_ATTRIBUTE_TO_OPENAPI_PROPERTY_MAP,
     SchemaCreator,
 )
 from litestar._openapi.schema_generation.utils import _get_normalized_schema_key, _type_or_first_not_none_inner_type
-from litestar.app import DEFAULT_OPENAPI_CONFIG
+from litestar.app import DEFAULT_OPENAPI_CONFIG, Litestar
 from litestar.di import Provide
 from litestar.enums import ParamType
 from litestar.openapi.spec import ExternalDocumentation, OpenAPIType, Reference
 from litestar.openapi.spec.example import Example
+from litestar.openapi.spec.parameter import Parameter as OpenAPIParameter
 from litestar.openapi.spec.schema import Schema
 from litestar.pagination import ClassicPagination, CursorPagination, OffsetPagination
-from litestar.params import Parameter, ParameterKwarg
+from litestar.params import KwargDefinition, Parameter, ParameterKwarg
 from litestar.testing import create_test_client
 from litestar.types.builtin_types import NoneType
 from litestar.typing import FieldDefinition
 from litestar.utils.helpers import get_name
 from tests.helpers import get_schema_for_field_definition
 from tests.models import DataclassPerson, DataclassPet
 
@@ -551,7 +552,56 @@
         FieldDefinition.from_kwarg(name="Lookup", annotation=Union[ModelA, ModelB, None])
     )
     assert schema.one_of == [
         Schema(type=OpenAPIType.NULL),
         Reference(ref="#/components/schemas/tests_unit_test_openapi_test_schema_test_type_union_with_none.ModelA"),
         Reference("#/components/schemas/tests_unit_test_openapi_test_schema_test_type_union_with_none.ModelB"),
     ]
+
+
+def test_default_only_on_field_definition() -> None:
+    field_definition = FieldDefinition.from_annotation(int, default=10)
+    assert field_definition.kwarg_definition is None
+
+    schema = get_schema_for_field_definition(field_definition)
+    assert schema.default == 10
+
+
+def test_default_not_provided_for_kwarg_but_for_field() -> None:
+    field_definition = FieldDefinition.from_annotation(int, default=10, kwarg_definition=KwargDefinition())
+    schema = get_schema_for_field_definition(field_definition)
+
+    assert schema.default == 10
+
+
+def test_routes_with_different_path_param_types_get_merged() -> None:
+    # https://github.com/litestar-org/litestar/issues/2700
+    @get("/{param:int}")
+    async def get_handler(param: int) -> None:
+        pass
+
+    @post("/{param:str}")
+    async def post_handler(param: str) -> None:
+        pass
+
+    app = Litestar([get_handler, post_handler])
+    assert app.openapi_schema.paths
+    paths = app.openapi_schema.paths["/{param}"]
+    assert paths.get is not None
+    assert paths.post is not None
+
+
+def test_unconsumed_path_parameters_are_documented() -> None:
+    # https://github.com/litestar-org/litestar/issues/3290
+    @get("/{param:str}")
+    async def handler() -> None:
+        pass
+
+    app = Litestar([handler])
+    params = app.openapi_schema.paths["/{param}"].get.parameters  # type: ignore[index, union-attr]
+    assert params
+    assert len(params) == 1
+    param = params[0]
+    assert isinstance(param, OpenAPIParameter)
+    assert param.name == "param"
+    assert param.required is True
+    assert param.param_in is ParamType.PATH
```

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_security_schemes.py` & `litestar-2.8.0/tests/unit/test_openapi/test_security_schemes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_spec_generation.py` & `litestar-2.8.0/tests/unit/test_openapi/test_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_tags.py` & `litestar-2.8.0/tests/unit/test_openapi/test_tags.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py` & `litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py` & `litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_plugins/test_base.py` & `litestar-2.8.0/tests/unit/test_plugins/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_plugins/test_sqlalchemy.py` & `litestar-2.8.0/tests/unit/test_plugins/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_repository/models_bigint.py` & `litestar-2.8.0/tests/unit/test_repository/models_bigint.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_repository/models_uuid.py` & `litestar-2.8.0/tests/unit/test_repository/models_uuid.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_repository/test_generic_mock_repository.py` & `litestar-2.8.0/tests/unit/test_repository/test_generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_base_response.py` & `litestar-2.8.0/tests/unit/test_response/test_base_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_file_response.py` & `litestar-2.8.0/tests/unit/test_response/test_file_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_redirect_response.py` & `litestar-2.8.0/tests/unit/test_response/test_redirect_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_response_cookies.py` & `litestar-2.8.0/tests/unit/test_response/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_response_headers.py` & `litestar-2.8.0/tests/unit/test_response/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_response_to_asgi_response.py` & `litestar-2.8.0/tests/unit/test_response/test_response_to_asgi_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_serialization.py` & `litestar-2.8.0/tests/unit/test_response/test_serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_sse.py` & `litestar-2.8.0/tests/unit/test_response/test_sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_streaming_response.py` & `litestar-2.8.0/tests/unit/test_response/test_streaming_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_type_decoders.py` & `litestar-2.8.0/tests/unit/test_response/test_type_decoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_response/test_type_encoders.py` & `litestar-2.8.0/tests/unit/test_response/test_type_encoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_security/test_security.py` & `litestar-2.8.0/tests/unit/test_security/test_security.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_security/test_session_auth.py` & `litestar-2.8.0/tests/unit/test_security/test_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_security/test_jwt/test_auth.py` & `litestar-2.8.0/tests/unit/test_security/test_jwt/test_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_security/test_jwt/test_integration.py` & `litestar-2.8.0/tests/unit/test_security/test_jwt/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_security/test_jwt/test_token.py` & `litestar-2.8.0/tests/unit/test_security/test_jwt/test_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_signature/test_parsing.py` & `litestar-2.8.0/tests/unit/test_signature/test_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_signature/test_validation.py` & `litestar-2.8.0/tests/unit/test_signature/test_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_static_files/conftest.py` & `litestar-2.8.0/tests/unit/test_static_files/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_static_files/test_create_static_router.py` & `litestar-2.8.0/tests/unit/test_static_files/test_create_static_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_static_files/test_file_serving_resolution.py` & `litestar-2.8.0/tests/unit/test_static_files/test_file_serving_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_static_files/test_html_mode.py` & `litestar-2.8.0/tests/unit/test_static_files/test_html_mode.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_static_files/test_static_files_validation.py` & `litestar-2.8.0/tests/unit/test_static_files/test_static_files_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_template/test_built_in.py` & `litestar-2.8.0/tests/unit/test_template/test_built_in.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_template/test_builtin_functions.py` & `litestar-2.8.0/tests/unit/test_template/test_builtin_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_template/test_context.py` & `litestar-2.8.0/tests/unit/test_template/test_context.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_template/test_csrf_token.py` & `litestar-2.8.0/tests/unit/test_template/test_csrf_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_template/test_template.py` & `litestar-2.8.0/tests/unit/test_template/test_template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_testing/test_lifespan_handler.py` & `litestar-2.8.0/tests/unit/test_testing/test_lifespan_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_testing/test_request_factory.py` & `litestar-2.8.0/tests/unit/test_testing/test_request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_testing/test_test_client.py` & `litestar-2.8.0/tests/unit/test_testing/test_test_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_types/test_protocols.py` & `litestar-2.8.0/tests/unit/test_types/test_protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_dataclass.py` & `litestar-2.8.0/tests/unit/test_utils/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_deprecation.py` & `litestar-2.8.0/tests/unit/test_utils/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_helpers.py` & `litestar-2.8.0/tests/unit/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_module_loader.py` & `litestar-2.8.0/tests/unit/test_utils/test_module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_path.py` & `litestar-2.8.0/tests/unit/test_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_predicates.py` & `litestar-2.8.0/tests/unit/test_utils/test_predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_scope.py` & `litestar-2.8.0/tests/unit/test_utils/test_scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_sequence.py` & `litestar-2.8.0/tests/unit/test_utils/test_sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_sync.py` & `litestar-2.8.0/tests/unit/test_utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/tests/unit/test_utils/test_version.py` & `litestar-2.8.0/tests/unit/test_utils/test_version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/LICENSE` & `litestar-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.7.1/README.md` & `litestar-2.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 - [OpenAPI 3.1 schema generation](#openapi)
 - [Life Cycle Hooks](#request-life-cycle-hooks)
 - [Route Guards based Authorization](#route-guards)
 - Support for `dataclasses`, `TypedDict`, [pydantic version 1 and version 2](https://docs.pydantic.dev/latest/),
   [msgspec](https://github.com/jcrist/msgspec) and [attrs](https://www.attrs.org/en/stable/)
 - Layered parameter declaration
 - [Automatic API documentation with](#redoc-swagger-ui-and-stoplight-elements-api-documentation):
+  - [Scalar](https://github.com/scalar/scalar/)
   - [RapiDoc](https://github.com/rapi-doc/RapiDoc)
   - [Redoc](https://github.com/Redocly/redoc)
   - [Stoplight Elements](https://github.com/stoplightio/elements)
   - [Swagger-UI](https://swagger.io/tools/swagger-ui/)
 - [Trio](https://trio.readthedocs.io/en/stable/) support (built-in, via [AnyIO](https://anyio.readthedocs.io/))
 - Ultra-fast validation, serialization and deserialization using [msgspec](https://github.com/jcrist/msgspec)
 - SQLAlchemy integration
@@ -124,18 +125,18 @@
 
 <a href="https://github.com/scalar/scalar/?utm_source=litestar&utm_medium=website&utm_campaign=main-badge" target="_blank" title="Scalar.com - Document, Discover and Test APIs with Scalar."><img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/sponsors/scalar.svg" width="180" alt="Scalar.com"></a>
 <a href="https://telemetrysports.com/" title="Telemetry Sports - Changing the way data influences the sports experience"><img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/sponsors/telemetry-sports/unofficial-telemetry-whitebg.svg" width="150" alt="Telemetry Sports"></a>
 <a href="https://www.stok.kr/" title="Stok - Stack Up Your Assets!"><img src="https://avatars.githubusercontent.com/u/144093421?s=400&v=4" width="150" alt="Stok"></a>
 
 <a href="https://docs.litestar.dev/dev/#sponsors" class="external-link" target="_blank">Check out our sponsors in the docs</a>
 
-If you would like to support the work that we do please consider [becoming a sponsor][sponsor-github]
-on [GitHub][sponsor-github] or [Open Collective][sponsor-oc].
+If you would like to support the work that we do please consider [becoming a sponsor][sponsor-polar]
+via [Polar.sh][sponsor-polar] (preferred), [GitHub][sponsor-github] or [Open Collective][sponsor-oc].
 
-We also participate in pledge-based sponsorship with [Polar][sponsor-polar].
+Also, exclusively with [Polar][sponsor-polar], you can engage in pledge-based sponsorships.
 
 [sponsor-github]: https://github.com/sponsors/litestar-org
 [sponsor-oc]: https://opencollective.com/litestar
 [sponsor-polar]: https://polar.sh/litestar-org
 
 ## Features
 
@@ -549,14 +550,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/hugovk"><img src="https://avatars.githubusercontent.com/u/1324225?v=4?s=100" width="100px;" alt="Hugo van Kemenade"/><br /><sub><b>Hugo van Kemenade</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=hugovk" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://error418.github.io"><img src="https://avatars.githubusercontent.com/u/7716544?v=4?s=100" width="100px;" alt="Michael Gerbig"/><br /><sub><b>Michael Gerbig</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=error418" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/crisog"><img src="https://avatars.githubusercontent.com/u/40803711?v=4?s=100" width="100px;" alt="CrisOG"/><br /><sub><b>CrisOG</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Acrisog" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/haryle"><img src="https://avatars.githubusercontent.com/u/64817481?v=4?s=100" width="100px;" alt="harryle"/><br /><sub><b>harryle</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Tests">⚠️</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.b-list.org/"><img src="https://avatars.githubusercontent.com/u/12384?v=4?s=100" width="100px;" alt="James Bennett"/><br /><sub><b>James Bennett</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Aubernostrum" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sherbang"><img src="https://avatars.githubusercontent.com/u/275015?v=4?s=100" width="100px;" alt="sherbang"/><br /><sub><b>sherbang</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sherbang" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/carlsmedstad"><img src="https://avatars.githubusercontent.com/u/6952324?v=4?s=100" width="100px;" alt="Carl Smedstad"/><br /><sub><b>Carl Smedstad</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=carlsmedstad" title="Tests">⚠️</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.7.1/pyproject.toml` & `litestar-2.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,26 @@
   "rich>=13.0.0",
   "rich-click",
 ]
 description = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 keywords = ["api", "rest", "asgi", "litestar", "starlite"]
 license = {text = "MIT"}
 maintainers = [
-  {name = "Cody Fincher", email = "cody.fincher@gmail.com"},
-  {name = "Jacob Coffee", email = "jacob@z7x.org"},
-  {name = "Janek Nouvertné", email = "provinzkraut@posteo.de"},
-  {name = "Peter Schutt", email = "peter.github@proton.me"},
+  {name = "Litestar Developers", email = "hello@litestar.dev"},
+  {name = "Cody Fincher", email = "cody@litestar.dev"},
+  {name = "Jacob Coffee", email = "jacob@litestar.dev"},
+  {name = "Janek Nouvertné", email = "provinzkraut@litestar.dev"},
+  {name = "Peter Schutt", email = "peter@litestar.dev"},
+  {name = "Visakh Unnikrishnan", email = "guacs@litestar.dev"},
+  {name = "Alc", email = "alc@litestar.dev"}
 ]
 name = "litestar"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
-version = "2.7.1"
+version = "2.8.0"
 
 [project.urls]
 Blog = "https://blog.litestar.dev"
 Changelog = "https://github.com/litestar-org/litestar/releases/"
 Discord = "https://discord.gg/litestar-919193495116337154"
 Documentation = "https://docs.litestar.dev/"
 Homepage = "https://litestar.dev/"
@@ -85,15 +88,15 @@
 minijinja = ["minijinja>=1.0.0"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
 piccolo = ["piccolo"]
 picologging = ["picologging"]
 prometheus = ["prometheus-client"]
 pydantic = ["pydantic", "email-validator", "pydantic-extra-types"]
 redis = ["redis[hiredis]>=4.4.4"]
-sqlalchemy = ["advanced-alchemy>=0.2.2,<1.0.0"]
+sqlalchemy = ["advanced-alchemy>=0.2.2,<0.9.0"]
 standard = ["jinja2", "jsbeautifier", "uvicorn[standard]", "uvloop>=0.18.0; sys_platform != 'win32'", "fast-query-parsers>=1.0.2"]
 structlog = ["structlog"]
 
 [project.scripts]
 litestar = "litestar.__main__:run_cli"
 
 [tool.hatch.metadata]
@@ -127,45 +130,45 @@
   "psycopg2-binary",
   "psutil>=5.9.8",
   "hypercorn>=0.16.0",
   "daphne>=4.0.0",
 ]
 dev-contrib = ["opentelemetry-sdk", "httpx-sse"]
 docs = [
-  "sphinx>=7.1.2",
-  "sphinx-autobuild>=2021.3.14",
-  "sphinx-copybutton>=0.5.2",
-  "sphinx-toolbox>=3.5.0",
-  "sphinx-design>=0.5.0",
-  "sphinx-click>=4.4.0",
-  "sphinxcontrib-mermaid>=0.9.2",
-  "auto-pytabs[sphinx]>=0.4.0",
-  "litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git",
+    "sphinx>=7.1.2",
+    "sphinx-autobuild>=2021.3.14",
+    "sphinx-copybutton>=0.5.2",
+    "sphinx-toolbox>=3.5.0",
+    "sphinx-design>=0.5.0",
+    "sphinx-click>=4.4.0",
+    "sphinxcontrib-mermaid>=0.9.2",
+    "auto-pytabs[sphinx]>=0.4.0",
+    "litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git",
+    "sphinx-paramlinks>=0.6.0",
 ]
 linting = [
   "ruff>=0.2.1",
   "mypy",
   "pre-commit",
   "slotscheck",
   "codecov-cli",
   "pyright==1.1.344",
   "asyncpg-stubs",
   "types-beautifulsoup4",
-  "types-pytest-lazy-fixture",
   "types-python-jose",
   "types-pyyaml",
   "types-redis",
   "types-psutil",
 ]
 test = [
   "covdefaults",
   "pytest<8.0.0",
   "pytest-asyncio",
   "pytest-cov",
-  "pytest-lazy-fixture",
+  "pytest-lazy-fixtures",
   "pytest-mock",
   "pytest-rerunfailures",
   "pytest-timeout",
   "pytest-xdist",
   "time-machine",
 ]
 
@@ -281,14 +284,20 @@
 ]
 include = ["litestar", "tests"]
 pythonVersion = "3.8"
 reportUnnecessaryTypeIgnoreComments = true
 
 [tool.slotscheck]
 strict-imports = false
+exclude-classes = """
+(
+  # github.com/python/cpython/pull/106771
+  (^litestar.events.emitter:BaseEventEmitterBackend)
+)
+"""
 
 [tool.ruff]
 lint.select = [
   "A", # flake8-builtins
   "B", # flake8-bugbear
   "BLE", # flake8-blind-except
   "C4", # flake8-comprehensions
@@ -400,14 +409,15 @@
   "SIM",
   "TCH",
   "TRY",
 ]
 "tests/unit/test_contrib/test_sqlalchemy/**/*.*" = ["UP006"]
 "tools/**/*.*" = ["D", "ARG", "EM", "TRY", "G", "FBT"]
 "tools/prepare_release.py" = ["S603", "S607"]
+"tests/unit/test_openapi/test_typescript_converter/test_converter.py" = ["W293"]
 
 [tool.ruff.format]
 docstring-code-format = true
 docstring-code-line-length = 88
 
 [tool.unasyncd]
 add_editors_note = true
```

### Comparing `litestar-2.7.1/PKG-INFO` & `litestar-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: litestar
-Version: 2.7.1
+Version: 2.8.0
 Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Project-URL: Blog, https://blog.litestar.dev
 Project-URL: Changelog, https://github.com/litestar-org/litestar/releases/
 Project-URL: Discord, https://discord.gg/litestar-919193495116337154
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Homepage, https://litestar.dev/
 Project-URL: Issue Tracker, https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Project-URL: Reddit, https://www.reddit.com/r/LitestarAPI
 Project-URL: Repository, https://github.com/litestar-org/litestar
 Project-URL: Twitter, https://twitter.com/LitestarAPI
 Author-email: Cody Fincher <cody.fincher@gmail.com>, Jacob Coffee <jacob@z7x.org>, Janek Nouvertné <provinzkraut@posteo.de>, Na'aman Hirschfeld <nhirschfeld@gmail.com>, Peter Schutt <peter.github@proton.me>
-Maintainer-email: Cody Fincher <cody.fincher@gmail.com>, Jacob Coffee <jacob@z7x.org>, Janek Nouvertné <provinzkraut@posteo.de>, Peter Schutt <peter.github@proton.me>
+Maintainer-email: Litestar Developers <hello@litestar.dev>, Cody Fincher <cody@litestar.dev>, Jacob Coffee <jacob@litestar.dev>, Janek Nouvertné <provinzkraut@litestar.dev>, Peter Schutt <peter@litestar.dev>, Visakh Unnikrishnan <guacs@litestar.dev>, Alc <alc@litestar.dev>
 License: MIT
 License-File: LICENSE
 Keywords: api,asgi,litestar,rest,starlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -86,15 +86,15 @@
 Provides-Extra: pydantic
 Requires-Dist: email-validator; extra == 'pydantic'
 Requires-Dist: pydantic; extra == 'pydantic'
 Requires-Dist: pydantic-extra-types; extra == 'pydantic'
 Provides-Extra: redis
 Requires-Dist: redis[hiredis]>=4.4.4; extra == 'redis'
 Provides-Extra: sqlalchemy
-Requires-Dist: advanced-alchemy<1.0.0,>=0.2.2; extra == 'sqlalchemy'
+Requires-Dist: advanced-alchemy<0.9.0,>=0.2.2; extra == 'sqlalchemy'
 Provides-Extra: standard
 Requires-Dist: fast-query-parsers>=1.0.2; extra == 'standard'
 Requires-Dist: jinja2; extra == 'standard'
 Requires-Dist: jsbeautifier; extra == 'standard'
 Requires-Dist: uvicorn[standard]; extra == 'standard'
 Requires-Dist: uvloop>=0.18.0; (sys_platform != 'win32') and extra == 'standard'
 Provides-Extra: structlog
@@ -189,14 +189,15 @@
 - [OpenAPI 3.1 schema generation](#openapi)
 - [Life Cycle Hooks](#request-life-cycle-hooks)
 - [Route Guards based Authorization](#route-guards)
 - Support for `dataclasses`, `TypedDict`, [pydantic version 1 and version 2](https://docs.pydantic.dev/latest/),
   [msgspec](https://github.com/jcrist/msgspec) and [attrs](https://www.attrs.org/en/stable/)
 - Layered parameter declaration
 - [Automatic API documentation with](#redoc-swagger-ui-and-stoplight-elements-api-documentation):
+  - [Scalar](https://github.com/scalar/scalar/)
   - [RapiDoc](https://github.com/rapi-doc/RapiDoc)
   - [Redoc](https://github.com/Redocly/redoc)
   - [Stoplight Elements](https://github.com/stoplightio/elements)
   - [Swagger-UI](https://swagger.io/tools/swagger-ui/)
 - [Trio](https://trio.readthedocs.io/en/stable/) support (built-in, via [AnyIO](https://anyio.readthedocs.io/))
 - Ultra-fast validation, serialization and deserialization using [msgspec](https://github.com/jcrist/msgspec)
 - SQLAlchemy integration
@@ -227,18 +228,18 @@
 
 <a href="https://github.com/scalar/scalar/?utm_source=litestar&utm_medium=website&utm_campaign=main-badge" target="_blank" title="Scalar.com - Document, Discover and Test APIs with Scalar."><img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/sponsors/scalar.svg" width="180" alt="Scalar.com"></a>
 <a href="https://telemetrysports.com/" title="Telemetry Sports - Changing the way data influences the sports experience"><img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/sponsors/telemetry-sports/unofficial-telemetry-whitebg.svg" width="150" alt="Telemetry Sports"></a>
 <a href="https://www.stok.kr/" title="Stok - Stack Up Your Assets!"><img src="https://avatars.githubusercontent.com/u/144093421?s=400&v=4" width="150" alt="Stok"></a>
 
 <a href="https://docs.litestar.dev/dev/#sponsors" class="external-link" target="_blank">Check out our sponsors in the docs</a>
 
-If you would like to support the work that we do please consider [becoming a sponsor][sponsor-github]
-on [GitHub][sponsor-github] or [Open Collective][sponsor-oc].
+If you would like to support the work that we do please consider [becoming a sponsor][sponsor-polar]
+via [Polar.sh][sponsor-polar] (preferred), [GitHub][sponsor-github] or [Open Collective][sponsor-oc].
 
-We also participate in pledge-based sponsorship with [Polar][sponsor-polar].
+Also, exclusively with [Polar][sponsor-polar], you can engage in pledge-based sponsorships.
 
 [sponsor-github]: https://github.com/sponsors/litestar-org
 [sponsor-oc]: https://opencollective.com/litestar
 [sponsor-polar]: https://polar.sh/litestar-org
 
 ## Features
 
@@ -652,14 +653,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/hugovk"><img src="https://avatars.githubusercontent.com/u/1324225?v=4?s=100" width="100px;" alt="Hugo van Kemenade"/><br /><sub><b>Hugo van Kemenade</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=hugovk" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://error418.github.io"><img src="https://avatars.githubusercontent.com/u/7716544?v=4?s=100" width="100px;" alt="Michael Gerbig"/><br /><sub><b>Michael Gerbig</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=error418" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/crisog"><img src="https://avatars.githubusercontent.com/u/40803711?v=4?s=100" width="100px;" alt="CrisOG"/><br /><sub><b>CrisOG</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Acrisog" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/haryle"><img src="https://avatars.githubusercontent.com/u/64817481?v=4?s=100" width="100px;" alt="harryle"/><br /><sub><b>harryle</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Tests">⚠️</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.b-list.org/"><img src="https://avatars.githubusercontent.com/u/12384?v=4?s=100" width="100px;" alt="James Bennett"/><br /><sub><b>James Bennett</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Aubernostrum" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sherbang"><img src="https://avatars.githubusercontent.com/u/275015?v=4?s=100" width="100px;" alt="sherbang"/><br /><sub><b>sherbang</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sherbang" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/carlsmedstad"><img src="https://avatars.githubusercontent.com/u/6952324?v=4?s=100" width="100px;" alt="Carl Smedstad"/><br /><sub><b>Carl Smedstad</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=carlsmedstad" title="Tests">⚠️</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

