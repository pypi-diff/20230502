# Comparing `tmp/flippers-0.0.1b2.tar.gz` & `tmp/flippers-0.0.1b3.tar.gz`

## Comparing `flippers-0.0.1b2.tar` & `flippers-0.0.1b3.tar`

### file list

```diff
@@ -1,151 +1,84 @@
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.readthedocs.yaml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/11e49b9bfc7b431f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/14c6912ce062eddd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/151eaa52aba8d31
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/15ee0f747f3dda8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/165af332925958ff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/1940af3ff053410d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/1a2b24dee338e210
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/1aa9d647363adab7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/1d0d124b58cfaffa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/1e3392f12df1aceb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/1e6198984a1ed3a
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/28e32a1c44a09181
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/322e4c86c1949ccb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/3429e365036c75a6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/375566bba2e19a43
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/37d7055dff96776
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/38c6fffb7b8384c0
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/3de2bf792e874fe1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/3e02f51642418089
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/41d42e8f1102b9c3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/43b7b493d3b9bc89
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/4607160293d06ae5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/472011ba6784b5fe
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/49ed699980f8c8e4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/4aab33487ec736fb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/4e36d0014cedca2c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/505fd30ac19e4726
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/50723dfdf930c7ad
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/51575a3149cfaf75
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/51dd085ecbe5e10c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/520c97372fa216
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/5844ee5d1d2331ac
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/5ba01bb7d1f8106c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/5bad432461bd277f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/5c314e10e54b0acf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/633941d992a26326
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/64eef40dbdfffae3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/65c88036b66ad761
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/664976237e951cfc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/6bf6a6748aca4273
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/6c09a300b0c7b351
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/6cceff6308da3f04
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/7051b17918cec802
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/728ba0dfec1b45d8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/72e965575fd914a1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/738f5231814dd1ef
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/76981811187cf921
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/799cecd6f105ec37
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/7b6a5e358e5f305a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/7d0fe95eaeace77c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/7e9ff8d57c18b453
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/7ebde5be36aab494
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8016f55e8004113f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/81bb06a111af6445
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/826a55a2cfbc50bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/85b028620555b117
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8641e7f7c0d08d1a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/87a723e12f4d76f4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8d314705a49f77b1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8db39b3d65c6f3ed
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8e67b22653ec69ff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8f09c7a9696e23ae
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8f12180cd37e65cd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/8f91bbd72b724201
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/9016bd5ba5eabd82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/913d2ee92b8d25c1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/92eb68718838d2bb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/967c2c537cef7c5b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/97507edda065c89e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/99a45d57eb7a8292
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/99b900dbfbd10e4d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/9be4a4e5f798a2d6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/9c2ac2950c10b926
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/9cf07406b992c2e5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/9d1ed0eae4a1540f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/9fc0064578d0de9d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/a1f074a94e9fa00c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/a2226b00d69e4ed4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/a6fd10a91cfbb217
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/a73c6c5e4cb29215
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/a9b6beefbaa63e0c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/acdd86439d058bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/b421f0274a6f75e7
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/b8ebdedc25fd3cf2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/b932656dd2f6c0aa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/ba868f27708bca66
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/bb421a4208c14b70
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/bbd9b7d3a71a060b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/bd0aa8279668d36e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/be59a319dd648c88
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/bf461f3b40a9308
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/c11ec6f43f83dbd0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/c2d74ee6defe54b5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/c2f009e95b2ae9b5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/c4aa37f9a45b3a64
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/c8e6ef220caee2ae
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/c91fb796a3bcdf03
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/caaaa6814693baee
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/cea56c91f8540792
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/ceb254c3e92ea5a8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/cf4dab4d47c57caf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/d00330e2468d3095
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/d2ad1bd655bba12
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/d555e63182a21335
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/d59d96d78ea123bd
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/d6cc3035e8f17e5b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/d92088ddf0bae5bd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/db4691805c51d68c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/dc711b40ba2da92a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/e32ad372dc5b2c0c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/e48ae9de7f15d26a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/e51b4c9b0400ab29
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/e712c363945039cd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/ed5a4c1e84c33780
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/f4358e41be168488
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/f7ab79bb10bcff32
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/f7efd715d628cfc6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/fc30c8d9b48325e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/fcd41e1e6f00bdf9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/fd7032fe8c28e87c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/fdee859da3db7a27
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/ff5a7cb0d2be88fd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.ruff_cache/content/ffbace36d4f36e9c
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/make.bat
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/requirements.txt
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/source/conf.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/source/index.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/source/_static/custom.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 flippers-0.0.1b2/docs/source/reference/reference.rst
--rw-r--r--   0        0        0   178081 2020-02-02 00:00:00.000000 flippers-0.0.1b2/examples/LabelModels.ipynb
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/__about__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/_typing.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/_core/__init__.py
--rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/_core/_core.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/models/__init__.py
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/models/_base.py
--rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 flippers-0.0.1b2/flippers/models/_snorkel.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 flippers-0.0.1b2/scripts/download_wrench_datasets.sh
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 flippers-0.0.1b2/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 flippers-0.0.1b2/LICENSE
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 flippers-0.0.1b2/README.md
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 flippers-0.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 flippers-0.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.readthedocs.yaml
+-rw-r--r--   0        0        0    97312 2020-02-02 00:00:00.000000 flippers-0.0.1b3/LDA-Copy1.ipynb
+-rw-r--r--   0        0        0    86117 2020-02-02 00:00:00.000000 flippers-0.0.1b3/LDA.ipynb
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/1015da5ee1d6ae09
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/101f92c76019d482
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/174575f6a8de99f9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/222ffeab82898c23
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/24d706a41a5505e6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/2619755b39779213
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/325fe9c721fee38b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/32df89f30cbc04d0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/32e73651997bc833
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/35ac780044c6113
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/3e9c803c3aed46b5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/434179e472510be0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/4349414af1af160b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/46bff405bb5f9a55
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/51a86f2544beaac0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/57c243f290383c75
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/5e121a9c5f4af371
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/61670e66e8896811
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/62b3397ef6b23cc6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/6da9204864500947
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/6e36880ea88b0859
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/707a2630ead89062
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/71aabd6e1213d25d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/75172405e8805037
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/7680b266cdb5323d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/7e140b818a0e35df
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/84f7eef6f0847552
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/8aa97df51a043d6b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/905064e4094bb559
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/92432148d9c34749
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/931f99e805ef72f7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/98a676691af497e5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/a759e5f3179c9c3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/a986cdd8da71d7e3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/b11f13d1da690084
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/b4233a4bb09ad706
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/b7bcfa3cc7a39193
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/c161e876a1fa68c0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/c60274caf2f8821
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/c8545ca9ed816bcd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/ca78102643423a6c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/ce06fdf2705b37fa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/d4a51c2c60a9afbc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/db5d9887bb35ef11
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/de69c8ba4e171810
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e00199a4465c1154
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e304e58799828dce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e32422aeb15174b7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e5b99527c8bf3efc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/eb039d293b99e1a9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/eb068414cbba1a66
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/efb46ea7d6adfd16
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/make.bat
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/requirements.txt
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/conf.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/index.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/_static/custom.css
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/reference/reference.rst
+-rw-r--r--   0        0        0   216648 2020-02-02 00:00:00.000000 flippers-0.0.1b3/examples/ComparisonWithSnorkel.ipynb
+-rw-r--r--   0        0        0   255575 2020-02-02 00:00:00.000000 flippers-0.0.1b3/examples/HyperParameterTuning.ipynb
+-rw-r--r--   0        0        0    94666 2020-02-02 00:00:00.000000 flippers-0.0.1b3/examples/LabelModels.ipynb
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/__about__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/_typing.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/_core/__init__.py
+-rw-r--r--   0        0        0    18312 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/_core/_core.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/models/__init__.py
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/models/_base.py
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/models/_snorkel.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 flippers-0.0.1b3/scripts/download_wrench_datasets.sh
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.gitignore
+-rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 flippers-0.0.1b3/LICENSE
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 flippers-0.0.1b3/README.md
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 flippers-0.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 flippers-0.0.1b3/PKG-INFO
```

### Comparing `flippers-0.0.1b2/docs/Makefile` & `flippers-0.0.1b3/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = source
-BUILDDIR      = build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = source
+BUILDDIR      = build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `flippers-0.0.1b2/docs/make.bat` & `flippers-0.0.1b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flippers-0.0.1b2/docs/source/conf.py` & `flippers-0.0.1b3/docs/source/conf.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-import os
-import sys
-from datetime import datetime
-
-sys.path.insert(0, os.path.abspath("../.."))
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-# Import the theme and set it as the default
-
-project = "flippers"
-copyright = f"2023 - {datetime.now().year}, Liam Toran"
-author = "Liam Toran"
-release = "alpha"
-
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = [
-    "sphinx.ext.napoleon",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.autosectionlabel",
-    "sphinx_argparse_cli",
-    "sphinx_copybutton",
-]
-
-templates_path = ["_templates"]
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
-autosectionlabel_prefix_document = True
-autosummary_imported_members = True
-autosummary_generate = True
-autosummary_recursive = True
-
-autodoc_typehints = "description"
-autoclass_content = "both"
-autodoc_mock_imports = ["torch", "tqdm", "_base.py", "_core.py"]
-autodoc_default_options = {
-    "members": True,
-    "inherited-members": True,
-    "show-inheritance": True,
-    "member-order": "bysource",
-    "special-members": "*predict, *predict_proba, *save, *load",
-    "exclude-members": "__weakref__",
-}
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-html_theme = "pydata_sphinx_theme"
-html_static_path = ["_static"]
-html_css_files = [
-    "custom.css",
-]
-html_sidebars = {
-    "**": ["search-field.html", "sidebar-nav-bs.html", "sidebar-ethical-ads.html"]
-}
-html_theme_options = {
-    "github_url": "https://github.com/liamtoran/flippers",
-}
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+import os
+import sys
+from datetime import datetime
+
+sys.path.insert(0, os.path.abspath("../.."))
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+# Import the theme and set it as the default
+
+project = "flippers"
+copyright = f"2023 - {datetime.now().year}, Liam Toran"
+author = "Liam Toran"
+release = "alpha"
+
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = [
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosectionlabel",
+    "sphinx_argparse_cli",
+    "sphinx_copybutton",
+]
+
+templates_path = ["_templates"]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+autosectionlabel_prefix_document = True
+autosummary_imported_members = True
+autosummary_generate = True
+autosummary_recursive = True
+
+autodoc_typehints = "description"
+autoclass_content = "both"
+autodoc_mock_imports = ["torch", "tqdm", "_base.py", "_core.py"]
+autodoc_default_options = {
+    "members": True,
+    "inherited-members": True,
+    "show-inheritance": True,
+    "member-order": "bysource",
+    "special-members": "*predict, *predict_proba, *save, *load",
+    "exclude-members": "__weakref__",
+}
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+html_theme = "pydata_sphinx_theme"
+html_static_path = ["_static"]
+html_css_files = [
+    "custom.css",
+]
+html_sidebars = {
+    "**": ["search-field.html", "sidebar-nav-bs.html", "sidebar-ethical-ads.html"]
+}
+html_theme_options = {
+    "github_url": "https://github.com/liamtoran/flippers",
+}
```

### Comparing `flippers-0.0.1b2/docs/source/index.rst` & `flippers-0.0.1b3/docs/source/index.rst`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-.. flippers documentation master file, created by
-   sphinx-quickstart on Sun Mar 26 01:49:07 2023.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-#######################
-flippers Documentation
-#######################
-
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-
-   pages/installation
-   pages/overview
-   pages/related
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Applications
-
-   apps/notebook
-   apps/console
-   apps/preview
-   apps/hub
-
-.. toctree::
-   :maxdepth: 2
-   :caption: API Reference
-   :hidden:
-
-   reference/flippers
-
-******************
-Indices and tables
-******************
-
-* :ref:`genindex`
-* :ref:`modindex`
+.. flippers documentation master file, created by
+   sphinx-quickstart on Sun Mar 26 01:49:07 2023.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+#######################
+flippers Documentation
+#######################
+
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Contents:
+
+   pages/installation
+   pages/overview
+   pages/related
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Applications
+
+   apps/notebook
+   apps/console
+   apps/preview
+   apps/hub
+
+.. toctree::
+   :maxdepth: 2
+   :caption: API Reference
+   :hidden:
+
+   reference/flippers
+
+******************
+Indices and tables
+******************
+
+* :ref:`genindex`
+* :ref:`modindex`
 * :ref:`search`
```

### Comparing `flippers-0.0.1b2/.gitignore` & `flippers-0.0.1b3/.gitignore`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# Junk
-*Untitled*
-
-# Data
-*.json
-*.csv
-datasets*
-*.zip
-
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-*flippers*.rst
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
+# Junk
+*Untitled*
+
+# Data
+*.json
+*.csv
+datasets*
+*.zip
+
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+pip-wheel-metadata/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+*flippers*.rst
+
+# PyBuilder
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
```

### Comparing `flippers-0.0.1b2/LICENSE` & `flippers-0.0.1b3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [2023-] [Liam Toran]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [2023-] [Liam Toran]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `flippers-0.0.1b2/README.md` & `flippers-0.0.1b3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-# flippers - A Weak Supervision Library 
-
-![GitHub last commit](https://img.shields.io/github/last-commit/liamtoran/flippers)
-![GitHub](https://img.shields.io/github/license/liamtoran/flippers)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flippers)
-![Read the Docs](https://img.shields.io/readthedocs/flippers)
-![GitHub](https://img.shields.io/github/license/liamtoran/flippers)
-
-(in construction)
-
-`flippers` is a Python library for weak supervision, which allows you to leverage your domain knowledge, heuristics and other weak supervision sources to generate high-quality labels for your training data. 
-
-# Features
-`flippers` includes a number of features for weak supervision, including:
-- Simple tools to analyse your labeling functions,
-- Multiple label models including a from-scratch implementation of the label model used in the `snorkel` library and featuring enhanced ways to predict probabilities,
-- An extensive [documentation](https://flippers.readthedocs.io/en/latest/) with [tutorials](missing_link) and an [API reference](https://flippers.readthedocs.io/en/latest/reference/flippers.html).
-
-# Installation
-To install the latest version of `flippers`, simply run:
-
-```bash
-pip install flippers
-```
-
-# Quick Start 
-## Documentation
-To quickly get started with `flippers`, you can begin by exploring the [documentation](https://flippers.readthedocs.io/en/latest/) and running through the [examples](missing_link) provided. The examples cover a variety of use cases and techniques, which can help you to get a feel for how to apply `flippers` to your own projects. 
-## Example
-- Analyzing your labeling functions:
-```python
-import flippers
-
-analysis = flippers.analyis(L_train)
-```
-- Training a Label Model and doing inference:
-
-```python
-label_model = flippers.models.SnorkelModel(polarities)
-
-label_model.fit(L_train, class_balances)
-
-label_model.predict_proba(L, strategy="all")
-```
-
-# Discussion
-## Troubleshooting
-If you have any questions or issues with `flippers`, please consult the [documentation](https://flippers.readthedocs.io/en/latest/) or reach out in the [GitHub issues](https://github.com/liamtoran/flippers/issues) page for support.
-
-
-## Contributing
-
-`flippers` is an open-source project, and contributions are welcome! If you would like to contribute to `flippers`, please read the `CONTRIBUTING.md` file for guidelines and instructions.
-
-## Related projects
-- [wrench](https://github.com/JieyuZ2/wrench): A weak supervision library created by for benchmarking label models and weak supervision techniques. `flippers` uses its list of datasets as benchmarks.  
-- [snorkel](https://github.com/snorkel-team/snorkel): A cornerstone weak supervision library created by Snorkel in 2016, now sadly abandonned.
-
+# flippers - A Weak Supervision Library 
+
+![GitHub last commit](https://img.shields.io/github/last-commit/liamtoran/flippers)
+![PyPI](https://img.shields.io/pypi/v/flippers)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flippers)
+![Code Style](https://img.shields.io/badge/code%20style-black-black)
+![Read the Docs](https://img.shields.io/readthedocs/flippers)
+![GitHub](https://img.shields.io/github/license/liamtoran/flippers)
+
+(in construction)
+
+`flippers` is a Python library for weak supervision, which allows you to leverage your domain knowledge, heuristics and other weak supervision sources to generate high-quality labels for your training data. 
+
+# Features
+`flippers` includes a number of features for weak supervision, including:
+- Simple tools to analyse your labeling functions,
+- Multiple label models including a from-scratch implementation of the label model used in the `snorkel` library and featuring enhanced ways to predict probabilities,
+- An extensive [documentation](https://flippers.readthedocs.io/en/latest/) with [tutorials](missing_link) and an [API reference](https://flippers.readthedocs.io/en/latest/reference/flippers.html).
+
+# Installation
+To install the latest version of `flippers`, simply run:
+
+```bash
+pip install flippers
+```
+
+# Quick Start 
+## Documentation
+To quickly get started with `flippers`, you can begin by exploring the [documentation](https://flippers.readthedocs.io/en/latest/) and running through the [examples](missing_link) provided. The examples cover a variety of use cases and techniques, which can help you to get a feel for how to apply `flippers` to your own projects. 
+## Example
+- Analyzing your labeling functions:
+```python
+analysis = flippers.analyis(L_train)
+```
+- Training a Label Model and doing inference:
+
+```python
+label_model = flippers.models.SnorkelModel(polarities,  class_balances)
+
+label_model.fit(L_train)
+
+label_model.predict_proba(L)
+```
+
+# Discussion
+## Troubleshooting
+If you have any questions or issues with `flippers`, please consult the [documentation](https://flippers.readthedocs.io/en/latest/) or reach out in the [GitHub issues](https://github.com/liamtoran/flippers/issues) page for support.
+
+
+## Contributing
+
+`flippers` is an open-source project, and contributions are welcome! If you would like to contribute to `flippers`, please read the `CONTRIBUTING.md` file for guidelines and instructions.
+
+## Related projects
+- [wrench](https://github.com/JieyuZ2/wrench): A weak supervision library created by for benchmarking label models and weak supervision techniques. `flippers` uses its list of datasets as benchmarks.  
+- [snorkel](https://github.com/snorkel-team/snorkel): A cornerstone weak supervision library created by Snorkel in 2016, now sadly abandonned.
+
```

### Comparing `flippers-0.0.1b2/PKG-INFO` & `flippers-0.0.1b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: flippers
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: `flippers` is a weak supervision library for creating high quality labels using your domain kownledge and weak supervision sources.
 Project-URL: Documentation, https://github.com/liamtoran/flippers#readme
 Project-URL: Issues, https://github.com/liamtoran/flippers/issues
 Project-URL: Source, https://github.com/liamtoran/flippers
 Author-email: Liam Toran <liam.toran@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
+Keywords: data,data analysis,data augmentation,data cleaning,data engineering,data labeling,data preparation,data science,data wrangling,machine learning,weak supervision
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: scikit-learn
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # flippers - A Weak Supervision Library 
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/liamtoran/flippers)
-![GitHub](https://img.shields.io/github/license/liamtoran/flippers)
+![PyPI](https://img.shields.io/pypi/v/flippers)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flippers)
+![Code Style](https://img.shields.io/badge/code%20style-black-black)
 ![Read the Docs](https://img.shields.io/readthedocs/flippers)
 ![GitHub](https://img.shields.io/github/license/liamtoran/flippers)
 
 (in construction)
 
 `flippers` is a Python library for weak supervision, which allows you to leverage your domain knowledge, heuristics and other weak supervision sources to generate high-quality labels for your training data. 
 
@@ -49,26 +52,24 @@
 
 # Quick Start 
 ## Documentation
 To quickly get started with `flippers`, you can begin by exploring the [documentation](https://flippers.readthedocs.io/en/latest/) and running through the [examples](missing_link) provided. The examples cover a variety of use cases and techniques, which can help you to get a feel for how to apply `flippers` to your own projects. 
 ## Example
 - Analyzing your labeling functions:
 ```python
-import flippers
-
 analysis = flippers.analyis(L_train)
 ```
 - Training a Label Model and doing inference:
 
 ```python
-label_model = flippers.models.SnorkelModel(polarities)
+label_model = flippers.models.SnorkelModel(polarities,  class_balances)
 
-label_model.fit(L_train, class_balances)
+label_model.fit(L_train)
 
-label_model.predict_proba(L, strategy="all")
+label_model.predict_proba(L)
 ```
 
 # Discussion
 ## Troubleshooting
 If you have any questions or issues with `flippers`, please consult the [documentation](https://flippers.readthedocs.io/en/latest/) or reach out in the [GitHub issues](https://github.com/liamtoran/flippers/issues) page for support.
```

