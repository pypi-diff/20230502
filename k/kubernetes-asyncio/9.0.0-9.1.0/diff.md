# Comparing `tmp/kubernetes_asyncio-9.0.0.tar.gz` & `tmp/kubernetes_asyncio-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubernetes_asyncio-9.0.0.tar", last modified: Sun Mar 24 09:02:14 2019, max compression
+gzip compressed data, was "dist/kubernetes_asyncio-9.1.0.tar", last modified: Fri May  3 22:02:24 2019, max compression
```

## Comparing `kubernetes_asyncio-9.0.0.tar` & `kubernetes_asyncio-9.1.0.tar`

### file list

```diff
@@ -1,685 +1,685 @@
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     2472 2019-03-23 20:49:21.000000 kubernetes_asyncio-9.0.0/setup.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    11354 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/LICENSE
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      174 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/requirements.txt
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      917 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/PKG-INFO
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      527 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/setup.cfg
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      185 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/test-requirements.txt
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      974 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/tox.ini
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    19268 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/kube_config.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     1379 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/google_auth_test.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     2674 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/openid.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     2634 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/dateutil.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      632 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/config_exception.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3041 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/openid_test.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     6987 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/exec_provider_test.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      822 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/__init__.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3531 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/incluster_config.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    34210 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/kube_config_test.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      940 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/google_auth.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     2203 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/dateutil_test.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     4704 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/incluster_config_test.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3622 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/exec_provider.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      828 2019-03-23 20:49:21.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/__init__.py
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13180 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12576 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3315 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_flex_volume.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6352 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7855 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_webhook_client_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4154 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3998 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state_waiting.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8317 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_versions.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8632 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7328 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_controller_revision.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9911 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6342 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6590 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6596 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6496 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6276 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3685 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_capabilities.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4338 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_host_path_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7729 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresource_scale.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5686 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_glusterfs_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7344 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7164 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6720 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    23407 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4079 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_error.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6691 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7251 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3575 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_client_ip_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6123 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_scale_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6814 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7181 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4114 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_load_balancer_ingress.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4093 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_policy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4920 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rolling_update_daemon_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5646 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_projection.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6220 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8293 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_ceph_fs_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6834 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_token_review_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6929 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4218 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_update_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5412 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7543 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_aws_elastic_block_store_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4188 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_update_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6666 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4338 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_flocker_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6190 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3395 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_stateful_set_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4771 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_env_from_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4792 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_ref.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5344 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_portworx_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13077 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7221 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_local_subject_access_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7858 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_node_config_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10789 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6410 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_binding_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_scale.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9149 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_resource_attributes.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    14774 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7210 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_access_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7350 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_glusterfs_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4486 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_token_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6414 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12786 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5743 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_taint.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3135 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_config_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3725 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_job_template_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3918 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4429 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_photon_persistent_disk_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6710 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5804 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_affinity_term.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6779 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4267 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ip_block.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4906 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_key_selector.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3505 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6675 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3226 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4955 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_daemon_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7092 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_object_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4129 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_attached_volume.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4072 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7081 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8725 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8656 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9872 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_object_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6100 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_lease.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7196 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_mount.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5302 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_git_repo_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6924 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_resource_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5776 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_projection.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6617 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8203 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3117 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_session_affinity_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4545 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6242 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3205 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_downward_api_projection.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7436 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5179 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_service_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7274 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_binding.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7089 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7163 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoints.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5072 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_object_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7916 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_rollback.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5087 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4727 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_affinity.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13448 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_security_context.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3121 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6739 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6502 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4828 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event_series.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9209 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4657 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_downward_api_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7495 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_webhook_client_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7197 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6340 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoints_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4002 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_external_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4678 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7988 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_os_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6100 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8079 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6584 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5371 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_nfs_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3176 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_initializer.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10967 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6944 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5283 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_cross_version_object_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6297 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4599 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_non_resource_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    15004 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7798 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6582 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_controller_revision_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13330 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_system_info.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13816 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_iscsi_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6500 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_component_status_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7741 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7933 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4836 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_label_selector.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6873 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_fc_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10822 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6364 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3735 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_watch_event.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    15004 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4041 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresources.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6957 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_access_review_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6671 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5101 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_field_selector.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3279 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4148 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_update_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7052 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6906 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4118 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_update_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4310 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_topology_selector_label_requirement.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4539 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5606 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_user_info.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6354 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4786 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_host_path.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6658 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4827 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoint_port.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7512 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_gce_persistent_disk_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8129 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6627 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_http_get_action.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6574 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_priority_class_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5240 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_azure_file_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4633 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_path.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6954 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6561 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cinder_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7344 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7366 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_local_subject_access_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4000 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4742 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_initializer.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13503 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5742 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_env_var_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7312 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4221 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_preferred_scheduling_term.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6660 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6458 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7386 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7548 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_lease_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8667 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_policy_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6596 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_priority_class_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4009 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_host_port_range.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6615 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4858 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_peer.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    23097 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3881 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6874 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_token_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7139 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3541 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_selector.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6273 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3479 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/runtime_raw_extension.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10796 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10619 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rbd_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9597 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6644 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6692 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_controller_revision_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6452 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11405 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5299 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_env_var.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8414 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_status_details.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6392 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4178 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_update_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    14034 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_storage_class.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6534 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4282 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4622 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_supplemental_groups_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6944 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4013 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_webhook.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7694 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7363 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5353 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6375 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_account_token_projection.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8203 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_os_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4454 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_access_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6202 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_template.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10777 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7189 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_port.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5665 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoint_subset.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6027 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoint_address.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3854 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6859 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6374 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12759 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4482 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_local_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3813 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_aggregation_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3263 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_rollback_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7868 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_rules_review_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4873 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4971 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11785 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5613 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_status_cause.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9747 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7566 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4867 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_ref.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3127 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_endpoint.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6722 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4999 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_service_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12974 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_scale.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3702 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_lifecycle.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3917 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_identifier.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4654 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_non_resource_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6353 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_eviction.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    17071 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6426 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_downward_api_volume_file.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5734 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scoped_resource_selector_requirement.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9731 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_version.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6658 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10816 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_csi_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7284 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4052 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13267 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4616 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_user_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6542 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_binding_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6430 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3184 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6688 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6465 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_component_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4768 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_peer.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7908 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_anti_affinity.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5274 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7601 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5246 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_typed_local_object_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4439 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_selector_term.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3240 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_local_object_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5208 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cross_version_object_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6849 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6829 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6392 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6206 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10048 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_probe.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3512 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3400 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rolling_update_stateful_set_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6790 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6206 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_metric_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6501 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_subject.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4882 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_ref.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7415 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8023 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6529 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7396 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8632 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state_terminated.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5691 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_dns_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3816 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_exec_action.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6550 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_azure_file_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11557 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7019 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5296 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_egress_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4172 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_image.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4541 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_token_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8994 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_attributes.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6458 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6588 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5283 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_cross_version_object_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4573 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_group_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6733 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5184 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8581 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_names.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3806 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_aggregation_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6652 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_account_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4715 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_server_address_by_client_cidr.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3304 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6138 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6669 2019-03-23 20:49:19.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_list_meta.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    31027 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5292 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11528 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_security_context.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4437 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_fs_group_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6542 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6692 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_controller_revision_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3987 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_id_range.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5230 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6733 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4262 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9314 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_priority_class.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7303 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_binding.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7752 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4293 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6501 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3243 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_daemon_endpoints.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6559 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7328 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_controller_revision.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7512 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_rule_with_operations.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12786 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4803 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_requirements.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4493 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_fs_group_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3261 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6302 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3609 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_topology_selector_term.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3822 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_non_resource_attributes.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6292 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4560 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_user_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6736 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cinder_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5672 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_selector_requirement.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7711 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_webhook_client_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6936 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3305 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_rollback_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3153 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7241 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    54318 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/__init__.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9876 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_group.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6412 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3244 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8072 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_rollback.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5428 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_ingress_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7081 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3470 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4334 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_se_linux_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4524 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_port.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6888 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6166 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6460 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4290 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_se_linux_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9918 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_webhook.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    27692 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    40603 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12465 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4861 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_key_selector.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5299 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_service_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6210 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6735 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_rolling_update_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7325 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13819 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_class.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4289 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_object_field_selector.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    31487 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11215 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3257 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state_running.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8041 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12600 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8991 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_column_definition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3457 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6548 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4052 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_webhook_throttle_config.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6224 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3448 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_readiness_gate.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8124 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range_item.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7975 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_access_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9266 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5925 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_component_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5130 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_empty_dir_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8218 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5709 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_projection.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4036 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4554 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_group_version_for_discovery.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3651 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_dns_config_option.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4191 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_device.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7284 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5260 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_event_series.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3284 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9287 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_priority_class.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7367 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4629 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_group_strategy_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6936 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3877 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_non_resource_attributes.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7193 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3714 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_job_template_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    27007 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_object_meta.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7003 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6880 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_resource_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11965 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_io_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3414 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_load_balancer_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3071 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_node_affinity.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6814 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5675 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_group_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6440 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_class_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3967 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_address.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8570 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_policy_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6791 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6428 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6849 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6696 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3771 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_aggregation_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4038 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_external_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6820 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7065 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_object_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6183 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7129 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_binding.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6570 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6410 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7177 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3336 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_rule_value.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    18120 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_event.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3816 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_sysctl.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7232 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5036 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_object_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6390 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    12378 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_io_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6616 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6561 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_external_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6894 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6770 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_affinity.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9025 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3943 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_id_range.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4212 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_ip_block.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6583 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_external_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11742 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_delete_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6828 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6894 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6785 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6368 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6280 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7023 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11864 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    29322 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3844 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_http_header.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3435 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_stateful_set_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7213 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_controller_revision.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7326 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3254 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6171 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_binding.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6504 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6801 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_rolling_update_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6390 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_template_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4333 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_handler.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7106 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_access_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5491 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_label_selector_requirement.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7342 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6256 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7037 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_quobyte_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4166 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_update_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6494 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3958 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4053 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_host_port_range.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3775 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_external_documentation.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3470 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scope_selector.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5701 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_user_info.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8506 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7464 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6520 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_binding_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5513 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_ingress_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4567 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5186 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_key_to_path.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    17028 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6820 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6929 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_condition.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4122 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3659 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_template_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7168 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6584 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4015 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_env_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6588 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5387 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7052 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6559 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8548 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_ceph_fs_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9025 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4742 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_host_path.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8118 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6796 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6751 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_vsphere_virtual_disk_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6394 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_lease_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4068 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_error.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3994 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4947 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_tls.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8243 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_policy_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    10284 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rbd_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6550 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_storage_class_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7350 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_config_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7435 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6640 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7355 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8410 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_owner_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7993 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_rules_review_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    30695 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_json_schema_props.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6520 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6638 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rolling_update_deployment.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6348 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4654 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6936 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4360 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_initializers.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4261 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_port.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3156 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_scale_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7879 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_toleration.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9165 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/version_info.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6475 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_target.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7019 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_token_review.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7824 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_affinity.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4178 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_strategy.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6412 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6210 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     2999 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_preconditions.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6821 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9910 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_account.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8471 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_port.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    11363 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_resource.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6256 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_metric_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4013 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_error.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6168 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4101 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apiregistration_v1beta1_service_reference.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3188 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6406 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6244 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3776 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_host_alias.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4931 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_conversion.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9317 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7602 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3287 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_flex_volume.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6578 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role_binding_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7290 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role_binding.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5381 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_egress_rule.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     3350 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_validation.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9184 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8239 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_azure_disk_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4084 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_tcp_socket_action.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4656 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_projected_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5385 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_se_linux_options.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     5574 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_value_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6232 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6028 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6724 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_token_review_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13479 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_spec.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)    13361 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_iscsi_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4955 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_daemon_set.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     7054 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_flex_persistent_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6442 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6839 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_flex_volume_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     8875 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_status.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4361 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_weighted_pod_affinity_term.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6394 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_event_list.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4054 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_env_source.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     4359 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_backend.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     6821 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration.py
--rw-r--r--   0 tomek     (1001) tomek     (1001)     9911 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_status.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     7466 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/configuration.py
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3969 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/extensions_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3991 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apis_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3986 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiregistration_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     9280 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authentication_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3976 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/networking_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3982 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authorization_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   151364 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/policy_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3845 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/version_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   255101 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_v1alpha1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    73300 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiregistration_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   168811 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/custom_objects_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   554610 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/extensions_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3991 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3998 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/admissionregistration_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3959 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   116862 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/admissionregistration_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3972 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/settings_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    58441 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/scheduling_v1alpha1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3980 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/certificates_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    75846 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/events_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     9320 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authentication_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    93868 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    82024 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/certificates_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    97283 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_v2beta2_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)  1466901 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/core_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    97283 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_v2beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3971 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    26711 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authorization_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    73510 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiregistration_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    58413 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/scheduling_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3976 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/scheduling_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    26841 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authorization_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3984 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authentication_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    93914 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_v2alpha1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3987 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/core_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    75902 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/coordination_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   112965 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3968 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/events_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3957 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     4778 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/__init__.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    58761 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_v1alpha1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    76048 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiextensions_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    76936 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/networking_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     7173 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/logs_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    97053 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    76540 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/settings_v1alpha1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   254417 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    58029 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/auditregistration_v1alpha1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    59835 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/admissionregistration_v1alpha1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3982 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiextensions_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3980 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/coordination_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   491395 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3961 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/policy_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   301189 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   128358 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   492645 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_v1beta2_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    92713 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_v1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3990 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/auditregistration_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3970 2019-03-23 20:49:20.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)   254987 2019-03-23 20:49:21.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_v1beta1_api.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    24982 2019-03-23 20:49:21.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api_client.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    11005 2019-03-23 20:49:21.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/rest.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    59207 2019-03-23 20:49:21.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/__init__.py
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/watch/
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     8111 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/watch/watch_test.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      613 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/watch/__init__.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     6882 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/watch/watch.py
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/stream/
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     2768 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/stream/ws_client.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      623 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/stream/__init__.py
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3348 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio/stream/ws_client_test.py
-drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/
--rw-rw-r--   0 tomek     (1001) tomek     (1001)       19 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/top_level.txt
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      917 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/PKG-INFO
--rw-rw-r--   0 tomek     (1001) tomek     (1001)        1 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/dependency_links.txt
--rw-rw-r--   0 tomek     (1001) tomek     (1001)    40101 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/SOURCES.txt
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      114 2019-03-24 09:02:14.000000 kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/requires.txt
--rw-rw-r--   0 tomek     (1001) tomek     (1001)      117 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/MANIFEST.in
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     3788 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/README.md
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     4213 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/CHANGELOG.md
--rw-rw-r--   0 tomek     (1001) tomek     (1001)     1449 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.0.0/CONTRIBUTING.md
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:24.000000 kubernetes_asyncio-9.1.0/
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     2472 2019-05-03 22:01:12.000000 kubernetes_asyncio-9.1.0/setup.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    11354 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.1.0/LICENSE
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      174 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.1.0/requirements.txt
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      917 2019-05-03 22:02:24.000000 kubernetes_asyncio-9.1.0/PKG-INFO
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      527 2019-05-03 22:02:24.000000 kubernetes_asyncio-9.1.0/setup.cfg
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      185 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.1.0/test-requirements.txt
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      974 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.1.0/tox.ini
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:24.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    22049 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/kube_config.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     1379 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/google_auth_test.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     2674 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/openid.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     2634 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/dateutil.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      632 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/config_exception.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3041 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/openid_test.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     6987 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/exec_provider_test.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      822 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/__init__.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3531 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/incluster_config.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    39607 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/kube_config_test.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      940 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/google_auth.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     2203 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/dateutil_test.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     4704 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/incluster_config_test.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3622 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/exec_provider.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      828 2019-05-03 22:01:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/__init__.py
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:24.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13180 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12576 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3315 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_flex_volume.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6352 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7855 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_webhook_client_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4154 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3998 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state_waiting.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8317 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_versions.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8632 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7328 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_controller_revision.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9911 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6342 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6590 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6596 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6496 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6276 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3685 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_capabilities.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4338 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_host_path_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7729 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresource_scale.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5686 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_glusterfs_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7344 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7164 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6720 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    23407 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4079 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_error.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6691 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7251 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3575 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_client_ip_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6123 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_scale_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6814 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7181 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4114 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_load_balancer_ingress.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4093 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_policy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4920 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rolling_update_daemon_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5646 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_projection.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6220 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8293 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_ceph_fs_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6834 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_token_review_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6929 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4218 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_update_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5412 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7543 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_aws_elastic_block_store_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4188 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_update_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6666 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4338 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_flocker_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6190 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3395 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_stateful_set_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4771 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_env_from_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4792 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_ref.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5344 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_portworx_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13077 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7221 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_local_subject_access_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7858 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_node_config_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10789 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6410 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_binding_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_scale.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9149 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_resource_attributes.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    14774 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7210 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_access_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7350 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_glusterfs_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4486 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_token_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6414 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12786 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5743 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_taint.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3135 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_config_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3725 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_job_template_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3918 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4429 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_photon_persistent_disk_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6710 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5804 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_affinity_term.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6779 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4267 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ip_block.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4906 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_key_selector.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3505 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6675 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3226 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4955 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_daemon_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7092 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_object_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4129 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_attached_volume.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4072 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7081 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8725 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8656 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9872 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_object_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6100 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_lease.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7196 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_mount.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5302 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_git_repo_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6924 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_resource_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5776 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_projection.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6617 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8203 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3117 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_session_affinity_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4545 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6242 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3205 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_downward_api_projection.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7436 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5179 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_service_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7274 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_binding.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7089 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7163 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoints.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5072 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_object_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7916 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_rollback.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5087 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4727 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_affinity.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13448 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_security_context.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3121 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6739 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6502 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4828 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event_series.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9209 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4657 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_downward_api_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7495 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_webhook_client_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7197 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6340 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoints_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4002 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_external_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4678 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7988 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_os_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6100 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8079 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6584 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5371 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_nfs_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3176 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_initializer.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10967 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6944 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5283 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_cross_version_object_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6297 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4599 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_non_resource_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    15004 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7798 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6582 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_controller_revision_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13330 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_system_info.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13816 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_iscsi_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6500 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_component_status_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7741 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7933 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4836 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_label_selector.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6873 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_fc_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10822 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6364 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3735 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_watch_event.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    15004 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4041 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresources.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6957 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_access_review_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6671 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5101 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_field_selector.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3279 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4148 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_update_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7052 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6906 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4118 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_update_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4310 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_topology_selector_label_requirement.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4539 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5606 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_user_info.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6354 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4786 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_host_path.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6658 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4827 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoint_port.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7512 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_gce_persistent_disk_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8129 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6627 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_http_get_action.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6574 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_priority_class_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5240 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_azure_file_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4633 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_path.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6954 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6762 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6561 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cinder_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7344 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7366 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_local_subject_access_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4000 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4742 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_initializer.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13503 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5742 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_env_var_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7312 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4221 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_preferred_scheduling_term.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6660 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6458 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7386 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7548 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_lease_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8667 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_policy_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6596 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_priority_class_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4009 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_host_port_range.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6615 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4858 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_peer.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    23097 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3881 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6874 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_token_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7139 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3541 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_selector.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6273 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3479 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/runtime_raw_extension.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10796 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10619 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rbd_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9597 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6644 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6692 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_controller_revision_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6452 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11405 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5299 2019-05-03 21:32:10.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_env_var.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8414 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_status_details.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6392 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4178 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_update_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    14034 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_storage_class.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6534 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4282 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4622 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_supplemental_groups_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6944 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4013 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_webhook.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7694 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7363 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5353 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6375 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_account_token_projection.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8203 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_os_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4454 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_access_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6202 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_template.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10777 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7189 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_port.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5665 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoint_subset.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6027 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoint_address.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3854 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6859 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6374 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12759 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4482 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_local_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3813 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_aggregation_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3263 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_rollback_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7868 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_rules_review_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4873 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4971 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11785 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5613 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_status_cause.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9747 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7566 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4867 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_ref.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3127 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_endpoint.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6722 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4999 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_service_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12974 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_scale.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3702 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_lifecycle.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3917 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_identifier.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4654 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_non_resource_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6353 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_eviction.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    17071 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6426 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_downward_api_volume_file.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5734 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scoped_resource_selector_requirement.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9731 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_version.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6658 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10816 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_csi_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7284 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4052 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13267 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4616 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_user_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6542 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_binding_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6430 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3184 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6688 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6465 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_component_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4768 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_peer.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7908 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_anti_affinity.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5274 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7601 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5246 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_typed_local_object_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4439 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_selector_term.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3240 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_local_object_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5208 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cross_version_object_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6849 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6829 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6392 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6206 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10048 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_probe.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3512 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3400 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rolling_update_stateful_set_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6790 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6206 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_metric_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6501 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_subject.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4882 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_ref.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7415 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8023 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6529 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7396 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8632 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state_terminated.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5691 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_dns_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3816 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_exec_action.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6550 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_azure_file_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11557 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7019 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5296 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_egress_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4172 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_image.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4541 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_token_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8994 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_attributes.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6458 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6588 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5283 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_cross_version_object_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4573 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_group_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6733 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5184 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8581 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_names.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3806 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_aggregation_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6652 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_account_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4715 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_server_address_by_client_cidr.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3304 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6138 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6669 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_list_meta.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    31027 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5292 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11528 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_security_context.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4437 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_fs_group_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6542 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6692 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_controller_revision_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3987 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_id_range.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5230 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6907 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6733 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4262 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9314 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_priority_class.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7303 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_binding.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7752 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4293 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6501 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3243 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_daemon_endpoints.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6559 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7328 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_controller_revision.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7512 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_rule_with_operations.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12786 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4803 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_requirements.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4493 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_fs_group_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3261 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6302 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3609 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_topology_selector_term.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3822 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_non_resource_attributes.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6292 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4560 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_user_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6736 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cinder_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5672 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_selector_requirement.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7711 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_webhook_client_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6936 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3305 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_rollback_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3153 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7241 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    54318 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/__init__.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9876 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_group.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6412 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3244 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8072 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_rollback.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5428 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_ingress_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7081 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3470 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4334 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_se_linux_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4524 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_port.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6888 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6166 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6460 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4290 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_se_linux_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9918 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_webhook.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    27692 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    40603 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12465 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4861 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_key_selector.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5299 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_service_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6210 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6735 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_rolling_update_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7325 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13819 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_class.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4289 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_object_field_selector.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    31487 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11215 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3257 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state_running.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8041 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6878 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12600 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8991 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_column_definition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3457 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6548 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4052 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_webhook_throttle_config.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6224 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3448 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_readiness_gate.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8124 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range_item.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7975 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_access_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9266 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5925 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_component_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5130 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_empty_dir_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8218 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5709 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_projection.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4036 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4554 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_group_version_for_discovery.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3651 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_dns_config_option.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4191 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_device.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7284 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5260 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_event_series.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3284 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9287 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_priority_class.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7367 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4629 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_group_strategy_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6936 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3877 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_non_resource_attributes.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7193 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3714 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_job_template_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    27007 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_object_meta.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7003 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6880 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_resource_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11965 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_io_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3414 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_load_balancer_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3071 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_node_affinity.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6814 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5675 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_group_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6440 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_class_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3967 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_address.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8570 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_policy_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6791 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6428 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6849 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6696 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3771 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_aggregation_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4038 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_external_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6820 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7065 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_object_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6183 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7129 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_binding.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6570 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6410 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7177 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3336 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_rule_value.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    18120 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_event.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3816 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_sysctl.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7232 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5036 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_object_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6390 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    12378 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_io_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6616 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6561 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_external_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6894 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6770 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_affinity.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9025 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3943 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_id_range.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4212 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_ip_block.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6583 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_external_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11742 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_delete_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6828 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6894 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6785 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6368 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6280 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7023 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11864 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    29322 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3844 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_http_header.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3435 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_stateful_set_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7213 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_controller_revision.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7326 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3254 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6171 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_binding.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6504 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6801 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_rolling_update_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6390 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_template_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4333 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_handler.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7106 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_access_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5491 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_label_selector_requirement.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7342 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6256 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7037 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_quobyte_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4166 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_update_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6494 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3958 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4053 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_host_port_range.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3775 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_external_documentation.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3470 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scope_selector.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5701 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_user_info.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8506 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7464 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6520 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_binding_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5513 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_ingress_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4567 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5186 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_key_to_path.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    17028 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6820 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6929 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_condition.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4122 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3659 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_template_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7168 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6584 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4015 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_env_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6588 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5387 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7052 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6559 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8548 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_ceph_fs_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9025 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4742 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_host_path.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8118 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6796 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6751 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_vsphere_virtual_disk_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6394 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_lease_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4068 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_error.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3994 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4947 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_tls.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8243 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_policy_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    10284 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rbd_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6550 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_storage_class_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7350 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_config_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7435 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6640 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7355 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8410 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_owner_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7993 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_rules_review_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    30695 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_json_schema_props.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6520 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6638 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rolling_update_deployment.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6348 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4654 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6936 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4360 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_initializers.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4261 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_port.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3156 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_scale_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7879 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_toleration.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9165 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/version_info.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6475 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_target.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7019 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_token_review.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7824 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_affinity.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4178 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_strategy.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6412 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6210 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     2999 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_preconditions.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6821 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9910 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_account.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8471 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_port.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    11363 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_resource.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6256 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_metric_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4013 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_error.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6168 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4101 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apiregistration_v1beta1_service_reference.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3188 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6406 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6244 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3776 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_host_alias.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4931 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_conversion.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9317 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7602 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3287 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_flex_volume.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6578 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role_binding_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7290 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role_binding.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5381 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_egress_rule.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     3350 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_validation.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9184 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8239 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_azure_disk_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4084 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_tcp_socket_action.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4656 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_projected_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6832 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5385 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_se_linux_options.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     5574 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_value_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6232 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6028 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6724 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_token_review_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13479 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_spec.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)    13361 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_iscsi_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4955 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_daemon_set.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     7054 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_flex_persistent_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6442 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6839 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_flex_volume_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     8875 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_status.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4361 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_weighted_pod_affinity_term.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6394 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_event_list.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4054 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_env_source.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     4359 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_backend.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     6821 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration.py
+-rw-r--r--   0 tomek     (1001) tomek     (1001)     9911 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_status.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     7466 2019-05-03 22:01:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/configuration.py
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3969 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/extensions_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3991 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apis_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3986 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiregistration_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     9280 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authentication_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3976 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/networking_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3982 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authorization_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   151364 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/policy_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3845 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/version_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   255101 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_v1alpha1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    73300 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiregistration_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   168811 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/custom_objects_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   554610 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/extensions_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3991 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3998 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/admissionregistration_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3959 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   116862 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/admissionregistration_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3972 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/settings_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    58441 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/scheduling_v1alpha1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3980 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/certificates_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    75846 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/events_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     9320 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authentication_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    93868 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    82024 2019-05-03 21:32:11.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/certificates_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    97283 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_v2beta2_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)  1466901 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/core_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    97283 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_v2beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3971 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    26711 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authorization_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    73510 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiregistration_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    58413 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/scheduling_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3976 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/scheduling_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    26841 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authorization_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3984 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authentication_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    93914 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_v2alpha1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3987 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/core_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    75902 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/coordination_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   112965 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3968 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/events_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3957 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     4778 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/__init__.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    58761 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_v1alpha1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    76048 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiextensions_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    76936 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/networking_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     7173 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/logs_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    97053 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    76540 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/settings_v1alpha1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   254417 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    58029 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/auditregistration_v1alpha1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    59835 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/admissionregistration_v1alpha1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3982 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiextensions_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3980 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/coordination_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   491395 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3961 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/policy_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   301189 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   128358 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   492645 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_v1beta2_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    92713 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_v1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3990 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/auditregistration_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3970 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)   254987 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_v1beta1_api.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    24982 2019-05-03 22:01:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api_client.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    11005 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/rest.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    59207 2019-05-03 22:01:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/__init__.py
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:24.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/watch/
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     8111 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/watch/watch_test.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      613 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/watch/__init__.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     7054 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/watch/watch.py
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:24.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/stream/
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     2768 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/stream/ws_client.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      623 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/stream/__init__.py
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     3348 2019-05-03 21:32:12.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio/stream/ws_client_test.py
+drwxrwxr-x   0 tomek     (1001) tomek     (1001)        0 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)       19 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/top_level.txt
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      917 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/PKG-INFO
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)        1 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)    40101 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      114 2019-05-03 22:02:23.000000 kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/requires.txt
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)      117 2019-03-23 20:42:18.000000 kubernetes_asyncio-9.1.0/MANIFEST.in
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     4035 2019-05-03 21:18:34.000000 kubernetes_asyncio-9.1.0/README.md
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     5282 2019-05-03 21:42:52.000000 kubernetes_asyncio-9.1.0/CHANGELOG.md
+-rw-rw-r--   0 tomek     (1001) tomek     (1001)     1123 2019-05-03 21:16:57.000000 kubernetes_asyncio-9.1.0/CONTRIBUTING.md
```

### Comparing `kubernetes_asyncio-9.0.0/setup.py` & `kubernetes_asyncio-9.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup
 
 # Do not edit these constants. They will be updated automatically
 # by scripts/update-client.sh.
-CLIENT_VERSION = "9.0.0"
+CLIENT_VERSION = "9.1.0"
 PACKAGE_NAME = "kubernetes_asyncio"
 DEVELOPMENT_STATUS = "5 - Production/Stable"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
```

### Comparing `kubernetes_asyncio-9.0.0/LICENSE` & `kubernetes_asyncio-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/PKG-INFO` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: kubernetes_asyncio
-Version: 9.0.0
+Name: kubernetes-asyncio
+Version: 9.1.0
 Summary: Kubernetes asynchronous python client
 Home-page: https://github.com/tomplus/kubernetes_asyncio
 Author: Kubernetes
 Author-email: UNKNOWN
 License: Apache License Version 2.0
 Description:     Python client for kubernetes http://kubernetes.io/
```

### Comparing `kubernetes_asyncio-9.0.0/setup.cfg` & `kubernetes_asyncio-9.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/tox.ini` & `kubernetes_asyncio-9.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/kube_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/kube_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,32 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
 import atexit
 import base64
+import copy
 import datetime
 import json
 import logging
 import os
+import platform
 import tempfile
 
 import yaml
 
 from kubernetes_asyncio.client import ApiClient, Configuration
 
 from .config_exception import ConfigException
 from .dateutil import UTC, parse_rfc3339
 from .exec_provider import ExecProvider
 from .google_auth import google_auth_credentials
 from .openid import OpenIDRequestor
 
 EXPIRY_SKEW_PREVENTION_DELAY = datetime.timedelta(minutes=5)
 KUBE_CONFIG_DEFAULT_LOCATION = os.environ.get('KUBECONFIG', '~/.kube/config')
+ENV_KUBECONFIG_PATH_SEPARATOR = ';' if platform.system() == 'Windows' else ':'
 PROVIDER_TYPE_OIDC = 'oidc'
 _temp_files = {}
 
 
 def _cleanup_temp_files():
     global _temp_files
     for temp_file in _temp_files.values():
@@ -124,15 +127,20 @@
 
 class KubeConfigLoader(object):
 
     def __init__(self, config_dict, active_context=None,
                  get_google_credentials=None,
                  config_base_path="",
                  config_persister=None):
-        self._config = ConfigNode('kube-config', config_dict)
+
+        if isinstance(config_dict, ConfigNode):
+            self._config = config_dict
+        else:
+            self._config = ConfigNode('kube-config', config_dict)
+
         self._current_context = None
         self._user = None
         self._cluster = None
         self.provider = None
         self.set_active_context(active_context)
         self._config_base_path = config_base_path
         self._config_persister = config_persister
@@ -304,42 +312,51 @@
                 return None
             self.token = "Bearer %s" % status['token']
             return True
         except Exception as e:
             logging.error(str(e))
 
     def _load_user_token(self):
+        base_path = self._get_base_path(self._user.path)
         token = FileOrData(
             self._user, 'tokenFile', 'token',
-            file_base_path=self._config_base_path,
+            file_base_path=base_path,
             base64_file_content=False).as_data()
         if token:
             self.token = "Bearer %s" % token
             return True
 
     def _load_user_pass_token(self):
         if 'username' in self._user and 'password' in self._user:
             basic_auth = self._user['username'] + ':' + self._user['password']
             self.token = 'Basic ' + base64.b64encode(
                 basic_auth.encode()).decode('utf-8')
             return True
 
+    def  _get_base_path(self, config_path):
+        if self._config_base_path is not None:
+            return self._config_base_path
+        if config_path is not None:
+            return os.path.abspath(os.path.dirname(config_path))
+        return ""
+
     def _load_cluster_info(self):
         if 'server' in self._cluster:
             self.host = self._cluster['server'].rstrip('/')
             if self.host.startswith("https"):
+                base_path = self._get_base_path(self._cluster.path)
                 self.ssl_ca_cert = FileOrData(
                     self._cluster, 'certificate-authority',
-                    file_base_path=self._config_base_path).as_file()
+                    file_base_path=base_path).as_file()
                 self.cert_file = FileOrData(
                     self._user, 'client-certificate',
-                    file_base_path=self._config_base_path).as_file()
+                    file_base_path=base_path).as_file()
                 self.key_file = FileOrData(
                     self._user, 'client-key',
-                    file_base_path=self._config_base_path).as_file()
+                    file_base_path=base_path).as_file()
         if 'insecure-skip-tls-verify' in self._cluster:
             self.verify_ssl = not self._cluster['insecure-skip-tls-verify']
 
     def _set_config(self, client_configuration):
 
         if 'token' in self.__dict__:
             client_configuration.api_key['authorization'] = self.token
@@ -364,17 +381,18 @@
 
 
 class ConfigNode(object):
     """Remembers each config key's path and construct a relevant exception
     message in case of missing keys. The assumption is all access keys are
     present in a well-formed kube-config."""
 
-    def __init__(self, name, value):
+    def __init__(self, name, value, path=None):
         self.name = name
         self.value = value
+        self.path = path
 
     def __contains__(self, key):
         return key in self.value
 
     def __len__(self):
         return len(self.value)
 
@@ -386,15 +404,15 @@
     def __getitem__(self, key):
         v = self.safe_get(key)
         if not v:
             raise ConfigException(
                 'Invalid kube-config file. Expected key %s in %s'
                 % (key, self.name))
         if isinstance(v, dict) or isinstance(v, list):
-            return ConfigNode('%s/%s' % (self.name, key), v)
+            return ConfigNode('%s/%s' % (self.name, key), v, self.path)
         else:
             return v
 
     def get_with_name(self, name, safe=False):
         if not isinstance(self.value, list):
             raise ConfigException(
                 'Invalid kube-config file. Expected %s to be a list'
@@ -411,28 +429,100 @@
                     result = v
                 else:
                     raise ConfigException(
                         'Invalid kube-config file. '
                         'Expected only one object with name %s in %s list'
                         % (name, self.name))
         if result is not None:
-            return ConfigNode('%s[name=%s]' % (self.name, name), result)
+            if isinstance(result, ConfigNode):
+                return result
+            else:
+                return ConfigNode(
+                    '%s[name=%s]' %
+                    (self.name, name), result, self.path)
         if safe:
             return None
         raise ConfigException(
             'Invalid kube-config file. '
             'Expected object with name %s in %s list' % (name, self.name))
 
 
-def _get_kube_config_loader_for_yaml_file(filename, **kwargs):
-    with open(filename) as f:
-        return KubeConfigLoader(
-            config_dict=yaml.safe_load(f),
-            config_base_path=os.path.abspath(os.path.dirname(filename)),
-            **kwargs)
+class KubeConfigMerger:
+
+    """Reads and merges configuration from one or more kube-config's.
+    The propery `config` can be passed to the KubeConfigLoader as config_dict.
+    It uses a path attribute from ConfigNode to store the path to kubeconfig.
+    This path is required to load certs from relative paths.
+    A method `save_changes` updates changed kubeconfig's (it compares current
+    state of dicts with).
+    """
+
+    def __init__(self, paths):
+        self.paths = []
+        self.config_files = {}
+        self.config_merged = None
+
+        for path in paths.split(ENV_KUBECONFIG_PATH_SEPARATOR):
+            if path:
+                path = os.path.expanduser(path)
+                if os.path.exists(path):
+                    self.paths.append(path)
+                    self.load_config(path)
+        self.config_saved = copy.deepcopy(self.config_files)
+
+    @property
+    def config(self):
+        return self.config_merged
+
+    def load_config(self, path):
+        with open(path) as f:
+            config = yaml.safe_load(f)
+
+        if self.config_merged is None:
+            config_merged = copy.deepcopy(config)
+            for item in ('clusters', 'contexts', 'users'):
+                config_merged[item] = []
+            self.config_merged = ConfigNode(path, config_merged, path)
+
+        for item in ('clusters', 'contexts', 'users'):
+            self._merge(item, config[item], path)
+        self.config_files[path] = config
+
+    def _merge(self, item, add_cfg, path):
+        for new_item in add_cfg:
+            for exists in self.config_merged.value[item]:
+                if exists['name'] == new_item['name']:
+                    break
+            else:
+                self.config_merged.value[item].append(ConfigNode(
+                    '{}/{}'.format(path, new_item), new_item, path))
+
+    def save_changes(self):
+        for path in self.paths:
+            if self.config_saved[path] != self.config_files[path]:
+                self.save_config(path)
+        self.config_saved = copy.deepcopy(self.config_files)
+
+    def save_config(self, path):
+        with open(path, 'w') as f:
+            yaml.safe_dump(self.config_files[path], f,
+                           default_flow_style=False)
+
+
+def _get_kube_config_loader_for_yaml_file(
+        filename, persist_config=False, **kwargs):
+
+    kcfg = KubeConfigMerger(filename)
+    if persist_config and 'config_persister' not in kwargs:
+        kwargs['config_persister'] = kcfg.save_changes()
+
+    return KubeConfigLoader(
+        config_dict=kcfg.config,
+        config_base_path=None,
+        **kwargs)
 
 
 def list_kube_config_contexts(config_file=None):
 
     if config_file is None:
         config_file = os.path.expanduser(KUBE_CONFIG_DEFAULT_LOCATION)
 
@@ -452,26 +542,19 @@
     :param client_configuration: The kubernetes.client.Configuration to
         set configs to.
     :param persist_config: If True, config file will be updated when changed
         (e.g GCP token refresh).
     """
 
     if config_file is None:
-        config_file = os.path.expanduser(KUBE_CONFIG_DEFAULT_LOCATION)
-
-    config_persister = None
-    if persist_config:
-        def _save_kube_config(config_map):
-            with open(config_file, 'w') as f:
-                yaml.safe_dump(config_map, f, default_flow_style=False)
-        config_persister = _save_kube_config
+        config_file = KUBE_CONFIG_DEFAULT_LOCATION
 
     loader = _get_kube_config_loader_for_yaml_file(
         config_file, active_context=context,
-        config_persister=config_persister)
+        persist_config=persist_config)
     if client_configuration is None:
         config = type.__call__(Configuration)
         await loader.load_and_set(config)
         Configuration.set_default(config)
     else:
         await loader.load_and_set(client_configuration)
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/google_auth_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/google_auth_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/openid.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/openid.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/dateutil.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/dateutil.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/config_exception.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/config_exception.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/openid_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/openid_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/exec_provider_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/exec_provider_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/__init__.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/incluster_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/incluster_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/kube_config_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/kube_config_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 
 import yaml
 from asynctest import Mock, TestCase, main, patch
 from six import PY3
 
 from .config_exception import ConfigException
 from .kube_config import (
-    ConfigNode, FileOrData, KubeConfigLoader, _cleanup_temp_files,
-    _create_temp_file_with_content, list_kube_config_contexts,
-    load_kube_config, new_client_from_config, refresh_token,
+    ENV_KUBECONFIG_PATH_SEPARATOR, ConfigNode,
+    FileOrData, KubeConfigLoader, KubeConfigMerger,
+    _cleanup_temp_files, _create_temp_file_with_content,
+    list_kube_config_contexts, load_kube_config,
+    new_client_from_config, refresh_token,
 )
 
 BEARER_TOKEN_FORMAT = "Bearer %s"
 
 NON_EXISTING_FILE = "zz_non_existing_file_472398324"
 
 
@@ -914,9 +916,171 @@
         with self.assertRaises(AssertionError):
             await refresh_token(loader, mock_config)
 
         self.assertEqual(BEARER_TOKEN_FORMAT % TEST_DATA_BASE64,
                          loader.token)
 
 
+class TestKubeConfigMerger(BaseTestCase):
+    TEST_KUBE_CONFIG_PART1 = {
+        "current-context": "no_user",
+        "contexts": [
+            {
+                "name": "no_user",
+                "context": {
+                    "cluster": "default"
+                }
+            },
+        ],
+        "clusters": [
+            {
+                "name": "default",
+                "cluster": {
+                    "server": TEST_HOST
+                }
+            },
+        ],
+        "users": []
+    }
+
+    TEST_KUBE_CONFIG_PART2 = {
+        "current-context": "",
+        "contexts": [
+            {
+                "name": "ssl",
+                "context": {
+                    "cluster": "ssl",
+                    "user": "ssl"
+                }
+            },
+            {
+                "name": "simple_token",
+                "context": {
+                    "cluster": "default",
+                    "user": "simple_token"
+                }
+            },
+        ],
+        "clusters": [
+            {
+                "name": "ssl",
+                "cluster": {
+                    "server": TEST_SSL_HOST,
+                    "certificate-authority-data":
+                        TEST_CERTIFICATE_AUTH_BASE64,
+                }
+            },
+        ],
+        "users": [
+            {
+                "name": "ssl",
+                "user": {
+                    "token": TEST_DATA_BASE64,
+                    "client-certificate-data": TEST_CLIENT_CERT_BASE64,
+                    "client-key-data": TEST_CLIENT_KEY_BASE64,
+                }
+            },
+        ]
+    }
+
+    TEST_KUBE_CONFIG_PART3 = {
+        "current-context": "no_user",
+        "contexts": [
+            {
+                "name": "expired_oidc",
+                "context": {
+                    "cluster": "default",
+                    "user": "expired_oidc"
+                }
+            },
+            {
+                "name": "ssl",
+                "context": {
+                    "cluster": "skipped-part2-defined-this-context",
+                    "user": "skipped"
+                }
+            },
+        ],
+        "clusters": [
+        ],
+        "users": [
+            {
+                "name": "expired_oidc",
+                "user": {
+                    "auth-provider": {
+                        "name": "oidc",
+                        "config": {
+                            "client-id": "tectonic-kubectl",
+                            "client-secret": "FAKE_SECRET",
+                            "id-token": TEST_OIDC_EXPIRED_LOGIN,
+                            "idp-certificate-authority-data": TEST_OIDC_CA,
+                            "idp-issuer-url": "https://example.org/identity",
+                            "refresh-token":
+                                "lucWJjEhlxZW01cXI3YmVlcYnpxNGhzk"
+                        }
+                    }
+                }
+            },
+            {
+                "name": "simple_token",
+                "user": {
+                    "token": TEST_DATA_BASE64,
+                    "username": TEST_USERNAME,  # should be ignored
+                    "password": TEST_PASSWORD,  # should be ignored
+                }
+            },
+        ]
+    }
+
+    def _create_multi_config(self):
+        files = []
+        for part in (
+                self.TEST_KUBE_CONFIG_PART1,
+                self.TEST_KUBE_CONFIG_PART2,
+                self.TEST_KUBE_CONFIG_PART3):
+            files.append(self._create_temp_file(yaml.safe_dump(part)))
+        return ENV_KUBECONFIG_PATH_SEPARATOR.join(files)
+
+    def test_list_kube_config_contexts(self):
+        kubeconfigs = self._create_multi_config()
+        expected_contexts = [
+            {'context': {'cluster': 'default'}, 'name': 'no_user'},
+            {'context': {'cluster': 'ssl', 'user': 'ssl'}, 'name': 'ssl'},
+            {'context': {'cluster': 'default', 'user': 'simple_token'},
+             'name': 'simple_token'},
+            {'context': {'cluster': 'default', 'user': 'expired_oidc'}, 'name': 'expired_oidc'}]
+
+        contexts, active_context = list_kube_config_contexts(
+            config_file=kubeconfigs)
+
+        self.assertEqual(contexts, expected_contexts)
+        self.assertEqual(active_context, expected_contexts[0])
+
+    async def test_new_client_from_config(self):
+        kubeconfigs = self._create_multi_config()
+        client = await new_client_from_config(
+            config_file=kubeconfigs, context="simple_token")
+        self.assertEqual(TEST_HOST, client.configuration.host)
+        self.assertEqual(BEARER_TOKEN_FORMAT % TEST_DATA_BASE64,
+                         client.configuration.api_key['authorization'])
+
+    def test_save_changes(self):
+        kubeconfigs = self._create_multi_config()
+
+        # load configuration, update token, save config
+        kconf = KubeConfigMerger(kubeconfigs)
+        user = kconf.config['users'].get_with_name('expired_oidc')['user']
+        provider = user['auth-provider']['config']
+        provider.value['id-token'] = "token-changed"
+        kconf.save_changes()
+
+        # re-read configuration
+        kconf = KubeConfigMerger(kubeconfigs)
+        user = kconf.config['users'].get_with_name('expired_oidc')['user']
+        provider = user['auth-provider']['config']
+
+        # new token
+        self.assertEqual(provider.value['id-token'], "token-changed")
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/google_auth.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/google_auth.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/dateutil_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/dateutil_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/incluster_config_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/incluster_config_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/config/exec_provider.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/config/exec_provider.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/__init__.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __project__ = 'kubernetes_asyncio'
 # The version is auto-updated. Please do not edit.
-__version__ = "9.0.0"
+__version__ = "9.1.0"
 
 import kubernetes_asyncio.client
 import kubernetes_asyncio.config
 import kubernetes_asyncio.watch
 import kubernetes_asyncio.stream
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_flex_volume.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_flex_volume.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_webhook_client_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_webhook_client_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state_waiting.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state_waiting.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_versions.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_versions.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_controller_revision.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_controller_revision.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_capabilities.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_capabilities.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_host_path_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_host_path_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresource_scale.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresource_scale.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_glusterfs_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_glusterfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_error.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_error.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_client_ip_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_client_ip_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_scale_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_scale_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_load_balancer_ingress.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_load_balancer_ingress.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_policy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_policy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rolling_update_daemon_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rolling_update_daemon_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_projection.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_projection.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_ceph_fs_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_ceph_fs_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_token_review_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_token_review_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_update_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_aws_elastic_block_store_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_aws_elastic_block_store_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_update_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_flocker_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_flocker_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_stateful_set_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_stateful_set_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_env_from_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_env_from_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_ref.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_ref.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_portworx_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_portworx_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_local_subject_access_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_local_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_node_config_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_node_config_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_binding_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_scale.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_scale.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_resource_attributes.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_access_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_glusterfs_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_glusterfs_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_token_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_token_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_taint.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_taint.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_config_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_config_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_job_template_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_job_template_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_photon_persistent_disk_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_photon_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_affinity_term.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ip_block.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ip_block.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_key_selector.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_key_selector.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_daemon_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_rolling_update_daemon_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_object_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_object_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_attached_volume.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_attached_volume.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_object_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_object_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_lease.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_lease.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_mount.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_mount.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_git_repo_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_git_repo_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_resource_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_resource_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_projection.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_projection.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_session_affinity_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_session_affinity_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_downward_api_projection.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_downward_api_projection.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_service_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_service_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_binding.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_binding.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoints.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoints.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_object_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_object_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_rollback.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_rollback.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_affinity.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_affinity.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_security_context.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_security_context.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event_series.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event_series.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_downward_api_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_downward_api_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_webhook_client_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_webhook_client_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoints_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoints_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_external_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_external_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_os_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_os_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_nfs_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_nfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_initializer.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_initializer.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_cross_version_object_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_cross_version_object_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_non_resource_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_non_resource_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_controller_revision_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_controller_revision_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_system_info.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_system_info.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_iscsi_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_iscsi_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_component_status_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_component_status_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_label_selector.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_label_selector.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_fc_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_fc_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_watch_event.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_watch_event.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresources.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_subresources.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_access_review_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_access_review_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_field_selector.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_field_selector.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_update_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_update_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_topology_selector_label_requirement.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_topology_selector_label_requirement.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_user_info.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_user_info.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_host_path.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_allowed_host_path.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoint_port.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoint_port.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_gce_persistent_disk_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_gce_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_http_get_action.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_http_get_action.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_priority_class_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_priority_class_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_azure_file_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_azure_file_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_path.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cinder_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cinder_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_local_subject_access_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_local_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_initializer.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_initializer.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_env_var_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_env_var_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_preferred_scheduling_term.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_lease_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_lease_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_policy_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_policy_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_priority_class_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_priority_class_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_host_port_range.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_host_port_range.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_peer.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_peer.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_token_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_token_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_selector.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_selector.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_scale_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/runtime_raw_extension.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/runtime_raw_extension.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rbd_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rbd_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_controller_revision_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_controller_revision_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_env_var.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_env_var.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_status_details.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_status_details.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_update_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_storage_class.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_storage_class.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_supplemental_groups_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_supplemental_groups_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_webhook.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_webhook.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_account_token_projection.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_account_token_projection.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_os_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_os_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_access_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_access_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_template.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_template.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_port.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_port.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoint_subset.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoint_subset.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_endpoint_address.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_endpoint_address.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_validating_webhook_configuration.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_local_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_local_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_aggregation_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_aggregation_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_rollback_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_rollback_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_rules_review_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_rules_review_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_status_cause.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_status_cause.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_ref.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_ref.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_endpoint.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_endpoint.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_service_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_service_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_scale.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_scale.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_lifecycle.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_lifecycle.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_identifier.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_non_resource_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_non_resource_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_eviction.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_eviction.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_downward_api_volume_file.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_downward_api_volume_file.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scoped_resource_selector_requirement.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scoped_resource_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_version.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_version.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_csi_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_csi_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_user_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_user_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_binding_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_component_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_component_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_peer.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_peer.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_anti_affinity.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_typed_local_object_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_typed_local_object_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_selector_term.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_selector_term.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_local_object_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_local_object_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cross_version_object_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cross_version_object_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_probe.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_probe.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rolling_update_stateful_set_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rolling_update_stateful_set_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_metric_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_metric_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_subject.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_subject.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_ref.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_ref.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state_terminated.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state_terminated.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_dns_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_dns_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_exec_action.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_exec_action.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_azure_file_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_azure_file_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_egress_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_egress_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_image.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_image.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_token_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_token_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_attributes.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_cross_version_object_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_cross_version_object_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_group_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_group_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_names.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_names.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_aggregation_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_aggregation_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_account_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_account_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_server_address_by_client_cidr.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_server_address_by_client_cidr.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_list_meta.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_list_meta.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_pod_security_policy_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_security_context.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_security_context.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_fs_group_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_fs_group_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_controller_revision_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_controller_revision_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_id_range.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_id_range.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_priority_class.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_priority_class.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_role_binding.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_role_binding.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_daemon_endpoints.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_daemon_endpoints.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_controller_revision.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_controller_revision.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_rule_with_operations.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_rule_with_operations.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_requirements.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_requirements.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_fs_group_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_fs_group_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_topology_selector_term.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_topology_selector_term.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_non_resource_attributes.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_non_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_user_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_run_as_user_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cinder_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cinder_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_selector_requirement.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_webhook_client_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apiextensions_v1beta1_webhook_client_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_rollback_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_rollback_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/__init__.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_group.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_group.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_stateful_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_self_subject_rules_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_rollback.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_rollback.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_ingress_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_ingress_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_attachment_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_attachment_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_se_linux_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_se_linux_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_port.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_port.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_se_linux_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_se_linux_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_webhook.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_webhook.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_key_selector.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_key_selector.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_service_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/admissionregistration_v1beta1_service_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_rolling_update_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_rolling_update_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_class.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_class.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_object_field_selector.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_object_field_selector.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_deployment_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_deployment_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_container_state_running.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_container_state_running.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_pod_security_policy_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_column_definition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_column_definition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_webhook_throttle_config.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_webhook_throttle_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_job_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_job_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_readiness_gate.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_readiness_gate.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range_item.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range_item.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_access_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_access_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_component_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_component_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_empty_dir_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_empty_dir_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_projection.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_projection.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_resource_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_group_version_for_discovery.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_group_version_for_discovery.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_dns_config_option.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_dns_config_option.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_device.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_device.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_event_series.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_event_series.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_limit_range_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_limit_range_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_priority_class.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_priority_class.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_group_strategy_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_run_as_group_strategy_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_non_resource_attributes.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_non_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_job_template_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_job_template_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_object_meta.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_object_meta.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_resource_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_resource_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_io_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_io_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_load_balancer_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_load_balancer_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_node_affinity.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_group_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_group_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_storage_class_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_storage_class_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_address.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_address.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_policy_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_policy_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_stateful_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_stateful_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2alpha1_cron_job.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2alpha1_cron_job.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_aggregation_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_aggregation_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_external_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_external_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cron_job.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cron_job.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_object_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_object_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_scale_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role_binding.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role_binding.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_horizontal_pod_autoscaler_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_rule_value.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_http_ingress_rule_value.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_event.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_event.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_sysctl.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_sysctl.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_object_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_object_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_api_service_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_api_service_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_io_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_io_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_quota_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_quota_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_external_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_external_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_daemon_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_affinity.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_affinity.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_id_range.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_id_range.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_ip_block.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_ip_block.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_external_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_external_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_delete_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_delete_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_daemon_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_resource_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_resource_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_http_header.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_http_header.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_stateful_set_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_stateful_set_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_controller_revision.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_controller_revision.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_rules_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_service_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_service_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_binding.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_binding.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_rolling_update_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_rolling_update_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_template_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_template_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_handler.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_handler.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_horizontal_pod_autoscaler_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_subject_access_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_label_selector_requirement.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_label_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_quobyte_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_quobyte_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_update_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_audit_sink_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/extensions_v1beta1_host_port_range.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/extensions_v1beta1_host_port_range.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_external_documentation.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_external_documentation.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scope_selector.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scope_selector.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_user_info.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_user_info.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_certificate_signing_request_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_cluster_role_binding.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_role_binding_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_ingress_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_ingress_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_scale_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_scale_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_key_to_path.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_key_to_path.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_replica_set_condition.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_replica_set_condition.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_deployment_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_template_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_namespace_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_namespace_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_env_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_env_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_pods_metric_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_ceph_fs_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_ceph_fs_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_replica_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_replica_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_host_path.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_host_path.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_access_review_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_attachment_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_vsphere_virtual_disk_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_vsphere_virtual_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_lease_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_lease_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_volume_error.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_volume_error.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_pods_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_tls.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_tls.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_policy_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_policy_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rbd_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rbd_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_storage_class_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_storage_class_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_node_config_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_node_config_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_binding.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_resource_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_self_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_owner_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_owner_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_subject_rules_review_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_subject_rules_review_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_json_schema_props.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_json_schema_props.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_cluster_role_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_rolling_update_deployment.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_rolling_update_deployment.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_daemon_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_daemon_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_persistent_volume_claim_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_initializers.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_initializers.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_port.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_port.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_scale_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_scale_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_toleration.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_toleration.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/version_info.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/version_info.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_target.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_target.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_token_review.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_token_review.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_pod_affinity.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_pod_affinity.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_strategy.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apps_v1beta1_deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_stateful_set_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_pod_preset.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_preconditions.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_preconditions.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_volume_attachment_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_account.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_account.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_service_port.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_service_port.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_api_resource.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_api_resource.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_metric_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_metric_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_volume_error.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_volume_error.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/apiregistration_v1beta1_service_reference.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/apiregistration_v1beta1_service_reference.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_event_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_event_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_host_alias.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_host_alias.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_conversion.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_conversion.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replication_controller_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replication_controller_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_flex_volume.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/policy_v1beta1_allowed_flex_volume.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role_binding_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_cluster_role_binding.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_cluster_role_binding.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_network_policy_egress_rule.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_network_policy_egress_rule.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_validation.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_validation.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_network_policy_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_network_policy_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_azure_disk_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_azure_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_tcp_socket_action.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_tcp_socket_action.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_projected_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_projected_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1alpha1_initializer_configuration_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_se_linux_options.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_se_linux_options.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta2_metric_value_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta2_metric_value_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_role.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_role.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_pod_disruption_budget_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_token_review_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_token_review_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_spec.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_custom_resource_definition_spec.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_iscsi_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_iscsi_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_daemon_set.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta2_rolling_update_daemon_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_flex_persistent_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_flex_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_secret_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_secret_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_flex_volume_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_flex_volume_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_replica_set_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_replica_set_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_weighted_pod_affinity_term.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_event_list.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_event_list.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1_config_map_env_source.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1_config_map_env_source.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_ingress_backend.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_ingress_backend.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v1beta1_mutating_webhook_configuration.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_status.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/models/v2beta1_horizontal_pod_autoscaler_status.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/configuration.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,9 +227,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1.13.5\n"\
-               "SDK Package Version: 9.0.0".\
+               "SDK Package Version: 9.1.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/extensions_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/extensions_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apis_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apis_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiregistration_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiregistration_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authentication_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authentication_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/networking_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/networking_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authorization_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/policy_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/policy_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/version_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_v1alpha1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_v1alpha1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiregistration_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiregistration_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/custom_objects_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/custom_objects_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/extensions_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/extensions_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/admissionregistration_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/admissionregistration_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/admissionregistration_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/admissionregistration_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/settings_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/scheduling_v1alpha1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/scheduling_v1alpha1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/certificates_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/certificates_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/events_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/events_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authentication_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authentication_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/certificates_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/certificates_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_v2beta2_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_v2beta2_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/core_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/core_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_v2beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_v2beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authorization_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authorization_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiregistration_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiregistration_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/scheduling_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/scheduling_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/scheduling_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/scheduling_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authorization_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authorization_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/authentication_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_v2alpha1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_v2alpha1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/core_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/coordination_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/coordination_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/events_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/__init__.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_v1alpha1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_v1alpha1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiextensions_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiextensions_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/networking_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/networking_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/logs_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/autoscaling_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/autoscaling_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/settings_v1alpha1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/settings_v1alpha1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/auditregistration_v1alpha1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/auditregistration_v1alpha1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/admissionregistration_v1alpha1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/admissionregistration_v1alpha1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apiextensions_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apiextensions_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/coordination_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/coordination_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/policy_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/policy_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/apps_v1beta2_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/apps_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/batch_v1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/batch_v1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/auditregistration_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/auditregistration_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/storage_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/storage_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api/rbac_authorization_v1beta1_api.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api/rbac_authorization_v1beta1_api.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/api_client.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/9.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/9.1.0/python'
 
     def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/rest.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/rest.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/client/__init__.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     OpenAPI spec version: v1.13.5
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "9.0.0"
+__version__ = "9.1.0"
 
 # import apis into sdk package
 from kubernetes_asyncio.client.api.admissionregistration_api import AdmissionregistrationApi
 from kubernetes_asyncio.client.api.admissionregistration_v1alpha1_api import AdmissionregistrationV1alpha1Api
 from kubernetes_asyncio.client.api.admissionregistration_v1beta1_api import AdmissionregistrationV1beta1Api
 from kubernetes_asyncio.client.api.apiextensions_api import ApiextensionsApi
 from kubernetes_asyncio.client.api.apiextensions_v1beta1_api import ApiextensionsV1beta1Api
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/watch/watch_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/watch/watch_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/watch/__init__.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/watch/watch.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/watch/watch.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
     def unmarshal_event(self, data: str, response_type):
         """Return the K8s response `data` in JSON format.
 
         """
         js = json.loads(data)
 
+        if 'object' not in js or 'type' not in js:
+            raise Exception("Malformed JSON response, the 'object' and/or 'type' field is missing. JSON: {}".format(js))
         # Make a copy of the original object and save it under the
         # `raw_object` key because we will replace the data under `object` with
         # a Python native type shortly.
         js['raw_object'] = js['object']
 
         # Something went wrong. A typical example would be that the user
         # supplied a resource version that was too old. In that case K8s would
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/stream/ws_client.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/stream/ws_client.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/stream/__init__.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio/stream/ws_client_test.py` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio/stream/ws_client_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/PKG-INFO` & `kubernetes_asyncio-9.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: kubernetes-asyncio
-Version: 9.0.0
+Name: kubernetes_asyncio
+Version: 9.1.0
 Summary: Kubernetes asynchronous python client
 Home-page: https://github.com/tomplus/kubernetes_asyncio
 Author: Kubernetes
 Author-email: UNKNOWN
 License: Apache License Version 2.0
 Description:     Python client for kubernetes http://kubernetes.io/
```

### Comparing `kubernetes_asyncio-9.0.0/kubernetes_asyncio.egg-info/SOURCES.txt` & `kubernetes_asyncio-9.1.0/kubernetes_asyncio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubernetes_asyncio-9.0.0/README.md` & `kubernetes_asyncio-9.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 
 ```
 pip install kubernetes_asyncio
 ```
 
 Requirements: Python 3.5.3+ ([required by aiohttp](https://aiohttp.readthedocs.io/en/stable/faq.html#why-is-python-3-5-3-the-lowest-supported-version)).
 
+## OpenAPI generator
+
+Starting from v9.0.0 [OpenAPI generator](https://github.com/openapitools/openapi-generator) is used to generate code instead of
+swagger-codegen. This change should be transparent from the client point of view.
+
 ## Example
 
 To list all pods:
 
 ```python
 import asyncio
 from kubernetes_asyncio import client, config
@@ -59,17 +64,17 @@
 
 This library is generated in the same way as the official Kubernetes Python Library. It uses swagger-codegen and the same concepts
 like streaming, watching or reading configuration. Because of an early stage of this library some differences still exist:
 
 |  | [synchronous library kubernetes-client/python](https://github.com/kubernetes-client/python) | [this library](https://github.com/tomplus/kubernetes_asyncio/) |
 |--|--------------------------------------------------------------------|---------------------------------------------------------------|
 | authentication method | gcp-token, azure-token, user-token, oidc-token, user-password, in-cluster | gcp-token (only via gcloud command), user-token, oidc-token, user-password, in-cluster |
-| refesh token | no | yes, optional |
 | python | 2.7 3.4 3.5 3.6 3.7 | 3.5.3 3.6 3.7 |
 | streaming data via websocket from PODs | bidirectional | read-only is already implemented |
+| generator | swagger-codegen | openapi-generator |
 
 ## Versions
 
 This library is versioned in the same way as the synchronous library. The first stable version is 7.0.0 and
 next major versions are comparable. This [compatibility table](https://github.com/kubernetes-client/python#compatibility)
 describes this library too.
```

### Comparing `kubernetes_asyncio-9.0.0/CHANGELOG.md` & `kubernetes_asyncio-9.1.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# v9.1.0
+
+* feat: check whether an object key is present on watch ([#71](https://github.com/tomplus/kubernetes_asyncio/pull/71), [@mickours](https://github.com/mickours))
+
+* feat: feat: merging kubeconfig files ([#69](https://github.com/tomplus/kubernetes_asyncio/pull/69), [@tomplus](https://github.com/tomplus))
+
+# v9.0.0
+
+* feat: switch to openapi-generator ([#58](https://github.com/tomplus/kubernetes_asyncio/pull/58), [@tomplus](https://github.com/tomplus))
+* feat: add fieldSelector parameter to list/watch methods in custom objects spec ([gen/#106](https://github.com/kubernetes-client/gen/pull/106))
+* feat: upgrade to API spec from Kubernetes 1.13 ([#58](https://github.com/tomplus/kubernetes_asyncio/pull/58), [@tomplus](https://github.com/tomplus))
+
+Breaking Changes:
+* Model v1beta1WebhookClientConfig is renamed to AdmissionregistrationV1beta1WebhookClientConfig, to avoid naming conflict
+   with ApiextensionsV1beta1WebhookClientConfig introduced in: kubernetes/kubernetes#67006
+* Delete request's body parameter is optional kubernetes/kubernetes#70032
+
 # v8.1.0
 
 * feat: watch improvement (context manager, close method) ([#61](https://github.com/tomplus/kubernetes_asyncio/pull/61), [@hubo1016](https://github.com/hubo1016))
 
 # v8.0.3
 
 * fix: use `yaml.safe_load`, `yaml.safe_dump` for security reasons ([#57](https://github.com/tomplus/kubernetes_asyncio/pull/57), [@tomplus](https://github.com/tomplus))
```

