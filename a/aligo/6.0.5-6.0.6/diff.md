# Comparing `tmp/aligo-6.0.5.tar.gz` & `tmp/aligo-6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-6.0.5.tar", last modified: Tue Jul 11 09:42:40 2023, max compression
+gzip compressed data, was "aligo-6.0.6.tar", last modified: Sun Jul 16 13:43:55 2023, max compression
```

## Comparing `aligo-6.0.5.tar` & `aligo-6.0.6.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.175145 aligo-6.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 09:42:33.000000 aligo-6.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-11 09:42:40.175145 aligo-6.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-11 09:42:33.000000 aligo-6.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-11 09:42:33.000000 aligo-6.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 09:42:33.000000 aligo-6.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:42:40.175145 aligo-6.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.143145 aligo-6.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.147145 aligo-6.0.5/src/aligo/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-11 09:42:39.000000 aligo-6.0.5/src/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.151145 aligo-6.0.5/src/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23234 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.155145 aligo-6.0.5/src/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    19221 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.155145 aligo-6.0.5/src/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.163145 aligo-6.0.5/src/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/PrivateShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.167145 aligo-6.0.5/src/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/PrivateShareResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.175145 aligo-6.0.5/src/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/DataClass.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/DriveCapacityDetail.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/DriveFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/EMailConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/FolderSizeInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/LoginDevice.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-11 09:42:33.000000 aligo-6.0.5/src/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:42:40.147145 aligo-6.0.5/src/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-11 09:42:40.000000 aligo-6.0.5/src/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-11 09:42:40.000000 aligo-6.0.5/src/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:42:40.000000 aligo-6.0.5/src/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 09:42:40.000000 aligo-6.0.5/src/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 09:42:40.000000 aligo-6.0.5/src/aligo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.846749 aligo-6.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 13:43:49.000000 aligo-6.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-16 13:43:55.846749 aligo-6.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-16 13:43:49.000000 aligo-6.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-16 13:43:49.000000 aligo-6.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-16 13:43:49.000000 aligo-6.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:43:55.846749 aligo-6.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.822749 aligo-6.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.822749 aligo-6.0.6/src/aligo/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.826749 aligo-6.0.6/src/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23234 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.830749 aligo-6.0.6/src/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.830749 aligo-6.0.6/src/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.834749 aligo-6.0.6/src/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/PrivateShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.838749 aligo-6.0.6/src/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/PrivateShareResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.846749 aligo-6.0.6/src/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/DataClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/DriveFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/EMailConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/FolderSizeInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/LoginDevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.822749 aligo-6.0.6/src/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/top_level.txt
```

### Comparing `aligo-6.0.5/LICENSE` & `aligo-6.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/PKG-INFO` & `aligo-6.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.0.5
+Version: 6.0.6
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.0.5/README.md` & `aligo-6.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/pyproject.toml` & `aligo-6.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Album.py` & `aligo-6.0.6/src/aligo/apis/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Aligo.py` & `aligo-6.0.6/src/aligo/apis/Aligo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Audio.py` & `aligo-6.0.6/src/aligo/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Compress.py` & `aligo-6.0.6/src/aligo/apis/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Copy.py` & `aligo-6.0.6/src/aligo/apis/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Create.py` & `aligo-6.0.6/src/aligo/apis/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/CustomShare.py` & `aligo-6.0.6/src/aligo/apis/CustomShare.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Download.py` & `aligo-6.0.6/src/aligo/apis/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Drive.py` & `aligo-6.0.6/src/aligo/apis/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Duplicate.py` & `aligo-6.0.6/src/aligo/apis/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/File.py` & `aligo-6.0.6/src/aligo/apis/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Move.py` & `aligo-6.0.6/src/aligo/apis/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Other.py` & `aligo-6.0.6/src/aligo/apis/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Recyclebin.py` & `aligo-6.0.6/src/aligo/apis/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Search.py` & `aligo-6.0.6/src/aligo/apis/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Share.py` & `aligo-6.0.6/src/aligo/apis/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Star.py` & `aligo-6.0.6/src/aligo/apis/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/SyncFolder.py` & `aligo-6.0.6/src/aligo/apis/SyncFolder.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Update.py` & `aligo-6.0.6/src/aligo/apis/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/apis/Video.py` & `aligo-6.0.6/src/aligo/apis/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Album.py` & `aligo-6.0.6/src/aligo/core/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Auth.py` & `aligo-6.0.6/src/aligo/core/Auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import coloredlogs
 import qrcode
 import qrcode_terminal
 import requests
 
 import aligo
 from aligo.core.Config import *
-from aligo.error import AligoStatus500, AligoRefreshFailed, AligoFatalError
+from aligo.error import AligoStatus500, AligoRefreshFailed, AligoFatalError, AligoShareLinkCreateExceedDailyLimit
 from aligo.types import *
 from aligo.types.Enum import *
 from .EMail import send_email
 from .LoginServer import LoginServer
 
 # 默认配置目录
 aligo_config_folder = Path.home().joinpath('.aligo')
@@ -417,14 +417,19 @@
                 if b'"DeviceSessionSignatureInvalid"' in response.content \
                         or b'"not found device info"' in response.content:
                     self._create_session()
                     continue
                 elif b'"InvalidResource.FileTypeFolder"' in response.content:
                     self.log.warning(
                         '请区分 文件 和 文件夹，有些操作是它们独有的，比如获取下载链接，很显然 文件夹 是没有的！')
+
+            if status_code == 403:
+                if b'"SharelinkCreateExceedDailyLimit"' in response.content:
+                    raise AligoShareLinkCreateExceedDailyLimit(response.content)
+
             return response
 
         self.log.info(f'重试 5 次仍失败，抛出异常')
         self.error_log_exit(response)
 
     def get(self, path: str, host: str = API_HOST, params: dict = None, headers: dict = None) -> requests.Response:
         """..."""
```

### Comparing `aligo-6.0.5/src/aligo/core/BaseAligo.py` & `aligo-6.0.6/src/aligo/core/BaseAligo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Compress.py` & `aligo-6.0.6/src/aligo/core/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Config.py` & `aligo-6.0.6/src/aligo/core/Config.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Copy.py` & `aligo-6.0.6/src/aligo/core/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Core.py` & `aligo-6.0.6/src/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Create.py` & `aligo-6.0.6/src/aligo/core/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Download.py` & `aligo-6.0.6/src/aligo/core/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Drive.py` & `aligo-6.0.6/src/aligo/core/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Duplicate.py` & `aligo-6.0.6/src/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/EMail.py` & `aligo-6.0.6/src/aligo/core/EMail.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/File.py` & `aligo-6.0.6/src/aligo/core/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/LoginServer.py` & `aligo-6.0.6/src/aligo/core/LoginServer.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Move.py` & `aligo-6.0.6/src/aligo/core/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Recyclebin.py` & `aligo-6.0.6/src/aligo/core/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Search.py` & `aligo-6.0.6/src/aligo/core/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Share.py` & `aligo-6.0.6/src/aligo/core/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Star.py` & `aligo-6.0.6/src/aligo/core/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Update.py` & `aligo-6.0.6/src/aligo/core/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/User.py` & `aligo-6.0.6/src/aligo/core/User.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/core/Video.py` & `aligo-6.0.6/src/aligo/core/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/AlbumListFilesRequest.py` & `aligo-6.0.6/src/aligo/request/AlbumListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/CreateFileRequest.py` & `aligo-6.0.6/src/aligo/request/CreateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/CreateShareLinkRequest.py` & `aligo-6.0.6/src/aligo/request/CreateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/GetFileListRequest.py` & `aligo-6.0.6/src/aligo/request/GetFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/GetFileRequest.py` & `aligo-6.0.6/src/aligo/request/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/GetRecycleBinListRequest.py` & `aligo-6.0.6/src/aligo/request/GetRecycleBinListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/GetShareFileListRequest.py` & `aligo-6.0.6/src/aligo/request/GetShareFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-6.0.6/src/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/GetShareLinkListRequest.py` & `aligo-6.0.6/src/aligo/request/GetShareLinkListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/GetStarredListRequest.py` & `aligo-6.0.6/src/aligo/request/GetStarredListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/SearchFileRequest.py` & `aligo-6.0.6/src/aligo/request/SearchFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/UpdateFileRequest.py` & `aligo-6.0.6/src/aligo/request/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/UpdateShareLinkRequest.py` & `aligo-6.0.6/src/aligo/request/UpdateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/request/__init__.py` & `aligo-6.0.6/src/aligo/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/response/CreateFileResponse.py` & `aligo-6.0.6/src/aligo/response/CreateFileResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/response/CreateShareLinkResponse.py` & `aligo-6.0.6/src/aligo/response/CreateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/response/DuplicateListResponse.py` & `aligo-6.0.6/src/aligo/response/DuplicateListResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/response/GetShareInfoResponse.py` & `aligo-6.0.6/src/aligo/response/GetShareInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/response/GetShareTokenResponse.py` & `aligo-6.0.6/src/aligo/response/GetShareTokenResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/response/UpdateShareLinkResponse.py` & `aligo-6.0.6/src/aligo/response/UpdateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/response/__init__.py` & `aligo-6.0.6/src/aligo/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/BaseAlbum.py` & `aligo-6.0.6/src/aligo/types/BaseAlbum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/BaseDrive.py` & `aligo-6.0.6/src/aligo/types/BaseDrive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/BaseFile.py` & `aligo-6.0.6/src/aligo/types/BaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/BaseShareFile.py` & `aligo-6.0.6/src/aligo/types/BaseShareFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/BaseUser.py` & `aligo-6.0.6/src/aligo/types/BaseUser.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/DataClass.py` & `aligo-6.0.6/src/aligo/types/DataClass.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/Enum.py` & `aligo-6.0.6/src/aligo/types/Enum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/ImageMedia.py` & `aligo-6.0.6/src/aligo/types/ImageMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/Null.py` & `aligo-6.0.6/src/aligo/types/Null.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/ShareLinkSchema.py` & `aligo-6.0.6/src/aligo/types/ShareLinkSchema.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/Token.py` & `aligo-6.0.6/src/aligo/types/Token.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/UserConfig.py` & `aligo-6.0.6/src/aligo/types/UserConfig.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/VideoMedia.py` & `aligo-6.0.6/src/aligo/types/VideoMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/VideoPreview.py` & `aligo-6.0.6/src/aligo/types/VideoPreview.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/VideoPreviewPlayInfo.py` & `aligo-6.0.6/src/aligo/types/VideoPreviewPlayInfo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo/types/__init__.py` & `aligo-6.0.6/src/aligo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.5/src/aligo.egg-info/PKG-INFO` & `aligo-6.0.6/src/aligo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.0.5
+Version: 6.0.6
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.0.5/src/aligo.egg-info/SOURCES.txt` & `aligo-6.0.6/src/aligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

