# Comparing `tmp/aligo-6.2.1.tar.gz` & `tmp/aligo-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-6.2.1.tar", last modified: Wed Mar 13 04:39:10 2024, max compression
+gzip compressed data, was "aligo-6.2.2.tar", last modified: Fri Apr  5 08:19:16 2024, max compression
```

## Comparing `aligo-6.2.1.tar` & `aligo-6.2.2.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.846134 aligo-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-13 04:39:02.000000 aligo-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-03-13 04:39:10.846134 aligo-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-03-13 04:39:02.000000 aligo-6.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-13 04:39:02.000000 aligo-6.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-13 04:39:02.000000 aligo-6.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 04:39:10.846134 aligo-6.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.806133 aligo-6.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.810133 aligo-6.2.1/src/aligo/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-13 04:39:09.000000 aligo-6.2.1/src/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.814133 aligo-6.2.1/src/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.818133 aligo-6.2.1/src/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20030 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/SBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.818133 aligo-6.2.1/src/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.830134 aligo-6.2.1/src/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetShareLinkVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/PrivateShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.838134 aligo-6.2.1/src/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/PrivateShareResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.846134 aligo-6.2.1/src/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/DriveCapacityDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/DriveFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/EMailConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/FolderSizeInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/LoginDevice.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/Type.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.846134 aligo-6.2.1/src/aligo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/utils/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:02.000000 aligo-6.2.1/src/aligo/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:39:10.846134 aligo-6.2.1/src/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-03-13 04:39:10.000000 aligo-6.2.1/src/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-03-13 04:39:10.000000 aligo-6.2.1/src/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 04:39:10.000000 aligo-6.2.1/src/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-13 04:39:10.000000 aligo-6.2.1/src/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 04:39:10.000000 aligo-6.2.1/src/aligo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 08:19:11.000000 aligo-6.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-05 08:19:16.947844 aligo-6.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-05 08:19:11.000000 aligo-6.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-05 08:19:11.000000 aligo-6.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 08:19:11.000000 aligo-6.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:19:16.947844 aligo-6.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.911844 aligo-6.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.915844 aligo-6.2.2/src/aligo/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.919844 aligo-6.2.2/src/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.923844 aligo-6.2.2/src/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20148 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/SBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.923844 aligo-6.2.2/src/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.931844 aligo-6.2.2/src/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareLinkVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/PrivateShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.939844 aligo-6.2.2/src/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/PrivateShareResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/src/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/DriveFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/EMailConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/FolderSizeInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/LoginDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/src/aligo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/utils/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/src/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/top_level.txt
```

### Comparing `aligo-6.2.1/LICENSE` & `aligo-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/PKG-INFO` & `aligo-6.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.2.1
+Version: 6.2.2
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.2.1/README.md` & `aligo-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/pyproject.toml` & `aligo-6.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Album.py` & `aligo-6.2.2/src/aligo/apis/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Aligo.py` & `aligo-6.2.2/src/aligo/apis/Aligo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Audio.py` & `aligo-6.2.2/src/aligo/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Compress.py` & `aligo-6.2.2/src/aligo/apis/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Copy.py` & `aligo-6.2.2/src/aligo/apis/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Create.py` & `aligo-6.2.2/src/aligo/apis/Create.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,11 +103,17 @@
             if file.is_file():
                 # 4. 如果是文件, 就上传, 并继续
                 x = self.upload_file(file.path, parent_file_id=folder.file_id, name=file.name, drive_id=drive_id,
                                      check_name_mode=check_name_mode)
                 result.append(x)
                 continue
             # 5. 否则为文件夹, 递归
-            x = self.upload_folder(folder_path=file.path, parent_file_id=folder.file_id, drive_id=drive_id,
-                                   check_name_mode=check_name_mode)
+            x = self.upload_folder(
+                file.path,
+                parent_file_id=folder.file_id,
+                drive_id=drive_id,
+                check_name_mode=check_name_mode,
+                folder_check_name_mode=folder_check_name_mode,
+                file_filter=file_filter
+            )
             result.append({file.name: x})
         return result
```

### Comparing `aligo-6.2.1/src/aligo/apis/CustomShare.py` & `aligo-6.2.2/src/aligo/apis/CustomShare.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Download.py` & `aligo-6.2.2/src/aligo/apis/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Drive.py` & `aligo-6.2.2/src/aligo/apis/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Duplicate.py` & `aligo-6.2.2/src/aligo/apis/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/File.py` & `aligo-6.2.2/src/aligo/apis/File.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,16 +214,15 @@
         :param drive_id:
         :param parent_file_id: 文件夹 id，默认 root
         :param callback: 回调函数
         :param _path: 当前文件基于指定文件夹的路径
         :return:
         """
         for f in self._core_get_file_list(GetFileListRequest(parent_file_id=parent_file_id, drive_id=drive_id)):
-            if f.type == 'file':
-                callback(_path, f)
-                continue
-            self.walk_files(callback, parent_file_id=f.file_id, drive_id=drive_id, _path=os.path.join(_path, f.name))
+            callback(_path, f)
+            if f.type == 'folder':
+                self.walk_files(callback, parent_file_id=f.file_id, drive_id=drive_id, _path=os.path.join(_path, f.name))
 
     def get_folder_size_info(self, file_id: str, drive_id: str = None) -> FolderSizeInfo:
         """获取文件夹信息，文件夹个数，以及文件个数及其大小，不递归"""
         response = self.post(ADRIVE_V1_FILE_GET_FOLDER_SIZE_INFO, body={'file_id': file_id, 'drive_id': drive_id})
         return self._result(response, FolderSizeInfo)
```

### Comparing `aligo-6.2.1/src/aligo/apis/Move.py` & `aligo-6.2.2/src/aligo/apis/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Other.py` & `aligo-6.2.2/src/aligo/apis/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Recyclebin.py` & `aligo-6.2.2/src/aligo/apis/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Search.py` & `aligo-6.2.2/src/aligo/apis/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Share.py` & `aligo-6.2.2/src/aligo/apis/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Star.py` & `aligo-6.2.2/src/aligo/apis/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/SyncFolder.py` & `aligo-6.2.2/src/aligo/apis/SyncFolder.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Update.py` & `aligo-6.2.2/src/aligo/apis/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/apis/Video.py` & `aligo-6.2.2/src/aligo/apis/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Album.py` & `aligo-6.2.2/src/aligo/core/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Audio.py` & `aligo-6.2.2/src/aligo/core/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Auth.py` & `aligo-6.2.2/src/aligo/core/Auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,18 +288,19 @@
             if self._port:
                 # noinspection HttpUrlsUsage
                 self.log.info(f'请访问 http://<YOUR_IP>:{self._port} 扫描二维码')
                 _thread.start_new_thread(self._show_qrcode_in_web, (qr_link,))
             if self._email:
                 self._send_email(qr_link)
         else:
-            qrcode_png = self._show(qr_link)
-            if qrcode_png:
-                self.log.info(f'二维码图片文件 {qrcode_png}')
-        self.log.info('等待扫描二维码')
+            self.log.info('等待扫描二维码，扫码结束后关闭二维码窗口')
+            self._show(qr_link)
+            # qrcode_png = self._show(qr_link)
+            # if qrcode_png:
+            #     self.log.info(f'二维码图片文件 {qrcode_png}')
 
         while True:
             response = self.session.post(
                 PASSPORT_HOST + NEWLOGIN_QRCODE_QUERY_DO,
                 data=data, params=UNI_PARAMS
             )
             login_data = response.json()['content']['data']
@@ -499,14 +500,15 @@
 
     def _show_qrcode_in_web(self, qr_link: str):
         """浏览器显示二维码"""
         qr_img = qrcode.make(qr_link)
         qr_img.get_image()
         qr_img_path = tempfile.mktemp()
         qr_img.save(qr_img_path)
+        # noinspection PyTypeChecker
         self._webServer = HTTPServer(('0.0.0.0', self._port), LoginServer)
         self._webServer.qrData = open(qr_img_path, 'rb').read()
         os.remove(qr_img_path)
         try:
             self._webServer.serve_forever()
         except OSError:
             self._webServer.shutdown()
```

### Comparing `aligo-6.2.1/src/aligo/core/BaseAligo.py` & `aligo-6.2.2/src/aligo/core/BaseAligo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Compress.py` & `aligo-6.2.2/src/aligo/core/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Config.py` & `aligo-6.2.2/src/aligo/core/Config.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Copy.py` & `aligo-6.2.2/src/aligo/core/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Core.py` & `aligo-6.2.2/src/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Create.py` & `aligo-6.2.2/src/aligo/core/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Download.py` & `aligo-6.2.2/src/aligo/core/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Drive.py` & `aligo-6.2.2/src/aligo/core/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Duplicate.py` & `aligo-6.2.2/src/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/EMail.py` & `aligo-6.2.2/src/aligo/core/EMail.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/File.py` & `aligo-6.2.2/src/aligo/core/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/LoginServer.py` & `aligo-6.2.2/src/aligo/core/LoginServer.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Move.py` & `aligo-6.2.2/src/aligo/core/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Other.py` & `aligo-6.2.2/src/aligo/core/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Recyclebin.py` & `aligo-6.2.2/src/aligo/core/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/SBox.py` & `aligo-6.2.2/src/aligo/core/SBox.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Search.py` & `aligo-6.2.2/src/aligo/core/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Share.py` & `aligo-6.2.2/src/aligo/core/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Star.py` & `aligo-6.2.2/src/aligo/core/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Update.py` & `aligo-6.2.2/src/aligo/core/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/User.py` & `aligo-6.2.2/src/aligo/core/User.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/core/Video.py` & `aligo-6.2.2/src/aligo/core/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/AlbumListFilesRequest.py` & `aligo-6.2.2/src/aligo/request/AlbumListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/CreateFileRequest.py` & `aligo-6.2.2/src/aligo/request/CreateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/CreateShareLinkRequest.py` & `aligo-6.2.2/src/aligo/request/CreateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/GetFileListRequest.py` & `aligo-6.2.2/src/aligo/request/GetFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/GetFileRequest.py` & `aligo-6.2.2/src/aligo/request/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/GetRecycleBinListRequest.py` & `aligo-6.2.2/src/aligo/request/GetRecycleBinListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/GetShareFileListRequest.py` & `aligo-6.2.2/src/aligo/request/GetShareFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-6.2.2/src/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/GetShareLinkListRequest.py` & `aligo-6.2.2/src/aligo/request/GetShareLinkListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/GetStarredListRequest.py` & `aligo-6.2.2/src/aligo/request/GetStarredListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/SearchFileRequest.py` & `aligo-6.2.2/src/aligo/request/SearchFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/UpdateFileRequest.py` & `aligo-6.2.2/src/aligo/request/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/UpdateShareLinkRequest.py` & `aligo-6.2.2/src/aligo/request/UpdateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/request/__init__.py` & `aligo-6.2.2/src/aligo/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/CreateFileResponse.py` & `aligo-6.2.2/src/aligo/response/CreateFileResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/CreateShareLinkResponse.py` & `aligo-6.2.2/src/aligo/response/CreateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/DuplicateListResponse.py` & `aligo-6.2.2/src/aligo/response/DuplicateListResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/GetShareInfoResponse.py` & `aligo-6.2.2/src/aligo/response/GetShareInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py` & `aligo-6.2.2/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/GetShareTokenResponse.py` & `aligo-6.2.2/src/aligo/response/GetShareTokenResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/UpdateShareLinkResponse.py` & `aligo-6.2.2/src/aligo/response/UpdateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/response/__init__.py` & `aligo-6.2.2/src/aligo/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/BaseAlbum.py` & `aligo-6.2.2/src/aligo/types/BaseAlbum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/BaseDrive.py` & `aligo-6.2.2/src/aligo/types/BaseDrive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/BaseFile.py` & `aligo-6.2.2/src/aligo/types/BaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/BaseShareFile.py` & `aligo-6.2.2/src/aligo/types/BaseShareFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/BaseUser.py` & `aligo-6.2.2/src/aligo/types/BaseUser.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/Enum.py` & `aligo-6.2.2/src/aligo/types/Enum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/ImageMedia.py` & `aligo-6.2.2/src/aligo/types/ImageMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/ListAlbumItem.py` & `aligo-6.2.2/src/aligo/types/ListAlbumItem.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/Null.py` & `aligo-6.2.2/src/aligo/types/Null.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/ShareLinkBaseFile.py` & `aligo-6.2.2/src/aligo/types/ShareLinkBaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/ShareLinkSchema.py` & `aligo-6.2.2/src/aligo/types/ShareLinkSchema.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/Token.py` & `aligo-6.2.2/src/aligo/types/Token.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/UserConfig.py` & `aligo-6.2.2/src/aligo/types/UserConfig.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/VideoMedia.py` & `aligo-6.2.2/src/aligo/types/VideoMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/VideoPreview.py` & `aligo-6.2.2/src/aligo/types/VideoPreview.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/VideoPreviewPlayInfo.py` & `aligo-6.2.2/src/aligo/types/VideoPreviewPlayInfo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo/types/__init__.py` & `aligo-6.2.2/src/aligo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.1/src/aligo.egg-info/PKG-INFO` & `aligo-6.2.2/src/aligo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.2.1
+Version: 6.2.2
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.2.1/src/aligo.egg-info/SOURCES.txt` & `aligo-6.2.2/src/aligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

