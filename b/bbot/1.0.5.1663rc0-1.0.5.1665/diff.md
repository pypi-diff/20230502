# Comparing `tmp/bbot-1.0.5.1663rc0.tar.gz` & `tmp/bbot-1.0.5.1665.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1663rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1665.tar", max compression
```

## Comparing `bbot-1.0.5.1663rc0.tar` & `bbot-1.0.5.1665.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0    32473 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/LICENSE
--rw-r--r--   0        0        0    51011 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/README.md
--rw-r--r--   0        0        0      211 2023-05-02 21:19:20.364283 bbot-1.0.5.1663rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     6536 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      376 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    13693 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8920 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     4261 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      632 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    30910 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1498 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-05-02 21:18:59.243972 bbot-1.0.5.1663rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3644 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1256 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     2875 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     6940 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    13841 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     8540 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    29454 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     4286 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5435 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1414 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    29037 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14848 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9574 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     2919 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/queueing.py
--rw-r--r--   0        0        0     1890 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     8474 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/threadpool.py
--rw-r--r--   0        0        0     3987 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3193 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0     9324 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    10967 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     7859 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3731 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1371 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3461 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2350 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    26022 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2197 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1225 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5502 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1065 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      847 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1167 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2169 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4550 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5107 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1116 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     5432 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      732 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     5001 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1160 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13578 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15617 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5763 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2516 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2954 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2862 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      866 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11117 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2164 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1093 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7290 2023-05-02 21:18:59.247972 bbot-1.0.5.1663rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     2723 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10120 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      658 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7395 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5490 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7748 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     1944 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9438 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      298 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16587 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     4773 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1274 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2037 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0      707 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11237 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    14828 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4245 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     4867 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11137 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1379 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2595 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1809 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1836 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1047 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1255 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      204 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3649 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     1747 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1532 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1620 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5360 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1533 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1310 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      746 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1584 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8262 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      742 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2255 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2578 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1071 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1198 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1432 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1607 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1527 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     8014 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6077 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11235 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      566 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3819 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2759 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2458 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1158 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1569 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1169 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2190 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2095 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      427 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    26114 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    22025 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4038 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    18609 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0      559 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0     2545 2023-05-02 21:18:59.251972 bbot-1.0.5.1663rc0/bbot/test/helpers.py
--rw-r--r--   0        0        0    74299 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/modules_test_classes.py
--rw-r--r--   0        0        0       15 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/pytest.ini
--rwxr-xr-x   0        0        0      578 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0      904 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_1/test_before_patching.py
--rw-r--r--   0        0        0     5859 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_1/test_modules_full.py
--rw-r--r--   0        0        0        0 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0      588 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_agent.py
--rw-r--r--   0        0        0     4739 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_cli.py
--rw-r--r--   0        0        0      932 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_cloud_helpers.py
--rw-r--r--   0        0        0      462 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_config.py
--rw-r--r--   0        0        0      722 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_depsinstaller.py
--rw-r--r--   0        0        0    15064 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_events.py
--rw-r--r--   0        0        0    34798 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_helpers.py
--rw-r--r--   0        0        0     7171 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_manager.py
--rw-r--r--   0        0        0    11616 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_modules_basic.py
--rw-r--r--   0        0        0      789 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_python_api.py
--rw-r--r--   0        0        0     3215 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_scan.py
--rw-r--r--   0        0        0     1395 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_scope.py
--rw-r--r--   0        0        0     2163 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_target.py
--rw-r--r--   0        0        0      707 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_threadpool.py
--rw-r--r--   0        0        0      476 2023-05-02 21:18:59.255972 bbot-1.0.5.1663rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-05-02 21:18:59.259972 bbot-1.0.5.1663rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-05-02 21:18:59.263973 bbot-1.0.5.1663rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-05-02 21:18:59.263973 bbot-1.0.5.1663rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-05-02 21:18:59.263973 bbot-1.0.5.1663rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1338 2023-05-02 21:19:20.364283 bbot-1.0.5.1663rc0/pyproject.toml
--rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1663rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/LICENSE
+-rw-r--r--   0        0        0    51011 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/README.md
+-rw-r--r--   0        0        0      209 2023-05-02 21:18:57.396709 bbot-1.0.5.1665/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     6536 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/agent/agent.py
+-rw-r--r--   0        0        0      376 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    13693 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8920 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     4261 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      632 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    30371 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1498 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3644 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1256 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     2875 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     6940 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    13841 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     8540 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    29454 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     4286 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5435 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1414 2023-05-02 21:18:24.484394 bbot-1.0.5.1665/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    29037 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14848 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9574 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     2919 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/queueing.py
+-rw-r--r--   0        0        0     1890 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     8474 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/threadpool.py
+-rw-r--r--   0        0        0     3987 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3193 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0     9324 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    10967 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     7859 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3731 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1371 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3461 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2350 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    26022 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/base.py
+-rw-r--r--   0        0        0     2197 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1225 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5502 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1065 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      847 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1167 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2169 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4550 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5107 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1116 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/c99.py
+-rw-r--r--   0        0        0     5432 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/censys.py
+-rw-r--r--   0        0        0      732 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     5001 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1160 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13578 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15617 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5763 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2516 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2954 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2862 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      866 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11117 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2164 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1093 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7290 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     2723 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/github.py
+-rw-r--r--   0        0        0    10120 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      658 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7395 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5546 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7748 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     1944 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9438 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      298 2023-05-02 21:18:24.488394 bbot-1.0.5.1665/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16587 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     4773 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1274 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2037 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0      707 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11237 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    13620 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4245 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     4867 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11137 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1379 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2586 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1809 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1827 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1047 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1255 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      204 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3649 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     1747 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1532 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1620 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5360 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1533 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1310 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      746 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1584 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8262 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      742 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2255 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2578 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1071 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1198 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1432 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1607 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1527 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/social.py
+-rw-r--r--   0        0        0     8014 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6077 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11235 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      566 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3819 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2759 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2458 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1158 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1569 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1169 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2190 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2095 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    26114 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    22025 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4038 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/__init__.py
+-rw-r--r--   0        0        0    18609 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0      559 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/conftest.py
+-rw-r--r--   0        0        0     2545 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/helpers.py
+-rw-r--r--   0        0        0    74299 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/modules_test_classes.py
+-rw-r--r--   0        0        0       15 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/pytest.ini
+-rwxr-xr-x   0        0        0      578 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0      904 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/test_step_1/test_before_patching.py
+-rw-r--r--   0        0        0     5859 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/test_step_1/test_modules_full.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0      588 2023-05-02 21:18:24.492394 bbot-1.0.5.1665/bbot/test/test_step_2/test_agent.py
+-rw-r--r--   0        0        0     4739 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_cli.py
+-rw-r--r--   0        0        0      932 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_cloud_helpers.py
+-rw-r--r--   0        0        0      462 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_config.py
+-rw-r--r--   0        0        0      722 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_depsinstaller.py
+-rw-r--r--   0        0        0    15064 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_events.py
+-rw-r--r--   0        0        0    34798 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_helpers.py
+-rw-r--r--   0        0        0     7171 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_manager.py
+-rw-r--r--   0        0        0    11616 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_modules_basic.py
+-rw-r--r--   0        0        0      789 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_python_api.py
+-rw-r--r--   0        0        0     3215 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_scan.py
+-rw-r--r--   0        0        0     1395 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_scope.py
+-rw-r--r--   0        0        0     2163 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_target.py
+-rw-r--r--   0        0        0      707 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/test/test_step_2/test_threadpool.py
+-rw-r--r--   0        0        0      476 2023-05-02 21:18:24.496394 bbot-1.0.5.1665/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-05-02 21:18:24.500394 bbot-1.0.5.1665/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-05-02 21:18:24.500394 bbot-1.0.5.1665/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-05-02 21:18:24.500394 bbot-1.0.5.1665/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-05-02 21:18:24.504394 bbot-1.0.5.1665/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1336 2023-05-02 21:18:57.396709 bbot-1.0.5.1665/pyproject.toml
+-rw-r--r--   0        0        0    52286 1970-01-01 00:00:00.000000 bbot-1.0.5.1665/PKG-INFO
```

### Comparing `bbot-1.0.5.1663rc0/LICENSE` & `bbot-1.0.5.1665/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/README.md` & `bbot-1.0.5.1665/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/agent/agent.py` & `bbot-1.0.5.1665/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/cli.py` & `bbot-1.0.5.1665/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1665/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1665/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1665/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1665/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/errors.py` & `bbot-1.0.5.1665/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/event/base.py` & `bbot-1.0.5.1665/bbot/core/event/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -443,16 +443,14 @@
         source_id = self.source_id
         if source_id:
             j["source"] = source_id
         if self.tags:
             j.update({"tags": list(self.tags)})
         if self.module:
             j.update({"module": str(self.module)})
-        if self.module_sequence:
-            j.update({"module_sequence": str(self.module_sequence)})
 
         # normalize non-primitive python objects
         for k, v in list(j.items()):
             if k == "data":
                 continue
             if type(v) not in (str, int, float, bool, list, type(None)):
                 try:
@@ -462,26 +460,14 @@
         return j
 
     @staticmethod
     def from_json(j):
         return event_from_json(j)
 
     @property
-    def module_sequence(self):
-        """
-        A human-friendly representation of the module name that includes modules from omitted source events
-
-        Helpful in identifying where a URL came from
-        """
-        module_name = getattr(self.module, "name", "")
-        if getattr(self.source, "_omit", False):
-            module_name = f"{self.source.module_sequence}->{module_name}"
-        return module_name
-
-    @property
     def module_priority(self):
         if self._module_priority is None:
             module = getattr(self, "module", None)
             self._module_priority = int(max(1, min(5, getattr(module, "priority", 3))))
         return self._module_priority
 
     @module_priority.setter
```

### Comparing `bbot-1.0.5.1663rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1665/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1665/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1665/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1665/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1665/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1665/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1665/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1665/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1665/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1665/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1665/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1665/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1665/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1665/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1665/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1665/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1665/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1665/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/queueing.py` & `bbot-1.0.5.1665/bbot/core/helpers/queueing.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1665/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/threadpool.py` & `bbot-1.0.5.1665/bbot/core/helpers/threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1665/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1665/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1665/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1665/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1665/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1665/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/defaults.yml` & `bbot-1.0.5.1665/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1665/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1665/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1665/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/base.py` & `bbot-1.0.5.1665/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1665/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1665/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1665/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1665/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1665/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1665/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1665/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1665/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1665/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/c99.py` & `bbot-1.0.5.1665/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/censys.py` & `bbot-1.0.5.1665/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1665/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1665/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/crt.py` & `bbot-1.0.5.1665/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1665/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1665/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1665/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1665/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1665/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1665/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1665/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1665/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1665/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1665/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1665/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/github.py` & `bbot-1.0.5.1665/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1665/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1665/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1665/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1665/bbot/modules/httpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,19 +132,19 @@
 
             # main URL
             httpx_ip = j.get("host", "unknown")
             tags = [f"status-{status_code}", f"ip-{httpx_ip}"]
             title = self.helpers.tagify(j.get("title", ""))
             if title:
                 tags.append(f"http-title-{title}")
-            url_event = self.make_event(url, "URL", source_event, tags=tags)
+            url_event = self.make_event(url, "URL", source_event, module=source_event.module, tags=tags)
             if url_event:
                 if url_event != source_event:
                     self.emit_event(url_event)
                 else:
                     url_event._resolved.set()
                 # HTTP response
-                self.emit_event(j, "HTTP_RESPONSE", url_event, internal=True)
+                self.emit_event(j, "HTTP_RESPONSE", url_event, module=source_event.module, internal=True)
 
     def cleanup(self):
         resume_file = self.helpers.current_dir / "resume.cfg"
         resume_file.unlink(missing_ok=True)
```

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1665/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1665/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1665/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1665/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1665/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1665/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1665/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1665/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1665/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1665/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1665/bbot/modules/massdns.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,103 +229,88 @@
                         hostname_hash = hash(hostname)
                         if hostname_hash not in hosts_yielded:
                             hosts_yielded.add(hostname_hash)
                             yield hostname
 
     def finish(self):
         found = sorted(self.found.items(), key=lambda x: len(x[-1]), reverse=True)
-        # if we have a lot of rounds to make, don't try mutations on less-populated domains
-        trimmed_found = []
-        if found:
-            avg_subdomains = sum([len(subdomains) for domain, subdomains in found[:50]]) / len(found[:50])
-            for i, (domain, subdomains) in enumerate(found):
-                # accept domains that are in the top 50 or have more than 5 percent of the average number of subdomains
-                if i < 50 or (len(subdomains) > 1 and len(subdomains) >= (avg_subdomains * 0.05)):
-                    trimmed_found.append((domain, subdomains))
-                else:
-                    self.verbose(
-                        f"Skipping mutations on {domain} because it only has {len(subdomains):,} subdomain(s) (avg: {avg_subdomains:,})"
-                    )
 
         base_mutations = set()
-        try:
-            for i, (domain, subdomains) in enumerate(trimmed_found):
-                self.verbose(f"{domain} has {len(subdomains):,} subdomains")
-                # keep looping as long as we're finding things
-                while 1:
-                    max_mem_percent = 90
-                    mem_status = self.helpers.memory_status()
-                    # abort if we don't have the memory
-                    mem_percent = mem_status.percent
-                    if mem_percent > max_mem_percent:
-                        free_memory = mem_status.available
-                        free_memory_human = self.helpers.bytes_to_human(free_memory)
-                        assert (
-                            False
-                        ), f"Cannot proceed with DNS mutations because system memory is at {mem_percent:.1f}% ({free_memory_human} remaining)"
-
-                    query = domain
-                    domain_hash = hash(domain)
-                    if self.scan.stopping:
-                        return
-
-                    mutations = set(base_mutations)
-
-                    def add_mutation(_domain_hash, m):
-                        h = hash((_domain_hash, m))
-                        if h not in self.mutations_tried:
-                            self.mutations_tried.add(h)
-                            mutations.add(m)
-
-                    # try every subdomain everywhere else
-                    for _domain, _subdomains in found:
-                        if _domain == domain:
+        for i, (domain, subdomains) in enumerate(found):
+            # keep looping as long as we're finding things
+            while 1:
+                max_mem_percent = 90
+                mem_status = self.helpers.memory_status()
+                # abort if we don't have the memory
+                mem_percent = mem_status.percent
+                if mem_percent > max_mem_percent:
+                    free_memory = mem_status.available
+                    free_memory_human = self.helpers.bytes_to_human(free_memory)
+                    self.hugewarning(
+                        f"Cannot proceed with DNS mutations because system memory is at {mem_percent:.1f}% ({free_memory_human} remaining)"
+                    )
+                    break
+
+                query = domain
+                domain_hash = hash(domain)
+                if self.scan.stopping:
+                    return
+
+                mutations = set(base_mutations)
+
+                def add_mutation(_domain_hash, m):
+                    h = hash((_domain_hash, m))
+                    if h not in self.mutations_tried:
+                        self.mutations_tried.add(h)
+                        mutations.add(m)
+
+                # try every subdomain everywhere else
+                for _domain, _subdomains in found:
+                    if _domain == domain:
+                        continue
+                    for s in _subdomains:
+                        first_segment = s.split(".")[0]
+                        # skip stuff with lots of numbers (e.g. PTRs)
+                        digits = self.digit_regex.findall(first_segment)
+                        excessive_digits = len(digits) > 2
+                        long_digits = any(len(d) > 3 for d in digits)
+                        if excessive_digits or long_digits:
                             continue
-                        for s in _subdomains:
-                            first_segment = s.split(".")[0]
-                            # skip stuff with lots of numbers (e.g. PTRs)
-                            digits = self.digit_regex.findall(first_segment)
-                            excessive_digits = len(digits) > 2
-                            long_digits = any(len(d) > 3 for d in digits)
-                            if excessive_digits or long_digits:
-                                continue
-                            add_mutation(domain_hash, first_segment)
-                            for word in self.helpers.extract_words(
-                                first_segment, word_regexes=self.helpers.word_cloud.dns_mutator.extract_word_regexes
-                            ):
-                                add_mutation(domain_hash, word)
-
-                    # numbers + devops mutations
-                    for mutation in self.helpers.word_cloud.mutations(
-                        subdomains, cloud=False, numbers=3, number_padding=1
-                    ):
-                        for delimiter in ("", ".", "-"):
-                            m = delimiter.join(mutation).lower()
-                            add_mutation(domain_hash, m)
-
-                    # special dns mutator
-                    for subdomain in self.helpers.word_cloud.dns_mutator.mutations(
-                        subdomains, max_mutations=self.max_mutations
-                    ):
-                        add_mutation(domain_hash, subdomain)
-
-                    if mutations:
-                        self.info(f"Trying {len(mutations):,} mutations against {domain} ({i+1}/{len(found)})")
-                        results = list(self.massdns(query, mutations))
-                        for hostname in results:
-                            source_event = self.get_source_event(hostname)
-                            if source_event is None:
-                                self.warning(f"Could not correlate source event from: {hostname}")
-                                continue
-                            self.emit_result(hostname, source_event, query)
-                        if results:
+                        add_mutation(domain_hash, first_segment)
+                        for word in self.helpers.extract_words(
+                            first_segment, word_regexes=self.helpers.word_cloud.dns_mutator.extract_word_regexes
+                        ):
+                            add_mutation(domain_hash, word)
+
+                # word cloud
+                for mutation in self.helpers.word_cloud.mutations(
+                    subdomains, cloud=False, numbers=3, number_padding=1
+                ):
+                    for delimiter in ("", ".", "-"):
+                        m = delimiter.join(mutation).lower()
+                        add_mutation(domain_hash, m)
+
+                # special dns mutator
+                for subdomain in self.helpers.word_cloud.dns_mutator.mutations(
+                    subdomains, max_mutations=self.max_mutations
+                ):
+                    add_mutation(domain_hash, subdomain)
+
+                if mutations:
+                    self.info(f"Trying {len(mutations):,} mutations against {domain} ({i+1}/{len(found)})")
+                    results = list(self.massdns(query, mutations))
+                    for hostname in results:
+                        source_event = self.get_source_event(hostname)
+                        if source_event is None:
+                            self.warning(f"Could not correlate source event from: {hostname}")
                             continue
-                    break
-        except AssertionError as e:
-            self.warning(e)
+                        self.emit_result(hostname, source_event, query)
+                    if results:
+                        continue
+                break
 
     def add_found(self, host):
         if not isinstance(host, str):
             host = host.data
         if self.helpers.is_subdomain(host):
             subdomain, domain = host.split(".", 1)
             if not self.helpers.is_ptr(subdomain):
```

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1665/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1665/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/otx.py` & `bbot-1.0.5.1665/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1665/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1665/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1665/bbot/modules/output/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.writerow(
             {
                 "Event type": getattr(event, "type", ""),
                 "Event data": getattr(event, "data", ""),
                 "IP Address": ",".join(
                     str(x) for x in getattr(event, "resolved_hosts", set()) if self.helpers.is_ip(x)
                 ),
-                "Source Module": str(getattr(event, "module_sequence", "")),
+                "Source Module": str(getattr(event, "module", "")),
                 "Scope Distance": str(getattr(event, "scope_distance", "")),
                 "Event Tags": ",".join(sorted(list(getattr(event, "tags", [])))),
             }
         )
 
     def cleanup(self):
         if getattr(self, "_file", None) is not None:
```

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1665/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1665/bbot/modules/output/human.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return True
 
     def handle_event(self, event):
         event_type = f"[{event.type}]"
         event_tags = ""
         if getattr(event, "tags", []):
             event_tags = f'\t({", ".join(sorted(getattr(event, "tags", [])))})'
-        event_str = f"{event_type:<20}\t{event.data_human}\t{event.module_sequence}{event_tags}"
+        event_str = f"{event_type:<20}\t{event.data_human}\t{event.module}{event_tags}"
         # log vulnerabilities in vivid colors
         if event.type == "VULNERABILITY":
             severity = event.data.get("severity", "INFO")
             if severity in self.vuln_severity_map:
                 loglevel = self.vuln_severity_map[severity]
                 log_to_stderr(event_str, level=loglevel, logname=False)
         elif event.type == "FINDING":
```

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1665/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1665/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1665/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1665/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1665/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1665/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1665/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1665/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1665/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1665/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1665/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1665/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1665/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/robots.py` & `bbot-1.0.5.1665/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1665/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1665/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1665/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1665/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1665/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/social.py` & `bbot-1.0.5.1665/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1665/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1665/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1665/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1665/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1665/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1665/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1665/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1665/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1665/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1665/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1665/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1665/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1665/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1665/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1665/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/scanner/target.py` & `bbot-1.0.5.1665/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1665/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/conftest.py` & `bbot-1.0.5.1665/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/helpers.py` & `bbot-1.0.5.1665/bbot/test/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/modules_test_classes.py` & `bbot-1.0.5.1665/bbot/test/modules_test_classes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1665/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test.conf` & `bbot-1.0.5.1665/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_1/test_before_patching.py` & `bbot-1.0.5.1665/bbot/test/test_step_1/test_before_patching.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_1/test_modules_full.py` & `bbot-1.0.5.1665/bbot/test/test_step_1/test_modules_full.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_agent.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_cli.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_cloud_helpers.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_depsinstaller.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_events.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_helpers.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_manager.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_modules_basic.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_python_api.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_scan.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_scope.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_target.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/test/test_step_2/test_threadpool.py` & `bbot-1.0.5.1665/bbot/test/test_step_2/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1665/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1665/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1665/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1665/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1663rc0/pyproject.toml` & `bbot-1.0.5.1665/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1663rc"
+version = "v1.0.5.1665"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1663rc0/PKG-INFO` & `bbot-1.0.5.1665/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1663rc0
+Version: 1.0.5.1665
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

