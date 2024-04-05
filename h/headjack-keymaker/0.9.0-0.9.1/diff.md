# Comparing `tmp/headjack_keymaker-0.9.0.tar.gz` & `tmp/headjack_keymaker-0.9.1.tar.gz`

## Comparing `headjack_keymaker-0.9.0.tar` & `headjack_keymaker-0.9.1.tar`

### file list

```diff
@@ -1,391 +1,391 @@
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.gitmodules
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/Makefile
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/netlify.toml
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.github/workflows/python-checks.yml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.pdm-build/.gitignore
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.pdm-build/keymaker.pth
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/.hugo_build.lock
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/README.md
--rwxr-xr-x   0        0        0     1065 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/build-docs.sh
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/archetypes/default.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/assets/jsconfig.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/assets/scss/_bootstrap-variables.scss
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/config/_default/config.toml
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/accessing-completions-chat-model/index.md
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/advanced-usage-and-customization/index.md
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/constraints/index.md
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/contributing/index.md
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/formatting-and-control-flow/index.md
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/getting-started/index.md
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/models/index.md
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/docs/streaming-and-decoding/index.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/0.1.0/posts/theme-doc/post.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/content/versions/_index.md
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/layouts/index.html
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/layouts/_default/baseof.html
--rw-r--r--   0        0        0   101153 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.content
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.json
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/favicon.png
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/css/termynal.css
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/images/discord.svg
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/images/github-mark.svg
--rw-r--r--   0        0        0    25173 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/images/keymaker-logo.png
--rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/images/keymaker-logo.svg
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/images/keymaker-logo.webp
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/static/js/termynal.js
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.eslintrc.js
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.git
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.gitignore
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/CHANGELOG.md
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/LICENSE
--rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/README.md
--rw-r--r--   0        0        0     9755 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/README.zh-cn.md
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/SECURITY.md
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/dependencies.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/go.mod
--rw-r--r--   0        0        0   324863 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/package-lock.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/package.json
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/tailwind.config.js
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/theme.toml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/FUNDING.yml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/dependabot.yml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/release.yml
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/Lighthouse-CI.yml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/build.yml
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/pages.yml
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/update-algolia-search-index.yml
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/update-dependencies.yml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/archetypes/default.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_custom.scss
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_override.scss
--rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_variables.scss
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/color.css
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/main.css
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/style.scss
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/tailwind.css
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_core/_base.scss
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_core/_layout.scss
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_core/_media.scss
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_mixin/_blur.scss
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_mixin/_compatibility.scss
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_mixin/_index.scss
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_mixin/_link.scss
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_404.scss
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_archive.scss
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_home.scss
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_index.scss
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_single.scss
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_special.scss
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_taxonomy.scss
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_cookieconsent.scss
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_details.scss
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_fixed-button.scss
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_footer.scss
--rw-r--r--   0        0        0    10501 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_header.scss
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_icon.scss
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_mask.scss
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_pagination.scss
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_archive/_tags.scss
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_archive/_terms.scss
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_admonition.scss
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_bilibili.scss
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_code.scss
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_comment.scss
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_echarts.scss
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_footer.scss
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_friend.scss
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_katex.scss
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_mapbox.scss
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_mermaid.scss
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_music.scss
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_related.scss
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_series.scss
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_showcase.scss
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_sponsor.scss
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_toc.scss
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/polyfill.yml
--rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/social.yml
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/cdn/jsdelivr.yml
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/apple.yml
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/facebook.yml
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/google.yml
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/twitter.yml
--rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/images/avatar.webp
--rw-r--r--   0        0        0     8137 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/sw.js
--rw-r--r--   0        0        0    31061 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/theme.js
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/aplayer.js
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/artalk.js
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/clipboard.js
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/cookieconsent.js
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/echarts.js
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/katex.js
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/tablesort.js
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/twemoji.js
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/twikoo.js
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/valine.js
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/shims/waline.js
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/version.template.svg
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/bilibili.svg
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/qq.svg
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/qqGroup.svg
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/thingiverse.svg
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/schema.json
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/css/_custom.scss
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/css/_override.scss
--rw-r--r--   0        0        0   119992 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/Apple-Devices-Preview.webp
--rw-r--r--   0        0        0    92580 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/Wavelength.webp
--rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/avatar.webp
--rw-r--r--   0        0        0   206162 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse-large.webp
--rw-r--r--   0        0        0    21426 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse-small.webp
--rw-r--r--   0        0        0   107566 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse.webp
--rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/screenshot.webp
--rw-r--r--   0        0        0  4365824 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/music/Wavelength.mp3
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/author.toml
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/hugo.en.toml
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/hugo.toml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/hugo.zh-cn.toml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/markup.toml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/mediaTypes.toml
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/menu.en.toml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/menu.zh-cn.toml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/outputFormats.toml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/outputs.toml
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/params.en.toml
--rw-r--r--   0        0        0    22046 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/params.toml
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/params.zh-cn.toml
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/permalinks.toml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/privacy.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/sitemap.toml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/taxonomies.toml
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/about/index.en.md
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/about/index.zh-cn.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/authors/_index.en.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/authors/_index.zh-cn.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/categories/documentation/_index.en.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/categories/documentation/_index.zh-cn.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/offline/index.en.md
--rw-r--r--   0        0        0    95094 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/featured-image.webp
--rw-r--r--   0        0        0    19622 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.en.md
--rw-r--r--   0        0        0    19577 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.zh-cn.md
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/featured-image.webp
--rw-r--r--   0        0        0    53734 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.en.md
--rw-r--r--   0        0        0    55712 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.zh-cn.md
--rw-r--r--   0        0        0    23755 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.en.md
--rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.zh-cn.md
--rw-r--r--   0        0        0    15844 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Install-PWA.webp
--rw-r--r--   0        0        0   249830 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Installed-PWA.webp
--rw-r--r--   0        0        0    15168 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/featured-image.webp
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.en.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.zh-cn.md
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/aplayer-tests/index.en.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/author-fallback-tests/index.en.md
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/author-single-tests/index.en.md
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/bilibili-tests/index.en.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/builtin-shortcodes-tests/index.en.md
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/echarts-tests/index.en.md
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/extend-shortcodes-tests/index.en.md
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/friend-link-tests/index.en.md
--rw-r--r--   0        0        0    52218 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/katex-tests/index.en.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/mapbox-tests/index.en.md
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/markdown-tests/index.en.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/mermaid-tests/index.en.md
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/music-tests/index.en.md
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/related-tests/index.en.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/series-taxonomy-tests/index.en.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/series-taxonomy-tests/index.zh-cn.md
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/showcase-tests/index.en.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/toc-tests/index.en.md
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/typeit-tests/index.en.md
--rw-r--r--   0        0        0   112108 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.webp
--rw-r--r--   0        0        0   140344 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.zh-cn.webp
--rw-r--r--   0        0        0   160484 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.webp
--rw-r--r--   0        0        0   172518 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.zh-cn.webp
--rw-r--r--   0        0        0   227870 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/featured-image.webp
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.en.md
--rw-r--r--   0        0        0    41867 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.zh-cn.md
--rw-r--r--   0        0        0   286589 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/language-switch.gif
--rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/featured-image.webp
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.en.md
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.zh-cn.md
--rw-r--r--   0        0        0    95672 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/featured-image.webp
--rw-r--r--   0        0        0    18785 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.en.md
--rw-r--r--   0        0        0    17488 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.zh-cn.md
--rw-r--r--   0        0        0   211304 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.webp
--rw-r--r--   0        0        0   200238 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.zh-cn.webp
--rw-r--r--   0        0        0    20254 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image-preview.webp
--rw-r--r--   0        0        0    27100 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image.webp
--rw-r--r--   0        0        0    40347 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.en.md
--rw-r--r--   0        0        0    38472 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.zh-cn.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/_index.en.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/_index.zh-cn.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/getting-start/_index.en.md
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/getting-start/_index.zh-cn.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/how-to-doit/_index.en.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/how-to-doit/_index.zh-cn.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/test-series/_index.en.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/series/test-series/_index.zh-cn.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/showcase/index.en.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/showcase/index.zh-cn.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/tags/configuration/_index.en.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/tags/configuration/_index.zh-cn.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/tags/content/_index.en.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/tags/content/_index.zh-cn.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/tags/installation/_index.en.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/tags/installation/_index.zh-cn.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/data/authors/Dillon.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/data/authors/PCloud.toml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/_redirects
--rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/android-chrome-192x192.png
--rw-r--r--   0        0        0    48161 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/android-chrome-512x512.png
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/apple-touch-icon.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/browserconfig.xml
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/favicon-16x16.png
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/favicon-32x32.png
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/favicon.ico
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/mstile-150x150.png
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/safari-pinned-tab.svg
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/site.webmanifest
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ar.toml
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ca.toml
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/de.toml
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/en.toml
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/es.toml
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/fr.toml
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/hi.toml
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/id.toml
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/it.toml
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ko.toml
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/pl.toml
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/pt-BR.toml
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/pt-PT.toml
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ro.toml
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ru.toml
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/sr.toml
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/te.toml
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/th.toml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/tr.toml
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/uk.toml
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/vi.toml
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/zh-CN.toml
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/zh-TW.toml
--rw-r--r--   0        0        0   493975 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/images/screenshot.png
--rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/images/tn.png
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/404.html
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/index.html
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/index.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/index.rss.xml
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/robots.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/sitemap.xml
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/baseof.html
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/section.html
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/single.html
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/single.md
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/summary.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/_markup/render-codeblock-mermaid.html
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/_markup/render-heading.html
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/_markup/render-image.html
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/_markup/render-link.html
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/assets.html
--rw-r--r--   0        0        0    25678 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/comment.html
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/footer.html
--rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/header.html
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/init.html
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/paginator.html
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/recentlyUpdated.html
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/related.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/author.html
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/checkbox.html
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/content.html
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/escape.html
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/fontawesome.html
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/fraction.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/getRemoteImage.html
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/id.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/path.html
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/resource.html
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/ruby.html
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/suffixValidation.html
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/head/link.html
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/head/meta.html
--rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/head/seo.html
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/home/profile.html
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/meta/author.html
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/analytics.html
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/compatibility.html
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/icon.html
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/image.html
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/link.html
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/script.html
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/share.html
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/social.html
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/style.html
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/rss/item.html
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/scratch/commentScript.html
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/scratch/configScript.html
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/scratch/script.html
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/scratch/style.html
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/single/footer.html
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/single/outdatedArticleReminder.html
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/single/sponsor.html
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/posts/rss.xml
--rw-r--r--   0        0        0    12543 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/posts/single.html
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/admonition.html
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/aplayer.html
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/audio.html
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/bilibili.html
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/echarts.html
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/friend.html
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/image.html
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/link.html
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/mapbox.html
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/math.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/mermaid.html
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/music.html
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/script.html
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/showcase.html
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/style.html
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/typeit.html
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/version.html
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/taxonomy/list.html
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/taxonomy/rss.xml
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/taxonomy/terms.html
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/__about__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/__init__.py
--rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/prompt.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/types.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/__init__.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/base.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/json.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/logical.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/model.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/options.py
--rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/parser.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/regex.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/constraints/stops.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/models/__init__.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/models/base.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/models/huggingface.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/models/litellm.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/models/llama_cpp.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/models/openai.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/utils/__init__.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/utils/chat.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/utils/exceptions.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/utils/formatted_completion.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/keymaker/utils/general.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/tests/constraints/test_options.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/tests/constraints/test_regex.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/.gitignore
--rw-r--r--   0        0        0    41865 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/README.md
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    42885 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.gitmodules
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/Makefile
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/netlify.toml
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.github/workflows/python-checks.yml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.pdm-build/.gitignore
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.pdm-build/keymaker.pth
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.pdm-build/keymaker-0.1.0+editable.dist-info/WHEEL
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/.hugo_build.lock
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/README.md
+-rwxr-xr-x   0        0        0     1065 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/build-docs.sh
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/archetypes/default.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/assets/jsconfig.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/assets/scss/_bootstrap-variables.scss
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/config/_default/config.toml
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/accessing-completions-chat-model/index.md
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/advanced-usage-and-customization/index.md
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/constraints/index.md
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/contributing/index.md
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/formatting-and-control-flow/index.md
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/getting-started/index.md
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/models/index.md
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/docs/streaming-and-decoding/index.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/0.1.0/posts/theme-doc/post.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/content/versions/_index.md
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/layouts/index.html
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/layouts/_default/baseof.html
+-rw-r--r--   0        0        0   101153 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.content
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.json
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/favicon.png
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/css/termynal.css
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/images/discord.svg
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/images/github-mark.svg
+-rw-r--r--   0        0        0    25173 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/images/keymaker-logo.png
+-rw-r--r--   0        0        0    28606 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/images/keymaker-logo.svg
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/images/keymaker-logo.webp
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/static/js/termynal.js
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.eslintrc.js
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.git
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.gitignore
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/CHANGELOG.md
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/LICENSE
+-rw-r--r--   0        0        0    10485 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/README.md
+-rw-r--r--   0        0        0     9755 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/README.zh-cn.md
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/SECURITY.md
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/dependencies.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/go.mod
+-rw-r--r--   0        0        0   324863 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/package-lock.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/package.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/tailwind.config.js
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/theme.toml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/FUNDING.yml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/dependabot.yml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/release.yml
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/Lighthouse-CI.yml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/pages.yml
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/update-algolia-search-index.yml
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/update-dependencies.yml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/archetypes/default.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_custom.scss
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_override.scss
+-rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_variables.scss
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/color.css
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/main.css
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/style.scss
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/tailwind.css
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_core/_base.scss
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_core/_layout.scss
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_core/_media.scss
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_mixin/_blur.scss
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_mixin/_compatibility.scss
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_mixin/_index.scss
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_mixin/_link.scss
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_404.scss
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_archive.scss
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_home.scss
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_index.scss
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_single.scss
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_special.scss
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_taxonomy.scss
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_cookieconsent.scss
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_details.scss
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_fixed-button.scss
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_footer.scss
+-rw-r--r--   0        0        0    10501 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_header.scss
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_icon.scss
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_mask.scss
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_pagination.scss
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_archive/_tags.scss
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_archive/_terms.scss
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_admonition.scss
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_bilibili.scss
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_code.scss
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_comment.scss
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_echarts.scss
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_footer.scss
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_friend.scss
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_katex.scss
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_mapbox.scss
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_mermaid.scss
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_music.scss
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_related.scss
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_series.scss
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_showcase.scss
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_sponsor.scss
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_toc.scss
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/polyfill.yml
+-rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/social.yml
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/cdn/jsdelivr.yml
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/apple.yml
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/facebook.yml
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/google.yml
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/twitter.yml
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/images/avatar.webp
+-rw-r--r--   0        0        0     8137 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/sw.js
+-rw-r--r--   0        0        0    31061 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/theme.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/aplayer.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/artalk.js
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/clipboard.js
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/cookieconsent.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/echarts.js
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/katex.js
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/tablesort.js
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/twemoji.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/twikoo.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/valine.js
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/shims/waline.js
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/version.template.svg
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/bilibili.svg
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/qq.svg
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/qqGroup.svg
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/thingiverse.svg
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/schema.json
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/css/_custom.scss
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/css/_override.scss
+-rw-r--r--   0        0        0   119992 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/Apple-Devices-Preview.webp
+-rw-r--r--   0        0        0    92580 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/Wavelength.webp
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/avatar.webp
+-rw-r--r--   0        0        0   206162 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/lighthouse-large.webp
+-rw-r--r--   0        0        0    21426 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/lighthouse-small.webp
+-rw-r--r--   0        0        0   107566 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/lighthouse.webp
+-rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/screenshot.webp
+-rw-r--r--   0        0        0  4365824 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/music/Wavelength.mp3
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/author.toml
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/hugo.en.toml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/hugo.toml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/hugo.zh-cn.toml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/markup.toml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/mediaTypes.toml
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/menu.en.toml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/menu.zh-cn.toml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/outputFormats.toml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/outputs.toml
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/params.en.toml
+-rw-r--r--   0        0        0    22046 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/params.toml
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/params.zh-cn.toml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/permalinks.toml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/privacy.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/sitemap.toml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/taxonomies.toml
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/about/index.en.md
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/about/index.zh-cn.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/authors/_index.en.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/authors/_index.zh-cn.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/categories/documentation/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/categories/documentation/_index.zh-cn.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/offline/index.en.md
+-rw-r--r--   0        0        0    95094 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/featured-image.webp
+-rw-r--r--   0        0        0    19622 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.en.md
+-rw-r--r--   0        0        0    19577 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.zh-cn.md
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/emoji-support/featured-image.webp
+-rw-r--r--   0        0        0    53734 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.en.md
+-rw-r--r--   0        0        0    55712 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.zh-cn.md
+-rw-r--r--   0        0        0    23755 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.en.md
+-rw-r--r--   0        0        0    23600 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.zh-cn.md
+-rw-r--r--   0        0        0    15844 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Install-PWA.webp
+-rw-r--r--   0        0        0   249830 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Installed-PWA.webp
+-rw-r--r--   0        0        0    15168 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/featured-image.webp
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.en.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.zh-cn.md
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/aplayer-tests/index.en.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/author-fallback-tests/index.en.md
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/author-single-tests/index.en.md
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/bilibili-tests/index.en.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/builtin-shortcodes-tests/index.en.md
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/echarts-tests/index.en.md
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/extend-shortcodes-tests/index.en.md
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/friend-link-tests/index.en.md
+-rw-r--r--   0        0        0    52218 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/katex-tests/index.en.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/mapbox-tests/index.en.md
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/markdown-tests/index.en.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/mermaid-tests/index.en.md
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/music-tests/index.en.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/related-tests/index.en.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/series-taxonomy-tests/index.en.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/series-taxonomy-tests/index.zh-cn.md
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/showcase-tests/index.en.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/toc-tests/index.en.md
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/typeit-tests/index.en.md
+-rw-r--r--   0        0        0   112108 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.webp
+-rw-r--r--   0        0        0   140344 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.zh-cn.webp
+-rw-r--r--   0        0        0   160484 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.webp
+-rw-r--r--   0        0        0   172518 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.zh-cn.webp
+-rw-r--r--   0        0        0   227870 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/featured-image.webp
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.en.md
+-rw-r--r--   0        0        0    41867 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.zh-cn.md
+-rw-r--r--   0        0        0   286589 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/language-switch.gif
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/featured-image.webp
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.en.md
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.zh-cn.md
+-rw-r--r--   0        0        0    95672 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/featured-image.webp
+-rw-r--r--   0        0        0    18785 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.en.md
+-rw-r--r--   0        0        0    17488 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.zh-cn.md
+-rw-r--r--   0        0        0   211304 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.webp
+-rw-r--r--   0        0        0   200238 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.zh-cn.webp
+-rw-r--r--   0        0        0    20254 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image-preview.webp
+-rw-r--r--   0        0        0    27100 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image.webp
+-rw-r--r--   0        0        0    40347 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.en.md
+-rw-r--r--   0        0        0    38472 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.zh-cn.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/_index.en.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/_index.zh-cn.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/getting-start/_index.en.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/getting-start/_index.zh-cn.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/how-to-doit/_index.en.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/how-to-doit/_index.zh-cn.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/test-series/_index.en.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/series/test-series/_index.zh-cn.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/showcase/index.en.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/showcase/index.zh-cn.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/tags/configuration/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/tags/configuration/_index.zh-cn.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/tags/content/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/tags/content/_index.zh-cn.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/tags/installation/_index.en.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/tags/installation/_index.zh-cn.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/data/authors/Dillon.toml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/data/authors/PCloud.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/_redirects
+-rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0    48161 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/apple-touch-icon.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/browserconfig.xml
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/favicon-16x16.png
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/favicon.ico
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/mstile-150x150.png
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/site.webmanifest
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ar.toml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ca.toml
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/de.toml
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/en.toml
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/es.toml
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/fr.toml
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/hi.toml
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/id.toml
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/it.toml
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ko.toml
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/pl.toml
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/pt-BR.toml
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/pt-PT.toml
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ro.toml
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ru.toml
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/sr.toml
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/te.toml
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/th.toml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/tr.toml
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/uk.toml
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/vi.toml
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/zh-CN.toml
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/zh-TW.toml
+-rw-r--r--   0        0        0   493975 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/images/screenshot.png
+-rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/images/tn.png
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/404.html
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/index.html
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/index.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/index.rss.xml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/robots.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/sitemap.xml
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/baseof.html
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/section.html
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/single.html
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/single.md
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/summary.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/_markup/render-codeblock-mermaid.html
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/_markup/render-heading.html
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/_markup/render-image.html
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/_markup/render-link.html
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/assets.html
+-rw-r--r--   0        0        0    25678 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/comment.html
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/footer.html
+-rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/header.html
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/init.html
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/paginator.html
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/recentlyUpdated.html
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/related.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/author.html
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/checkbox.html
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/content.html
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/escape.html
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/fontawesome.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/fraction.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/getRemoteImage.html
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/id.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/path.html
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/resource.html
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/ruby.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/suffixValidation.html
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/head/link.html
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/head/meta.html
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/head/seo.html
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/home/profile.html
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/meta/author.html
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/analytics.html
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/compatibility.html
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/icon.html
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/image.html
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/link.html
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/script.html
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/share.html
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/social.html
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/style.html
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/rss/item.html
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/scratch/commentScript.html
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/scratch/configScript.html
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/scratch/script.html
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/scratch/style.html
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/single/footer.html
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/single/outdatedArticleReminder.html
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/single/sponsor.html
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/posts/rss.xml
+-rw-r--r--   0        0        0    12543 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/posts/single.html
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/admonition.html
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/aplayer.html
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/audio.html
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/bilibili.html
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/echarts.html
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/friend.html
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/image.html
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/link.html
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/mapbox.html
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/math.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/mermaid.html
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/music.html
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/script.html
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/showcase.html
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/style.html
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/typeit.html
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/version.html
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/taxonomy/list.html
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/taxonomy/rss.xml
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/taxonomy/terms.html
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/__about__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/__init__.py
+-rw-r--r--   0        0        0    20712 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/prompt.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/types.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/__init__.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/base.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/json.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/logical.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/model.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/options.py
+-rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/parser.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/regex.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/constraints/stops.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/models/__init__.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/models/base.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/models/huggingface.py
+-rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/models/litellm.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/models/llama_cpp.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/models/openai.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/utils/__init__.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/utils/chat.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/utils/exceptions.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/utils/formatted_completion.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/keymaker/utils/general.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/tests/constraints/test_options.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/tests/constraints/test_regex.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/.gitignore
+-rw-r--r--   0        0        0    41865 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/README.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    42885 2020-02-02 00:00:00.000000 headjack_keymaker-0.9.1/PKG-INFO
```

### Comparing `headjack_keymaker-0.9.0/.pre-commit-config.yaml` & `headjack_keymaker-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/.github/workflows/python-checks.yml` & `headjack_keymaker-0.9.1/.github/workflows/python-checks.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA` & `headjack_keymaker-0.9.1/.pdm-build/keymaker-0.1.0+editable.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/build-docs.sh` & `headjack_keymaker-0.9.1/docs/build-docs.sh`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/assets/scss/_bootstrap-variables.scss` & `headjack_keymaker-0.9.1/docs/assets/scss/_bootstrap-variables.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/config/_default/config.toml` & `headjack_keymaker-0.9.1/docs/config/_default/config.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/accessing-completions-chat-model/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/accessing-completions-chat-model/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/advanced-usage-and-customization/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/advanced-usage-and-customization/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/constraints/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/constraints/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/contributing/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/formatting-and-control-flow/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/formatting-and-control-flow/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/getting-started/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/models/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/models/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/content/0.1.0/docs/streaming-and-decoding/index.md` & `headjack_keymaker-0.9.1/docs/content/0.1.0/docs/streaming-and-decoding/index.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/layouts/index.html` & `headjack_keymaker-0.9.1/docs/layouts/index.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/layouts/_default/baseof.html` & `headjack_keymaker-0.9.1/docs/layouts/_default/baseof.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.content` & `headjack_keymaker-0.9.1/docs/resources/_gen/assets/scss/css/style.scss_26962b449d539ee5c1301a7879e5bb0e.content`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/favicon.png` & `headjack_keymaker-0.9.1/docs/static/favicon.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/css/termynal.css` & `headjack_keymaker-0.9.1/docs/static/css/termynal.css`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/images/discord.svg` & `headjack_keymaker-0.9.1/docs/static/images/discord.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/images/github-mark.svg` & `headjack_keymaker-0.9.1/docs/static/images/github-mark.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/images/keymaker-logo.png` & `headjack_keymaker-0.9.1/docs/static/images/keymaker-logo.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/images/keymaker-logo.svg` & `headjack_keymaker-0.9.1/docs/static/images/keymaker-logo.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/images/keymaker-logo.webp` & `headjack_keymaker-0.9.1/docs/static/images/keymaker-logo.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/static/js/termynal.js` & `headjack_keymaker-0.9.1/docs/static/js/termynal.js`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/CHANGELOG.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/CODE_OF_CONDUCT.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/LICENSE` & `headjack_keymaker-0.9.1/docs/themes/DoIt/LICENSE`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/README.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/README.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/README.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/README.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/dependencies.json` & `headjack_keymaker-0.9.1/docs/themes/DoIt/dependencies.json`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/package-lock.json` & `headjack_keymaker-0.9.1/docs/themes/DoIt/package-lock.json`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/package.json` & `headjack_keymaker-0.9.1/docs/themes/DoIt/package.json`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/theme.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/theme.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/dependabot.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/bug-report.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/ISSUE_TEMPLATE/feature-request.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/Lighthouse-CI.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/Lighthouse-CI.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/build.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/codeql-analysis.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/pages.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/.github/workflows/update-algolia-search-index.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/.github/workflows/update-algolia-search-index.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_variables.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_variables.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/main.css` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_core/_base.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_core/_base.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_core/_media.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_core/_media.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_mixin/_compatibility.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_mixin/_compatibility.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_mixin/_link.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_mixin/_link.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_home.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_home.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_page/_single.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_page/_single.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_details.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_details.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_fixed-button.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_fixed-button.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_header.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_header.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_pagination.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_pagination.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_archive/_tags.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_archive/_tags.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_archive/_terms.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_archive/_terms.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_admonition.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_admonition.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_code.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_code.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_footer.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_footer.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_friend.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_friend.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_related.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_related.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_series.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_series.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_showcase.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_showcase.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_sponsor.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_sponsor.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/css/_partial/_single/_toc.scss` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/css/_partial/_single/_toc.scss`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/social.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/social.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/cdn/jsdelivr.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/cdn/jsdelivr.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/apple.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/apple.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/facebook.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/facebook.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/google.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/google.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/data/emoji/twitter.yml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/data/emoji/twitter.yml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/images/avatar.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/images/avatar.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/sw.js` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/sw.js`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/js/theme.js` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/js/theme.js`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/version.template.svg` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/version.template.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/bilibili.svg` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/bilibili.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/qq.svg` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/qq.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/qqGroup.svg` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/qqGroup.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/assets/svg/icons/thingiverse.svg` & `headjack_keymaker-0.9.1/docs/themes/DoIt/assets/svg/icons/thingiverse.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/schema.json` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/schema.json`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/Apple-Devices-Preview.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/Apple-Devices-Preview.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/Wavelength.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/Wavelength.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/avatar.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/avatar.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse-large.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/lighthouse-large.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse-small.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/lighthouse-small.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/lighthouse.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/lighthouse.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/images/screenshot.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/images/screenshot.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/assets/music/Wavelength.mp3` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/assets/music/Wavelength.mp3`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/hugo.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/hugo.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/markup.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/markup.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/menu.en.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/menu.en.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/menu.zh-cn.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/menu.zh-cn.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/params.en.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/params.en.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/params.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/params.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/config/_default/params.zh-cn.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/config/_default/params.zh-cn.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/about/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/about/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/about/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/about/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/featured-image.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/featured-image.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/basic-markdown-syntax/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/featured-image.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/emoji-support/featured-image.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/emoji-support/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/how-to-DoIt/create-diagrams/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Install-PWA.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Install-PWA.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Installed-PWA.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/Installed-PWA.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/featured-image.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/featured-image.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/pwa-support/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/aplayer-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/aplayer-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/builtin-shortcodes-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/builtin-shortcodes-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/echarts-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/echarts-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/extend-shortcodes-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/extend-shortcodes-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/friend-link-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/friend-link-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/katex-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/katex-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/markdown-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/markdown-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/mermaid-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/mermaid-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/showcase-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/showcase-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/toc-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/toc-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/tests/typeit-tests/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/tests/typeit-tests/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.zh-cn.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/basic-configuration-preview.zh-cn.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.zh-cn.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/complete-configuration-preview.zh-cn.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/featured-image.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/featured-image.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/language-switch.gif` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-basics/language-switch.gif`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/featured-image.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/featured-image.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-built-in-shortcodes/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/featured-image.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/featured-image.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.zh-cn.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-content/summary.zh-cn.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image-preview.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image-preview.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image.webp` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/featured-image.webp`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/posts/theme-documentation-extended-shortcodes/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/showcase/index.en.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/showcase/index.en.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/content/showcase/index.zh-cn.md` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/content/showcase/index.zh-cn.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/android-chrome-192x192.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/android-chrome-512x512.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/apple-touch-icon.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/favicon-16x16.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/favicon-32x32.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/favicon.ico` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/mstile-150x150.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/safari-pinned-tab.svg` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/exampleSite/static/site.webmanifest` & `headjack_keymaker-0.9.1/docs/themes/DoIt/exampleSite/static/site.webmanifest`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ar.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ar.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ca.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ca.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/de.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/de.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/en.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/en.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/es.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/es.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/fr.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/fr.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/hi.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/hi.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/id.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/id.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/it.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/it.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ko.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ko.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/pl.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/pl.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/pt-BR.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/pt-BR.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/pt-PT.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/pt-PT.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ro.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ro.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/ru.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/ru.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/sr.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/sr.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/te.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/te.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/th.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/th.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/tr.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/tr.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/uk.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/uk.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/vi.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/vi.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/zh-CN.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/zh-CN.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/i18n/zh-TW.toml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/i18n/zh-TW.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/images/screenshot.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/images/tn.png` & `headjack_keymaker-0.9.1/docs/themes/DoIt/images/tn.png`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/404.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/404.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/index.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/index.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/index.json` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/index.json`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/index.rss.xml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/index.rss.xml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/robots.txt` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/robots.txt`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/sitemap.xml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/sitemap.xml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/baseof.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/baseof.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/section.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/section.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/single.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/single.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/summary.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/summary.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/_default/_markup/render-heading.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/_default/_markup/render-heading.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/assets.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/assets.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/comment.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/comment.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/footer.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/footer.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/header.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/header.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/init.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/init.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/paginator.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/paginator.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/recentlyUpdated.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/recentlyUpdated.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/related.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/related.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/author.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/author.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/content.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/content.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/getRemoteImage.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/getRemoteImage.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/function/resource.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/function/resource.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/head/link.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/head/link.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/head/meta.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/head/meta.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/head/seo.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/head/seo.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/home/profile.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/home/profile.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/meta/author.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/meta/author.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/analytics.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/analytics.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/compatibility.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/compatibility.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/image.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/image.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/script.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/script.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/share.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/share.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/plugin/style.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/plugin/style.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/rss/item.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/rss/item.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/single/footer.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/single/footer.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/single/outdatedArticleReminder.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/single/outdatedArticleReminder.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/partials/single/sponsor.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/partials/single/sponsor.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/posts/rss.xml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/posts/rss.xml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/posts/single.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/posts/single.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/admonition.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/admonition.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/aplayer.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/aplayer.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/audio.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/audio.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/friend.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/friend.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/image.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/image.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/link.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/link.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/mapbox.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/mapbox.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/music.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/music.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/showcase.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/showcase.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/typeit.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/typeit.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/shortcodes/version.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/shortcodes/version.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/taxonomy/list.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/taxonomy/list.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/taxonomy/rss.xml` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/taxonomy/rss.xml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/docs/themes/DoIt/layouts/taxonomy/terms.html` & `headjack_keymaker-0.9.1/docs/themes/DoIt/layouts/taxonomy/terms.html`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/prompt.py` & `headjack_keymaker-0.9.1/keymaker/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     decoder: Optional[Decoder] = None
     stream: Optional[Callable[[Optional["Completion"]], Awaitable[Any]]] = None
     map_fn: Callable[[Completion], Stringable] = noop
     timeout: float = 10.0
     truncate: bool = False
     try_first: Optional[bool] = None
     token_tracker: Optional[TokenTracker] = None
+    exception_handler: Optional[Callable[[Exception, "CompletionConfig"], "CompletionConfig"]] = None
     gen_kwargs: Optional[dict] = None
 
     def __or__(self, other):
         if isinstance(other, CompletionConfig):
             combined = CompletionConfig()
             combined.model = self.model or other.model
             combined.constraint = self.constraint or other.constraint
@@ -285,15 +286,25 @@
         return prompt
 
     async def complete(self, *completion_args, **completion_kwargs) -> "Prompt":
         if "completion_config" in completion_kwargs:
             config = completion_kwargs["completion_config"]
         else:
             config = CompletionConfig(*completion_args, **completion_kwargs)
-        config = self._default_completion_config | config
+        config = config |self._default_completion_config
+
+        try:
+            return await self._complete(config)
+        except Exception as exc:
+            if config.exception_handler:
+                return await self.complete(completion_config=config.exception_handler(exc, config))
+            else:
+                raise exc
+
+    async def _complete(self, config) -> "Prompt":
 
         model = config.model
         constraint = config.constraint
         name = config.name
         max_tokens = config.max_tokens
         decoder = config.decoder
         stream = config.stream
```

### Comparing `headjack_keymaker-0.9.0/keymaker/types.py` & `headjack_keymaker-0.9.1/keymaker/types.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/base.py` & `headjack_keymaker-0.9.1/keymaker/constraints/base.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/json.py` & `headjack_keymaker-0.9.1/keymaker/constraints/json.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/logical.py` & `headjack_keymaker-0.9.1/keymaker/constraints/logical.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/model.py` & `headjack_keymaker-0.9.1/keymaker/constraints/model.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/options.py` & `headjack_keymaker-0.9.1/keymaker/constraints/options.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/parser.py` & `headjack_keymaker-0.9.1/keymaker/constraints/parser.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/regex.py` & `headjack_keymaker-0.9.1/keymaker/constraints/regex.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/constraints/stops.py` & `headjack_keymaker-0.9.1/keymaker/constraints/stops.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/models/__init__.py` & `headjack_keymaker-0.9.1/keymaker/models/__init__.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/models/base.py` & `headjack_keymaker-0.9.1/keymaker/models/base.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/models/huggingface.py` & `headjack_keymaker-0.9.1/keymaker/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/models/litellm.py` & `headjack_keymaker-0.9.1/keymaker/models/litellm.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/models/llama_cpp.py` & `headjack_keymaker-0.9.1/keymaker/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/models/openai.py` & `headjack_keymaker-0.9.1/keymaker/models/openai.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/utils/chat.py` & `headjack_keymaker-0.9.1/keymaker/utils/chat.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/utils/exceptions.py` & `headjack_keymaker-0.9.1/keymaker/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/keymaker/utils/general.py` & `headjack_keymaker-0.9.1/keymaker/utils/general.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/tests/constraints/test_options.py` & `headjack_keymaker-0.9.1/tests/constraints/test_options.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/tests/constraints/test_regex.py` & `headjack_keymaker-0.9.1/tests/constraints/test_regex.py`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/.gitignore` & `headjack_keymaker-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/README.md` & `headjack_keymaker-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/pyproject.toml` & `headjack_keymaker-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `headjack_keymaker-0.9.0/PKG-INFO` & `headjack_keymaker-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: headjack-keymaker
-Version: 0.9.0
+Version: 0.9.1
 Summary: The most powerful, flexible and extensible way to control the output of large language models.
 Project-URL: repository, https://github.com/KnowledgeForge/keymaker
 Author-email: circargs <nick@ouellet.dev>, Nick Ouellet <nick@ouellet.dev>
 License: Apache 2.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: lark>=1.1.5
 Requires-Dist: openai>=1.0.0
```

