# Comparing `tmp/jupyter_ai-0.6.0.tar.gz` & `tmp/jupyter_ai-0.6.1.tar.gz`

## Comparing `jupyter_ai-0.6.0.tar` & `jupyter_ai-0.6.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/.eslintignore
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/babel.config.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jest.config.js
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/tsconfig.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/_version.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/engine.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/extension.py
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/models.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/reply_processor.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/task_manager.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/tasks.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/__init__.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/ask.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/base.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/default.py
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/generate.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/learn.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/memory.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/actors/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
--rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js.LICENSE.txt
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
--rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js.LICENSE.txt
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
--rw-r--r--   0        0        0   468858 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
--rw-r--r--   0        0        0   460651 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js.LICENSE.txt
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/643.3e00b12acf02dce55cc2.js
--rw-r--r--   0        0        0   157416 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/673.68e7ac52ccd7076d341f.js
--rw-r--r--   0        0        0    40847 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/675.73a31f502181054c8492.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/675.73a31f502181054c8492.js.LICENSE.txt
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
--rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js.LICENSE.txt
--rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js
--rw-r--r--   0        0        0    15490 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/787.7f6980b88a058f8d58c8.js
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
--rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
--rw-r--r--   0        0        0   157436 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
--rw-r--r--   0        0        0  1568187 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js.LICENSE.txt
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
--rw-r--r--   0        0        0    11544 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/remoteEntry.7e74a3ad789008e8bd74.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   114416 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/schema/plugin.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/chat_handler.ts
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/handler.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/icons.ts
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/index.ts
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/inserter.ts
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/selection-watcher.ts
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/theme-provider.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/utils.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/__tests__/jupyter_gai.spec.ts
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/__tests__/widgets/closable-dialog.spec.tsx
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/chat-messages.tsx
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/open-task-dialog.tsx
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/types/svg.d.ts
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/src/widgets/closable-dialog.tsx
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/style/base.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/style/index.js
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/style/icons/chat.svg
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/style/icons/psychology.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/ui-tests/tests/jupyter_ai.spec.ts
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/LICENSE
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/README.md
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupyter_ai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.eslintignore
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/babel.config.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/conftest.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jest.config.js
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/tsconfig.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/_version.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/engine.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/extension.py
+-rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/models.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/reply_processor.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/task_manager.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/tasks.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/__init__.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/ask.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/base.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/default.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/generate.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/learn.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/memory.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/actors/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
+-rw-r--r--   0        0        0    79896 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js.LICENSE.txt
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
+-rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js.LICENSE.txt
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
+-rw-r--r--   0        0        0   468858 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
+-rw-r--r--   0        0        0   460651 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js.LICENSE.txt
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/643.3e00b12acf02dce55cc2.js
+-rw-r--r--   0        0        0   157416 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/673.68e7ac52ccd7076d341f.js
+-rw-r--r--   0        0        0    40847 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/675.73a31f502181054c8492.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/675.73a31f502181054c8492.js.LICENSE.txt
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
+-rw-r--r--   0        0        0    34117 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js.LICENSE.txt
+-rw-r--r--   0        0        0     9714 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js
+-rw-r--r--   0        0        0    15490 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/787.7f6980b88a058f8d58c8.js
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
+-rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
+-rw-r--r--   0        0        0   157436 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
+-rw-r--r--   0        0        0  1568187 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js.LICENSE.txt
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
+-rw-r--r--   0        0        0    11544 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/remoteEntry.585abad92d66f32304a2.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   114416 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/schema/plugin.json
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/chat_handler.ts
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/handler.ts
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/icons.ts
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/index.ts
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/inserter.ts
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/theme-provider.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/utils.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/__tests__/jupyter_gai.spec.ts
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/__tests__/widgets/closable-dialog.spec.tsx
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/open-task-dialog.tsx
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/src/widgets/closable-dialog.tsx
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/base.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/index.js
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/icons/chat.svg
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/style/icons/psychology.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/ui-tests/tests/jupyter_ai.spec.ts
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/README.md
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupyter_ai-0.6.1/PKG-INFO
```

### Comparing `jupyter_ai-0.6.0/.eslintrc.js` & `jupyter_ai-0.6.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/RELEASE.md` & `jupyter_ai-0.6.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jest.config.js` & `jupyter_ai-0.6.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/package.json` & `jupyter_ai-0.6.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.6.1'"}*

```diff
@@ -122,9 +122,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.0"
+    "version": "0.6.1"
 }
```

### Comparing `jupyter_ai-0.6.0/tsconfig.json` & `jupyter_ai-0.6.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/__init__.py` & `jupyter_ai-0.6.1/jupyter_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/engine.py` & `jupyter_ai-0.6.1/jupyter_ai/engine.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/extension.py` & `jupyter_ai-0.6.1/jupyter_ai/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/handlers.py` & `jupyter_ai-0.6.1/jupyter_ai/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/models.py` & `jupyter_ai-0.6.1/jupyter_ai/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/reply_processor.py` & `jupyter_ai-0.6.1/jupyter_ai/reply_processor.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/task_manager.py` & `jupyter_ai-0.6.1/jupyter_ai/task_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/tasks.py` & `jupyter_ai-0.6.1/jupyter_ai/tasks.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/actors/ask.py` & `jupyter_ai-0.6.1/jupyter_ai/actors/ask.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/actors/base.py` & `jupyter_ai-0.6.1/jupyter_ai/actors/base.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/actors/default.py` & `jupyter_ai-0.6.1/jupyter_ai/actors/default.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/actors/generate.py` & `jupyter_ai-0.6.1/jupyter_ai/actors/generate.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/actors/learn.py` & `jupyter_ai-0.6.1/jupyter_ai/actors/learn.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/actors/memory.py` & `jupyter_ai-0.6.1/jupyter_ai/actors/memory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/actors/router.py` & `jupyter_ai-0.6.1/jupyter_ai/actors/router.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/document_loaders/directory.py` & `jupyter_ai-0.6.1/jupyter_ai/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-0.6.1/jupyter_ai/document_loaders/splitter.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/package.json` & `jupyter_ai-0.6.1/jupyter_ai/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.585abad92d66f32304a2.js'}}",*

 * * "'version'": "'0.6.1'"}*

```diff
@@ -60,15 +60,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7e74a3ad789008e8bd74.js",
+            "load": "static/remoteEntry.585abad92d66f32304a2.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_ai"
                 },
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.0"
+    "version": "0.6.1"
 }
```

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.6.1'"}*

```diff
@@ -122,9 +122,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.0"
+    "version": "0.6.1"
 }
```

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-0.6.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/165.9dda3cd58dc434a135e2.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/296.bda9232f6e5ca4db8f1c.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/465.d994a7f1c5808a09fbe5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/586.d8af1e48008aba81c9a4.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/641.55df6eadf8891e5a1bbe.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/643.3e00b12acf02dce55cc2.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/643.3e00b12acf02dce55cc2.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/673.68e7ac52ccd7076d341f.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/673.68e7ac52ccd7076d341f.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/675.73a31f502181054c8492.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/675.73a31f502181054c8492.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/698.db0bf7bc349a78b068d5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/703.d52ed379ae2e07ba3d54.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/710.92355af1c50cee7b836f.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/785.89e5ffc932d4302b02fa.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/787.7f6980b88a058f8d58c8.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/787.7f6980b88a058f8d58c8.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/92.8c406c1018e3357f19d8.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/964.1d210ce1e570332cead5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/990.ef9212deeffc976b3352.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/remoteEntry.7e74a3ad789008e8bd74.js` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/remoteEntry.585abad92d66f32304a2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -160,15 +160,15 @@
                         (!f || !f.loaded && (!a != !f.eager ? a : i > f.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (f("@emotion/react", "11.10.5", (() => Promise.all([E.e(296), E.e(465), E.e(271), E.e(785)]).then((() => () => E(51465))))), f("@emotion/styled", "11.10.5", (() => Promise.all([E.e(92), E.e(271), E.e(211), E.e(799), E.e(560)]).then((() => () => E(43092))))), f("@jupyter-ai/core", "0.6.0", (() => Promise.all([E.e(675), E.e(673), E.e(271), E.e(222), E.e(787)]).then((() => () => E(65787))))), f("@mui/material", "5.11.8", (() => Promise.all([E.e(296), E.e(641), E.e(675), E.e(271), E.e(211), E.e(222), E.e(456)]).then((() => () => E(98641))))), f("date-fns", "2.29.3", (() => E.e(964).then((() => () => E(8964))))), f("react-markdown", "8.0.6", (() => Promise.all([E.e(698), E.e(165), E.e(271)]).then((() => () => E(4165))))), f("react-syntax-highlighter", "15.5.0", (() => Promise.all([E.e(990), E.e(271)]).then((() => () => E(67990))))), f("rehype-katex", "6.0.2", (() => Promise.all([E.e(698), E.e(586)]).then((() => () => E(66586))))), f("remark-math", "5.1.1", (() => E.e(703).then((() => () => E(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("@emotion/react", "11.10.5", (() => Promise.all([E.e(296), E.e(465), E.e(271), E.e(785)]).then((() => () => E(51465))))), f("@emotion/styled", "11.10.5", (() => Promise.all([E.e(92), E.e(271), E.e(211), E.e(799), E.e(560)]).then((() => () => E(43092))))), f("@jupyter-ai/core", "0.6.1", (() => Promise.all([E.e(675), E.e(673), E.e(271), E.e(222), E.e(787)]).then((() => () => E(65787))))), f("@mui/material", "5.11.8", (() => Promise.all([E.e(296), E.e(641), E.e(675), E.e(271), E.e(211), E.e(222), E.e(456)]).then((() => () => E(98641))))), f("date-fns", "2.29.3", (() => E.e(964).then((() => () => E(8964))))), f("react-markdown", "8.0.6", (() => Promise.all([E.e(698), E.e(165), E.e(271)]).then((() => () => E(4165))))), f("react-syntax-highlighter", "15.5.0", (() => Promise.all([E.e(990), E.e(271)]).then((() => () => E(67990))))), f("rehype-katex", "6.0.2", (() => Promise.all([E.e(698), E.e(586)]).then((() => () => E(66586))))), f("remark-math", "5.1.1", (() => E.e(703).then((() => () => E(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyter_ai-0.6.0/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-0.6.1/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/schema/plugin.json` & `jupyter_ai-0.6.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/chat_handler.ts` & `jupyter_ai-0.6.1/src/chat_handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/handler.ts` & `jupyter_ai-0.6.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/index.ts` & `jupyter_ai-0.6.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/inserter.ts` & `jupyter_ai-0.6.1/src/inserter.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/selection-watcher.ts` & `jupyter_ai-0.6.1/src/selection-watcher.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/theme-provider.ts` & `jupyter_ai-0.6.1/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/utils.ts` & `jupyter_ai-0.6.1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/__tests__/widgets/closable-dialog.spec.tsx` & `jupyter_ai-0.6.1/src/__tests__/widgets/closable-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/chat-code-view.tsx` & `jupyter_ai-0.6.1/src/components/chat-code-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/chat-input.tsx` & `jupyter_ai-0.6.1/src/components/chat-input.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/chat-messages.tsx` & `jupyter_ai-0.6.1/src/components/chat-messages.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/chat.tsx` & `jupyter_ai-0.6.1/src/components/chat.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/expandable-text-field.tsx` & `jupyter_ai-0.6.1/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/jl-theme-provider.tsx` & `jupyter_ai-0.6.1/src/components/jl-theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/open-task-dialog.tsx` & `jupyter_ai-0.6.1/src/components/open-task-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/components/scroll-container.tsx` & `jupyter_ai-0.6.1/src/components/scroll-container.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/contexts/collaborators-context.tsx` & `jupyter_ai-0.6.1/src/contexts/collaborators-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/contexts/selection-context.tsx` & `jupyter_ai-0.6.1/src/contexts/selection-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/widgets/chat-error.tsx` & `jupyter_ai-0.6.1/src/widgets/chat-error.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/widgets/chat-sidebar.tsx` & `jupyter_ai-0.6.1/src/widgets/chat-sidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/src/widgets/closable-dialog.tsx` & `jupyter_ai-0.6.1/src/widgets/closable-dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/style/icons/psychology.svg` & `jupyter_ai-0.6.1/style/icons/psychology.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/ui-tests/README.md` & `jupyter_ai-0.6.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/ui-tests/jupyter_server_test_config.py` & `jupyter_ai-0.6.1/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/ui-tests/tests/jupyter_ai.spec.ts` & `jupyter_ai-0.6.1/ui-tests/tests/jupyter_ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/.gitignore` & `jupyter_ai-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/LICENSE` & `jupyter_ai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/README.md` & `jupyter_ai-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.6.0/pyproject.toml` & `jupyter_ai-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 dependencies = [
     "jupyter_server>=1.6,<3",
     "jupyterlab>=3.5,<4",
     "pydantic",
     "openai~=0.26",
     "aiosqlite~=0.18",
     "importlib_metadata~=5.2.0",
-    "langchain~=0.0.144",
+    "langchain==0.0.153",
     "tiktoken", # required for OpenAIEmbeddings
     "jupyter_ai_magics",
     "ray==2.2.0", # latest ray version 2.3.0 requires grpcio installation from conda
     "faiss-cpu", # Not distributed by official repo
     "wcmatch",
 ]
```

### Comparing `jupyter_ai-0.6.0/PKG-INFO` & `jupyter_ai-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 0.6.0
+Version: 0.6.1
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -51,15 +51,15 @@
 Requires-Python: <3.11,>=3.7
 Requires-Dist: aiosqlite~=0.18
 Requires-Dist: faiss-cpu
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: jupyter-ai-magics
 Requires-Dist: jupyter-server<3,>=1.6
 Requires-Dist: jupyterlab<4,>=3.5
-Requires-Dist: langchain~=0.0.144
+Requires-Dist: langchain==0.0.153
 Requires-Dist: openai~=0.26
 Requires-Dist: pydantic
 Requires-Dist: ray==2.2.0
 Requires-Dist: tiktoken
 Requires-Dist: wcmatch
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
```

