# Comparing `tmp/nebari_workflow_controller-2023.4.3.tar.gz` & `tmp/nebari_workflow_controller-2023.5.1.tar.gz`

## Comparing `nebari_workflow_controller-2023.4.3.tar` & `nebari_workflow_controller-2023.5.1.tar`

### file list

```diff
@@ -1,186 +1,190 @@
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/.github/workflows/release.yaml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/__init__.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/__main__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/_version.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/app.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/nebari_workflow_controller/models.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_app.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/README.md
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/convert_workflows.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_conda_mount.yaml
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_file_mount.yaml
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_empty_subPath.yaml
--rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/disallowed_volume.yaml
--rw-r--r--   0        0        0     8826 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_conda_mount.yaml
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_file_mount.yaml
--rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_empty_subPath.yaml
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/volumes-existing.yaml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/archive-location.yaml
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/argo_cli_hello_world.yaml
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-artifacts.yaml
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-parameters-from-configmap.yaml
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-parameters.yaml
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-disable-archive.yaml
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-gc-workflow.yaml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-passing-subpath.yaml
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-passing.yaml
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-path-placeholders.yaml
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-repository-ref.yaml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifactory-artifact.yaml
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/browser_hello_world.yaml
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/ci-output-artifact.yaml
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/ci.yaml
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/coinflip-recursive.yaml
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/coinflip.yaml
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/colored-logs.yaml
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditional-artifacts.yaml
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditional-parameters.yaml
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditionals-complex.yaml
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditionals.yaml
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/continue-on-fail.yaml
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/custom-metrics.yaml
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemon-nginx.yaml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemon-step.yaml
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemoned-stateful-set-with-service.yaml
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-coinflip.yaml
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-conditional-artifacts.yaml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-conditional-parameters.yaml
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-continue-on-fail.yaml
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-custom-metrics.yaml
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-daemon-task.yaml
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-diamond-steps.yaml
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-diamond.yaml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-disable-failFast.yaml
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-enhanced-depends.yaml
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-inline-workflow.yaml
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-multiroot.yaml
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-nested.yaml
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-targets.yaml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-task-level-timeout.yaml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/data-transformations.yaml
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/default-pdb-support.yaml
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dns-config.yaml
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-code-output-variable.yaml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-dag-level.yaml
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-slack.yaml
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-step-level.yaml
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-with-artifacts.yaml
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-with-param.yaml
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handlers.yaml
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-destructure-json.yaml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-reusing-verbose-snippets.yaml
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-tag-template-workflow.yaml
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/fibonacci-seq-conditional-param.yaml
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/forever.yaml
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/fun-with-gifs.yaml
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/gc-ttl.yaml
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-outputs.yaml
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters-from-configmap-referenced-as-local-variable.yaml
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters-from-configmap.yaml
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters.yaml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/handle-large-output-results.yaml
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hdfs-artifact.yaml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-hybrid.yaml
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-windows.yaml
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-world.yaml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/http-hello-world.yaml
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/http-success-condition.yaml
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/image-pull-secrets.yaml
--rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/influxdb-ci.yaml
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/init-container.yaml
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-azure.yaml
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-gcs.yaml
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-git.yaml
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-http.yaml
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-oss.yaml
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-raw.yaml
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-s3.yaml
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/jupyterlab_pod.yaml
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-jobs.yaml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-json-patch-workflow.yaml
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-orchestration.yaml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-owner-reference.yaml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-patch-basic.yaml
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-patch.yaml
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-resource-log-selector.yaml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-set-owner-reference.yaml
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-wait-wf.yaml
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/key-only-artifact.yaml
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/kubectl_malicious.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/label-value-from-workflow.yaml
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/life-cycle-hooks-tmpl-level.yaml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/life-cycle-hooks-wf-level.yaml
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-arbitrary-sequential-steps.yaml
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-dag.yaml
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-maps.yaml
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-param-argument.yaml
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-param-result.yaml
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-sequence.yaml
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops.yaml
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/map-reduce.yaml
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/memoize-simple.yaml
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/nested-workflow.yaml
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/node-selector.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-azure.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-gcs.yaml
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-s3.yaml
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-parameter.yaml
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-limit.yaml
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested-dag.yaml
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested-workflow.yaml
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested.yaml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-template-limit.yaml
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation-dag.yaml
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation-script.yaml
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation.yaml
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-gc-strategy-with-label-selector.yaml
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-gc-strategy.yaml
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-metadata-wf-field.yaml
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-metadata.yaml
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-from-previous-step.yaml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-patch-wf-tmpl.yaml
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-patch.yaml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-yaml-patch.yaml
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/recursive-for-loop.yaml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resource-delete-with-flags.yaml
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resource-flags.yaml
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resubmit.yaml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-backoff.yaml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-conditional.yaml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-container-to-completion.yaml
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-container.yaml
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-on-error.yaml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-script.yaml
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-with-steps.yaml
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-bash.yaml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-javascript.yaml
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-python.yaml
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/secrets.yaml
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar-dind.yaml
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar-nginx.yaml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar.yaml
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/status-reference.yaml
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/step-level-timeout.yaml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/steps-inline-workflow.yaml
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/steps.yaml
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/suspend-template-outputs.yaml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/suspend-template.yaml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-mutex-tmpl-level.yaml
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-mutex-wf-level.yaml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-tmpl-level.yaml
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-wf-level.yaml
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/template-defaults.yaml
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/template-on-exit.yaml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/timeouts-step.yaml
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/timeouts-workflow.yaml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/volumes-emptydir.yaml
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/volumes-pvc.yaml
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/webhdfs-input-output-artifacts.yaml
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/work-avoidance.yaml
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/workflow-of-workflows.yaml
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/LICENSE
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/README.md
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/pyproject.toml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/nebari_workflow_controller/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/nebari_workflow_controller/__main__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/nebari_workflow_controller/_version.py
+-rw-r--r--   0        0        0    11937 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/nebari_workflow_controller/app.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/nebari_workflow_controller/models.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_app.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/README.md
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/convert_workflows.py
+-rw-r--r--   0        0        0    43422 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/jupyterlab_pod_spec.pkl
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/container_disallowed_conda_mount.yaml
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/container_disallowed_file_mount.yaml
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/container_empty_subPath.yaml
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/disallowed_volume.yaml
+-rw-r--r--   0        0        0     8826 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/initContainer_disallowed_conda_mount.yaml
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/initContainer_disallowed_file_mount.yaml
+-rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/initContainer_empty_subPath.yaml
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/volumes-existing.yaml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/archive-location.yaml
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/argo_cli_hello_world.yaml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/arguments-artifacts.yaml
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/arguments-parameters-from-configmap.yaml
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/arguments-parameters.yaml
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-disable-archive.yaml
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-gc-workflow.yaml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-passing-subpath.yaml
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-passing.yaml
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-path-placeholders.yaml
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-repository-ref.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifactory-artifact.yaml
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/browser_hello_world.yaml
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/ci-output-artifact.yaml
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/ci.yaml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/coinflip-recursive.yaml
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/coinflip.yaml
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/colored-logs.yaml
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditional-artifacts.yaml
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditional-parameters.yaml
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditionals-complex.yaml
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditionals.yaml
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/continue-on-fail.yaml
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/custom-metrics.yaml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/daemon-nginx.yaml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/daemon-step.yaml
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/daemoned-stateful-set-with-service.yaml
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-coinflip.yaml
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-conditional-artifacts.yaml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-conditional-parameters.yaml
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-continue-on-fail.yaml
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-custom-metrics.yaml
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-daemon-task.yaml
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-diamond-steps.yaml
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-diamond.yaml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-disable-failFast.yaml
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-enhanced-depends.yaml
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-inline-workflow.yaml
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-multiroot.yaml
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-nested.yaml
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-targets.yaml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-task-level-timeout.yaml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/data-transformations.yaml
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/default-pdb-support.yaml
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dns-config.yaml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-code-output-variable.yaml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-dag-level.yaml
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-slack.yaml
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-step-level.yaml
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-with-artifacts.yaml
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-with-param.yaml
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handlers.yaml
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/expression-destructure-json.yaml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/expression-reusing-verbose-snippets.yaml
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/expression-tag-template-workflow.yaml
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/fibonacci-seq-conditional-param.yaml
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/forever.yaml
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/fun-with-gifs.yaml
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/gc-ttl.yaml
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-outputs.yaml
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-parameters-from-configmap-referenced-as-local-variable.yaml
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-parameters-from-configmap.yaml
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-parameters.yaml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/handle-large-output-results.yaml
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hdfs-artifact.yaml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hello-hybrid.yaml
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hello-windows.yaml
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hello-world.yaml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/http-hello-world.yaml
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/http-success-condition.yaml
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/image-pull-secrets.yaml
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/influxdb-ci.yaml
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/init-container.yaml
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-azure.yaml
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-gcs.yaml
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-git.yaml
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-http.yaml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-oss.yaml
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-raw.yaml
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-s3.yaml
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/jupyterflow-override-example.yaml
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/jupyterlab_pod.yaml
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-jobs.yaml
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-json-patch-workflow.yaml
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-orchestration.yaml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-owner-reference.yaml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-patch-basic.yaml
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-patch.yaml
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-resource-log-selector.yaml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-set-owner-reference.yaml
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-wait-wf.yaml
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/key-only-artifact.yaml
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/kubectl_malicious.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/label-value-from-workflow.yaml
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/life-cycle-hooks-tmpl-level.yaml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/life-cycle-hooks-wf-level.yaml
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-arbitrary-sequential-steps.yaml
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-dag.yaml
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-maps.yaml
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-param-argument.yaml
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-param-result.yaml
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-sequence.yaml
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops.yaml
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/map-reduce.yaml
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/memoize-simple.yaml
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/nested-workflow.yaml
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/node-selector.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-artifact-azure.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-artifact-gcs.yaml
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-artifact-s3.yaml
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-parameter.yaml
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-limit.yaml
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-nested-dag.yaml
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-nested-workflow.yaml
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-nested.yaml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-template-limit.yaml
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parameter-aggregation-dag.yaml
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parameter-aggregation-script.yaml
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parameter-aggregation.yaml
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-gc-strategy-with-label-selector.yaml
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-gc-strategy.yaml
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-metadata-wf-field.yaml
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-metadata.yaml
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-from-previous-step.yaml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-patch-wf-tmpl.yaml
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-patch.yaml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-yaml-patch.yaml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/recursive-for-loop.yaml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/resource-delete-with-flags.yaml
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/resource-flags.yaml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/resubmit.yaml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-backoff.yaml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-conditional.yaml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-container-to-completion.yaml
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-container.yaml
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-on-error.yaml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-script.yaml
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-with-steps.yaml
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/scripts-bash.yaml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/scripts-javascript.yaml
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/scripts-python.yaml
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/secrets.yaml
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/sidecar-dind.yaml
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/sidecar-nginx.yaml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/sidecar.yaml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/status-reference.yaml
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/step-level-timeout.yaml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/steps-inline-workflow.yaml
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/steps.yaml
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/suspend-template-outputs.yaml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/suspend-template.yaml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-mutex-tmpl-level.yaml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-mutex-wf-level.yaml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-tmpl-level.yaml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-wf-level.yaml
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/template-defaults.yaml
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/template-on-exit.yaml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/timeouts-step.yaml
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/timeouts-workflow.yaml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/volumes-emptydir.yaml
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/volumes-pvc.yaml
+-rw-r--r--   0        0        0    18252 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/web-ui-resubmit.yaml
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/webhdfs-input-output-artifacts.yaml
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/work-avoidance.yaml
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/workflow-of-workflows.yaml
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/LICENSE
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/README.md
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nebari_workflow_controller-2023.5.1/PKG-INFO
```

### Comparing `nebari_workflow_controller-2023.4.3/.pre-commit-config.yaml` & `nebari_workflow_controller-2023.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/.github/workflows/release.yaml` & `nebari_workflow_controller-2023.5.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/nebari_workflow_controller/__init__.py` & `nebari_workflow_controller-2023.5.1/nebari_workflow_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/convert_workflows.py` & `nebari_workflow_controller-2023.5.1/tests/test_data/convert_workflows.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         - system:serviceaccounts:dev
         - system:authenticated
         uid: eac0d7ab-af84-4c3f-a5fd-71845ff9e8c9
         username: system:serviceaccount:dev:argo-admin
 """
 
 new_request = yaml.load(preamble, Loader=yaml.FullLoader)
-files = Path("./requests/pass").glob("*.yaml")
+files = Path("./requests/valid").glob("*.yaml")
 
 for request_file in files:
     with open(request_file, "r") as f:
         try:
             request = yaml.load(f, Loader=yaml.FullLoader)
         except Exception:
             print(str(request_file))
```

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_conda_mount.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/container_disallowed_conda_mount.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_disallowed_file_mount.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/container_disallowed_file_mount.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/container_empty_subPath.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/container_empty_subPath.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/disallowed_volume.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/disallowed_volume.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_conda_mount.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/initContainer_disallowed_conda_mount.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_disallowed_file_mount.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/initContainer_disallowed_file_mount.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/initContainer_empty_subPath.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/initContainer_empty_subPath.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/fail/volumes-existing.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/invalid/volumes-existing.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/archive-location.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/archive-location.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/argo_cli_hello_world.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/argo_cli_hello_world.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-artifacts.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/arguments-artifacts.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-parameters-from-configmap.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/arguments-parameters-from-configmap.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/arguments-parameters.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/arguments-parameters.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-disable-archive.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-disable-archive.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-gc-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-gc-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-passing-subpath.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-passing-subpath.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-passing.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-passing.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-path-placeholders.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-path-placeholders.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifact-repository-ref.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifact-repository-ref.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/artifactory-artifact.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/artifactory-artifact.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/browser_hello_world.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/browser_hello_world.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/ci-output-artifact.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/ci-output-artifact.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/ci.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/ci.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/coinflip-recursive.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/coinflip-recursive.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/coinflip.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/coinflip.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/colored-logs.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/colored-logs.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditional-artifacts.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditional-artifacts.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditional-parameters.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditional-parameters.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditionals-complex.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditionals-complex.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/conditionals.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/conditionals.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/continue-on-fail.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/continue-on-fail.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/custom-metrics.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/custom-metrics.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemon-nginx.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/daemon-nginx.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemon-step.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/daemon-step.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/daemoned-stateful-set-with-service.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/daemoned-stateful-set-with-service.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-coinflip.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-coinflip.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-conditional-artifacts.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-conditional-artifacts.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-conditional-parameters.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-conditional-parameters.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-continue-on-fail.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-continue-on-fail.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-custom-metrics.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-custom-metrics.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-daemon-task.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-daemon-task.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-diamond-steps.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-diamond-steps.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-diamond.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-diamond.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-disable-failFast.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-disable-failFast.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-enhanced-depends.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-enhanced-depends.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-inline-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-inline-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-multiroot.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-multiroot.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-nested.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-nested.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-targets.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-targets.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dag-task-level-timeout.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dag-task-level-timeout.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/data-transformations.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/data-transformations.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/default-pdb-support.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/default-pdb-support.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/dns-config.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/dns-config.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-code-output-variable.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-code-output-variable.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-dag-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-dag-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-slack.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-slack.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-step-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-step-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-with-artifacts.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-with-artifacts.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handler-with-param.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handler-with-param.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/exit-handlers.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/exit-handlers.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-destructure-json.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/expression-destructure-json.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-reusing-verbose-snippets.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/expression-reusing-verbose-snippets.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/expression-tag-template-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/expression-tag-template-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/fibonacci-seq-conditional-param.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/fibonacci-seq-conditional-param.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/forever.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/forever.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/fun-with-gifs.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/fun-with-gifs.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/gc-ttl.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/gc-ttl.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-outputs.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-outputs.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters-from-configmap-referenced-as-local-variable.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-parameters-from-configmap-referenced-as-local-variable.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters-from-configmap.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-parameters-from-configmap.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/global-parameters.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/global-parameters.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/handle-large-output-results.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/handle-large-output-results.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hdfs-artifact.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hdfs-artifact.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-hybrid.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hello-hybrid.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-windows.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hello-windows.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/hello-world.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/hello-world.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/http-hello-world.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/http-hello-world.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/http-success-condition.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/http-success-condition.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/image-pull-secrets.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/image-pull-secrets.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/influxdb-ci.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/influxdb-ci.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/init-container.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/init-container.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-azure.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-azure.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-gcs.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-gcs.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-git.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-git.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-http.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-http.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-oss.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-oss.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-raw.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-raw.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/input-artifact-s3.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/input-artifact-s3.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/jupyterlab_pod.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/jupyterlab_pod.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-jobs.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-jobs.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-json-patch-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-json-patch-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-orchestration.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-orchestration.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-owner-reference.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-owner-reference.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-patch-basic.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-patch-basic.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-patch.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-patch.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-resource-log-selector.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-resource-log-selector.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-set-owner-reference.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-set-owner-reference.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/k8s-wait-wf.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/k8s-wait-wf.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/key-only-artifact.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/key-only-artifact.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/kubectl_malicious.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/kubectl_malicious.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/label-value-from-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/label-value-from-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/life-cycle-hooks-tmpl-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/life-cycle-hooks-tmpl-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/life-cycle-hooks-wf-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/life-cycle-hooks-wf-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-arbitrary-sequential-steps.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-arbitrary-sequential-steps.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-dag.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-dag.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-maps.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-maps.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-param-argument.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-param-argument.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-param-result.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-param-result.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops-sequence.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops-sequence.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/loops.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/loops.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/map-reduce.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/map-reduce.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/memoize-simple.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/memoize-simple.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/nested-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/nested-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/node-selector.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/node-selector.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-azure.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-artifact-azure.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-gcs.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-artifact-gcs.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-artifact-s3.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-artifact-s3.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/output-parameter.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/output-parameter.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-limit.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-limit.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested-dag.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-nested-dag.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-nested-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-nested.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-nested.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parallelism-template-limit.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parallelism-template-limit.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation-dag.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parameter-aggregation-dag.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation-script.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parameter-aggregation-script.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/parameter-aggregation.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/parameter-aggregation.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-gc-strategy-with-label-selector.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-gc-strategy-with-label-selector.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-gc-strategy.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-gc-strategy.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-metadata-wf-field.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-metadata-wf-field.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-metadata.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-metadata.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-from-previous-step.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-from-previous-step.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-patch-wf-tmpl.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-patch-wf-tmpl.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-patch.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-patch.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/pod-spec-yaml-patch.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/pod-spec-yaml-patch.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/recursive-for-loop.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/recursive-for-loop.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resource-delete-with-flags.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/resource-delete-with-flags.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resource-flags.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/resource-flags.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/resubmit.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/resubmit.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-backoff.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-backoff.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-conditional.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-conditional.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-container-to-completion.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-container-to-completion.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-container.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-container.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-on-error.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-on-error.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-script.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-script.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/retry-with-steps.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/retry-with-steps.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-bash.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/scripts-bash.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-javascript.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/scripts-javascript.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/scripts-python.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/scripts-python.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/secrets.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/secrets.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar-dind.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/sidecar-dind.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar-nginx.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/sidecar-nginx.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/sidecar.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/sidecar.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/status-reference.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/status-reference.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/step-level-timeout.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/step-level-timeout.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/steps-inline-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/steps-inline-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/steps.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/steps.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/suspend-template-outputs.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/suspend-template-outputs.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/suspend-template.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/suspend-template.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-mutex-tmpl-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-mutex-tmpl-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-mutex-wf-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-mutex-wf-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-tmpl-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-tmpl-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/synchronization-wf-level.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/synchronization-wf-level.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/template-defaults.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/template-defaults.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/template-on-exit.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/template-on-exit.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/timeouts-step.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/timeouts-step.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/timeouts-workflow.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/timeouts-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/volumes-emptydir.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/volumes-emptydir.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/volumes-pvc.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/volumes-pvc.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/webhdfs-input-output-artifacts.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/webhdfs-input-output-artifacts.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/work-avoidance.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/work-avoidance.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/tests/test_data/requests/pass/workflow-of-workflows.yaml` & `nebari_workflow_controller-2023.5.1/tests/test_data/requests/valid/workflow-of-workflows.yaml`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/.gitignore` & `nebari_workflow_controller-2023.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/LICENSE` & `nebari_workflow_controller-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari_workflow_controller-2023.4.3/pyproject.toml` & `nebari_workflow_controller-2023.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "Intended Audience :: System Administrators",
 ]
 dependencies = [
     "python-keycloak==2.15.3",
     "fastapi==0.95.1",
     "uvicorn==0.21.1",
     "pydantic==1.10.7",
+    "jsonpatch==1.32",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==22.3.0",
     "flake8==3.8.4",
     "pre-commit",
```

### Comparing `nebari_workflow_controller-2023.4.3/PKG-INFO` & `nebari_workflow_controller-2023.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari-workflow-controller
-Version: 2023.4.3
+Version: 2023.5.1
 Summary: An admission controller for argo workflows in Nebari
 Project-URL: Documentation, https://github.com/nebari-dev/nebari-workflow-controller
 Project-URL: Source, https://github.com/nebari-dev/nebari-workflow-controller
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: admission-controller,argo-workflows,fastapi,kubernetes,nebari
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.8
 Requires-Dist: fastapi==0.95.1
+Requires-Dist: jsonpatch==1.32
 Requires-Dist: pydantic==1.10.7
 Requires-Dist: python-keycloak==2.15.3
 Requires-Dist: uvicorn==0.21.1
 Provides-Extra: dev
 Requires-Dist: black==22.3.0; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: flake8==3.8.4; extra == 'dev'
```

