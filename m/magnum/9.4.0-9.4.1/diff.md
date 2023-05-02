# Comparing `tmp/magnum-9.4.0.tar.gz` & `tmp/magnum-9.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/magnum-9.4.0.tar", last modified: Fri Jun 19 11:47:00 2020, max compression
+gzip compressed data, was "dist/magnum-9.4.1.tar", last modified: Wed Mar 24 15:40:57 2021, max compression
```

## Comparing `magnum-9.4.0.tar` & `magnum-9.4.1.tar`

### file list

```diff
@@ -1,1225 +1,1226 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/kubernetes-scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4414 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-scheduler/config.json.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-scheduler/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-scheduler/scheduler
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      185 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-scheduler/launch.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-scheduler/config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-scheduler/service.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10079 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/config.json.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/sources
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      173 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/launch.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/proxy
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-proxy/service.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4655 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/config.json.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/sources
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      457 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/launch.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/apiserver
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-apiserver/service.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/heat-container-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15194 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/config.json.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/Dockerfile
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      117 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/launch
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/tmpfiles.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/manifest.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5343 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/heat-config-notify
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/write-os-apply-config-templates.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/configure_container_agent.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/hooks/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3051 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/hooks/script
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3341 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/hooks/atomic
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3748 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/hooks/docker-compose
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6762 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/55-heat-config
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3500 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/scripts/50-heat-config-docker-compose
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/heat-container-agent/service.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4423 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/config.json.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/controller-manager
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/sources
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      331 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/launch.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-controller-manager/service.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/helm-client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/helm-client/Dockerfile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11681 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/config.json.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/kubelet
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/tmpfiles.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/sources
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      471 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/launch.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/manifest.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2020-06-19 11:45:04.000000 magnum-9.4.0/dockerfiles/kubernetes-kubelet/service.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14021 2020-06-19 11:47:00.000000 magnum-9.4.0/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/playbooks/pre/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/pre/prepare-workspace-images.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/pre/prepare-workspace.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1561 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/container-publish.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/container-builder-setup-gate.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/container-builder-vars.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4064 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/magnum-functional-base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4097 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/container-builder.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1900 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/container-builder-copy-logs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/playbooks/post/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2020-06-19 11:45:04.000000 magnum-9.4.0/playbooks/post/upload-logs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-19 11:45:04.000000 magnum-9.4.0/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-06-19 11:45:04.000000 magnum-9.4.0/.mailmap
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    54146 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2020-06-19 11:45:04.000000 magnum-9.4.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2020-06-19 11:45:04.000000 magnum-9.4.0/functional_creds.conf.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/examples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/examples/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/examples/etc/systemd/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/examples/etc/systemd/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/examples/etc/systemd/system/magnum-api.service
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/examples/etc/systemd/system/magnum-conductor.service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/examples/etc/init/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/examples/etc/init/magnum-conductor.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/examples/etc/init/magnum-api.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/examples/etc/logrotate.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/examples/etc/logrotate.d/magnum.logrotate
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30291 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/admin/troubleshooting-guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/admin/magnum-proxy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2942 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/admin/gmr.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/admin/configuring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/admin/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/api-microversion-history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30425 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/quickstart.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4096 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/functional-test.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11633 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/api-microversion.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4832 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/objects.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/reno.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26324 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/policies.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/contributor/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49470 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/images/MagnumVolumeIntegration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18055 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/images/cluster-create.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    72423 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/images/cluster-template-details.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50394 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/images/cluster-template.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2253 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/cli/magnum-status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2862 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/configuration/sample-policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/configuration/sample-config.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/configuration/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/configuration/samples/policy-yaml.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/configuration/samples/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5204 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/user/k8s-keystone-authN-authZ.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3508 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/user/glossary.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/user/cluster-type-definition.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13823 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/user/kubernetes-load-balancer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/user/heat-templates.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/user/rolling-upgrade.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   150414 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/verify.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2025 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      787 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/install-debian-manual.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7725 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/install-guide-from-source.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/doc/source/install/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3125 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/common/configure_2_edit_magnum_conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7805 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/common/prerequisites.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/common/configure_3_populate_database.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25665 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/launch-instance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/install-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3052 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2020-06-19 11:45:04.000000 magnum-9.4.0/doc/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2020-06-19 11:45:04.000000 magnum-9.4.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2020-06-19 11:45:04.000000 magnum-9.4.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2020-06-19 11:45:04.000000 magnum-9.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2020-06-19 11:47:00.000000 magnum-9.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2020-06-19 11:45:04.000000 magnum-9.4.0/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2020-06-19 11:45:04.000000 magnum-9.4.0/devstack/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1622 2020-06-19 11:45:04.000000 magnum-9.4.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2020-06-19 11:45:04.000000 magnum-9.4.0/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15559 2020-06-19 11:45:04.000000 magnum-9.4.0/devstack/lib/magnum
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8071 2020-06-19 11:45:04.000000 magnum-9.4.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2020-06-19 11:45:04.000000 magnum-9.4.0/.testr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-sha256-verification-for-hyperkube-fb2292c6a8bb00ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/allow-cluster-template-being-renamed-82f7d5d1f33a7957.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-opensuse-driver-f69b6d346ca82b87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/ignore-calico-devices-in-network-manager-e1bdb052834e11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/no-cinder-volume-87b9339e066c30a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/strip-ca-certificate-a09d0c31c45973df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-octavia-client-4e5520084eae3c2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-k8s-label-for-portal-network-cidr-a09edab29da6e7da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/remove-container-endpoint-3494eb8bd2406e87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-1663757-198e1aa8fa810984.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-2002981-trustee-auth-region-name-37796a4e6a274fb8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/swarm-integration-with-cinder-e3068138a3f75dbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/nodegroup-limit-89930d45ee06c621.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/change-bay-to-cluster-in-config-1f2b95d1176d7231.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/disable-ssh-password-authn-f2baf619710e52aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-prometheus-clusterip-b191fa163e3f1125.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-hostgw-backend-option-1d1f9d8d95ec374f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-1718947-0d4e67529e2817d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/kubelet-nfs-b51e572adfb56378.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/keystone_trustee_interface-6d63b74616dda1d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-policy-and-doc-in-code-0c19e479dbd953c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/boot-from-volume-7c73df68d7f325aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-cluster-floating-ip-enabled-default-value-4e24d4bf09fc08c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/pre-delete-cluster-5e27cfdf45e25805.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/flannel-cni-4a5c9f574325761e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/heat-container-agent-for-train-e63bc1559750fe9c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-keystone-auth-6c88c1a2d406fb61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-barbican-alternative-store-35ec3eda0abb0e25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/grafana_prometheus_tag_label-78540ea106677485.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-improve-floating-ip-enabled-84cd00224d6b7bc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-nginx-getting-oom-killed-76139fd8b57e6c15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/resize-api-2bf1fb164484dea9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/improve-k8s-master-kubelet-taint-0c56ffede270116d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-auto-healing-controller-333d1266918111e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/keystone-auth-repo-6970c05f44299326.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/affinity-policy-for-mesos-template-def-82627eb231aa4d28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/RBAC-and-client-incompatibility-fdfeab326dfda3bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s_fedora_atomic_apply_cluster_role-8a46c881de1a1fa3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-container_infra_prefix-516cc43fbc5a0617.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/dns-autoscale-90b63e3d71d7794e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/sync-service-account-keys-for-multi-masters-71217c4cf4dd472c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-federation-api-cf55d04f96772b0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-delete-vip-fip-b2ddf61ddbc080bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-kubelet-to-master-nodes-da2d4ea0d3a332cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/rotate-cluster-cert-9f84deb0adf9afb1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-upgrade-check-framework-5057ad67a7690a14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/prometheus-adapter-15fba9d739676e70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-magnum-notifications-8bd44cfe9e80f82b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/update-swarm-73d4340a881bff2f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-race-condition-for-k8s-multi-masters-29bd36de57df355a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/make-keypair-optional-fcf4a17e440d0879.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/rename-minion-to-node-9d32fe77d765f149.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/prometheus-operator-compatible-with-k8s-1-16-f8be99cf527075b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-1766284-k8s-fedora-admin-user-e760f9b0edf49391.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-octavia-for-k8s-service-d5d7fd041f9d76fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-2002728-kube-os-conf-region-46cd60537bdabdb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-proxy-of-grafana-script-8b408d9d103dfc06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-information-about-cluster-in-event-notifications-a3c992ab24b32fbd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/allow-setting-network-subnet-FIP-when-creating-cluster-ae0cda35ade28a9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-cluster-update-886bd2d1156bef88.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/stats-api-68bc66147ac027e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/traefik-compatible-with-k8s-1-16-9a9ef6d3ccc92fb4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-serveraddressoutputmapping-for-private-clusters-73a874bb4827d568.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/helm-install-ingress-nginx-fe2acec1dd3032e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/change-service-name-ce5c72642fe1d3d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/enable_cloud_provider_label-ed79295041bc46a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/set-traefik-tag-7d4aca5685147970.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-1614596-support-ssl-magnum-api-e4896928c6562e03.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/swarm-live-restore-b03ad192367abced.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/docker-volume-type-46044734f5a27661.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/availability_zone-2d73671f5ea065d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/client-embed-certs-322701471e4d6e1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-overlay-networks-to-swarm-4467986d7853fcd8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-octavia-ingress-controller-32c0b97031fd0dd4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-nodes-security-group-9d8dbb91b006d9dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-fedora-atomic-os-upgrade-9f47182b21c6c028.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/coredns-update-9b03da4b89be18ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/quota-api-182cd1bc9e706b17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-secure-etcd-cluster-coe-5abd22546f05a85b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-2004942-052321df27529562.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/podsecuritypolicy-2400063d73524e06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/allow-multimaster-no-fip-b11520485012d949.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/upgrade_api-1fecc206e5b0ef99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/default-policy-k8s-keystone-auth-fa74aa03dcc12ef3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/update-to-f27-cc8aa873cdf111bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/rollback-bay-on-update-failure-83e5ff8a7904d5c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/flannel-reboot-fix-f1382818daed4fa8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/use_podman-39532143be2296c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/calico-network-driver-0199c2459041ae81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s_fedora_protect_kubelet-8468ddcb92c2a624.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-auto-generate-name-052ea3fdf05fdbbf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/add-docker-storage-driver-to-baymodel-1ed9ba8d43ecfea1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/return-clusterid-for-resize-upgrade-6e841c7b568fa807.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/async-bay-operations-support-9819bd06122ea9e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/integrate-osprofiler-79bdf2d0cd8a39fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/cert-manager-api-ee0cf7f3b767bb5d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-cluster-creation-speedup-21b5b368184d7bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/update-kubernetes-dashboard-5196831c32d55aee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-keypair-override-on-create-ca8f12ffca41cd62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/helm-install-metrics-service-e7a5459417504a75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/configure-etcd-auth-bug-1759813-baac5e0fe8a2e97f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-cert-apimanager-527352622c5a9c3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/broken-kuberenetes-client-d2d1da6029825208.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/upgrade-api-975233ab93c0c092.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/CVE-2016-7404-f53e62a4a40e4d30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-k8s-coe-version-a8ea38f327ea6bb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/cluster_template_update_labels-10ce66c87795f11c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/helm-install-metrics-service-cd18be76c4ed0e5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/using-vxlan-for-flannel-backend-8d82a290ca97d6e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/configurable-k8s-health-polling-interval-75bb83b4701d48c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-auto-healing-3e07c16c55209b0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-1722522-d94743c6362a5e48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-global-stack-list-7a3a66169f5c4aa8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-1697655-add-etcd-volume-size-label-abde0060595bbbeb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/heapster-enabled-label-292ca1ddac68a156.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/helm-install-prometheus-operator-ea87752bc57a0945.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/containerd-598761bb536af6ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/heat-container-agent-tag-92848c1062c16c76.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-decouple-lbaas-c8f2d73313c40b98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support_nodes_affinity_policy-22253fb9cf6739ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/deploy-tiller-in-k8s-df12ee41d00dd7ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-mesos-slave-flags-de6cf8c4d2c3c916.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/kubernetes-cloud-config-6c9a4bfec47e3bb4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fix-fedora-proxy-a4b8d5fc4ec65e80.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/upgrade-to-k8s-v1.11.1-8065fd768873295d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-multi-dns-server-0528be20f0e6aa62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-container-monitoring-d4bb1cbd0a4e44cc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/k8s-fedora-atomic-rolling-upgrade-3d8edcdd91fa1529.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bug-1580704-32a0e91e285792ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/deprecate-send_cluster_metrics-8adaac64a979f720.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/support-all-tenants-for-admin-a042f5c520d35837.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/cinder-csi-enabled-label-ab2b8ade63c57cf3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/fedora_coreos-e66b44d86dea380f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/bp-add-kube-dashboard-8a9f7d7c73c2debd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/return-server-id-in-kubeminion-cb33f5141e0b7fa9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/ingress-controller-552ea956ceabdd25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/server-groups-for-both-master-and-workder-bdd491e4323955d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/notes/heat-container-agent-tag-fe7cec6b890329af.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8574 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/unreleased.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/rocky.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52681 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33751 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2020-06-19 11:45:04.000000 magnum-9.4.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3131 2020-06-19 11:45:04.000000 magnum-9.4.0/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2484 2020-06-19 11:47:00.000000 magnum-9.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2020-06-19 11:45:04.000000 magnum-9.4.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/templates/example/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/templates/example/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/templates/example/example_template/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/templates/example/example_template/example.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/templates/example/example_template/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/templates/example/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/COPYING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11483 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/kubeminion.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      590 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-minion.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1445 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3412 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-minion.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-docker.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/create-kubernetes-user.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-etcd.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-minion.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1428 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-kubeconfig.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/add-proxy.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3299 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert-client.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20106 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/kubecluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3687 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11221 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/kubemaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3234 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/config.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6305 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/openSUSE-Leap-42.1-JeOS-for-OpenStack-Magnum-K8s.kiwi
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1299 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/images.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6683 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/heat/dcos_centos_template_def.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8834 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/dcosslave.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/secgroup.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4626 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/dcosmaster.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/fragments/write-heat-params.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6611 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/fragments/configure-dcos.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5104 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/lb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19829 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/dcoscluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/scale_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      431 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/install_imagebuild_deps.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/elements-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      563 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/install.d/50-install-docker
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      122 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/post-install.d/60-enable-docker-service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      923 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/20-configure-docker-service
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      630 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/10-enable-overlay
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1025 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/validate_dcos_image.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/elements-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      727 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/extra-data.d/99-download-generate-config
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      167 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/post-install.d/99-add-norgoup
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/post-install.d/99-enable-ntp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/environment.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      339 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/environment.d/10-dcos-install-url
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2740 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/contrib/drivers/dcos_centos_v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      515 2020-06-19 11:45:04.000000 magnum-9.4.0/tools/flake8wrap.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2502 2020-06-19 11:45:04.000000 magnum-9.4.0/tools/cover.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1533 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/cmd/db_manage.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2718 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/cmd/api.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2628 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/cmd/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3375 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/cmd/driver_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/swarm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6469 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/swarm/test_swarm_python_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/swarm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/mesos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/mesos/test_mesos_python_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/mesos/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/k8s/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/k8s/test_k8s_python_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/k8s/test_magnum_python_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/k8s/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/api/v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2421 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/baymodelpatch_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/baypatch_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2509 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_templatepatch_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_template_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/cert_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/baymodel_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/bay_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_id_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/magnum_service_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/models/clusterpatch_model.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/cluster_template_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3730 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/baymodel_client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5820 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/bay_client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6399 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/cluster_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/cert_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/magnum_service_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/clients/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/v1/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6060 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/swarm_mode/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4769 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/swarm_mode/test_swarm_mode_python_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/swarm_mode/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    21518 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/python_client_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/k8s_ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/k8s_ironic/test_k8s_python_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/k8s_ironic/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3607 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19161 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/datagen.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3527 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/functional/k8s_coreos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/k8s_coreos/test_k8s_python_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/functional/k8s_coreos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4272 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/conf_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/policy_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/fake_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/contrib/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5231 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/contrib/gate_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10717 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/contrib/copy_instance_logs.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8987 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/contrib/post_test_hook.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1832 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/output_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5373 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3260 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/cmd/test_driver_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/cmd/test_db_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/cmd/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/cmd/test_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4999 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/cmd/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9703 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/test_k8s_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11632 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_nodegroup_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29079 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_cluster_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_conductor_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59894 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_k8s_cluster_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3375 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_indirection_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4904 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/common/test_trust_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23005 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/common/test_cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31727 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_swarm_cluster_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23960 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_mesos_cluster_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_federation_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2444 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_ca_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22416 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/test_monitors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/conductor/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4943 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/tasks/test_heat_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5304 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9509 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/test_scale_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conductor/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22261 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/service/test_periodic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/service/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5534 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_magnum_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10689 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6968 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_x509keypair.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8725 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_nodegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8231 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17862 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6135 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7375 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/test_cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/objects/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/servicegroup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/servicegroup/test_magnum_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/servicegroup/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30740 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/drivers/test_heat_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    94549 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/drivers/test_template_definition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/drivers/test_k8s_fedora_atomic_v1_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14320 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/test_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/test_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16217 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/test_attr_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5593 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/test_servicegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5996 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/test_hooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16026 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_magnum_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50401 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6642 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52056 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31661 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_nodegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17993 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44710 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11169 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_cluster_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10056 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5847 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14704 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    66227 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11777 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/auth-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/auth-root-access.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11173 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/test_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/auth-v1-access.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/noauth-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/test_expose.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10570 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4024 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/test_magnum_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11885 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4403 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/test_x509keypair.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3065 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/sqlalchemy/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10069 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/test_nodegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14527 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10339 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/test_federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9628 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/test_cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9789 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/test_hacking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2828 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conf/test_conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/conf/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3194 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11261 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3968 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_docker_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12645 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15573 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4717 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/common/x509/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2484 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/x509/test_operations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4756 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/x509/test_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10086 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/x509/test_sign.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/x509/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2130 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/common/cert_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4399 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_x509keypair_cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11405 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_barbican.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/cert_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1921 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_urlfetch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10304 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6992 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_octavia.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_short_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9278 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/tests/unit/template/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/template/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/unit/template/test_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/conductor/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/conductor/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/conductor_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/federation_conductor.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14893 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/cluster_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2495 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/ca_conductor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/conductor/handlers/common/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2079 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/common/trust_manager.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8650 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/common/cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3192 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/indirection_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5770 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/handlers/nodegroup_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/monitors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6571 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/utils.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3366 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/scale_manager.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5571 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/k8s_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/conductor/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/tasks/heat_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conductor/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/service/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10685 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/service/periodic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/service/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5467 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14538 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8862 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/x509keypair.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6026 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/magnum_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8663 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/nodegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5399 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3024 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10996 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/servicegroup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2139 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/servicegroup/magnum_service_periodic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/servicegroup/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/COPYING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16383 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/cluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3304 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13829 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmnode.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16265 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmmaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/template_def.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4058 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      203 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/run_openvswitch_neutron.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-heat-params-master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2141 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-master-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-worker-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10475 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmnode.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11758 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmmaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16276 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmcluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1416 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2686 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesosslave.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6252 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesos_slave_software_configs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3620 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesosmaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16168 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesoscluster.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-ext-ca-certs.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/write-heat-params-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/volume-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/write-heat-params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-proxy.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-slave.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/start-services-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/start-services-slave.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/COPYING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/scale_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      396 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/install_imagebuild_deps.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/Dockerfile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/docker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/docker/elements-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/docker/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      107 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/docker/post-install.d/60-disable-docker-service
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/docker/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      482 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/docker/pre-install.d/10-add-docker-repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/docker/package-installs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/elements-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/post-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      189 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/post-install.d/60-disable-upstart
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/pre-install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      545 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/pre-install.d/10-apt-repo
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/README.md
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      812 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/validate_image.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/COPYING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19326 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/kubeminion.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6968 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/fcct-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45453 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/kubecluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7235 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/user_data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32553 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/kubemaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10626 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion_software_configs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3544 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22076 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubecluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17414 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubemaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2825 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/elements-deps
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2454 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/Readme.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/package-installs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/add-docker-daemon-options.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/cfn-signal.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/configure-selinux.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-heat-params-master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/enable-services.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3932 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/network-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-heat-params-node.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-docker-socket.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-cluster-failure-service.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5473 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/make-cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1903 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/volume-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-swarm-master-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/configure-etcd.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/remove-docker-key.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/add-proxy.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-network-config.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-swarm-agent-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1967 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/network-config-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/lb_etcd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/network.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/no_private_network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/with_volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/with_master_lb_octavia.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/disable_floating_ip.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/disable_lb_floating_ip.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/no_master_lb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/with_master_lb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/enable_floating_ip.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/no_volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/with_etcd_volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/with_private_network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/no_etcd_volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/environments/enable_lb_floating_ip.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/enable-docker-registry.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/floating_ip_address_switcher_public.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/floating_ip_address_switcher_private.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/configure_docker_storage_driver_atomic.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/configure-docker-registry.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/network_switcher_private.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/network_switcher_existing.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/api_gateway_switcher_master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/configure-docker-storage.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/api_gateway_switcher_pool.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/fragments/atomic-install-openstack-ca.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6006 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/prometheus-operator.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2917 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/metrics-server.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/prometheus-adapter.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6566 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/ingress-nginx.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-controller.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/install-clients.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15414 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-cinder-csi.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/start-container-agent.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10555 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-healing.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/install-cri.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5807 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/make-cert.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5318 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-octavia.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20127 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6893 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/upgrade-kubernetes.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11572 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-minion.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5282 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-traefik.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5867 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-scaling.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-services-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9726 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/kube-apiserver-to-kubelet-role.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/install-helm-modules.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6190 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-helm-tiller.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5280 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/configure-etcd.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7177 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/core-dns-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/write-kube-os-config.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-services-minion.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/disable-selinux.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/wc-notify-master.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/flannel-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18133 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-prometheus-monitoring.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4381 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-keystone-auth.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/add-proxy.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3973 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/make-cert-client.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12992 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/kube-dashboard-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-cert-api-manager.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18095 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/calico-service.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/templates/lb_api.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/k8s_scale_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8363 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8966 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/k8s_monitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7607 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/swarm_fedora_template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10785 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/k8s_fedora_template_def.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    22669 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/template_def.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    28929 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11849 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/k8s_template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8462 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/swarm_mode_template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4263 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/k8s_coreos_template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/heat/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/COPYING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19581 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/kubeminion.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45204 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/kubecluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32470 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/kubemaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59046 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/tools/grafana-prometheus-dashboard.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/COPYING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15708 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/kubeminion.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-controller-manager.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-minion.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-docker-mount.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2871 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-apiserver.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2047 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params-master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3622 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-dashboard.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4070 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-minion.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-master-kubeconfig.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3983 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert-client.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2794 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service-client.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-docker.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-etcd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/add-ext-ca-certs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-network-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/add-proxy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/create-kube-namespace.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/wc-notify.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1311 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-scheduler.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-kubeconfig.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-coredns.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26277 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/kubecluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22817 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/kubemaster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/template_def.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/drivers/k8s_coreos_v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/expose.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1941 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/app.wsgi
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5102 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/versioned_method.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/middleware/auth_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/middleware/parsable_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2559 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/http_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4347 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10062 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/attr_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/rest_api_version_history.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5363 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/api/controllers/v1/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23286 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8208 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/quota.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    24714 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16870 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17992 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6360 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/cluster_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16162 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/nodegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/collection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3658 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/magnum_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6557 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6984 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21505 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11044 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/link.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7985 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3326 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/servicegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/db/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10399 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35260 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/env.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2b5f24dd95de_rename_service_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/05d3e97de9ee_add_volume_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/e0653b2d5271_add_fixed_subnet_column_to_baymodel_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/bb42b7cad130_remove_node_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2411 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/ac92cbae311c_add_nodegoup_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/a1136d335540_add_docker_storage_driver_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/049f81f6f584_remove_ssh_authorized_key_from_baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5977879072a7_add_env_to_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/085e601a39f6_remove_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/35cff7c86221_add_private_network_to_baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3b6c4c42adb4_add_unique_constraints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/6f21dc920bb_add_cert_uuid_to_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5793cd26898d_add_bay_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/456126c6c9e9_create_baylock_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1561 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/ee92b41b8809_create_quotas_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/68ce16dfd341_add_master_lb_enabled_column_to_baymodel_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/40f325033343_add_bay_create_timeout_to_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3be65537a94a_add_network_driver_baymodel_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/d072f58ab240_modify_x509keypair_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3a938526b35d_add_docker_volume_size.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/53882537ac57_add_host_column_to_pod.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/966a99e70ff_add_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2ae93c9c6191_add_public_column_to_baymodel_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/9a1539f1cd2c_add_federation_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/bc46ba6cf949_add_keypair_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/27ad304554e2_adding_magnum_service_functionality.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5518af8dbc21_rename_cert_uuid.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/fcb4efee8f8b_add_version_info_to_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1201 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/720f640f43d1_rename_bay_table_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1322 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/cbbc65a86986_add_health_status_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/adc3b7679ae_add_registry_trust_id_to_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/ef08a5e057bd_remove_pod.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/fb03fdef8919_rename_baymodel_to_clustertemplate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/4e263f236334_add_registry_enabled.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1afee1db6cd0_add_master_flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/59e7664a8ba1_add_container_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/52bcaf58fecb_add_master_flavor_id_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/6f21dc998bb_add_master_addresses_to_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1c1ff5e56048_rename_container_image_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/156ceb17fb0a_add_bay_status_reason.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/a0e7c8450ab1_add_labels_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/e772b2598d9_add_container_command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/47380964133d_add_network_subnet_fip_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/33ef79969018_add_memory_to_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/aa0cc27839af_add_docker_volume_size_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5ad410481b88_rename_insecure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/e647f5931da8_add_insecure_registry_to_baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4516 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/461d798132c7_change_cluster_to_support_nodegroups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/4ea34a59a64c_add_discovery_url_to_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1d045384b966_add_insecure_baymodel_attr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/c04e925e65c2_nodegroups_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1481f5b560dd_add_labels_column_to_baymodel_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/14328d6a57e3_add_master_count_to_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/421102d1f2d2_create_x509keypair_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2d8657c0cdc_add_bay_uuid.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/041d9a0f1159_add_flavor_id_to_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/04c625aa95ba_change_storage_driver_to_string.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/29affeaa2bc2_rename_bay_master_address.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/592131657ca1_add_coe_column_to_baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/87e62e3c7abc_add_hidden_to_cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2d1354bbf76e_ssh_authorized_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6124 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5d4caa6e0a42_create_trustee_for_each_bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2ace4006498_rename_bay_minions_address.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1f196a3dabae_remove_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2386 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3bea56f25597_multi_tenant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/417917e778f5_add_server_type_to_baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/b1f612248cab_add_floating_ip_enabled_column_to_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/4956f03cabad_add_cluster_distro.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/859fb45df249_remove_replication_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/57fbdf2327a2_remove_baylock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic/script.py.mako
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22390 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/docker_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/barbican.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1853 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2371 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/drivers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2137 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1970 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/octavia.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/kubernetes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1876 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/paths.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/docker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/magnum_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3195 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/trust.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1970 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/glance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/certificates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/x509.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/cluster_heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2711 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/cluster_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/conf/nova.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/common/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/common/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/bay.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5015 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3054 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/baymodel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2698 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/magnum_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/nodegroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5141 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9263 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1488 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/cinder.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12790 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/keystone.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9404 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/name_generator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/common/x509/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10172 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/x509/operations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/x509/extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/x509/validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/x509/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3571 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/octavia.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/common/cert_manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8603 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/cert_manager/barbican_cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7309 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/cert_manager/local_cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/cert_manager/x509keypair_cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2839 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/cert_manager/cert_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/cert_manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2152 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5250 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/rpc.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2822 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/urlfetch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/rpc_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5838 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6152 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4152 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/short_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3358 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/docker_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/nova.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13591 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/common/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/magnum/hacking/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6064 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:45:04.000000 magnum-9.4.0/magnum/hacking/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/etc/magnum/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-06-19 11:45:04.000000 magnum-9.4.0/etc/magnum/magnum-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2020-06-19 11:45:04.000000 magnum-9.4.0/etc/magnum/api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2749 2020-06-19 11:45:04.000000 magnum-9.4.0/etc/magnum/keystone_auth_default_policy.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2020-06-19 11:45:04.000000 magnum-9.4.0/etc/magnum/magnum-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2020-06-19 11:45:04.000000 magnum-9.4.0/etc/magnum/README-magnum.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-06-19 11:45:04.000000 magnum-9.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   119169 2020-06-19 11:47:00.000000 magnum-9.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2020-06-19 11:45:04.000000 magnum-9.4.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5956 2020-06-19 11:45:04.000000 magnum-9.4.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6976 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/flatten_attributes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6005 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/create-trustee-user-for-each-bay.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6278 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/tls-support-magnum.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18077 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/async-container-operation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10402 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/resource-quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19706 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/containers-service.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6530 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/open-dcos.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6802 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/stats-api-spec.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/magnum-horizon-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19422 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/container-networking-model.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19477 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/container-volume-integration-model.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12077 2020-06-19 11:45:04.000000 magnum-9.4.0/specs/bay-drivers.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8548 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/clustertemplates.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17986 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/mservices.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/certificates.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/bays.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2287 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1416 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/urls.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6573 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8024 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/baymodels.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6658 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/clusters.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-19 11:47:00.000000 magnum-9.4.0/api-ref/source/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/bay-get-all-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/baymodel-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/versions-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/quota-get-one-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/clustertemplate-get-all-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/clustertemplate-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-get-one-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/quota-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/baymodel-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/bay-get-one-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/clustertemplate-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/certificates-ca-show-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/versions-01-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/bay-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/bay-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/baymodel-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/bay-create-req.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       81 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/quota-delete-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/certificates-ca-sign-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-resize-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/quota-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/quota-get-all-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/mservice-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/baymodel-get-all-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-upgrade-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/clustertemplate-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/quota-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-resize-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-get-all-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/stats-get-resp.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      102 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/quota-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/cluster-upgrade-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/samples/certificates-ca-sign-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/stats.inc
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2378 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/quotas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2020-06-19 11:45:04.000000 magnum-9.4.0/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2020-06-19 11:45:04.000000 magnum-9.4.0/bindep.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-06-19 11:45:04.000000 magnum-9.4.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-03-24 15:40:07.000000 magnum-9.4.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-03-24 15:40:07.000000 magnum-9.4.1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-03-24 15:40:07.000000 magnum-9.4.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2021-03-24 15:40:08.000000 magnum-9.4.1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7997 2021-03-24 15:40:08.000000 magnum-9.4.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14021 2021-03-24 15:40:57.000000 magnum-9.4.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2021-03-24 15:40:08.000000 magnum-9.4.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   119379 2021-03-24 15:40:57.000000 magnum-9.4.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2021-03-24 15:40:07.000000 magnum-9.4.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-03-24 15:40:07.000000 magnum-9.4.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2021-03-24 15:40:57.858353 magnum-9.4.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2021-03-24 15:40:08.000000 magnum-9.4.1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.722349 magnum-9.4.1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.738349 magnum-9.4.1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8024 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/baymodels.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/bays.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2021-03-24 15:40:08.000000 magnum-9.4.1/api-ref/source/certificates.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6658 2021-03-24 15:40:08.000000 magnum-9.4.1/api-ref/source/clusters.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8548 2021-03-24 15:40:08.000000 magnum-9.4.1/api-ref/source/clustertemplates.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6573 2021-03-24 15:40:08.000000 magnum-9.4.1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/mservices.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17986 2021-03-24 15:40:08.000000 magnum-9.4.1/api-ref/source/parameters.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2378 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/quotas.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/api-ref/source/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/bay-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/bay-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/bay-get-all-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/bay-get-one-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/bay-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/baymodel-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/baymodel-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/baymodel-get-all-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/baymodel-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/certificates-ca-show-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/certificates-ca-sign-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/certificates-ca-sign-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-get-all-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-get-one-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-resize-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-resize-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-upgrade-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/cluster-upgrade-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/clustertemplate-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/clustertemplate-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/clustertemplate-get-all-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/clustertemplate-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/mservice-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/quota-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/quota-create-resp.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       81 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/quota-delete-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/quota-get-all-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/quota-get-one-resp.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      102 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/quota-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/quota-update-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/stats-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/versions-01-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/samples/versions-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/stats.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1416 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/urls.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2287 2021-03-24 15:40:07.000000 magnum-9.4.1/api-ref/source/versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-24 15:40:07.000000 magnum-9.4.1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2021-03-24 15:40:08.000000 magnum-9.4.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.722349 magnum-9.4.1/contrib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.722349 magnum-9.4.1/contrib/drivers/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2740 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/elements-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/environment.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      339 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/environment.d/10-dcos-install-url
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      727 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/extra-data.d/99-download-generate-config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      167 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/post-install.d/99-add-norgoup
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/post-install.d/99-enable-ntp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/elements-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      563 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/install.d/50-install-docker
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.742349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      122 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/post-install.d/60-enable-docker-service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.746349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      630 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/10-enable-overlay
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      923 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/20-configure-docker-service
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      431 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/install_imagebuild_deps.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1025 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/validate_dcos_image.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2834 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/scale_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.746349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19829 2021-03-24 15:40:08.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/dcoscluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4626 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/dcosmaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8834 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/dcosslave.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.746349 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6611 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/fragments/configure-dcos.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/fragments/write-heat-params.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5104 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/lb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/secgroup.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/dcos_centos_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.746349 magnum-9.4.1/contrib/drivers/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6683 2021-03-24 15:40:08.000000 magnum-9.4.1/contrib/drivers/heat/dcos_centos_template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.746349 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.746349 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3234 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/config.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1299 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/images.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6305 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/openSUSE-Leap-42.1-JeOS-for-OpenStack-Magnum-K8s.kiwi
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2021-03-24 15:40:08.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.746349 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/COPYING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3687 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/add-proxy.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-docker.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-etcd.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1428 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      590 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-minion.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3412 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-minion.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/create-kubernetes-user.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3299 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert-client.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1445 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-minion.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-kubeconfig.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20106 2021-03-24 15:40:08.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/kubecluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11221 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/kubemaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11483 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/kubeminion.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.722349 magnum-9.4.1/contrib/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/contrib/templates/example/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/templates/example/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/contrib/templates/example/example_template/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/templates/example/example_template/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/templates/example/example_template/example.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2021-03-24 15:40:07.000000 magnum-9.4.1/contrib/templates/example/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2021-03-24 15:40:07.000000 magnum-9.4.1/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15559 2021-03-24 15:40:08.000000 magnum-9.4.1/devstack/lib/magnum
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1622 2021-03-24 15:40:08.000000 magnum-9.4.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2021-03-24 15:40:07.000000 magnum-9.4.1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.726349 magnum-9.4.1/doc/examples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.726349 magnum-9.4.1/doc/examples/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/examples/etc/init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/examples/etc/init/magnum-api.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/examples/etc/init/magnum-conductor.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/examples/etc/logrotate.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/examples/etc/logrotate.d/magnum.logrotate
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.726349 magnum-9.4.1/doc/examples/etc/systemd/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/examples/etc/systemd/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/examples/etc/systemd/system/magnum-api.service
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/examples/etc/systemd/system/magnum-conductor.service
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/admin/configuring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2942 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/admin/gmr.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/admin/magnum-proxy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30291 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/admin/troubleshooting-guide.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2253 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/cli/magnum-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2862 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/configuration/sample-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/configuration/sample-policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.750350 magnum-9.4.1/doc/source/configuration/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/configuration/samples/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/configuration/samples/policy-yaml.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.754350 magnum-9.4.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/contributor/api-microversion-history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11633 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/contributor/api-microversion.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4096 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/contributor/functional-test.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4832 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/contributor/objects.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26324 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/contributor/policies.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30425 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/contributor/quickstart.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/contributor/reno.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/contributor/troubleshooting.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.754350 magnum-9.4.1/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49470 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/images/MagnumVolumeIntegration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18055 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/images/cluster-create.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    72423 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/images/cluster-template-details.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50394 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/images/cluster-template.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3052 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.754350 magnum-9.4.1/doc/source/install/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.754350 magnum-9.4.1/doc/source/install/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3125 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/common/configure_2_edit_magnum_conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/common/configure_3_populate_database.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7805 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/common/prerequisites.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      787 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/install-debian-manual.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7725 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/install-guide-from-source.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2025 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25665 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/install/launch-instance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.758350 magnum-9.4.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/user/cluster-type-definition.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3508 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/user/glossary.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/user/heat-templates.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   150414 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5204 2021-03-24 15:40:08.000000 magnum-9.4.1/doc/source/user/k8s-keystone-authN-authZ.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13823 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/user/kubernetes-load-balancer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2021-03-24 15:40:07.000000 magnum-9.4.1/doc/source/user/rolling-upgrade.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.726349 magnum-9.4.1/dockerfiles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.758350 magnum-9.4.1/dockerfiles/heat-container-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2021-03-24 15:40:08.000000 magnum-9.4.1/dockerfiles/heat-container-agent/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15194 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/config.json.template
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      117 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/launch
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/manifest.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.758350 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3500 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/50-heat-config-docker-compose
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6762 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/55-heat-config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/configure_container_agent.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5343 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/heat-config-notify
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.758350 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/hooks/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3341 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/hooks/atomic
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3748 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/hooks/docker-compose
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3051 2021-03-24 15:40:08.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/hooks/script
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/scripts/write-os-apply-config-templates.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/service.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/heat-container-agent/tmpfiles.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.758350 magnum-9.4.1/dockerfiles/helm-client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2021-03-24 15:40:08.000000 magnum-9.4.1/dockerfiles/helm-client/Dockerfile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.758350 magnum-9.4.1/dockerfiles/kubernetes-apiserver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-apiserver/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-apiserver/apiserver
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-apiserver/config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4655 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-apiserver/config.json.template
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      457 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-apiserver/launch.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-apiserver/service.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-apiserver/sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.758350 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4423 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/config.json.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/controller-manager
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      331 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/launch.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/service.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-controller-manager/sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.762350 magnum-9.4.1/dockerfiles/kubernetes-kubelet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11681 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/config.json.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/kubelet
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      471 2021-03-24 15:40:08.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/launch.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/manifest.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/service.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/sources
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-kubelet/tmpfiles.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.762350 magnum-9.4.1/dockerfiles/kubernetes-proxy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-proxy/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-proxy/config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10079 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-proxy/config.json.template
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      173 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-proxy/launch.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-proxy/proxy
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-proxy/service.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-proxy/sources
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.762350 magnum-9.4.1/dockerfiles/kubernetes-scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-scheduler/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      542 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-scheduler/config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4414 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-scheduler/config.json.template
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      185 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-scheduler/launch.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-scheduler/scheduler
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2021-03-24 15:40:07.000000 magnum-9.4.1/dockerfiles/kubernetes-scheduler/service.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.726349 magnum-9.4.1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.762350 magnum-9.4.1/etc/magnum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-03-24 15:40:07.000000 magnum-9.4.1/etc/magnum/README-magnum.conf.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2021-03-24 15:40:07.000000 magnum-9.4.1/etc/magnum/api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2749 2021-03-24 15:40:07.000000 magnum-9.4.1/etc/magnum/keystone_auth_default_policy.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-03-24 15:40:07.000000 magnum-9.4.1/etc/magnum/magnum-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-03-24 15:40:07.000000 magnum-9.4.1/etc/magnum/magnum-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2021-03-24 15:40:07.000000 magnum-9.4.1/functional_creds.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3131 2021-03-24 15:40:08.000000 magnum-9.4.1/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.762350 magnum-9.4.1/magnum/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.766350 magnum-9.4.1/magnum/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1941 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/app.wsgi
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10062 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/attr_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.766350 magnum-9.4.1/magnum/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7985 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2029 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/link.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3326 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.766350 magnum-9.4.1/magnum/api/controllers/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11044 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/v1/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23286 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16870 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6984 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/certificate.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    24714 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6360 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/cluster_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21505 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/v1/collection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17992 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/v1/federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3658 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/v1/magnum_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16162 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/nodegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8208 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/controllers/v1/stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6557 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/v1/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5363 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/controllers/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/expose.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4347 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2559 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/http_error.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.770350 magnum-9.4.1/magnum/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/middleware/auth_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/middleware/parsable_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/rest_api_version_history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/servicegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5102 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/api/validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/api/versioned_method.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.770350 magnum-9.4.1/magnum/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/cmd/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2718 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/cmd/api.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2628 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/cmd/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/cmd/db_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3375 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/cmd/driver_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1533 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.770350 magnum-9.4.1/magnum/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.770350 magnum-9.4.1/magnum/common/cert_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/cert_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8603 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/cert_manager/barbican_cert_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2839 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/cert_manager/cert_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7309 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/cert_manager/local_cert_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/cert_manager/x509keypair_cert_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1488 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9263 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2152 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6152 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3358 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/docker_utils.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13591 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/exception.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12790 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/name_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4152 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3571 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/octavia.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.774350 magnum-9.4.1/magnum/common/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3054 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5015 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/policies/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5141 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2698 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/magnum_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/nodegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/policies/stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5838 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2530 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5250 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/rpc_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/common/short_id.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2822 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/urlfetch.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9404 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.774350 magnum-9.4.1/magnum/common/x509/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/x509/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/x509/extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10172 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/x509/operations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/common/x509/validator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.774350 magnum-9.4.1/magnum/conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/conductor/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.774350 magnum-9.4.1/magnum/conductor/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/handlers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2495 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/conductor/handlers/ca_conductor.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14893 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/conductor/handlers/cluster_conductor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.774350 magnum-9.4.1/magnum/conductor/handlers/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/handlers/common/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8650 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/conductor/handlers/common/cert_manager.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2079 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/handlers/common/trust_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/handlers/conductor_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/handlers/federation_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3192 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/handlers/indirection_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5770 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/handlers/nodegroup_conductor.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5571 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/k8s_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/monitors.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3366 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/conductor/scale_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.774350 magnum-9.4.1/magnum/conductor/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conductor/tasks/heat_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6571 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/conductor/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.778350 magnum-9.4.1/magnum/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2137 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/barbican.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/certificates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/cluster_heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/cluster_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/docker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/docker_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2371 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/drivers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/glance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1853 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/conf/kubernetes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/magnum_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1970 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1970 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/octavia.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2711 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1876 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/paths.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3195 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/trust.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/conf/x509.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.778350 magnum-9.4.1/magnum/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22390 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.778350 magnum-9.4.1/magnum/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.782351 magnum-9.4.1/magnum/db/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.790351 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/041d9a0f1159_add_flavor_id_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/049f81f6f584_remove_ssh_authorized_key_from_baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/04c625aa95ba_change_storage_driver_to_string.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/05d3e97de9ee_add_volume_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/085e601a39f6_remove_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/14328d6a57e3_add_master_count_to_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1481f5b560dd_add_labels_column_to_baymodel_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/156ceb17fb0a_add_bay_status_reason.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1afee1db6cd0_add_master_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1c1ff5e56048_rename_container_image_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1d045384b966_add_insecure_baymodel_attr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1f196a3dabae_remove_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6124 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/27ad304554e2_adding_magnum_service_functionality.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/29affeaa2bc2_rename_bay_master_address.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2ace4006498_rename_bay_minions_address.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2ae93c9c6191_add_public_column_to_baymodel_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2b5f24dd95de_rename_service_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2d1354bbf76e_ssh_authorized_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2d8657c0cdc_add_bay_uuid.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/33ef79969018_add_memory_to_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/35cff7c86221_add_private_network_to_baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3a938526b35d_add_docker_volume_size.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3b6c4c42adb4_add_unique_constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3be65537a94a_add_network_driver_baymodel_column.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2386 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3bea56f25597_multi_tenant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/40f325033343_add_bay_create_timeout_to_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/417917e778f5_add_server_type_to_baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/421102d1f2d2_create_x509keypair_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/456126c6c9e9_create_baylock_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4516 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/461d798132c7_change_cluster_to_support_nodegroups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/47380964133d_add_network_subnet_fip_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/4956f03cabad_add_cluster_distro.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/4e263f236334_add_registry_enabled.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/4ea34a59a64c_add_discovery_url_to_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/52bcaf58fecb_add_master_flavor_id_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/53882537ac57_add_host_column_to_pod.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5518af8dbc21_rename_cert_uuid.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5793cd26898d_add_bay_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/57fbdf2327a2_remove_baylock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/592131657ca1_add_coe_column_to_baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5977879072a7_add_env_to_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/59e7664a8ba1_add_container_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5ad410481b88_rename_insecure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5d4caa6e0a42_create_trustee_for_each_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/68ce16dfd341_add_master_lb_enabled_column_to_baymodel_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/6f21dc920bb_add_cert_uuid_to_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/6f21dc998bb_add_master_addresses_to_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1201 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/720f640f43d1_rename_bay_table_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/859fb45df249_remove_replication_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/87e62e3c7abc_add_hidden_to_cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/966a99e70ff_add_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1755 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/9a1539f1cd2c_add_federation_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/a0e7c8450ab1_add_labels_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/a1136d335540_add_docker_storage_driver_column.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/aa0cc27839af_add_docker_volume_size_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2411 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/ac92cbae311c_add_nodegoup_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/adc3b7679ae_add_registry_trust_id_to_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/b1f612248cab_add_floating_ip_enabled_column_to_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/bb42b7cad130_remove_node_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/bc46ba6cf949_add_keypair_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/c04e925e65c2_nodegroups_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1322 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/cbbc65a86986_add_health_status_to_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/d072f58ab240_modify_x509keypair_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/e0653b2d5271_add_fixed_subnet_column_to_baymodel_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/e647f5931da8_add_insecure_registry_to_baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/e772b2598d9_add_container_command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1561 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/ee92b41b8809_create_quotas_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/ef08a5e057bd_remove_pod.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/fb03fdef8919_rename_baymodel_to_clustertemplate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/fcb4efee8f8b_add_version_info_to_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/sqlalchemy/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35260 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10399 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/db/sqlalchemy/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.790351 magnum-9.4.1/magnum/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.790351 magnum-9.4.1/magnum/drivers/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8363 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8966 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/k8s_monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/k8s_scale_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.790351 magnum-9.4.1/magnum/drivers/common/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.790351 magnum-9.4.1/magnum/drivers/common/templates/environments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/disable_floating_ip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/disable_lb_floating_ip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/enable_floating_ip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/enable_lb_floating_ip.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/no_etcd_volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/no_master_lb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/no_private_network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/no_volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/with_etcd_volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/with_master_lb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/with_master_lb_octavia.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/with_private_network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/environments/with_volume.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.794351 magnum-9.4.1/magnum/drivers/common/templates/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/api_gateway_switcher_master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/api_gateway_switcher_pool.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/atomic-install-openstack-ca.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/configure-docker-registry.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/configure-docker-storage.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/configure_docker_storage_driver_atomic.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/enable-docker-registry.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/floating_ip_address_switcher_private.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/floating_ip_address_switcher_public.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/network_switcher_existing.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/fragments/network_switcher_private.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.726349 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.798351 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/add-proxy.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18095 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/calico-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5280 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/configure-etcd.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20127 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11572 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-minion.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7177 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/core-dns-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/disable-selinux.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10555 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-healing.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5867 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-scaling.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-cert-api-manager.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15361 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-cinder-csi.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6190 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-helm-tiller.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-controller.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-octavia.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5282 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-traefik.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4381 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-keystone-auth.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18133 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-prometheus-monitoring.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-services-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-services-minion.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/flannel-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/install-clients.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/install-cri.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/install-helm-modules.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9726 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/kube-apiserver-to-kubelet-role.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12992 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/kube-dashboard-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3973 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/make-cert-client.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5807 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/make-cert.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/start-container-agent.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6893 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/upgrade-kubernetes.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/wc-notify-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5318 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/write-kube-os-config.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.798351 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6566 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/ingress-nginx.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2917 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/metrics-server.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/prometheus-adapter.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6006 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/prometheus-operator.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/lb_api.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/common/templates/lb_etcd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/network.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.726349 magnum-9.4.1/magnum/drivers/common/templates/swarm/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.798351 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/add-docker-daemon-options.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/add-proxy.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/cfn-signal.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/configure-etcd.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/configure-selinux.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/enable-services.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5473 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/make-cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1967 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/network-config-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3932 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/network-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/remove-docker-key.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1903 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/volume-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-cluster-failure-service.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-docker-socket.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-heat-params-master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-heat-params-node.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-network-config.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-swarm-agent-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-swarm-master-service.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.802351 magnum-9.4.1/magnum/drivers/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/heat/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    28929 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/heat/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4263 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/heat/k8s_coreos_template_def.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10785 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/heat/k8s_fedora_template_def.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12492 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/heat/k8s_template_def.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7607 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/heat/swarm_fedora_template_def.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9105 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/heat/swarm_mode_template_def.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23252 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/heat/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.802351 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.802351 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/COPYING
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/add-ext-ca-certs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/add-proxy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-docker.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-etcd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/create-kube-namespace.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-coredns.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-docker-mount.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2871 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-apiserver.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-controller-manager.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-dashboard.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-minion.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1311 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-scheduler.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3622 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4070 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-minion.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2794 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service-client.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3983 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert-client.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/wc-notify.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2047 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params-master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-kubeconfig.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-master-kubeconfig.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-network-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26277 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/kubecluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22817 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/kubemaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15708 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/kubeminion.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_coreos_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/COPYING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45204 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/kubecluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32470 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/kubemaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19581 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/kubeminion.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59046 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/tools/grafana-prometheus-dashboard.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/COPYING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6968 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/fcct-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45453 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/kubecluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32553 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/kubemaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19326 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/kubeminion.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7235 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/user_data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.730349 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.806351 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2454 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/Readme.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/elements-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/package-installs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2825 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22076 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubecluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17414 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubemaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3544 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10626 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion_software_configs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/COPYING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/docker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/docker/elements-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/docker/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/docker/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      107 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/docker/post-install.d/60-disable-docker-service
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/docker/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      482 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/docker/pre-install.d/10-add-docker-repo
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      396 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/install_imagebuild_deps.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/elements-deps
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/package-installs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/post-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      189 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/post-install.d/60-disable-upstart
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/pre-install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      545 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/pre-install.d/10-apt-repo
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      812 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/validate_image.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/scale_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.810351 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-ext-ca-certs.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-proxy.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-slave.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/start-services-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/start-services-slave.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/volume-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/write-heat-params-master.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/write-heat-params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6252 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesos_slave_software_configs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16168 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesoscluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3620 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesosmaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2686 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesosslave.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.814351 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.730349 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.814351 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/README.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      203 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/run_openvswitch_neutron.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4058 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.814351 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/COPYING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3304 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16383 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/cluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16265 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmmaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13829 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmnode.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.814351 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1416 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/monitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/template_def.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.814351 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.814351 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-heat-params-master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2141 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-master-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-worker-service.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16276 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmcluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11758 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmmaster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10475 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmnode.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.814351 magnum-9.4.1/magnum/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/hacking/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6064 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3024 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14538 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/objects/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10996 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/objects/cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8862 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5399 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6026 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/magnum_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8663 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/objects/nodegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5467 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/objects/x509keypair.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/service/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10685 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/service/periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/servicegroup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/servicegroup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2139 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/servicegroup/magnum_service_periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5373 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/conf_fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/tests/contrib/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10717 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/contrib/copy_instance_logs.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5231 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/contrib/gate_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8987 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/contrib/post_test_hook.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/fake_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4272 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/tests/functional/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6060 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/tests/functional/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.818352 magnum-9.4.1/magnum/tests/functional/api/v1/clients/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/clients/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5820 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/clients/bay_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3730 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/clients/baymodel_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/clients/cert_client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6399 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/clients/cluster_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/clients/cluster_template_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/clients/magnum_service_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/api/v1/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/bay_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/baymodel_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2421 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/baymodelpatch_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/baypatch_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/cert_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_id_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_template_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2509 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_templatepatch_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/clusterpatch_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/api/v1/models/magnum_service_model.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3527 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19161 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/datagen.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3607 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/k8s/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/k8s/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/k8s/test_k8s_python_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/k8s/test_magnum_python_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/k8s_coreos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/k8s_coreos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/k8s_coreos/test_k8s_python_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/k8s_ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/k8s_ironic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/k8s_ironic/test_k8s_python_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/mesos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/mesos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/mesos/test_mesos_python_client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    21518 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/python_client_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/swarm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/swarm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6469 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/swarm/test_swarm_python_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/functional/swarm_mode/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/swarm_mode/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4769 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/functional/swarm_mode/test_swarm_mode_python_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1832 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/output_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/policy_fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.822352 magnum-9.4.1/magnum/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.826352 magnum-9.4.1/magnum/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10570 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.826352 magnum-9.4.1/magnum/tests/unit/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/auth-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/auth-root-access.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/auth-v1-access.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/noauth-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16026 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11173 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/test_root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.826352 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44710 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_bay.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52056 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_baymodel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11777 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50401 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11169 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_cluster_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    66227 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17993 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_magnum_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31661 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_nodegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14704 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5847 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10056 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6642 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/api/test_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16217 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/test_attr_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/test_expose.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5996 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/test_hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5593 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/test_servicegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14320 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/api/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.830352 magnum-9.4.1/magnum/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4999 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/cmd/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/cmd/test_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/cmd/test_db_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3260 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/cmd/test_driver_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.830352 magnum-9.4.1/magnum/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.830352 magnum-9.4.1/magnum/tests/unit/common/cert_manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/cert_manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11405 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_barbican.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_cert_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4399 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_x509keypair_cert_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15573 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4717 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3968 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_docker_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10304 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12645 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6992 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_octavia.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3194 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9278 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2130 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/test_short_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1921 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_urlfetch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11261 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.830352 magnum-9.4.1/magnum/tests/unit/common/x509/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/x509/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2484 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/x509/test_operations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10086 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/common/x509/test_sign.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4756 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/common/x509/test_validator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.834352 magnum-9.4.1/magnum/tests/unit/conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conductor/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.834352 magnum-9.4.1/magnum/tests/unit/conductor/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.834352 magnum-9.4.1/magnum/tests/unit/conductor/handlers/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23005 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/common/test_cert_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4904 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/common/test_trust_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2444 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_ca_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29079 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_cluster_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_conductor_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_federation_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3375 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_indirection_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59894 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_k8s_cluster_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23960 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_mesos_cluster_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11632 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_nodegroup_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31727 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_swarm_cluster_conductor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.834352 magnum-9.4.1/magnum/tests/unit/conductor/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conductor/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4943 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/tasks/test_heat_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/test_k8s_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22416 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/test_monitors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5304 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9509 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/test_scale_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9703 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conductor/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.834352 magnum-9.4.1/magnum/tests/unit/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2828 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/conf/test_conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.834352 magnum-9.4.1/magnum/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.834352 magnum-9.4.1/magnum/tests/unit/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3065 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/sqlalchemy/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11885 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9628 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/test_cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10339 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/test_federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4024 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/test_magnum_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10069 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/test_nodegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4403 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/db/test_x509keypair.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14527 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/db/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/magnum/tests/unit/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30740 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/drivers/test_heat_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/drivers/test_k8s_fedora_atomic_v1_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    94549 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/drivers/test_template_definition.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/magnum/tests/unit/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10689 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/objects/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7375 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/objects/test_cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8231 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/objects/test_federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6135 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/objects/test_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5534 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/objects/test_magnum_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8725 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/objects/test_nodegroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17862 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/objects/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6968 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/objects/test_x509keypair.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/objects/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/magnum/tests/unit/service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/service/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22261 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/service/test_periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/magnum/tests/unit/servicegroup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/servicegroup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/servicegroup/test_magnum_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/magnum/tests/unit/template/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/template/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/unit/template/test_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9789 2021-03-24 15:40:08.000000 magnum-9.4.1/magnum/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2021-03-24 15:40:07.000000 magnum-9.4.1/magnum/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.762350 magnum-9.4.1/magnum.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54210 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-03-24 15:40:57.000000 magnum-9.4.1/magnum.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1900 2021-03-24 15:40:07.000000 magnum-9.4.1/playbooks/container-builder-copy-logs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2021-03-24 15:40:08.000000 magnum-9.4.1/playbooks/container-builder-setup-gate.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2021-03-24 15:40:08.000000 magnum-9.4.1/playbooks/container-builder-vars.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4097 2021-03-24 15:40:08.000000 magnum-9.4.1/playbooks/container-builder.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1561 2021-03-24 15:40:08.000000 magnum-9.4.1/playbooks/container-publish.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4064 2021-03-24 15:40:07.000000 magnum-9.4.1/playbooks/magnum-functional-base.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/playbooks/post/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-03-24 15:40:07.000000 magnum-9.4.1/playbooks/post/upload-logs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.838352 magnum-9.4.1/playbooks/pre/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-03-24 15:40:07.000000 magnum-9.4.1/playbooks/pre/prepare-workspace-images.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2021-03-24 15:40:07.000000 magnum-9.4.1/playbooks/pre/prepare-workspace.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.734349 magnum-9.4.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.854353 magnum-9.4.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/CVE-2016-7404-f53e62a4a40e4d30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/RBAC-and-client-incompatibility-fdfeab326dfda3bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-container_infra_prefix-516cc43fbc5a0617.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-docker-storage-driver-to-baymodel-1ed9ba8d43ecfea1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-federation-api-cf55d04f96772b0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-hostgw-backend-option-1d1f9d8d95ec374f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-information-about-cluster-in-event-notifications-a3c992ab24b32fbd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-k8s-label-for-portal-network-cidr-a09edab29da6e7da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-kubelet-to-master-nodes-da2d4ea0d3a332cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-octavia-client-4e5520084eae3c2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-opensuse-driver-f69b6d346ca82b87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-overlay-networks-to-swarm-4467986d7853fcd8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/add-upgrade-check-framework-5057ad67a7690a14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/affinity-policy-for-mesos-template-def-82627eb231aa4d28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/allow-cluster-template-being-renamed-82f7d5d1f33a7957.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/allow-multimaster-no-fip-b11520485012d949.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/allow-setting-network-subnet-FIP-when-creating-cluster-ae0cda35ade28a9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/async-bay-operations-support-9819bd06122ea9e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/availability_zone-2d73671f5ea065d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/boot-from-volume-7c73df68d7f325aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-add-kube-dashboard-8a9f7d7c73c2debd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-auto-generate-name-052ea3fdf05fdbbf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-barbican-alternative-store-35ec3eda0abb0e25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-container-monitoring-d4bb1cbd0a4e44cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-decouple-lbaas-c8f2d73313c40b98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-keypair-override-on-create-ca8f12ffca41cd62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-magnum-notifications-8bd44cfe9e80f82b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-mesos-slave-flags-de6cf8c4d2c3c916.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bp-secure-etcd-cluster-coe-5abd22546f05a85b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/broken-kuberenetes-client-d2d1da6029825208.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-1580704-32a0e91e285792ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-1614596-support-ssl-magnum-api-e4896928c6562e03.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-1663757-198e1aa8fa810984.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-1697655-add-etcd-volume-size-label-abde0060595bbbeb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-1718947-0d4e67529e2817d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-1722522-d94743c6362a5e48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-1766284-k8s-fedora-admin-user-e760f9b0edf49391.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-2002728-kube-os-conf-region-46cd60537bdabdb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-2002981-trustee-auth-region-name-37796a4e6a274fb8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/bug-2004942-052321df27529562.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/calico-network-driver-0199c2459041ae81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/cert-manager-api-ee0cf7f3b767bb5d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/change-bay-to-cluster-in-config-1f2b95d1176d7231.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/change-service-name-ce5c72642fe1d3d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/cinder-csi-enabled-label-ab2b8ade63c57cf3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/client-embed-certs-322701471e4d6e1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/cluster_template_update_labels-10ce66c87795f11c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/configurable-k8s-health-polling-interval-75bb83b4701d48c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/configure-etcd-auth-bug-1759813-baac5e0fe8a2e97f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/containerd-598761bb536af6ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/coredns-update-9b03da4b89be18ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/default-policy-k8s-keystone-auth-fa74aa03dcc12ef3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/deploy-tiller-in-k8s-df12ee41d00dd7ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/deprecate-send_cluster_metrics-8adaac64a979f720.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/disable-ssh-password-authn-f2baf619710e52aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/dns-autoscale-90b63e3d71d7794e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/docker-volume-type-46044734f5a27661.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/enable_cloud_provider_label-ed79295041bc46a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/ensure-delete-complete-2f9bb53616e1e02b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fedora_coreos-e66b44d86dea380f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-cert-apimanager-527352622c5a9c3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-cluster-floating-ip-enabled-default-value-4e24d4bf09fc08c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-cluster-update-886bd2d1156bef88.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-fedora-proxy-a4b8d5fc4ec65e80.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-global-stack-list-7a3a66169f5c4aa8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-k8s-coe-version-a8ea38f327ea6bb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-nginx-getting-oom-killed-76139fd8b57e6c15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-proxy-of-grafana-script-8b408d9d103dfc06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-race-condition-for-k8s-multi-masters-29bd36de57df355a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/fix-serveraddressoutputmapping-for-private-clusters-73a874bb4827d568.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/flannel-cni-4a5c9f574325761e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/flannel-reboot-fix-f1382818daed4fa8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/grafana_prometheus_tag_label-78540ea106677485.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/heapster-enabled-label-292ca1ddac68a156.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/heat-container-agent-for-train-e63bc1559750fe9c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/heat-container-agent-tag-92848c1062c16c76.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/heat-container-agent-tag-fe7cec6b890329af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/helm-install-ingress-nginx-fe2acec1dd3032e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/helm-install-metrics-service-cd18be76c4ed0e5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/helm-install-metrics-service-e7a5459417504a75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/helm-install-prometheus-operator-ea87752bc57a0945.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/ignore-calico-devices-in-network-manager-e1bdb052834e11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/improve-k8s-master-kubelet-taint-0c56ffede270116d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/ingress-controller-552ea956ceabdd25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/integrate-osprofiler-79bdf2d0cd8a39fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-cluster-creation-speedup-21b5b368184d7bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-delete-vip-fip-b2ddf61ddbc080bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-fedora-atomic-rolling-upgrade-3d8edcdd91fa1529.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-improve-floating-ip-enabled-84cd00224d6b7bc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-keystone-auth-6c88c1a2d406fb61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-nodes-security-group-9d8dbb91b006d9dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-octavia-ingress-controller-32c0b97031fd0dd4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s-prometheus-clusterip-b191fa163e3f1125.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s_fedora_atomic_apply_cluster_role-8a46c881de1a1fa3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/k8s_fedora_protect_kubelet-8468ddcb92c2a624.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/keystone-auth-repo-6970c05f44299326.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/keystone_trustee_interface-6d63b74616dda1d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/kubelet-nfs-b51e572adfb56378.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/kubernetes-cloud-config-6c9a4bfec47e3bb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/make-keypair-optional-fcf4a17e440d0879.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/no-cinder-volume-87b9339e066c30a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/nodegroup-limit-89930d45ee06c621.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/podsecuritypolicy-2400063d73524e06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/pre-delete-cluster-5e27cfdf45e25805.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/prometheus-adapter-15fba9d739676e70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/prometheus-operator-compatible-with-k8s-1-16-f8be99cf527075b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/quota-api-182cd1bc9e706b17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/remove-container-endpoint-3494eb8bd2406e87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/rename-minion-to-node-9d32fe77d765f149.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/resize-api-2bf1fb164484dea9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/return-clusterid-for-resize-upgrade-6e841c7b568fa807.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/return-server-id-in-kubeminion-cb33f5141e0b7fa9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/rollback-bay-on-update-failure-83e5ff8a7904d5c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/rotate-cluster-cert-9f84deb0adf9afb1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/server-groups-for-both-master-and-workder-bdd491e4323955d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/set-traefik-tag-7d4aca5685147970.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/stats-api-68bc66147ac027e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/strip-ca-certificate-a09d0c31c45973df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-all-tenants-for-admin-a042f5c520d35837.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-auto-healing-3e07c16c55209b0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-auto-healing-controller-333d1266918111e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-fedora-atomic-os-upgrade-9f47182b21c6c028.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-multi-dns-server-0528be20f0e6aa62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-octavia-for-k8s-service-d5d7fd041f9d76fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-policy-and-doc-in-code-0c19e479dbd953c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support-sha256-verification-for-hyperkube-fb2292c6a8bb00ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/support_nodes_affinity_policy-22253fb9cf6739ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/swarm-integration-with-cinder-e3068138a3f75dbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/swarm-live-restore-b03ad192367abced.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/sync-service-account-keys-for-multi-masters-71217c4cf4dd472c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/traefik-compatible-with-k8s-1-16-9a9ef6d3ccc92fb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/update-kubernetes-dashboard-5196831c32d55aee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/update-swarm-73d4340a881bff2f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/update-to-f27-cc8aa873cdf111bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/upgrade-api-975233ab93c0c092.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/upgrade-to-k8s-v1.11.1-8065fd768873295d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/upgrade_api-1fecc206e5b0ef99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/use_podman-39532143be2296c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/notes/using-vxlan-for-flannel-backend-8d82a290ca97d6e2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8574 2021-03-24 15:40:08.000000 magnum-9.4.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2021-03-24 15:40:08.000000 magnum-9.4.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.734349 magnum-9.4.1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.734349 magnum-9.4.1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52681 2021-03-24 15:40:08.000000 magnum-9.4.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.734349 magnum-9.4.1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2021-03-24 15:40:08.000000 magnum-9.4.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.734349 magnum-9.4.1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33751 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-03-24 15:40:07.000000 magnum-9.4.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2021-03-24 15:40:08.000000 magnum-9.4.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2484 2021-03-24 15:40:57.862353 magnum-9.4.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-03-24 15:40:08.000000 magnum-9.4.1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18077 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/async-container-operation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12077 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/bay-drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19422 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/container-networking-model.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19477 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/container-volume-integration-model.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19706 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/containers-service.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6005 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/create-trustee-user-for-each-bay.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6976 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/flatten_attributes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/magnum-horizon-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6530 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/open-dcos.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10402 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/resource-quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6802 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/stats-api-spec.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6278 2021-03-24 15:40:07.000000 magnum-9.4.1/specs/tls-support-magnum.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2021-03-24 15:40:08.000000 magnum-9.4.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-03-24 15:40:57.858353 magnum-9.4.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2502 2021-03-24 15:40:08.000000 magnum-9.4.1/tools/cover.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      515 2021-03-24 15:40:07.000000 magnum-9.4.1/tools/flake8wrap.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5956 2021-03-24 15:40:08.000000 magnum-9.4.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-scheduler/config.json.template` & `magnum-9.4.1/dockerfiles/kubernetes-scheduler/config.json.template`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-scheduler/Dockerfile` & `magnum-9.4.1/dockerfiles/kubernetes-scheduler/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-scheduler/config` & `magnum-9.4.1/dockerfiles/kubernetes-apiserver/config`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-proxy/config.json.template` & `magnum-9.4.1/dockerfiles/kubernetes-proxy/config.json.template`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-proxy/Dockerfile` & `magnum-9.4.1/dockerfiles/kubernetes-proxy/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-proxy/config` & `magnum-9.4.1/dockerfiles/kubernetes-controller-manager/config`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-apiserver/config.json.template` & `magnum-9.4.1/dockerfiles/kubernetes-apiserver/config.json.template`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-apiserver/Dockerfile` & `magnum-9.4.1/dockerfiles/kubernetes-apiserver/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-apiserver/apiserver` & `magnum-9.4.1/dockerfiles/kubernetes-apiserver/apiserver`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-apiserver/config` & `magnum-9.4.1/dockerfiles/kubernetes-kubelet/config`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/config.json.template` & `magnum-9.4.1/dockerfiles/heat-container-agent/config.json.template`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/Dockerfile` & `magnum-9.4.1/dockerfiles/heat-container-agent/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/heat-config-notify` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/heat-config-notify`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/write-os-apply-config-templates.sh` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/write-os-apply-config-templates.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/configure_container_agent.sh` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/configure_container_agent.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/hooks/script` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/hooks/script`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/hooks/atomic` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/hooks/atomic`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/hooks/docker-compose` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/hooks/docker-compose`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/55-heat-config` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/55-heat-config`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/heat-container-agent/scripts/50-heat-config-docker-compose` & `magnum-9.4.1/dockerfiles/heat-container-agent/scripts/50-heat-config-docker-compose`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-controller-manager/config.json.template` & `magnum-9.4.1/dockerfiles/kubernetes-controller-manager/config.json.template`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-controller-manager/Dockerfile` & `magnum-9.4.1/dockerfiles/kubernetes-controller-manager/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-controller-manager/config` & `magnum-9.4.1/dockerfiles/kubernetes-proxy/config`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-kubelet/config.json.template` & `magnum-9.4.1/dockerfiles/kubernetes-kubelet/config.json.template`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-kubelet/Dockerfile` & `magnum-9.4.1/dockerfiles/kubernetes-kubelet/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-kubelet/kubelet` & `magnum-9.4.1/dockerfiles/kubernetes-kubelet/kubelet`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/dockerfiles/kubernetes-kubelet/config` & `magnum-9.4.1/dockerfiles/kubernetes-scheduler/config`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/AUTHORS` & `magnum-9.4.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/playbooks/pre/prepare-workspace.yaml` & `magnum-9.4.1/playbooks/pre/prepare-workspace.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/playbooks/container-publish.yaml` & `magnum-9.4.1/playbooks/container-publish.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/playbooks/container-builder-vars.yaml` & `magnum-9.4.1/playbooks/container-builder-vars.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/playbooks/magnum-functional-base.yaml` & `magnum-9.4.1/playbooks/magnum-functional-base.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/playbooks/container-builder.yaml` & `magnum-9.4.1/playbooks/container-builder.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/playbooks/container-builder-copy-logs.yaml` & `magnum-9.4.1/playbooks/container-builder-copy-logs.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum.egg-info/requires.txt` & `magnum-9.4.1/magnum.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 [:(python_version=='2.7' or python_version=='2.6' or python_version=='3.3')]
 enum34>=1.0.4
 
 [osprofiler]
 osprofiler>=1.4.0
 
 [test]
-bandit!=1.6.0,>=1.1.0
+bandit<=1.6.2,>=1.1.0
 bashate>=0.5.1
 coverage!=4.4,>=4.0
 doc8>=0.6.0
 fixtures>=3.0.0
 hacking!=0.13.0,<0.14,>=0.12.0
 mock>=2.0.0
 os-testr>=1.0.0
```

### Comparing `magnum-9.4.0/magnum.egg-info/PKG-INFO` & `magnum-9.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum
-Version: 9.4.0
+Version: 9.4.1
 Summary: Container Management project for OpenStack
 Home-page: http://docs.openstack.org/magnum/latest/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `magnum-9.4.0/magnum.egg-info/SOURCES.txt` & `magnum-9.4.1/magnum.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -936,14 +936,15 @@
 releasenotes/notes/default-policy-k8s-keystone-auth-fa74aa03dcc12ef3.yaml
 releasenotes/notes/deploy-tiller-in-k8s-df12ee41d00dd7ff.yaml
 releasenotes/notes/deprecate-send_cluster_metrics-8adaac64a979f720.yaml
 releasenotes/notes/disable-ssh-password-authn-f2baf619710e52aa.yaml
 releasenotes/notes/dns-autoscale-90b63e3d71d7794e.yaml
 releasenotes/notes/docker-volume-type-46044734f5a27661.yaml
 releasenotes/notes/enable_cloud_provider_label-ed79295041bc46a8.yaml
+releasenotes/notes/ensure-delete-complete-2f9bb53616e1e02b.yaml
 releasenotes/notes/fedora_coreos-e66b44d86dea380f.yaml
 releasenotes/notes/fix-cert-apimanager-527352622c5a9c3b.yaml
 releasenotes/notes/fix-cluster-floating-ip-enabled-default-value-4e24d4bf09fc08c8.yaml
 releasenotes/notes/fix-cluster-update-886bd2d1156bef88.yaml
 releasenotes/notes/fix-fedora-proxy-a4b8d5fc4ec65e80.yaml
 releasenotes/notes/fix-global-stack-list-7a3a66169f5c4aa8.yaml
 releasenotes/notes/fix-k8s-coe-version-a8ea38f327ea6bb3.yaml
```

### Comparing `magnum-9.4.0/magnum.egg-info/entry_points.txt` & `magnum-9.4.1/magnum.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/HACKING.rst` & `magnum-9.4.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/admin/troubleshooting-guide.rst` & `magnum-9.4.1/doc/source/admin/troubleshooting-guide.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/admin/magnum-proxy.rst` & `magnum-9.4.1/doc/source/admin/magnum-proxy.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/admin/gmr.rst` & `magnum-9.4.1/doc/source/admin/gmr.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/admin/configuring.rst` & `magnum-9.4.1/doc/source/admin/configuring.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/admin/index.rst` & `magnum-9.4.1/doc/source/admin/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/quickstart.rst` & `magnum-9.4.1/doc/source/contributor/quickstart.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/functional-test.rst` & `magnum-9.4.1/doc/source/contributor/functional-test.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/api-microversion.rst` & `magnum-9.4.1/doc/source/contributor/api-microversion.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/objects.rst` & `magnum-9.4.1/doc/source/contributor/objects.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/reno.rst` & `magnum-9.4.1/doc/source/contributor/reno.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/troubleshooting.rst` & `magnum-9.4.1/doc/source/contributor/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/policies.rst` & `magnum-9.4.1/doc/source/contributor/policies.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/contributor/index.rst` & `magnum-9.4.1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/images/MagnumVolumeIntegration.png` & `magnum-9.4.1/doc/source/images/MagnumVolumeIntegration.png`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/images/cluster-create.png` & `magnum-9.4.1/doc/source/images/cluster-create.png`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/images/cluster-template-details.png` & `magnum-9.4.1/doc/source/images/cluster-template-details.png`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/images/cluster-template.png` & `magnum-9.4.1/doc/source/images/cluster-template.png`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/cli/magnum-status.rst` & `magnum-9.4.1/doc/source/cli/magnum-status.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/conf.py` & `magnum-9.4.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/user/k8s-keystone-authN-authZ.rst` & `magnum-9.4.1/doc/source/user/k8s-keystone-authN-authZ.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/user/glossary.rst` & `magnum-9.4.1/doc/source/user/glossary.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/user/cluster-type-definition.rst` & `magnum-9.4.1/doc/source/user/cluster-type-definition.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/user/kubernetes-load-balancer.rst` & `magnum-9.4.1/doc/source/user/kubernetes-load-balancer.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/user/heat-templates.rst` & `magnum-9.4.1/doc/source/user/heat-templates.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/user/rolling-upgrade.rst` & `magnum-9.4.1/doc/source/user/rolling-upgrade.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/user/index.rst` & `magnum-9.4.1/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/verify.rst` & `magnum-9.4.1/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/install.rst` & `magnum-9.4.1/doc/source/install/install.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/install-rdo.rst` & `magnum-9.4.1/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/install-debian-manual.rst` & `magnum-9.4.1/doc/source/install/install-debian-manual.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/install-guide-from-source.rst` & `magnum-9.4.1/doc/source/install/install-guide-from-source.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/common/configure_2_edit_magnum_conf.rst` & `magnum-9.4.1/doc/source/install/common/configure_2_edit_magnum_conf.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/common/prerequisites.rst` & `magnum-9.4.1/doc/source/install/common/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/get_started.rst` & `magnum-9.4.1/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/launch-instance.rst` & `magnum-9.4.1/doc/source/install/launch-instance.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/install-ubuntu.rst` & `magnum-9.4.1/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/index.rst` & `magnum-9.4.1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/install/install-obs.rst` & `magnum-9.4.1/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/doc/source/index.rst` & `magnum-9.4.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/README.rst` & `magnum-9.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/CONTRIBUTING.rst` & `magnum-9.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/PKG-INFO` & `magnum-9.4.1/magnum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum
-Version: 9.4.0
+Version: 9.4.1
 Summary: Container Management project for OpenStack
 Home-page: http://docs.openstack.org/magnum/latest/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `magnum-9.4.0/devstack/settings` & `magnum-9.4.1/devstack/settings`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/devstack/plugin.sh` & `magnum-9.4.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/devstack/README.rst` & `magnum-9.4.1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/devstack/lib/magnum` & `magnum-9.4.1/devstack/lib/magnum`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/.zuul.yaml` & `magnum-9.4.1/.zuul.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -305,27 +305,25 @@
     secrets:
       - magnum_docker_login
     timeout: 1200
 
 - project:
     templates:
       - openstack-cover-jobs
-      - openstack-lower-constraints-jobs
       - openstack-python-jobs
       - openstack-python3-train-jobs
       - check-requirements
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - magnum-functional-api
         - magnum-functional-api-python2
         - openstack-tox-cover:
            voting: false
-        - magnum-container-build
     gate:
       queue: magnum
       jobs:
         - magnum-functional-api
         - magnum-functional-api-python2
     experimental:
       jobs:
```

### Comparing `magnum-9.4.0/releasenotes/notes/remove-container-endpoint-3494eb8bd2406e87.yaml` & `magnum-9.4.1/releasenotes/notes/remove-container-endpoint-3494eb8bd2406e87.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/bug-1663757-198e1aa8fa810984.yaml` & `magnum-9.4.1/releasenotes/notes/bug-1663757-198e1aa8fa810984.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/change-bay-to-cluster-in-config-1f2b95d1176d7231.yaml` & `magnum-9.4.1/releasenotes/notes/change-bay-to-cluster-in-config-1f2b95d1176d7231.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/add-hostgw-backend-option-1d1f9d8d95ec374f.yaml` & `magnum-9.4.1/releasenotes/notes/add-hostgw-backend-option-1d1f9d8d95ec374f.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/support-policy-and-doc-in-code-0c19e479dbd953c9.yaml` & `magnum-9.4.1/releasenotes/notes/support-policy-and-doc-in-code-0c19e479dbd953c9.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/boot-from-volume-7c73df68d7f325aa.yaml` & `magnum-9.4.1/releasenotes/notes/boot-from-volume-7c73df68d7f325aa.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/k8s-improve-floating-ip-enabled-84cd00224d6b7bc1.yaml` & `magnum-9.4.1/releasenotes/notes/k8s-improve-floating-ip-enabled-84cd00224d6b7bc1.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/RBAC-and-client-incompatibility-fdfeab326dfda3bf.yaml` & `magnum-9.4.1/releasenotes/notes/RBAC-and-client-incompatibility-fdfeab326dfda3bf.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/add-container_infra_prefix-516cc43fbc5a0617.yaml` & `magnum-9.4.1/releasenotes/notes/add-container_infra_prefix-516cc43fbc5a0617.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/fix-race-condition-for-k8s-multi-masters-29bd36de57df355a.yaml` & `magnum-9.4.1/releasenotes/notes/fix-race-condition-for-k8s-multi-masters-29bd36de57df355a.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/add-information-about-cluster-in-event-notifications-a3c992ab24b32fbd.yaml` & `magnum-9.4.1/releasenotes/notes/add-information-about-cluster-in-event-notifications-a3c992ab24b32fbd.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/docker-volume-type-46044734f5a27661.yaml` & `magnum-9.4.1/releasenotes/notes/docker-volume-type-46044734f5a27661.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/k8s-nodes-security-group-9d8dbb91b006d9dd.yaml` & `magnum-9.4.1/releasenotes/notes/k8s-nodes-security-group-9d8dbb91b006d9dd.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/upgrade_api-1fecc206e5b0ef99.yaml` & `magnum-9.4.1/releasenotes/notes/upgrade_api-1fecc206e5b0ef99.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/use_podman-39532143be2296c2.yaml` & `magnum-9.4.1/releasenotes/notes/use_podman-39532143be2296c2.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/k8s_fedora_protect_kubelet-8468ddcb92c2a624.yaml` & `magnum-9.4.1/releasenotes/notes/k8s_fedora_protect_kubelet-8468ddcb92c2a624.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/add-docker-storage-driver-to-baymodel-1ed9ba8d43ecfea1.yaml` & `magnum-9.4.1/releasenotes/notes/add-docker-storage-driver-to-baymodel-1ed9ba8d43ecfea1.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/async-bay-operations-support-9819bd06122ea9e5.yaml` & `magnum-9.4.1/releasenotes/notes/async-bay-operations-support-9819bd06122ea9e5.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/bp-keypair-override-on-create-ca8f12ffca41cd62.yaml` & `magnum-9.4.1/releasenotes/notes/bp-keypair-override-on-create-ca8f12ffca41cd62.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/helm-install-metrics-service-e7a5459417504a75.yaml` & `magnum-9.4.1/releasenotes/notes/helm-install-metrics-service-e7a5459417504a75.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/broken-kuberenetes-client-d2d1da6029825208.yaml` & `magnum-9.4.1/releasenotes/notes/broken-kuberenetes-client-d2d1da6029825208.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/CVE-2016-7404-f53e62a4a40e4d30.yaml` & `magnum-9.4.1/releasenotes/notes/CVE-2016-7404-f53e62a4a40e4d30.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/configurable-k8s-health-polling-interval-75bb83b4701d48c5.yaml` & `magnum-9.4.1/releasenotes/notes/configurable-k8s-health-polling-interval-75bb83b4701d48c5.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/fix-global-stack-list-7a3a66169f5c4aa8.yaml` & `magnum-9.4.1/releasenotes/notes/fix-global-stack-list-7a3a66169f5c4aa8.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/containerd-598761bb536af6ba.yaml` & `magnum-9.4.1/releasenotes/notes/containerd-598761bb536af6ba.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/deploy-tiller-in-k8s-df12ee41d00dd7ff.yaml` & `magnum-9.4.1/releasenotes/notes/deploy-tiller-in-k8s-df12ee41d00dd7ff.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/kubernetes-cloud-config-6c9a4bfec47e3bb4.yaml` & `magnum-9.4.1/releasenotes/notes/kubernetes-cloud-config-6c9a4bfec47e3bb4.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/k8s-fedora-atomic-rolling-upgrade-3d8edcdd91fa1529.yaml` & `magnum-9.4.1/releasenotes/notes/k8s-fedora-atomic-rolling-upgrade-3d8edcdd91fa1529.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/deprecate-send_cluster_metrics-8adaac64a979f720.yaml` & `magnum-9.4.1/releasenotes/notes/deprecate-send_cluster_metrics-8adaac64a979f720.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/notes/fedora_coreos-e66b44d86dea380f.yaml` & `magnum-9.4.1/releasenotes/notes/fedora_coreos-e66b44d86dea380f.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/source/conf.py` & `magnum-9.4.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `magnum-9.4.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `magnum-9.4.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `magnum-9.4.1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/releasenotes/source/index.rst` & `magnum-9.4.1/releasenotes/source/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/lower-constraints.txt` & `magnum-9.4.1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/setup.cfg` & `magnum-9.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/requirements.txt` & `magnum-9.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/templates/example/example_template/example.yaml` & `magnum-9.4.1/contrib/templates/example/example_template/example.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/templates/example/example_template/__init__.py` & `magnum-9.4.1/contrib/templates/example/example_template/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/templates/example/setup.py` & `magnum-9.4.1/contrib/templates/example/setup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/COPYING` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/COPYING`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/kubeminion.yaml` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/kubeminion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-minion.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-minion.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-master.yaml` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-master.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-master.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-master.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-minion.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-kubernetes-minion.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-docker.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-docker.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-etcd.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-etcd.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-minion.yaml` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-heat-params-minion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-master.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/configure-flanneld-master.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-kubeconfig.yaml` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/write-kubeconfig.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/add-proxy.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/add-proxy.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert-client.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/fragments/make-cert-client.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/kubecluster.yaml` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/kubecluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/README.md` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/README.md`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/templates/kubemaster.yaml` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/templates/kubemaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/version.py` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/template_def.py` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/driver.py` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/config.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/config.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/openSUSE-Leap-42.1-JeOS-for-OpenStack-Magnum-K8s.kiwi` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/openSUSE-Leap-42.1-JeOS-for-OpenStack-Magnum-K8s.kiwi`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/images.sh` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/images.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/image/README.md` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/image/README.md`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/k8s_opensuse_v1/setup.py` & `magnum-9.4.1/contrib/drivers/k8s_opensuse_v1/setup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/heat/dcos_centos_template_def.py` & `magnum-9.4.1/contrib/drivers/heat/dcos_centos_template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/dcosslave.yaml` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/dcosslave.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/secgroup.yaml` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/secgroup.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/dcosmaster.yaml` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/dcosmaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/fragments/write-heat-params.sh` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/fragments/write-heat-params.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/fragments/configure-dcos.sh` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/fragments/configure-dcos.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/lb.yaml` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/lb.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/templates/dcoscluster.yaml` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/templates/dcoscluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/version.py` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/template_def.py` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/monitor.py` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/scale_manager.py` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/scale_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/driver.py` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/README.md` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/README.md`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/install.d/50-install-docker` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/install.d/50-install-docker`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/20-configure-docker-service` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/20-configure-docker-service`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/10-enable-overlay` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/docker/pre-install.d/10-enable-overlay`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/validate_dcos_image.sh` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/validate_dcos_image.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/dcos/extra-data.d/99-download-generate-config` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/dcos/extra-data.d/99-download-generate-config`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/contrib/drivers/dcos_centos_v1/image/README.md` & `magnum-9.4.1/contrib/drivers/dcos_centos_v1/image/README.md`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/tools/flake8wrap.sh` & `magnum-9.4.1/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/tools/cover.sh` & `magnum-9.4.1/tools/cover.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/cmd/status.py` & `magnum-9.4.1/magnum/cmd/status.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/cmd/db_manage.py` & `magnum-9.4.1/magnum/cmd/db_manage.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/cmd/api.py` & `magnum-9.4.1/magnum/cmd/api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/cmd/conductor.py` & `magnum-9.4.1/magnum/cmd/conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/cmd/driver_manage.py` & `magnum-9.4.1/magnum/cmd/driver_manage.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/cmd/__init__.py` & `magnum-9.4.1/magnum/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/swarm/test_swarm_python_client.py` & `magnum-9.4.1/magnum/tests/functional/swarm/test_swarm_python_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/mesos/test_mesos_python_client.py` & `magnum-9.4.1/magnum/tests/functional/mesos/test_mesos_python_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/k8s/test_k8s_python_client.py` & `magnum-9.4.1/magnum/tests/functional/k8s/test_k8s_python_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/k8s/test_magnum_python_client.py` & `magnum-9.4.1/magnum/tests/functional/k8s/test_magnum_python_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/baymodelpatch_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/baymodelpatch_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/baypatch_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/baypatch_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_templatepatch_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_templatepatch_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_template_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_template_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/cert_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/cert_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/baymodel_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/baymodel_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/bay_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/bay_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/cluster_id_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/cluster_id_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/magnum_service_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/magnum_service_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/models/clusterpatch_model.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/models/clusterpatch_model.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/clients/cluster_template_client.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/clients/cluster_template_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/clients/baymodel_client.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/clients/baymodel_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/clients/bay_client.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/clients/bay_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/clients/cluster_client.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/clients/cluster_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/clients/cert_client.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/clients/cert_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/v1/clients/magnum_service_client.py` & `magnum-9.4.1/magnum/tests/functional/api/v1/clients/magnum_service_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/api/base.py` & `magnum-9.4.1/magnum/tests/functional/api/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/swarm_mode/test_swarm_mode_python_client.py` & `magnum-9.4.1/magnum/tests/functional/swarm_mode/test_swarm_mode_python_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/python_client_base.py` & `magnum-9.4.1/magnum/tests/functional/python_client_base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/k8s_ironic/test_k8s_python_client.py` & `magnum-9.4.1/magnum/tests/functional/k8s_ironic/test_k8s_python_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/common/models.py` & `magnum-9.4.1/magnum/tests/functional/common/models.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/common/utils.py` & `magnum-9.4.1/magnum/tests/functional/common/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/common/manager.py` & `magnum-9.4.1/magnum/tests/functional/common/manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/common/config.py` & `magnum-9.4.1/magnum/tests/functional/common/config.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/common/datagen.py` & `magnum-9.4.1/magnum/tests/functional/common/datagen.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/common/client.py` & `magnum-9.4.1/magnum/tests/functional/common/client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/common/base.py` & `magnum-9.4.1/magnum/tests/functional/common/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/__init__.py` & `magnum-9.4.1/magnum/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/functional/k8s_coreos/test_k8s_python_client.py` & `magnum-9.4.1/magnum/tests/functional/k8s_coreos/test_k8s_python_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/fakes.py` & `magnum-9.4.1/magnum/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/conf_fixture.py` & `magnum-9.4.1/magnum/tests/conf_fixture.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/utils.py` & `magnum-9.4.1/magnum/tests/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/policy_fixture.py` & `magnum-9.4.1/magnum/tests/policy_fixture.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/fake_notifier.py` & `magnum-9.4.1/magnum/tests/fake_notifier.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/contrib/gate_hook.sh` & `magnum-9.4.1/magnum/tests/contrib/gate_hook.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/contrib/copy_instance_logs.sh` & `magnum-9.4.1/magnum/tests/contrib/copy_instance_logs.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/contrib/post_test_hook.sh` & `magnum-9.4.1/magnum/tests/contrib/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/output_fixture.py` & `magnum-9.4.1/magnum/tests/output_fixture.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/base.py` & `magnum-9.4.1/magnum/tests/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/cmd/test_driver_manage.py` & `magnum-9.4.1/magnum/tests/unit/cmd/test_driver_manage.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/cmd/test_db_manage.py` & `magnum-9.4.1/magnum/tests/unit/cmd/test_db_manage.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/cmd/test_status.py` & `magnum-9.4.1/magnum/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/cmd/test_conductor.py` & `magnum-9.4.1/magnum/tests/unit/cmd/test_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/cmd/test_api.py` & `magnum-9.4.1/magnum/tests/unit/cmd/test_api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/test_utils.py` & `magnum-9.4.1/magnum/tests/unit/conductor/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/test_k8s_api.py` & `magnum-9.4.1/magnum/tests/unit/conductor/test_k8s_api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_nodegroup_conductor.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_nodegroup_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_cluster_conductor.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_cluster_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_conductor_listener.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_conductor_listener.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_k8s_cluster_conductor.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_k8s_cluster_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_indirection_api.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_indirection_api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/common/test_trust_manager.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/common/test_trust_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/common/test_cert_manager.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/common/test_cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_swarm_cluster_conductor.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_swarm_cluster_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_mesos_cluster_conductor.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_mesos_cluster_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_federation_conductor.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_federation_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/handlers/test_ca_conductor.py` & `magnum-9.4.1/magnum/tests/unit/conductor/handlers/test_ca_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/test_monitors.py` & `magnum-9.4.1/magnum/tests/unit/conductor/test_monitors.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/tasks/test_heat_tasks.py` & `magnum-9.4.1/magnum/tests/unit/conductor/tasks/test_heat_tasks.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/test_rpcapi.py` & `magnum-9.4.1/magnum/tests/unit/conductor/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conductor/test_scale_manager.py` & `magnum-9.4.1/magnum/tests/unit/conductor/test_scale_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/service/test_periodic.py` & `magnum-9.4.1/magnum/tests/unit/service/test_periodic.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_magnum_service.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_cluster.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_x509keypair.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_x509keypair.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_nodegroup.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_nodegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/utils.py` & `magnum-9.4.1/magnum/tests/unit/objects/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_federation.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_federation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_objects.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_objects.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_fields.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_fields.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/objects/test_cluster_template.py` & `magnum-9.4.1/magnum/tests/unit/objects/test_cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/servicegroup/test_magnum_service.py` & `magnum-9.4.1/magnum/tests/unit/servicegroup/test_magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/drivers/test_heat_driver.py` & `magnum-9.4.1/magnum/tests/unit/drivers/test_heat_driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/drivers/test_template_definition.py` & `magnum-9.4.1/magnum/tests/unit/drivers/test_template_definition.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/drivers/test_k8s_fedora_atomic_v1_driver.py` & `magnum-9.4.1/magnum/tests/unit/drivers/test_k8s_fedora_atomic_v1_driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/test_validation.py` & `magnum-9.4.1/magnum/tests/unit/api/test_validation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/test_app.py` & `magnum-9.4.1/magnum/tests/unit/api/test_app.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/test_attr_validator.py` & `magnum-9.4.1/magnum/tests/unit/api/test_attr_validator.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/test_servicegroup.py` & `magnum-9.4.1/magnum/tests/unit/api/test_servicegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/utils.py` & `magnum-9.4.1/magnum/tests/unit/api/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/test_hooks.py` & `magnum-9.4.1/magnum/tests/unit/api/test_hooks.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/test_base.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/test_base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_magnum_service.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_cluster.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_utils.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_baymodel.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_nodegroup.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_nodegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_federation.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_federation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_bay.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_cluster_actions.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_cluster_actions.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_types.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_types.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_stats.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_stats.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_quota.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_quota.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_cluster_template.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/v1/test_certificate.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/v1/test_certificate.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/auth-paste.ini` & `magnum-9.4.1/magnum/tests/unit/api/controllers/auth-paste.ini`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/auth-root-access.ini` & `magnum-9.4.1/magnum/tests/unit/api/controllers/auth-root-access.ini`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/test_root.py` & `magnum-9.4.1/magnum/tests/unit/api/controllers/test_root.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/controllers/auth-v1-access.ini` & `magnum-9.4.1/magnum/tests/unit/api/controllers/auth-v1-access.ini`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/test_expose.py` & `magnum-9.4.1/magnum/tests/unit/api/test_expose.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/api/base.py` & `magnum-9.4.1/magnum/tests/unit/api/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/test_magnum_service.py` & `magnum-9.4.1/magnum/tests/unit/db/test_magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/test_cluster.py` & `magnum-9.4.1/magnum/tests/unit/db/test_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/test_x509keypair.py` & `magnum-9.4.1/magnum/tests/unit/db/test_x509keypair.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/sqlalchemy/test_types.py` & `magnum-9.4.1/magnum/tests/unit/db/sqlalchemy/test_types.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/test_nodegroup.py` & `magnum-9.4.1/magnum/tests/unit/db/test_nodegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/utils.py` & `magnum-9.4.1/magnum/tests/unit/db/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/test_federation.py` & `magnum-9.4.1/magnum/tests/unit/db/test_federation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/test_quota.py` & `magnum-9.4.1/magnum/tests/unit/db/test_quota.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/base.py` & `magnum-9.4.1/magnum/tests/unit/db/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/db/test_cluster_template.py` & `magnum-9.4.1/magnum/tests/unit/db/test_cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/test_hacking.py` & `magnum-9.4.1/magnum/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/conf/test_conf.py` & `magnum-9.4.1/magnum/tests/unit/conf/test_conf.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_profiler.py` & `magnum-9.4.1/magnum/tests/unit/common/test_profiler.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_utils.py` & `magnum-9.4.1/magnum/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_docker_utils.py` & `magnum-9.4.1/magnum/tests/unit/common/test_docker_utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_neutron.py` & `magnum-9.4.1/magnum/tests/unit/common/test_neutron.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_clients.py` & `magnum-9.4.1/magnum/tests/unit/common/test_clients.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_context.py` & `magnum-9.4.1/magnum/tests/unit/common/test_context.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/x509/test_operations.py` & `magnum-9.4.1/magnum/tests/unit/common/x509/test_operations.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/x509/test_validator.py` & `magnum-9.4.1/magnum/tests/unit/common/x509/test_validator.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/x509/test_sign.py` & `magnum-9.4.1/magnum/tests/unit/common/x509/test_sign.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_service.py` & `magnum-9.4.1/magnum/tests/unit/common/test_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_x509keypair_cert_manager.py` & `magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_x509keypair_cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_cert_manager.py` & `magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_barbican.py` & `magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_barbican.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/cert_manager/test_local.py` & `magnum-9.4.1/magnum/tests/unit/common/cert_manager/test_local.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_exception.py` & `magnum-9.4.1/magnum/tests/unit/common/test_exception.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_urlfetch.py` & `magnum-9.4.1/magnum/tests/unit/common/test_urlfetch.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_keystone.py` & `magnum-9.4.1/magnum/tests/unit/common/test_keystone.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_octavia.py` & `magnum-9.4.1/magnum/tests/unit/common/test_octavia.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_short_id.py` & `magnum-9.4.1/magnum/tests/unit/common/test_short_id.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_rpc.py` & `magnum-9.4.1/magnum/tests/unit/common/test_rpc.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/common/test_policy.py` & `magnum-9.4.1/magnum/tests/unit/common/test_policy.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/tests/unit/template/test_template.py` & `magnum-9.4.1/magnum/tests/unit/template/test_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/conductor_listener.py` & `magnum-9.4.1/magnum/conductor/handlers/conductor_listener.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/federation_conductor.py` & `magnum-9.4.1/magnum/conductor/handlers/federation_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/cluster_conductor.py` & `magnum-9.4.1/magnum/conductor/handlers/cluster_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/ca_conductor.py` & `magnum-9.4.1/magnum/conductor/handlers/ca_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/common/trust_manager.py` & `magnum-9.4.1/magnum/conductor/handlers/common/trust_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/common/cert_manager.py` & `magnum-9.4.1/magnum/conductor/handlers/common/cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/indirection_api.py` & `magnum-9.4.1/magnum/conductor/handlers/indirection_api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/handlers/nodegroup_conductor.py` & `magnum-9.4.1/magnum/conductor/handlers/nodegroup_conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/monitors.py` & `magnum-9.4.1/magnum/conductor/monitors.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/api.py` & `magnum-9.4.1/magnum/conductor/api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/utils.py` & `magnum-9.4.1/magnum/conductor/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/scale_manager.py` & `magnum-9.4.1/magnum/conductor/scale_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/k8s_api.py` & `magnum-9.4.1/magnum/conductor/k8s_api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/tasks/heat_tasks.py` & `magnum-9.4.1/magnum/conductor/tasks/heat_tasks.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conductor/tasks/__init__.py` & `magnum-9.4.1/magnum/conductor/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/service/periodic.py` & `magnum-9.4.1/magnum/service/periodic.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/quota.py` & `magnum-9.4.1/magnum/objects/quota.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/cluster.py` & `magnum-9.4.1/magnum/objects/cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/federation.py` & `magnum-9.4.1/magnum/objects/federation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/x509keypair.py` & `magnum-9.4.1/magnum/objects/x509keypair.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/magnum_service.py` & `magnum-9.4.1/magnum/objects/magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/nodegroup.py` & `magnum-9.4.1/magnum/objects/nodegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/fields.py` & `magnum-9.4.1/magnum/objects/fields.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/stats.py` & `magnum-9.4.1/magnum/objects/stats.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/base.py` & `magnum-9.4.1/magnum/objects/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/certificate.py` & `magnum-9.4.1/magnum/objects/certificate.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/cluster_template.py` & `magnum-9.4.1/magnum/objects/cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/objects/__init__.py` & `magnum-9.4.1/magnum/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/i18n.py` & `magnum-9.4.1/magnum/i18n.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/servicegroup/magnum_service_periodic.py` & `magnum-9.4.1/magnum/servicegroup/magnum_service_periodic.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/COPYING` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/COPYING`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/cluster.yaml` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/cluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/README.md` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/README.md`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmnode.yaml` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmnode.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmmaster.yaml` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/swarmmaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/version.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/template_def.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/monitor.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/driver.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/Dockerfile` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/README.rst` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/image/openvswitch/README.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-heat-params-master.yaml` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-heat-params-master.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-master-service.sh` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-master-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-worker-service.sh` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/fragments/write-swarm-worker-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmnode.yaml` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmnode.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmmaster.yaml` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmmaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmcluster.yaml` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/templates/swarmcluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/version.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/template_def.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/monitor.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/swarm_fedora_atomic_v2/driver.py` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v2/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesosslave.yaml` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesosslave.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesos_slave_software_configs.yaml` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesos_slave_software_configs.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesosmaster.yaml` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesosmaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/mesoscluster.yaml` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/mesoscluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-ext-ca-certs.sh` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-ext-ca-certs.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-master.sh` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-master.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/volume-service.sh` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/volume-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/write-heat-params.yaml` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/write-heat-params.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-proxy.sh` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/add-proxy.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-slave.sh` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/templates/fragments/configure-mesos-slave.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/COPYING` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/COPYING`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/version.py` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/template_def.py` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/monitor.py` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/scale_manager.py` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/scale_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/driver.py` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/Dockerfile` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/Dockerfile`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/mesos/pre-install.d/10-apt-repo` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/mesos/pre-install.d/10-apt-repo`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/mesos_ubuntu_v1/image/validate_image.sh` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/image/validate_image.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/COPYING` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/COPYING`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/kubeminion.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/kubeminion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/fcct-config.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/fcct-config.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/kubecluster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/kubecluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/user_data.json` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/user_data.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/templates/kubemaster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/templates/kubemaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/version.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/template_def.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_coreos_v1/driver.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion_software_configs.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion_software_configs.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubeminion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubecluster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubecluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/templates/kubemaster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/templates/kubemaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/version.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/template_def.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/driver.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/Readme.md` & `magnum-9.4.1/magnum/drivers/k8s_fedora_ironic_v1/image/kubernetes/Readme.md`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/add-docker-daemon-options.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/add-docker-daemon-options.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-heat-params-master.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-heat-params-master.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/network-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/network-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-heat-params-node.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-heat-params-node.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/make-cert.py` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/make-cert.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/volume-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/volume-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-swarm-master-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-swarm-master-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/configure-etcd.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/configure-etcd.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/add-proxy.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/add-proxy.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/write-swarm-agent-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/write-swarm-agent-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/swarm/fragments/network-config-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/swarm/fragments/network-config-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/lb_etcd.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/lb_etcd.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/network.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/network.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/environments/with_master_lb_octavia.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/environments/with_master_lb_octavia.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/environments/disable_floating_ip.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/environments/disable_floating_ip.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/environments/no_master_lb.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/environments/no_master_lb.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/environments/with_master_lb.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/environments/with_master_lb.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/environments/enable_floating_ip.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/environments/enable_floating_ip.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/fragments/configure_docker_storage_driver_atomic.sh` & `magnum-9.4.1/magnum/drivers/common/templates/fragments/configure_docker_storage_driver_atomic.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/fragments/configure-docker-registry.sh` & `magnum-9.4.1/magnum/drivers/common/templates/fragments/configure-docker-registry.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/fragments/api_gateway_switcher_master.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/fragments/api_gateway_switcher_master.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/fragments/configure-docker-storage.sh` & `magnum-9.4.1/magnum/drivers/common/templates/fragments/configure-docker-storage.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/fragments/api_gateway_switcher_pool.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/fragments/api_gateway_switcher_pool.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/prometheus-operator.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/prometheus-operator.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/metrics-server.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/metrics-server.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/prometheus-adapter.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/prometheus-adapter.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/helm/ingress-nginx.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/helm/ingress-nginx.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-controller.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-controller.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/install-clients.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/install-clients.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-cinder-csi.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-cinder-csi.sh`

 * *Files 1% similar despite different names*

```diff
@@ -482,17 +482,14 @@
 apiVersion: storage.k8s.io/v1beta1
 kind: CSIDriver
 metadata:
   name: cinder.csi.openstack.org
 spec:
   attachRequired: true
   podInfoOnMount: true
-  volumeLifecycleModes:
-  - Persistent
-  - Ephemeral
 EOF
 
     echo "Waiting for Kubernetes API..."
     until  [ "ok" = "$(curl --silent http://127.0.0.1:8080/healthz)" ]
     do
         sleep 5
     done
```

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/start-container-agent.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/start-container-agent.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-healing.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-healing.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/install-cri.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/install-cri.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/make-cert.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/make-cert.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params-master.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/write-heat-params-master.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-octavia.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-octavia.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-master.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-master.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/upgrade-kubernetes.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/upgrade-kubernetes.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-minion.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/configure-kubernetes-minion.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-traefik.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-ingress-traefik.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-scaling.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-auto-scaling.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-services-master.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-services-master.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/kube-apiserver-to-kubelet-role.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/kube-apiserver-to-kubelet-role.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/install-helm-modules.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/install-helm-modules.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-helm-tiller.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-helm-tiller.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/configure-etcd.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/configure-etcd.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/core-dns-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/core-dns-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/write-kube-os-config.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/write-kube-os-config.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-services-minion.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-services-minion.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/wc-notify-master.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/wc-notify-master.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/flannel-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/flannel-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-prometheus-monitoring.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-prometheus-monitoring.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/enable-keystone-auth.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/enable-keystone-auth.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/add-proxy.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/add-proxy.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/make-cert-client.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/make-cert-client.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/kube-dashboard-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/kube-dashboard-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/kubernetes/fragments/calico-service.sh` & `magnum-9.4.1/magnum/drivers/common/templates/kubernetes/fragments/calico-service.sh`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/templates/lb_api.yaml` & `magnum-9.4.1/magnum/drivers/common/templates/lb_api.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/k8s_scale_manager.py` & `magnum-9.4.1/magnum/drivers/common/k8s_scale_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/driver.py` & `magnum-9.4.1/magnum/drivers/common/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/common/k8s_monitor.py` & `magnum-9.4.1/magnum/drivers/common/k8s_monitor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/heat/swarm_fedora_template_def.py` & `magnum-9.4.1/magnum/drivers/heat/swarm_fedora_template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/heat/k8s_fedora_template_def.py` & `magnum-9.4.1/magnum/drivers/heat/k8s_fedora_template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/heat/template_def.py` & `magnum-9.4.1/magnum/drivers/heat/template_def.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,15 +387,23 @@
         kwargs = {
             'service_type': 'identity',
             'interface': CONF.trust.trustee_keystone_interface,
             'version': 3
         }
         if CONF.trust.trustee_keystone_region_name:
             kwargs['region_name'] = CONF.trust.trustee_keystone_region_name
-        extra_params['auth_url'] = osc.url_for(**kwargs).rstrip('/')
+        # NOTE: Sometimes, version discovery fails when Magnum cannot talk to
+        # Keystone via specified trustee_keystone_interface intended for
+        # cluster instances either because it is not unreachable from the
+        # controller or CA certs are missing for TLS enabled interface and the
+        # returned auth_url may not be suffixed with /v3 in which case append
+        # the url with the suffix so that instances can still talk to Keystone.
+        auth_url = osc.url_for(**kwargs).rstrip('/')
+        extra_params['auth_url'] = auth_url + ('' if auth_url.endswith('/v3')
+                                               else '/v3')
 
         return super(BaseTemplateDefinition,
                      self).get_params(context, cluster_template, cluster,
                                       extra_params=extra_params,
                                       **kwargs)
 
     def resolve_ambiguous_values(self, context, heat_param, heat_value, value):
```

### Comparing `magnum-9.4.0/magnum/drivers/heat/driver.py` & `magnum-9.4.1/magnum/drivers/heat/driver.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -489,37 +489,37 @@
 
         try:
             # Do not resolve outputs by default. Resolving all
             # node IPs is expensive on heat.
             stack = self.openstack_client.heat().stacks.get(
                 self.nodegroup.stack_id, resolve_outputs=False)
 
-            # poll_and_check is detached and polling long time to check
-            # status, so another user/client can call delete cluster/stack.
-            if stack.stack_status == fields.ClusterStatus.DELETE_COMPLETE:
-                if self.nodegroup.is_default:
-                    self._check_delete_complete()
-                else:
-                    self.nodegroup.destroy()
-                    return
-
             if stack.stack_status in (fields.ClusterStatus.CREATE_COMPLETE,
                                       fields.ClusterStatus.UPDATE_COMPLETE):
                 # Resolve all outputs if the stack is COMPLETE
                 stack = self.openstack_client.heat().stacks.get(
                     self.nodegroup.stack_id, resolve_outputs=True)
 
                 self._sync_cluster_and_template_status(stack)
             elif stack.stack_status != self.nodegroup.status:
                 self.template_def.nodegroup_output_mappings = list()
                 self.template_def.update_outputs(
                     stack, self.cluster_template, self.cluster,
                     nodegroups=[self.nodegroup])
                 self._sync_cluster_status(stack)
 
+            # poll_and_check is detached and polling long time to check
+            # status, so another user/client can call delete cluster/stack.
+            if stack.stack_status == fields.ClusterStatus.DELETE_COMPLETE:
+                if self.nodegroup.is_default:
+                    self._check_delete_complete()
+                else:
+                    self.nodegroup.destroy()
+                    return
+
             if stack.stack_status in (fields.ClusterStatus.CREATE_FAILED,
                                       fields.ClusterStatus.DELETE_FAILED,
                                       fields.ClusterStatus.UPDATE_FAILED,
                                       fields.ClusterStatus.ROLLBACK_COMPLETE,
                                       fields.ClusterStatus.ROLLBACK_FAILED):
                 self._sync_cluster_and_template_status(stack)
                 self._nodegroup_failed(stack)
```

### Comparing `magnum-9.4.0/magnum/drivers/heat/k8s_template_def.py` & `magnum-9.4.1/magnum/drivers/heat/k8s_template_def.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,15 +198,24 @@
         return extra_params
 
     def get_params(self, context, cluster_template, cluster, **kwargs):
         extra_params = kwargs.pop('extra_params', {})
 
         extra_params['discovery_url'] = self.get_discovery_url(cluster)
         osc = self.get_osc(context)
-        extra_params['magnum_url'] = osc.magnum_url()
+        # NOTE: Sometimes, version discovery fails when Magnum cannot talk to
+        # Keystone via specified magnum_client.endpoint_type intended for
+        # cluster instances either because it is not unreachable from the
+        # controller or CA certs are missing for TLS enabled interface and the
+        # returned auth_url may not be suffixed with /v1 in which case append
+        # the url with the suffix so that instances can still talk to Magnum.
+        magnum_url = osc.magnum_url()
+        extra_params['magnum_url'] = magnum_url + ('' if
+                                                   magnum_url.endswith('/v1')
+                                                   else '/v1')
 
         if cluster_template.tls_disabled:
             extra_params['loadbalancing_protocol'] = 'HTTP'
             extra_params['kubernetes_port'] = 8080
 
         extra_params['octavia_enabled'] = keystone.is_octavia_enabled()
```

### Comparing `magnum-9.4.0/magnum/drivers/heat/swarm_mode_template_def.py` & `magnum-9.4.1/magnum/drivers/heat/swarm_mode_template_def.py`

 * *Files 18% similar despite different names*

```diff
@@ -113,15 +113,24 @@
 
     def get_params(self, context, cluster_template, cluster, **kwargs):
         extra_params = kwargs.pop('extra_params', {})
         # HACK(apmelton) - This uses the user's bearer token, ideally
         # it should be replaced with an actual trust token with only
         # access to do what the template needs it to do.
         osc = self.get_osc(context)
-        extra_params['magnum_url'] = osc.magnum_url()
+        # NOTE: Sometimes, version discovery fails when Magnum cannot talk to
+        # Keystone via specified magnum_client.endpoint_type intended for
+        # cluster instances either because it is not unreachable from the
+        # controller or CA certs are missing for TLS enabled interface and the
+        # returned auth_url may not be suffixed with /v1 in which case append
+        # the url with the suffix so that instances can still talk to Magnum.
+        magnum_url = osc.magnum_url()
+        extra_params['magnum_url'] = magnum_url + ('' if
+                                                   magnum_url.endswith('/v1')
+                                                   else '/v1')
 
         label_list = ['rexray_preempt', 'availability_zone']
 
         extra_params['auth_url'] = context.auth_url
         extra_params['nodes_affinity_policy'] = \
             CONF.cluster.nodes_affinity_policy
```

### Comparing `magnum-9.4.0/magnum/drivers/heat/k8s_coreos_template_def.py` & `magnum-9.4.1/magnum/drivers/heat/k8s_coreos_template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/COPYING` & `magnum-9.4.1/magnum/drivers/mesos_ubuntu_v1/COPYING`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/kubeminion.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/kubeminion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/kubecluster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/kubecluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/templates/kubemaster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/templates/kubemaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/version.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_coreos_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/template_def.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/driver.py` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_fedora_atomic_v1/tools/grafana-prometheus-dashboard.json` & `magnum-9.4.1/magnum/drivers/k8s_fedora_atomic_v1/tools/grafana-prometheus-dashboard.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/COPYING` & `magnum-9.4.1/magnum/drivers/swarm_fedora_atomic_v1/templates/COPYING`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/kubeminion.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/kubeminion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-controller-manager.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-controller-manager.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-minion.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-minion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-docker-mount.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-docker-mount.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-apiserver.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-apiserver.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params-master.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params-master.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-master.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-master.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-dashboard.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-dashboard.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-minion.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kubelet-minion.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-master.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-proxy-master.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert-client.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert-client.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service-client.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service-client.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-docker.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-docker.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-etcd.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/configure-etcd.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-heat-params.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/add-ext-ca-certs.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/add-ext-ca-certs.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-network-config.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-network-config.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-network-service.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/add-proxy.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/add-proxy.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/create-kube-namespace.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/create-kube-namespace.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/wc-notify.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/wc-notify.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-scheduler.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-kube-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/write-kubeconfig.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/write-kubeconfig.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/make-cert.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-coredns.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/fragments/enable-coredns.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/kubecluster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/kubecluster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/templates/kubemaster.yaml` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/templates/kubemaster.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/version.py` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/template_def.py` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/template_def.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/drivers/k8s_coreos_v1/driver.py` & `magnum-9.4.1/magnum/drivers/k8s_coreos_v1/driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/version.py` & `magnum-9.4.1/magnum/version.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/expose.py` & `magnum-9.4.1/magnum/api/expose.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/app.py` & `magnum-9.4.1/magnum/api/app.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/app.wsgi` & `magnum-9.4.1/magnum/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/utils.py` & `magnum-9.4.1/magnum/api/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/versioned_method.py` & `magnum-9.4.1/magnum/api/versioned_method.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/middleware/auth_token.py` & `magnum-9.4.1/magnum/api/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/middleware/parsable_error.py` & `magnum-9.4.1/magnum/api/middleware/parsable_error.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/middleware/__init__.py` & `magnum-9.4.1/magnum/api/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/http_error.py` & `magnum-9.4.1/magnum/api/http_error.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/validation.py` & `magnum-9.4.1/magnum/api/validation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/hooks.py` & `magnum-9.4.1/magnum/api/hooks.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/attr_validator.py` & `magnum-9.4.1/magnum/api/attr_validator.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/config.py` & `magnum-9.4.1/magnum/api/config.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/rest_api_version_history.rst` & `magnum-9.4.1/magnum/api/rest_api_version_history.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/versions.py` & `magnum-9.4.1/magnum/api/controllers/versions.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/bay.py` & `magnum-9.4.1/magnum/api/controllers/v1/bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/quota.py` & `magnum-9.4.1/magnum/api/controllers/v1/quota.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/cluster.py` & `magnum-9.4.1/magnum/api/controllers/v1/cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/baymodel.py` & `magnum-9.4.1/magnum/api/controllers/v1/baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/federation.py` & `magnum-9.4.1/magnum/api/controllers/v1/federation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/cluster_actions.py` & `magnum-9.4.1/magnum/api/controllers/v1/cluster_actions.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/nodegroup.py` & `magnum-9.4.1/magnum/api/controllers/v1/nodegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/collection.py` & `magnum-9.4.1/magnum/api/controllers/v1/collection.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/stats.py` & `magnum-9.4.1/magnum/api/controllers/v1/stats.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/magnum_services.py` & `magnum-9.4.1/magnum/api/controllers/v1/magnum_services.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/types.py` & `magnum-9.4.1/magnum/api/controllers/v1/types.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/certificate.py` & `magnum-9.4.1/magnum/api/controllers/v1/certificate.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/cluster_template.py` & `magnum-9.4.1/magnum/api/controllers/v1/cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/v1/__init__.py` & `magnum-9.4.1/magnum/api/controllers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/link.py` & `magnum-9.4.1/magnum/api/controllers/link.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/base.py` & `magnum-9.4.1/magnum/api/controllers/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/controllers/root.py` & `magnum-9.4.1/magnum/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/api/servicegroup.py` & `magnum-9.4.1/magnum/api/servicegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/models.py` & `magnum-9.4.1/magnum/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/api.py` & `magnum-9.4.1/magnum/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/env.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2b5f24dd95de_rename_service_port.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2b5f24dd95de_rename_service_port.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/05d3e97de9ee_add_volume_driver.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/05d3e97de9ee_add_volume_driver.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/e0653b2d5271_add_fixed_subnet_column_to_baymodel_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/e0653b2d5271_add_fixed_subnet_column_to_baymodel_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/bb42b7cad130_remove_node_object.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/bb42b7cad130_remove_node_object.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/ac92cbae311c_add_nodegoup_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/ac92cbae311c_add_nodegoup_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/a1136d335540_add_docker_storage_driver_column.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/a1136d335540_add_docker_storage_driver_column.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/049f81f6f584_remove_ssh_authorized_key_from_baymodel.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/049f81f6f584_remove_ssh_authorized_key_from_baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5977879072a7_add_env_to_container.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5977879072a7_add_env_to_container.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/085e601a39f6_remove_service.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/085e601a39f6_remove_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/35cff7c86221_add_private_network_to_baymodel.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/35cff7c86221_add_private_network_to_baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3b6c4c42adb4_add_unique_constraints.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3b6c4c42adb4_add_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/6f21dc920bb_add_cert_uuid_to_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/6f21dc920bb_add_cert_uuid_to_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5793cd26898d_add_bay_status.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5793cd26898d_add_bay_status.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/456126c6c9e9_create_baylock_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/456126c6c9e9_create_baylock_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/ee92b41b8809_create_quotas_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/ee92b41b8809_create_quotas_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/68ce16dfd341_add_master_lb_enabled_column_to_baymodel_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/68ce16dfd341_add_master_lb_enabled_column_to_baymodel_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/40f325033343_add_bay_create_timeout_to_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/40f325033343_add_bay_create_timeout_to_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3be65537a94a_add_network_driver_baymodel_column.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3be65537a94a_add_network_driver_baymodel_column.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/d072f58ab240_modify_x509keypair_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/d072f58ab240_modify_x509keypair_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3a938526b35d_add_docker_volume_size.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3a938526b35d_add_docker_volume_size.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/53882537ac57_add_host_column_to_pod.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/53882537ac57_add_host_column_to_pod.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/966a99e70ff_add_proxy.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/966a99e70ff_add_proxy.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2ae93c9c6191_add_public_column_to_baymodel_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2ae93c9c6191_add_public_column_to_baymodel_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/9a1539f1cd2c_add_federation_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/9a1539f1cd2c_add_federation_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/bc46ba6cf949_add_keypair_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/bc46ba6cf949_add_keypair_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/27ad304554e2_adding_magnum_service_functionality.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/27ad304554e2_adding_magnum_service_functionality.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5518af8dbc21_rename_cert_uuid.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5518af8dbc21_rename_cert_uuid.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/fcb4efee8f8b_add_version_info_to_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/fcb4efee8f8b_add_version_info_to_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/720f640f43d1_rename_bay_table_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/720f640f43d1_rename_bay_table_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/cbbc65a86986_add_health_status_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/cbbc65a86986_add_health_status_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/adc3b7679ae_add_registry_trust_id_to_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/adc3b7679ae_add_registry_trust_id_to_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/ef08a5e057bd_remove_pod.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/ef08a5e057bd_remove_pod.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/fb03fdef8919_rename_baymodel_to_clustertemplate.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/fb03fdef8919_rename_baymodel_to_clustertemplate.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/4e263f236334_add_registry_enabled.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/4e263f236334_add_registry_enabled.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1afee1db6cd0_add_master_flavor.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1afee1db6cd0_add_master_flavor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/59e7664a8ba1_add_container_status.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/59e7664a8ba1_add_container_status.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/52bcaf58fecb_add_master_flavor_id_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/52bcaf58fecb_add_master_flavor_id_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/6f21dc998bb_add_master_addresses_to_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/6f21dc998bb_add_master_addresses_to_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1c1ff5e56048_rename_container_image_id.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1c1ff5e56048_rename_container_image_id.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/156ceb17fb0a_add_bay_status_reason.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/156ceb17fb0a_add_bay_status_reason.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/a0e7c8450ab1_add_labels_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/a0e7c8450ab1_add_labels_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/e772b2598d9_add_container_command.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/e772b2598d9_add_container_command.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/47380964133d_add_network_subnet_fip_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/47380964133d_add_network_subnet_fip_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/33ef79969018_add_memory_to_container.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/33ef79969018_add_memory_to_container.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/aa0cc27839af_add_docker_volume_size_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/aa0cc27839af_add_docker_volume_size_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5ad410481b88_rename_insecure.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5ad410481b88_rename_insecure.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/e647f5931da8_add_insecure_registry_to_baymodel.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/e647f5931da8_add_insecure_registry_to_baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/461d798132c7_change_cluster_to_support_nodegroups.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/461d798132c7_change_cluster_to_support_nodegroups.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/4ea34a59a64c_add_discovery_url_to_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/4ea34a59a64c_add_discovery_url_to_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1d045384b966_add_insecure_baymodel_attr.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1d045384b966_add_insecure_baymodel_attr.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/c04e925e65c2_nodegroups_v2.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/c04e925e65c2_nodegroups_v2.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1481f5b560dd_add_labels_column_to_baymodel_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1481f5b560dd_add_labels_column_to_baymodel_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/14328d6a57e3_add_master_count_to_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/14328d6a57e3_add_master_count_to_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/421102d1f2d2_create_x509keypair_table.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/421102d1f2d2_create_x509keypair_table.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2d8657c0cdc_add_bay_uuid.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2d8657c0cdc_add_bay_uuid.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/041d9a0f1159_add_flavor_id_to_cluster.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/041d9a0f1159_add_flavor_id_to_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/04c625aa95ba_change_storage_driver_to_string.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/04c625aa95ba_change_storage_driver_to_string.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/29affeaa2bc2_rename_bay_master_address.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/29affeaa2bc2_rename_bay_master_address.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/592131657ca1_add_coe_column_to_baymodel.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/592131657ca1_add_coe_column_to_baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/87e62e3c7abc_add_hidden_to_cluster_template.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/87e62e3c7abc_add_hidden_to_cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2d1354bbf76e_ssh_authorized_key.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2d1354bbf76e_ssh_authorized_key.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2581ebaf0cb2_initial_migration.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/5d4caa6e0a42_create_trustee_for_each_bay.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/5d4caa6e0a42_create_trustee_for_each_bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/2ace4006498_rename_bay_minions_address.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/2ace4006498_rename_bay_minions_address.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/1f196a3dabae_remove_container.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/1f196a3dabae_remove_container.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/3bea56f25597_multi_tenant.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/3bea56f25597_multi_tenant.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/417917e778f5_add_server_type_to_baymodel.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/417917e778f5_add_server_type_to_baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/b1f612248cab_add_floating_ip_enabled_column_to_.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/b1f612248cab_add_floating_ip_enabled_column_to_.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/4956f03cabad_add_cluster_distro.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/4956f03cabad_add_cluster_distro.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/859fb45df249_remove_replication_controller.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/859fb45df249_remove_replication_controller.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic/versions/57fbdf2327a2_remove_baylock.py` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic/versions/57fbdf2327a2_remove_baylock.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/alembic.ini` & `magnum-9.4.1/magnum/db/sqlalchemy/alembic.ini`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/sqlalchemy/migration.py` & `magnum-9.4.1/magnum/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/api.py` & `magnum-9.4.1/magnum/db/api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/db/migration.py` & `magnum-9.4.1/magnum/db/migration.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/docker_registry.py` & `magnum-9.4.1/magnum/conf/docker_registry.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/heat.py` & `magnum-9.4.1/magnum/conf/heat.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/quota.py` & `magnum-9.4.1/magnum/conf/quota.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/cinder.py` & `magnum-9.4.1/magnum/conf/cinder.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/barbican.py` & `magnum-9.4.1/magnum/conf/barbican.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/cluster.py` & `magnum-9.4.1/magnum/conf/cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/keystone.py` & `magnum-9.4.1/magnum/conf/keystone.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/drivers.py` & `magnum-9.4.1/magnum/conf/drivers.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/api.py` & `magnum-9.4.1/magnum/conf/api.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/utils.py` & `magnum-9.4.1/magnum/conf/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/profiler.py` & `magnum-9.4.1/magnum/conf/profiler.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/octavia.py` & `magnum-9.4.1/magnum/conf/octavia.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/rpc.py` & `magnum-9.4.1/magnum/conf/rpc.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/conductor.py` & `magnum-9.4.1/magnum/conf/conductor.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/kubernetes.py` & `magnum-9.4.1/magnum/conf/kubernetes.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/paths.py` & `magnum-9.4.1/magnum/conf/paths.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/docker.py` & `magnum-9.4.1/magnum/conf/docker.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/services.py` & `magnum-9.4.1/magnum/conf/services.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/magnum_client.py` & `magnum-9.4.1/magnum/conf/magnum_client.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/database.py` & `magnum-9.4.1/magnum/conf/database.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/trust.py` & `magnum-9.4.1/magnum/conf/trust.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/neutron.py` & `magnum-9.4.1/magnum/conf/neutron.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/glance.py` & `magnum-9.4.1/magnum/conf/glance.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/certificates.py` & `magnum-9.4.1/magnum/conf/certificates.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/x509.py` & `magnum-9.4.1/magnum/conf/x509.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/cluster_heat.py` & `magnum-9.4.1/magnum/conf/cluster_heat.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/__init__.py` & `magnum-9.4.1/magnum/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/opts.py` & `magnum-9.4.1/magnum/conf/opts.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/cluster_templates.py` & `magnum-9.4.1/magnum/conf/cluster_templates.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/conf/nova.py` & `magnum-9.4.1/magnum/conf/nova.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/bay.py` & `magnum-9.4.1/magnum/common/policies/bay.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/quota.py` & `magnum-9.4.1/magnum/common/policies/quota.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/cluster.py` & `magnum-9.4.1/magnum/common/policies/cluster.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/baymodel.py` & `magnum-9.4.1/magnum/common/policies/baymodel.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/federation.py` & `magnum-9.4.1/magnum/common/policies/federation.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/magnum_service.py` & `magnum-9.4.1/magnum/common/policies/magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/nodegroup.py` & `magnum-9.4.1/magnum/common/policies/nodegroup.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/stats.py` & `magnum-9.4.1/magnum/common/policies/stats.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/base.py` & `magnum-9.4.1/magnum/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/certificate.py` & `magnum-9.4.1/magnum/common/policies/certificate.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/cluster_template.py` & `magnum-9.4.1/magnum/common/policies/cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policies/__init__.py` & `magnum-9.4.1/magnum/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/clients.py` & `magnum-9.4.1/magnum/common/clients.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/cinder.py` & `magnum-9.4.1/magnum/common/cinder.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/keystone.py` & `magnum-9.4.1/magnum/common/keystone.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/utils.py` & `magnum-9.4.1/magnum/common/utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/name_generator.py` & `magnum-9.4.1/magnum/common/name_generator.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/x509/operations.py` & `magnum-9.4.1/magnum/common/x509/operations.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/x509/extensions.py` & `magnum-9.4.1/magnum/common/x509/extensions.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/x509/validator.py` & `magnum-9.4.1/magnum/common/x509/validator.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/profiler.py` & `magnum-9.4.1/magnum/common/profiler.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/octavia.py` & `magnum-9.4.1/magnum/common/octavia.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/cert_manager/barbican_cert_manager.py` & `magnum-9.4.1/magnum/common/cert_manager/barbican_cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/cert_manager/local_cert_manager.py` & `magnum-9.4.1/magnum/common/cert_manager/local_cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/cert_manager/x509keypair_cert_manager.py` & `magnum-9.4.1/magnum/common/cert_manager/x509keypair_cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/cert_manager/cert_manager.py` & `magnum-9.4.1/magnum/common/cert_manager/cert_manager.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/cert_manager/__init__.py` & `magnum-9.4.1/magnum/common/cert_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/config.py` & `magnum-9.4.1/magnum/common/config.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/rpc.py` & `magnum-9.4.1/magnum/common/rpc.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/urlfetch.py` & `magnum-9.4.1/magnum/common/urlfetch.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/rpc_service.py` & `magnum-9.4.1/magnum/common/rpc_service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/policy.py` & `magnum-9.4.1/magnum/common/policy.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/context.py` & `magnum-9.4.1/magnum/common/context.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/neutron.py` & `magnum-9.4.1/magnum/common/neutron.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/service.py` & `magnum-9.4.1/magnum/common/service.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/short_id.py` & `magnum-9.4.1/magnum/common/short_id.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/docker_utils.py` & `magnum-9.4.1/magnum/common/docker_utils.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/nova.py` & `magnum-9.4.1/magnum/common/nova.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/common/exception.py` & `magnum-9.4.1/magnum/common/exception.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/__init__.py` & `magnum-9.4.1/magnum/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/magnum/hacking/checks.py` & `magnum-9.4.1/magnum/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/etc/magnum/api-paste.ini` & `magnum-9.4.1/etc/magnum/api-paste.ini`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/etc/magnum/keystone_auth_default_policy.sample` & `magnum-9.4.1/etc/magnum/keystone_auth_default_policy.sample`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/LICENSE` & `magnum-9.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/ChangeLog` & `magnum-9.4.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+9.4.1
+-----
+
+* Drop lower constraints testing
+* [fix] Sync nodegroup status before delete\_complete
+* Remove volumeLifecycleModes in Cinder CSI
+* [fix] Append v3/v1 to auth\_url/magnum\_url if discovery fails
+
 9.4.0
 -----
 
 * resize: Send only nodes\_to\_remove and node\_count
 * More verbose logs for cluster ops
 * Support proxy for helm install
 * [hca] Use train-stable-3 as default for stable/train
```

### Comparing `magnum-9.4.0/test-requirements.txt` & `magnum-9.4.1/test-requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
 # Despite above warning added by global sync process, please use
 # ascii betical order.
 
-bandit!=1.6.0,>=1.1.0 # Apache-2.0
+bandit>=1.1.0,<=1.6.2 # Apache-2.0
 bashate>=0.5.1 # Apache-2.0
 coverage!=4.4,>=4.0 # Apache-2.0
 doc8>=0.6.0 # Apache-2.0
 fixtures>=3.0.0 # Apache-2.0/BSD
 hacking!=0.13.0,<0.14,>=0.12.0 # Apache-2.0
 mock>=2.0.0 # BSD
 oslotest>=3.2.0 # Apache-2.0
```

### Comparing `magnum-9.4.0/tox.ini` & `magnum-9.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/flatten_attributes.rst` & `magnum-9.4.1/specs/flatten_attributes.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/create-trustee-user-for-each-bay.rst` & `magnum-9.4.1/specs/create-trustee-user-for-each-bay.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/tls-support-magnum.rst` & `magnum-9.4.1/specs/tls-support-magnum.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/async-container-operation.rst` & `magnum-9.4.1/specs/async-container-operation.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/resource-quotas.rst` & `magnum-9.4.1/specs/resource-quotas.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/containers-service.rst` & `magnum-9.4.1/specs/containers-service.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/open-dcos.rst` & `magnum-9.4.1/specs/open-dcos.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/stats-api-spec.rst` & `magnum-9.4.1/specs/stats-api-spec.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/magnum-horizon-plugin.rst` & `magnum-9.4.1/specs/magnum-horizon-plugin.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/container-networking-model.rst` & `magnum-9.4.1/specs/container-networking-model.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/container-volume-integration-model.rst` & `magnum-9.4.1/specs/container-volume-integration-model.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/specs/bay-drivers.rst` & `magnum-9.4.1/specs/bay-drivers.rst`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/clustertemplates.inc` & `magnum-9.4.1/api-ref/source/clustertemplates.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/parameters.yaml` & `magnum-9.4.1/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/mservices.inc` & `magnum-9.4.1/api-ref/source/mservices.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/certificates.inc` & `magnum-9.4.1/api-ref/source/certificates.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/bays.inc` & `magnum-9.4.1/api-ref/source/bays.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/versions.inc` & `magnum-9.4.1/api-ref/source/versions.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/urls.inc` & `magnum-9.4.1/api-ref/source/urls.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/conf.py` & `magnum-9.4.1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/status.yaml` & `magnum-9.4.1/api-ref/source/status.yaml`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/baymodels.inc` & `magnum-9.4.1/api-ref/source/baymodels.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/clusters.inc` & `magnum-9.4.1/api-ref/source/clusters.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/bay-get-all-resp.json` & `magnum-9.4.1/api-ref/source/samples/bay-get-all-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/clustertemplate-get-all-resp.json` & `magnum-9.4.1/api-ref/source/samples/clustertemplate-get-all-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/clustertemplate-create-req.json` & `magnum-9.4.1/api-ref/source/samples/baymodel-create-req.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/cluster-get-one-resp.json` & `magnum-9.4.1/api-ref/source/samples/cluster-get-one-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/baymodel-create-req.json` & `magnum-9.4.1/api-ref/source/samples/clustertemplate-create-req.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/bay-get-one-resp.json` & `magnum-9.4.1/api-ref/source/samples/bay-get-one-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/clustertemplate-create-resp.json` & `magnum-9.4.1/api-ref/source/samples/clustertemplate-create-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/certificates-ca-show-resp.json` & `magnum-9.4.1/api-ref/source/samples/certificates-ca-show-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/versions-01-get-resp.json` & `magnum-9.4.1/api-ref/source/samples/versions-01-get-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/baymodel-create-resp.json` & `magnum-9.4.1/api-ref/source/samples/baymodel-create-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/certificates-ca-sign-resp.json` & `magnum-9.4.1/api-ref/source/samples/certificates-ca-sign-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/baymodel-get-all-resp.json` & `magnum-9.4.1/api-ref/source/samples/baymodel-get-all-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/samples/cluster-get-all-resp.json` & `magnum-9.4.1/api-ref/source/samples/cluster-get-all-resp.json`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/stats.inc` & `magnum-9.4.1/api-ref/source/stats.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/api-ref/source/quotas.inc` & `magnum-9.4.1/api-ref/source/quotas.inc`

 * *Files identical despite different names*

### Comparing `magnum-9.4.0/setup.py` & `magnum-9.4.1/setup.py`

 * *Files identical despite different names*

