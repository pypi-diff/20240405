# Comparing `tmp/mountaineer-0.3.2.dev3.tar.gz` & `tmp/mountaineer-0.3.2.dev4.tar.gz`

## Comparing `mountaineer-0.3.2.dev3.tar` & `mountaineer-0.3.2.dev4.tar`

### file list

```diff
@@ -1,258 +1,259 @@
--rw-r--r--   0     1001      127      269 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src_go/build.rs
--rw-r--r--   0     1001      127     5657 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src_go/go.sum
--rw-r--r--   0     1001      127     5750 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src_go/src/lib.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.3.2.dev3/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.gitattributes
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/README.md
--rw-r--r--   0     1001      127    14036 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/poetry.lock
--rw-r--r--   0     1001      127      759 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    19767 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3404 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/.gitignore
--rw-r--r--   0     1001      127     1750 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/LICENSE
--rw-r--r--   0     1001      127     4976 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/Makefile
--rw-r--r--   0     1001      127    14891 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/README.md
--rw-r--r--   0     1001      127      105 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127093 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      775 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      559 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127       59 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   107805 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     7904 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1925 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      190 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      137 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3373 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    61104 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1214 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127       30 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      310 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127       61 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127       80 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9375 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/database.md
--rw-r--r--   0     1001      127     4667 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12265 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     4080 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1823 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/poetry.lock
--rw-r--r--   0     1001      127      479 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/media/header.png
--rw-r--r--   0     1001      127      954 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     7884 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9707 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/actions/test_passthrough.py
--rw-r--r--   0     1001      127     9074 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/actions/test_sideeffect.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    12132 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     3474 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127     8065 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     5001 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4153 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2799 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127     1236 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     8602 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5281 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127      494 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6571 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     3239 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127     8419 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2565 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      397 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12321 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6835 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/actions/passthrough.py
--rw-r--r--   0     1001      127    11635 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/actions/sideeffect.py
--rw-r--r--   0     1001      127     4352 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    18916 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/cache.py
--rw-r--r--   0     1001      127    18059 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/cli.py
--rw-r--r--   0     1001      127    10656 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     3958 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127     9737 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    28180 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127     9820 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     3317 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     2424 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/config.py
--rw-r--r--   0     1001      127       40 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/constants.py
--rw-r--r--   0     1001      127    14854 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/controller.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3188 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1188 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    15443 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     1975 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/logging.py
--rw-r--r--   0     1001      127    12599 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/render.py
--rw-r--r--   0     1001      127     3228 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6299 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     5942 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8378 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/watch.py
--rw-r--r--   0     1001      127     3087 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/watch_server.py
--rw-r--r--   0     1001      127      866 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/mountaineer/webservice.py
--rw-r--r--   0     1001      127   123447 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/lexers.rs
--rw-r--r--   0     1001      127     8366 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-04-03 00:25:12.000000 mountaineer-0.3.2.dev3/src/timeout.rs
--rw-r--r--   0     1001      127    32093 2024-04-03 00:25:35.000000 mountaineer-0.3.2.dev3/Cargo.lock
--rw-r--r--   0     1001      127     1502 2024-04-03 00:25:27.000000 mountaineer-0.3.2.dev3/pyproject.toml
--rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.3.2.dev3/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src_go/build.rs
+-rw-r--r--   0     1001      127     5657 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src_go/go.sum
+-rw-r--r--   0     1001      127     5750 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.3.2.dev4/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    14036 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    19767 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3404 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/LICENSE
+-rw-r--r--   0     1001      127     4976 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/Makefile
+-rw-r--r--   0     1001      127    14891 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/README.md
+-rw-r--r--   0     1001      127      105 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127093 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      775 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      489 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      559 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       59 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   107805 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      724 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     7904 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1925 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      190 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      137 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3373 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    61104 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1214 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127       30 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      310 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127       61 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4677 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12265 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     4080 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      479 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/media/header.png
+-rw-r--r--   0     1001      127      954 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     7884 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9707 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/actions/test_passthrough.py
+-rw-r--r--   0     1001      127     9074 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/actions/test_sideeffect.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    12565 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     3474 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127     8065 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     5001 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4153 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127     1236 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127     8602 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5281 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      494 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6571 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     3239 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127     1924 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8419 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2565 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      397 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12321 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6835 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/actions/passthrough.py
+-rw-r--r--   0     1001      127    11635 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/actions/sideeffect.py
+-rw-r--r--   0     1001      127     4352 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    18916 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/cache.py
+-rw-r--r--   0     1001      127    18059 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/cli.py
+-rw-r--r--   0     1001      127    10826 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     3958 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127     9737 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    28180 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127     9899 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     3317 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     2424 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/config.py
+-rw-r--r--   0     1001      127       40 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/constants.py
+-rw-r--r--   0     1001      127    14854 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/controller.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1188 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    15443 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2039 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/logging.py
+-rw-r--r--   0     1001      127    12599 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/render.py
+-rw-r--r--   0     1001      127     3228 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6299 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8378 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/watch.py
+-rw-r--r--   0     1001      127     3087 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127      866 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   124933 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/lexers.rs
+-rw-r--r--   0     1001      127     8366 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-04-05 15:05:46.000000 mountaineer-0.3.2.dev4/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-04-05 15:06:06.000000 mountaineer-0.3.2.dev4/Cargo.lock
+-rw-r--r--   0     1001      127     1607 2024-04-05 15:06:02.000000 mountaineer-0.3.2.dev4/pyproject.toml
+-rw-r--r--   0        0        0    15354 1970-01-01 00:00:00.000000 mountaineer-0.3.2.dev4/PKG-INFO
```

### Comparing `mountaineer-0.3.2.dev3/src_go/build.rs` & `mountaineer-0.3.2.dev4/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src_go/go/js_build.go` & `mountaineer-0.3.2.dev4/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src_go/src/lib.rs` & `mountaineer-0.3.2.dev4/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/Cargo.toml` & `mountaineer-0.3.2.dev4/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.3.2-dev3"
+version = "0.3.2-dev4"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.3.2.dev3/.github/poetry.lock` & `mountaineer-0.3.2.dev4/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/.github/pyproject.toml` & `mountaineer-0.3.2.dev4/.github/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "scripts"
 version = "0.1.0"
 description = ""
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
-readme = "README.md"
+readme = "README_SCRIPTS.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 packaging = "^24.0"
 toml = "^0.10.2"
```

### Comparing `mountaineer-0.3.2.dev3/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.3.2.dev4/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/.github/scripts/check_dependencies.py` & `mountaineer-0.3.2.dev4/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/.github/scripts/update_version.py` & `mountaineer-0.3.2.dev4/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/.github/workflows/publish_docs.yml` & `mountaineer-0.3.2.dev4/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/.github/workflows/test.yml` & `mountaineer-0.3.2.dev4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/.gitignore` & `mountaineer-0.3.2.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/Dockerfile` & `mountaineer-0.3.2.dev4/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/LICENSE` & `mountaineer-0.3.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/Makefile` & `mountaineer-0.3.2.dev4/Makefile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/README.md` & `mountaineer-0.3.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/benchmarking/poetry.lock` & `mountaineer-0.3.2.dev4/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/README.md` & `mountaineer-0.3.2.dev4/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/app.py` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.3.2.dev4/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/poetry.lock` & `mountaineer-0.3.2.dev4/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/ci_webapp/pyproject.toml` & `mountaineer-0.3.2.dev4/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/README.md` & `mountaineer-0.3.2.dev4/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.3.2.dev4/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/poetry.lock` & `mountaineer-0.3.2.dev4/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/create_mountaineer_app/pyproject.toml` & `mountaineer-0.3.2.dev4/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/client_actions.md` & `mountaineer-0.3.2.dev4/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/cma.md` & `mountaineer-0.3.2.dev4/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/database.md` & `mountaineer-0.3.2.dev4/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/deploy.md` & `mountaineer-0.3.2.dev4/docs_website/docs/deploy.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 This page contains a reasonable default configuration to get you started. We make heavy use of multi-stage builds to cache dependencies and minimize the size of your final image that your webservers will have to pull down.
 
 ## Docker
 
 First, add the following to your `.dockerignore` file. This will prevent Docker from trying to copy over heavy artifacts that aren't needed for the build.
 
 ```title=".dockerignore"
-node_modules
-_server
-_ssr
-_static
+**/node_modules
+**/_server
+**/_ssr
+**/_static
 ```
 
 ### Image 1: Frontend Dependencies
 
 Our first stage uses `npm` to fetch your frontend dependencies. This is an isolated context since it's the only place we need node / npm in the build pipeline.
 
 ```docker
@@ -99,16 +99,15 @@
 USER appuser
 
 ENV PATH="/venv/bin:$PATH"
 
 WORKDIR /usr/src/app
 
 COPY --from=venv-dependencies /venv /venv
-COPY {my_webapp} ./{my_webapp}
-COPY --from=server-hooks-builder /usr/src/app/{my_webapp}/views/_* ./{my_webapp}/views/
+COPY --from=server-hooks-builder /usr/src/app/{my_webapp}/views /venv/lib/python3.11/site-packages/{my_webapp}/views
 
 # Run the application
 CMD ["/venv/bin/uvicorn", "{my_webapp}.main:app", "--host", "0.0.0.0", "--port", "3000"]
 ```
 
 ## Common Errors
```

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/error_handling.md` & `mountaineer-0.3.2.dev4/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/index.md` & `mountaineer-0.3.2.dev4/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/internal/core_library.md` & `mountaineer-0.3.2.dev4/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/links.md` & `mountaineer-0.3.2.dev4/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.3.2.dev4/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.3.2.dev4/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/media/network_debug.png` & `mountaineer-0.3.2.dev4/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.3.2.dev4/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/metadata.md` & `mountaineer-0.3.2.dev4/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/postcss.md` & `mountaineer-0.3.2.dev4/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/quickstart.md` & `mountaineer-0.3.2.dev4/docs_website/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/static_analysis.md` & `mountaineer-0.3.2.dev4/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/structure.md` & `mountaineer-0.3.2.dev4/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.3.2.dev4/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/docs/views.md` & `mountaineer-0.3.2.dev4/docs_website/docs/views.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/mkdocs.yml` & `mountaineer-0.3.2.dev4/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/docs_website/poetry.lock` & `mountaineer-0.3.2.dev4/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/media/header.png` & `mountaineer-0.3.2.dev4/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__init__.py` & `mountaineer-0.3.2.dev4/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/actions/test_fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/actions/test_passthrough.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/actions/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/actions/test_sideeffect.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/actions/test_sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,24 +154,33 @@
                         schema_ref=OpenAPIProperty.from_meta(
                             title="",
                             variable_type=OpenAPISchemaType.STRING,
                         ),
                         in_location=ParameterLocationType.QUERY,
                         required=True,
                     ),
-                    # Cookies should be skipped
+                    # Cookies and headers should be skipped
                     URLParameterDefinition.from_meta(
                         name="auth_cookie",
                         schema_ref=OpenAPIProperty.from_meta(
                             title="",
                             variable_type=OpenAPISchemaType.STRING,
                         ),
                         in_location=ParameterLocationType.COOKIE,
                         required=True,
                     ),
+                    URLParameterDefinition.from_meta(
+                        name="auth_header",
+                        schema_ref=OpenAPIProperty.from_meta(
+                            title="",
+                            variable_type=OpenAPISchemaType.STRING,
+                        ),
+                        in_location=ParameterLocationType.HEADER,
+                        required=True,
+                    ),
                     # Optional query parameter
                     URLParameterDefinition.from_meta(
                         name="query_param_optional_id",
                         schema_ref=OpenAPIProperty.from_meta(
                             title="",
                             variable_type=OpenAPISchemaType.STRING,
                         ),
```

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     SourceMapParser,
     SourceMapSchema,
 )
 from mountaineer.test_utilities import benchmark_function
 
 
 @pytest.mark.asyncio
-@benchmark_function(0.2)
+@benchmark_function(0.2, time_budget_seconds=10)
 async def test_parse_source_map_parse(
     start_timing,
     end_timing,
 ):
     parser = SourceMapParser(get_fixture_path("home_controller_source_map.js.map"))
     start_timing()
     parser.parse()
```

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_app.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_cache.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_cli.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_controller.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_paths.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/__tests__/test_watch.py` & `mountaineer-0.3.2.dev4/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/actions/fields.py` & `mountaineer-0.3.2.dev4/mountaineer/actions/fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/actions/passthrough.py` & `mountaineer-0.3.2.dev4/mountaineer/actions/passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/actions/sideeffect.py` & `mountaineer-0.3.2.dev4/mountaineer/actions/sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/annotation_helpers.py` & `mountaineer-0.3.2.dev4/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/app.py` & `mountaineer-0.3.2.dev4/mountaineer/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/cache.py` & `mountaineer-0.3.2.dev4/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/cli.py` & `mountaineer-0.3.2.dev4/mountaineer/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/client_builder/build_actions.py` & `mountaineer-0.3.2.dev4/mountaineer/client_builder/build_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,18 @@
     def build_action_parameters(self, action: ActionDefinition):
         parameters_dict: dict[Any, Any] = {}
         typehint_dict: dict[Any, Any] = {}
         request_types: list[str] = []
 
         for parameter in action.parameters:
             typehint_key, typehint_value = get_typehint_for_parameter(parameter)
-            if parameter.in_location == ParameterLocationType.COOKIE:
+            if parameter.in_location in {
+                ParameterLocationType.COOKIE,
+                ParameterLocationType.HEADER,
+            }:
                 continue
             parameters_dict[parameter.name] = TSLiteral(parameter.name)
             typehint_dict[typehint_key] = typehint_value
 
         if (
             action.requestBody is not None
             and action.requestBody.content_schema.schema_ref.ref
@@ -178,15 +181,18 @@
 
         if action.parameters:
             for parameter in action.parameters:
                 if parameter.in_location == ParameterLocationType.PATH:
                     common_params["path"][parameter.name] = TSLiteral(parameter.name)
                 elif parameter.in_location == ParameterLocationType.QUERY:
                     common_params["query"][parameter.name] = TSLiteral(parameter.name)
-                elif parameter.in_location == ParameterLocationType.COOKIE:
+                elif parameter.in_location in {
+                    ParameterLocationType.COOKIE,
+                    ParameterLocationType.HEADER,
+                }:
                     # No-op, cookies will be sent automatically by fetch()
                     continue
                 else:
                     raise NotImplementedError(
                         f"Parameter location {parameter.in_location} not supported"
                     )
```

### Comparing `mountaineer-0.3.2.dev3/mountaineer/client_builder/build_links.py` & `mountaineer-0.3.2.dev4/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.3.2.dev4/mountaineer/client_builder/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/client_builder/builder.py` & `mountaineer-0.3.2.dev4/mountaineer/client_builder/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/client_builder/openapi.py` & `mountaineer-0.3.2.dev4/mountaineer/client_builder/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,21 @@
     BOOLEAN = "boolean"
     ARRAY = "array"
     # Typically used to indicate an optional type within an anyOf statement
     NULL = "null"
 
 
 class ParameterLocationType(StrEnum):
+    # https://swagger.io/specification: Parameter Object
     PATH = "path"
     QUERY = "query"
 
     # https://swagger.io/docs/specification/authentication/cookie-authentication/
     COOKIE = "cookie"
+    HEADER = "header"
 
 
 class ActionType(StrEnum):
     GET = "get"
     POST = "post"
     PUT = "put"
     PATCH = "patch"
```

### Comparing `mountaineer-0.3.2.dev3/mountaineer/client_builder/typescript.py` & `mountaineer-0.3.2.dev4/mountaineer/client_builder/typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/config.py` & `mountaineer-0.3.2.dev4/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/controller.py` & `mountaineer-0.3.2.dev4/mountaineer/controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/controllers/exception_controller.py` & `mountaineer-0.3.2.dev4/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/cropper.py` & `mountaineer-0.3.2.dev4/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/database/cli.py` & `mountaineer-0.3.2.dev4/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/database/config.py` & `mountaineer-0.3.2.dev4/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/database/dependencies/core.py` & `mountaineer-0.3.2.dev4/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/database/sqlmodel.py` & `mountaineer-0.3.2.dev4/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/database/validator.py` & `mountaineer-0.3.2.dev4/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/dependencies/base.py` & `mountaineer-0.3.2.dev4/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/dependencies/core/core.py` & `mountaineer-0.3.2.dev4/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/exceptions.py` & `mountaineer-0.3.2.dev4/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/io.py` & `mountaineer-0.3.2.dev4/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/js_compiler/base.py` & `mountaineer-0.3.2.dev4/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/js_compiler/javascript.py` & `mountaineer-0.3.2.dev4/mountaineer/js_compiler/javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/js_compiler/postcss.py` & `mountaineer-0.3.2.dev4/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.3.2.dev4/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/logging.py` & `mountaineer-0.3.2.dev4/mountaineer/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class JsonFormatter(Formatter):
     def format(self, record):
         log_record = {
             "level": record.levelname,
             "name": record.name,
+            "timestamp": self.formatTime(record, self.datefmt),
             "message": record.getMessage(),
         }
         if record.exc_info:
             log_record["exception"] = self.formatException(record.exc_info)
         return json_dumps(log_record)
```

### Comparing `mountaineer-0.3.2.dev3/mountaineer/paths.py` & `mountaineer-0.3.2.dev4/mountaineer/paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/render.py` & `mountaineer-0.3.2.dev4/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/ssr.py` & `mountaineer-0.3.2.dev4/mountaineer/ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/static/api.ts` & `mountaineer-0.3.2.dev4/mountaineer/static/api.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/static/live_reload.ts` & `mountaineer-0.3.2.dev4/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/test_utilities.py` & `mountaineer-0.3.2.dev4/mountaineer/test_utilities.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """
 Utilities for client unit and integration tests
 """
 from functools import wraps
 from inspect import isawaitable, iscoroutinefunction, signature
 from tempfile import NamedTemporaryFile
 from time import monotonic_ns
+from typing import Any
 
 import pytest
 from sqlalchemy import text
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.ext.asyncio import AsyncEngine
 
 from mountaineer.database import SQLModel
 from mountaineer.logging import LOGGER
 
 
 class ExecutionTooLong(Exception):
     pass
 
 
-def benchmark_function(max_time_seconds: int | float):
+def benchmark_function(
+    max_time_seconds: int | float, time_budget_seconds: int | float = 5
+):
     """
     Wrap test functions in a timer that will enforce that the core logic completes
     in less than `max_time_seconds` seconds. Injects `start_timing` and `end_timing` into
     the function kwargs that will be called. Client callers should call these to scope
     where they want us to measure the core logic.
 
+    :param time_budget_seconds: How many seconds we have to run benchmarking. This function will run
+      at least 1 benchmark always, but the time budget allows users to better calibrate benchmark duration
+      by taking the average of multiple runs.
+
     """
     import pyinstrument
 
     def wrapper_fn(test_func):
         # We want to remove our custom functions from the signature, since pytest will natively
         # try to inject fixtures in this place
         orig_sig = signature(test_func)
@@ -44,57 +51,81 @@
         # pytest.mark.asyncio), otherwise we should raise an error because pytest won't know how
         # to run it
         if not iscoroutinefunction(test_func):
             raise Exception(
                 f"Test function {test_func.__name__} is not a coroutine function. Please decorate it with pytest.mark.asyncio"
             )
 
-        @wraps(test_func)
-        async def wrapper(*args, **kwargs):
-            bound = new_sig.bind(*args, **kwargs)
-            bound.apply_defaults()
-
+        async def single_time_test(fn, *args, **kwargs):
             # Try to run the test function regularly, and time it
-            # Instrumenting profilers at this point typically will slow down execution time
+            # Instrumenting profilers typically will slow down execution time so we want
+            # to take time of the raw, non-instrumented function for benchmarking
             start: float | None = None
             end: float | None = None
 
             def start_timing():
                 nonlocal start
                 start = monotonic_ns()
 
             def end_timing():
                 nonlocal end
                 end = monotonic_ns()
 
-            try:
-                result = test_func(
-                    *args, **kwargs, start_timing=start_timing, end_timing=end_timing
-                )
-                if isawaitable(result):
-                    result = await result
+            result = test_func(
+                *args, **kwargs, start_timing=start_timing, end_timing=end_timing
+            )
+            if isawaitable(result):
+                result = await result
+
+            return (start, end, result)
+
+        @wraps(test_func)
+        async def wrapper(*args, **kwargs):
+            bound = new_sig.bind(*args, **kwargs)
+            bound.apply_defaults()
 
-                if start is None:
-                    raise Exception("Test function did not call start_timing")
-                if end is None:
-                    raise Exception("Test function did not call end_timing")
+            average_duration: float | None = None
 
-                LOGGER.info(f"Test function took: {(end - start) / 1e9}")
+            try:
+                timed_durations: list[tuple[int, int]] = []
+                results: list[Any] = []
+                global_start = monotonic_ns()
+
+                while monotonic_ns() - global_start < time_budget_seconds * 1e9:
+                    start, end, result = await single_time_test(
+                        test_func, *args, **kwargs
+                    )
+
+                    if start is None:
+                        raise Exception("Test function did not call start_timing")
+                    if end is None:
+                        raise Exception("Test function did not call end_timing")
+
+                    timed_durations.append((start, end))
+                    results.append(result)
+
+                average_duration = sum(
+                    (end - start) for start, end in timed_durations
+                ) / len(timed_durations)
+
+                LOGGER.info(
+                    f"Collected {len(results)} timed durations in {(monotonic_ns() - global_start) / 1e9}"
+                )
+                LOGGER.info(f"Test function took average: {average_duration / 1e9}")
 
-                if (end - start) / 1e9 > max_time_seconds:
+                if average_duration / 1e9 > max_time_seconds:
                     raise ExecutionTooLong()
 
-                return result
+                return results[0]
 
             except ExecutionTooLong as e:
                 LOGGER.error(f"Test function failed due to: {e}")
 
                 # This should already be true, but we want to be explicit to help mypy
-                assert start is not None
-                assert end is not None
+                assert average_duration is not None
 
                 profiler = pyinstrument.Profiler()
                 output_filename: str | None = None
 
                 def start_timing():
                     nonlocal profiler
                     profiler.start()
@@ -111,15 +142,15 @@
                 result = test_func(
                     *args, **kwargs, start_timing=start_timing, end_timing=end_timing
                 )
                 if isawaitable(result):
                     await result
 
                 pytest.fail(
-                    f"Test function failed in {end-start}s and profiles generated; Pyinstrument: {output_filename}"
+                    f"Test function failed in {average_duration/1e9}s and profiles generated; Pyinstrument: {output_filename}"
                 )
 
         wrapper.__signature__ = new_sig  # type: ignore
         return wrapper
 
     return wrapper_fn
```

### Comparing `mountaineer-0.3.2.dev3/mountaineer/views/package-lock.json` & `mountaineer-0.3.2.dev4/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/watch.py` & `mountaineer-0.3.2.dev4/mountaineer/watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/watch_server.py` & `mountaineer-0.3.2.dev4/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/mountaineer/webservice.py` & `mountaineer-0.3.2.dev4/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/poetry.lock` & `mountaineer-0.3.2.dev4/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is automatically @generated by Poetry 1.7.1 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
 
 [[package]]
 name = "annotated-types"
 version = "0.6.0"
 description = "Reusable constraint types to use with typing.Annotated"
 optional = false
 python-versions = ">=3.8"
@@ -684,21 +684,21 @@
 docs = ["furo (==2021.6.18b36)", "myst-parser (==0.15.1)", "sphinx (==4.2.0)", "sphinxcontrib-programoutput (==0.17)"]
 examples = ["django", "numpy"]
 test = ["flaky", "greenlet (>=3.0.0a1)", "ipython", "pytest", "pytest-asyncio (==0.12.0)", "sphinx-autobuild (==2021.3.14)", "trio"]
 types = ["typing-extensions"]
 
 [[package]]
 name = "pyright"
-version = "1.1.352"
+version = "1.1.357"
 description = "Command line wrapper for pyright"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pyright-1.1.352-py3-none-any.whl", hash = "sha256:0040cf173c6a60704e553bfd129dfe54de59cc76d0b2b80f77cfab4f50701d64"},
-    {file = "pyright-1.1.352.tar.gz", hash = "sha256:a621c0dfbcf1291b3610641a07380fefaa1d0e182890a1b2a7f13b446e8109a9"},
+    {file = "pyright-1.1.357-py3-none-any.whl", hash = "sha256:1cf29ee38e4928131895cd8e90eef37b5b77e2ed72a14e6e8e2405266f5f0aca"},
+    {file = "pyright-1.1.357.tar.gz", hash = "sha256:7c66261116c78c5fa9629134fe85c54cc5302ab73e376be4b0a99d89c80a9403"},
 ]
 
 [package.dependencies]
 nodeenv = ">=1.6.0"
 
 [package.extras]
 all = ["twine (>=3.4.1)"]
@@ -777,14 +777,15 @@
     {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc"},
     {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673"},
     {file = "PyYAML-6.0.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b"},
     {file = "PyYAML-6.0.1-cp311-cp311-win32.whl", hash = "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741"},
     {file = "PyYAML-6.0.1-cp311-cp311-win_amd64.whl", hash = "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34"},
     {file = "PyYAML-6.0.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28"},
     {file = "PyYAML-6.0.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9"},
+    {file = "PyYAML-6.0.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef"},
     {file = "PyYAML-6.0.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0"},
     {file = "PyYAML-6.0.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4"},
     {file = "PyYAML-6.0.1-cp312-cp312-win32.whl", hash = "sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54"},
     {file = "PyYAML-6.0.1-cp312-cp312-win_amd64.whl", hash = "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df"},
     {file = "PyYAML-6.0.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47"},
     {file = "PyYAML-6.0.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98"},
     {file = "PyYAML-6.0.1-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c"},
@@ -873,15 +874,17 @@
 version = "2.0.26"
 description = "Database Abstraction Library"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "SQLAlchemy-2.0.26-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:56524d767713054f8758217b3a811f6a736e0ae34e7afc33b594926589aa9609"},
     {file = "SQLAlchemy-2.0.26-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c2d8a2c68b279617f13088bdc0fc0e9b5126f8017f8882ff08ee41909fab0713"},
+    {file = "SQLAlchemy-2.0.26-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:84d377645913d47f0dc802b415bcfe7fb085d86646a12278d77c12eb75b5e1b4"},
     {file = "SQLAlchemy-2.0.26-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4fc0628d2026926404dabc903dc5628f7d936a792aa3a1fc54a20182df8e2172"},
+    {file = "SQLAlchemy-2.0.26-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:872f2907ade52601a1e729e85d16913c24dc1f6e7c57d11739f18dcfafde29db"},
     {file = "SQLAlchemy-2.0.26-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:ba46fa770578b3cf3b5b77dadb7e94fda7692dd4d1989268ef3dcb65f31c40a3"},
     {file = "SQLAlchemy-2.0.26-cp310-cp310-win32.whl", hash = "sha256:651d10fdba7984bf100222d6e4acc496fec46493262b6170be1981ef860c6184"},
     {file = "SQLAlchemy-2.0.26-cp310-cp310-win_amd64.whl", hash = "sha256:8f95ede696ab0d7328862d69f29b643d35b668c4f3619cb2f0281adc16e64c1b"},
     {file = "SQLAlchemy-2.0.26-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:fab1bb909bd24accf2024a69edd4f885ded182c079c4dbcd515b4842f86b07cb"},
     {file = "SQLAlchemy-2.0.26-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b7ee16afd083bb6bb5ab3962ac7f0eafd1d196c6399388af35fef3d1c6d6d9bb"},
     {file = "SQLAlchemy-2.0.26-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:379af901ceb524cbee5e15c1713bf9fd71dc28053286b7917525d01b938b9628"},
     {file = "SQLAlchemy-2.0.26-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:94a78f56ea13f4d6e9efcd2a2d08cc13531918e0516563f6303c4ad98c81e21d"},
@@ -894,27 +897,33 @@
     {file = "SQLAlchemy-2.0.26-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5901eed6d0e23ca4b04d66a561799d4f0fe55fcbfc7ca203bb8c3277f442085b"},
     {file = "SQLAlchemy-2.0.26-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d25fe55aab9b20ae4a9523bb269074202be9d92a145fcc0b752fff409754b5f6"},
     {file = "SQLAlchemy-2.0.26-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:5310958d08b4bafc311052be42a3b7d61a93a2bf126ddde07b85f712e7e4ac7b"},
     {file = "SQLAlchemy-2.0.26-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:fd133afb7e6c59fad365ffa97fb06b1001f88e29e1de351bef3d2b1224e2f132"},
     {file = "SQLAlchemy-2.0.26-cp312-cp312-win32.whl", hash = "sha256:dc32ecf643c4904dd413e6a95a3f2c8a89ccd6f15083e586dcf8f42eb4e317ae"},
     {file = "SQLAlchemy-2.0.26-cp312-cp312-win_amd64.whl", hash = "sha256:6e25f029e8ad6d893538b5abe8537e7f09e21d8e96caee46a7e2199f3ddd77b0"},
     {file = "SQLAlchemy-2.0.26-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:99a9a8204b8937aa72421e31c493bfc12fd063a8310a0522e5a9b98e6323977c"},
+    {file = "SQLAlchemy-2.0.26-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:691d68a4fca30c9a676623d094b600797699530e175b6524a9f57e3273f5fa8d"},
     {file = "SQLAlchemy-2.0.26-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:79a74a4ca4310c812f97bf0f13ce00ed73c890954b5a20b32484a9ab60e567e9"},
+    {file = "SQLAlchemy-2.0.26-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:f2efbbeb18c0e1c53b670a46a009fbde7b58e05b397a808c7e598532b17c6f4b"},
     {file = "SQLAlchemy-2.0.26-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3fc557f5402206c18ec3d288422f8e5fa764306d49f4efbc6090a7407bf54938"},
     {file = "SQLAlchemy-2.0.26-cp37-cp37m-win32.whl", hash = "sha256:a9846ffee3283cff4ec476e7ee289314290fcb2384aab5045c6f481c5c4d011f"},
     {file = "SQLAlchemy-2.0.26-cp37-cp37m-win_amd64.whl", hash = "sha256:ed4667d3d5d6e203a271d684d5b213ebcd618f7a8bc605752a8865eb9e67a79a"},
     {file = "SQLAlchemy-2.0.26-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:79e629df3f69f849a1482a2d063596b23e32036b83547397e68725e6e0d0a9ab"},
     {file = "SQLAlchemy-2.0.26-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4b4d848b095173e0a9e377127b814490499e55f5168f617ae2c07653c326b9d1"},
+    {file = "SQLAlchemy-2.0.26-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3f06afe8e96d7f221cc0b59334dc400151be22f432785e895e37030579d253c3"},
     {file = "SQLAlchemy-2.0.26-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f75ac12d302205e60f77f46bd162d40dc37438f1f8db160d2491a78b19a0bd61"},
+    {file = "SQLAlchemy-2.0.26-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:ec3717c1efee8ad4b97f6211978351de3abe1e4b5f73e32f775c7becec021c5c"},
     {file = "SQLAlchemy-2.0.26-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:06ed4d6bb2365222fb9b0a05478a2d23ad8c1dd874047a9ae1ca1d45f18a255e"},
     {file = "SQLAlchemy-2.0.26-cp38-cp38-win32.whl", hash = "sha256:caa79a6caeb4a3cc4ddb9aba9205c383f5d3bcb60d814e87e74570514754e073"},
     {file = "SQLAlchemy-2.0.26-cp38-cp38-win_amd64.whl", hash = "sha256:996b41c38e34a980e9f810d6e2709a3196e29ee34e46e3c16f96c63da10a9da1"},
     {file = "SQLAlchemy-2.0.26-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4f57af0866f6629eae2d24d022ba1a4c1bac9b16d45027bbfcda4c9d5b0d8f26"},
     {file = "SQLAlchemy-2.0.26-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e1a532bc33163fb19c4759a36504a23e63032bc8d47cee1c66b0b70a04a0957b"},
+    {file = "SQLAlchemy-2.0.26-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:02a4f954ccb17bd8cff56662efc806c5301508233dc38d0253a5fdb2f33ca3ba"},
     {file = "SQLAlchemy-2.0.26-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a678f728fb075e74aaa7fdc27f8af8f03f82d02e7419362cc8c2a605c16a4114"},
+    {file = "SQLAlchemy-2.0.26-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:8b39462c9588d4780f041e1b84d2ba038ac01c441c961bbee622dd8f53dec69f"},
     {file = "SQLAlchemy-2.0.26-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:98f4d0d2bda2921af5b0c2ca99207cdab00f2922da46a6336c62c8d6814303a7"},
     {file = "SQLAlchemy-2.0.26-cp39-cp39-win32.whl", hash = "sha256:6d68e6b507a3dd20c0add86ac0a0ca061d43c9a0162a122baa5fe952f14240f1"},
     {file = "SQLAlchemy-2.0.26-cp39-cp39-win_amd64.whl", hash = "sha256:fb97a9b93b953084692a52a7877957b7a88dfcedc0c5652124f5aebf5999f7fe"},
     {file = "SQLAlchemy-2.0.26-py3-none-any.whl", hash = "sha256:1128b2cdf49107659f6d1f452695f43a20694cc9305a86e97b70793a1c74eeb4"},
     {file = "SQLAlchemy-2.0.26.tar.gz", hash = "sha256:e1bcd8fcb30305e27355d553608c2c229d3e589fb7ff406da7d7e5d50fa14d0d"},
 ]
```

### Comparing `mountaineer-0.3.2.dev3/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.3.2.dev4/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.3.2.dev4/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/benches/lexers_benchmark.rs` & `mountaineer-0.3.2.dev4/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/benches/source_map_benchmark.rs` & `mountaineer-0.3.2.dev4/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/benches/ssr_benchmark.rs` & `mountaineer-0.3.2.dev4/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/lexers.rs` & `mountaineer-0.3.2.dev4/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/lib.rs` & `mountaineer-0.3.2.dev4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/logging.rs` & `mountaineer-0.3.2.dev4/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/source_map.rs` & `mountaineer-0.3.2.dev4/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/ssr.rs` & `mountaineer-0.3.2.dev4/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/src/timeout.rs` & `mountaineer-0.3.2.dev4/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.3.2.dev3/Cargo.lock` & `mountaineer-0.3.2.dev4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.3.2-dev3"
+version = "0.3.2-dev4"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.3.2.dev3/pyproject.toml` & `mountaineer-0.3.2.dev4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = [ "maturin>=1.3.0",]
 build-backend = "maturin"
 
 [project]
 name = "mountaineer"
 dependencies = [ "pydantic", "fastapi", "inflection", "click", "tqdm", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]",]
+exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.3.2.dev3"
+version = "0.3.2.dev4"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
```

### Comparing `mountaineer-0.3.2.dev3/PKG-INFO` & `mountaineer-0.3.2.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.3.2.dev3
+Version: 0.3.2.dev4
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: tqdm
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
```

