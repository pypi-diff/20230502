# Comparing `tmp/tailer_sdk-1.3.8-py3-none-any.whl.zip` & `tmp/tailer_sdk-1.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 62114 bytes, number of entries: 16
+Zip file size: 62219 bytes, number of entries: 16
 -rwx------  2.0 unx        0 b- defN 22-Jan-03 16:49 tailer_sdk/__init__.py
--rw-r--r--  2.0 unx   153077 b- defN 22-Oct-05 11:26 tailer_sdk/sql_dag_generator.py
+-rw-r--r--  2.0 unx   152004 b- defN 22-Oct-25 06:02 tailer_sdk/sql_dag_generator.py
 -rwx------  2.0 unx     7170 b- defN 22-Jan-03 16:49 tailer_sdk/tailer_auth.py
 -rwx------  2.0 unx    16580 b- defN 22-Jan-03 16:49 tailer_sdk/tailer_config.py
--rw-r--r--  2.0 unx    35034 b- defN 22-Sep-28 09:03 tailer_sdk/tailer_configuration_manager.py
+-rw-r--r--  2.0 unx    36352 b- defN 22-Nov-09 10:02 tailer_sdk/tailer_configuration_manager.py
 -rwx------  2.0 unx     2421 b- defN 22-Jan-03 16:49 tailer_sdk/tailer_crypto.py
 -rwx------  2.0 unx     4194 b- defN 22-Jan-03 16:49 tailer_sdk/tailer_gcp_cf_manager.py
 -rwx------  2.0 unx     1192 b- defN 22-Jan-03 16:49 tailer_sdk/tailer_help.py
 -rw-r--r--  2.0 unx     9800 b- defN 22-Oct-05 07:09 tailer_sdk/tailer_misc.py
--rw-r--r--  2.0 unx     4830 b- defN 22-Oct-05 07:20 tailer_sdk/tailersdk.py
--rwx------  2.0 unx    35149 b- defN 22-Oct-05 11:26 tailer_sdk-1.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3980 b- defN 22-Oct-05 11:26 tailer_sdk-1.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-05 11:26 tailer_sdk-1.3.8.dist-info/WHEEL
--rwx------  2.0 unx       54 b- defN 22-Oct-05 11:26 tailer_sdk-1.3.8.dist-info/entry_points.txt
--rwx------  2.0 unx       11 b- defN 22-Oct-05 11:26 tailer_sdk-1.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1353 b- defN 22-Oct-05 11:26 tailer_sdk-1.3.8.dist-info/RECORD
-16 files, 274937 bytes uncompressed, 59878 bytes compressed:  78.2%
+-rw-r--r--  2.0 unx     5249 b- defN 22-Nov-09 09:59 tailer_sdk/tailersdk.py
+-rwx------  2.0 unx    35149 b- defN 22-Nov-24 09:07 tailer_sdk-1.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4073 b- defN 22-Nov-24 09:07 tailer_sdk-1.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Nov-24 09:07 tailer_sdk-1.3.9.dist-info/WHEEL
+-rwx------  2.0 unx       53 b- defN 22-Nov-24 09:07 tailer_sdk-1.3.9.dist-info/entry_points.txt
+-rwx------  2.0 unx       11 b- defN 22-Nov-24 09:07 tailer_sdk-1.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1353 b- defN 22-Nov-24 09:07 tailer_sdk-1.3.9.dist-info/RECORD
+16 files, 275693 bytes uncompressed, 59983 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: tailer_sdk/tailer_misc.py
 Comment: 
 
 Filename: tailer_sdk/tailersdk.py
 Comment: 
 
-Filename: tailer_sdk-1.3.8.dist-info/LICENSE
+Filename: tailer_sdk-1.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: tailer_sdk-1.3.8.dist-info/METADATA
+Filename: tailer_sdk-1.3.9.dist-info/METADATA
 Comment: 
 
-Filename: tailer_sdk-1.3.8.dist-info/WHEEL
+Filename: tailer_sdk-1.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: tailer_sdk-1.3.8.dist-info/entry_points.txt
+Filename: tailer_sdk-1.3.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: tailer_sdk-1.3.8.dist-info/top_level.txt
+Filename: tailer_sdk-1.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tailer_sdk-1.3.8.dist-info/RECORD
+Filename: tailer_sdk-1.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tailer_sdk/sql_dag_generator.py

```diff
@@ -359,15 +359,14 @@
     return output_payload
 
 
 def build_header_for_direct_execution():
 
     output_payload = """
 import argparse
-import etcd3
 import copy
 import socket
 import redis
 from pottery import Redlock
 import sqlparse
 import concurrent.futures
 
@@ -529,36 +528,29 @@
 
         try:
             # Create the Secret Manager client.
             secret_manager_client = secretmanager.SecretManagerServiceClient()
 
             # Build the resource name of the secret version.
             #
-            if lock_manager == "etcd":
-                secret_id = "tailer-etcd-infos"
-            elif lock_manager == "redis":
+            if lock_manager == "redis":
                 secret_id = "tailer-redis-infos"
             else:
                 raise Exception("Lock manager {} is not valid.".format(lock_manager))
 
             secret_name = "projects/{}/secrets/{}/versions/latest".format(os.environ["PROJECT_ID"], secret_id)
 
             # Access the secret version.
             #
             secret_response = secret_manager_client.access_secret_version(request={"name": secret_name})
             secret_payload = json.loads(secret_response.payload.data.decode('UTF-8'))
 
             # Get Lock Manager information
             #
-            if lock_manager == "etcd":
-                lock_manager_host_address = secret_payload["etcd_host"]
-                lock_manager_host_port = int(secret_payload["etcd_port"])
-                lock_manager_user = secret_payload["etcd_user"]
-                lock_manager_secret = secret_payload["etcd_secret"]
-            elif lock_manager == "redis":
+            if lock_manager == "redis":
                 lock_manager_host_address = secret_payload["redis_host"]
                 lock_manager_host_port = int(secret_payload["redis_port"])
                 lock_manager_user = ""
                 lock_manager_secret = secret_payload["redis_secret"]
 
             logging.info("Connecting to {} : {}:{}".format(lock_manager, lock_manager_host_address, str(lock_manager_host_port)))
 
@@ -591,25 +583,15 @@
                     if (dag_run_doc is not None) and ("killswitch" in dag_run_doc.keys()) and (dag_run_doc["killswitch"] is True):
                         raise Exception("Killed.")
                     else:
                         time.sleep(2)
 
                 # Instantiation lock manager client
                 #
-                if lock_manager == "etcd":
-
-                    lock_manager_instance = etcd3.client(
-                                                host=lock_manager_host_address,
-                                                port=lock_manager_host_port,
-                                                user=lock_manager_user,
-                                                password=lock_manager_secret)
-
-                    lock_instance = lock_manager_instance.lock(_dag_name, ttl=15)
-
-                elif lock_manager == "redis":
+                if lock_manager == "redis":
 
                     lock_manager_instance = \
                         redis.Redis(
                             host=lock_manager_host_address,
                             port=lock_manager_host_port,
                             db=0,
                             password=lock_manager_secret,
@@ -828,21 +810,18 @@
         dag_activated = dag_configuration["activated"]
     except KeyError:
         print("No activated attribute found in DAGs config. Setting to default : True")
         dag_activated = True
 
     if dag_activated is True:
 
-        # retrieving the lock manager if specified
+        # Forcing lock manager to REDIS
         #
-        try:
-            lock_manager = dag_configuration["configuration"]["lock_manager"]
-        except KeyError:
-            print("No lock manager specified in configuration, setting default : redis")
-            lock_manager = "redis"
+        print("Forcing lock manager, setting default : redis")
+        lock_manager = "redis"
 
         # Allright, we are going to execute this DAG.
         # First of all, we need to check that we are above the DAG concurrency threshold.
         #
         try:
 
             check_dag_concurrency(
```

## tailer_sdk/tailer_configuration_manager.py

```diff
@@ -767,14 +767,20 @@
                                 tailer_configuration=tailer_configuration,
                                 firebase_user=firebase_user,
                                 context_id=context_choice.strip())
 
     if ret_code is False:
         return False, None, None
 
+    # Process TTS SQL payload
+    #
+    if read_configuration["configuration_type"] == "table-to-storage":
+        read_configuration["sql"] = \
+            (base64.b64decode(read_configuration["sql"])).decode("utf-8")
+
     # Transform configuration to string
     #
     configuration_string = json.dumps(read_configuration, indent=4)
 
     # Parse configuration string against context
     #
     ret_code, configuration_string = \
@@ -783,14 +789,22 @@
             context_data=context_data)
 
     if ret_code is False:
         return False, None, None
 
     contextualized_configuration = json.loads(configuration_string)
 
+    # Encode TTS SQL query
+    #
+    if read_configuration["configuration_type"] == "table-to-storage":
+        contextualized_configuration["sql"] = \
+            str(
+                base64.b64encode(contextualized_configuration["sql"].encode("utf-8")),
+                "utf-8")
+
     # Process configuration ID and configuration name
     #
     contextualized_configuration["configuration_name"] = contextualized_configuration["configuration_id"]
     contextualized_configuration["configuration_id"] = contextualized_configuration["account"].strip() \
         + "_" + context_data["configuration_id"].strip() \
         + "_" + contextualized_configuration["configuration_id"].strip()
 
@@ -839,220 +853,226 @@
         return configuration_processor_xml_conversion(read_configuration)
 
     return read_configuration
 
 
 def process(args, tailer_sdk_version):
 
-    print("Tailer Configuration Manager.")
+    try:
 
-    # Get configuration
-    #
-    tailer_configuration = tailer_config.get_tailer_configuration_file()
+        print("Tailer Configuration Manager.")
 
-    # Get firebase user
-    #
-    firebase_user = tailer_auth.get_refreshed_firebase_user(
-        tailer_configuration)
+        # Get configuration
+        #
+        tailer_configuration = tailer_config.get_tailer_configuration_file()
+
+        # Get firebase user
+        #
+        firebase_user = tailer_auth.get_refreshed_firebase_user(
+            tailer_configuration)
+
+        if args.command == "deploy":
+            if len(args.arguments) >= 2:
+                if args.arguments[1] is not None:
+                    if args.arguments[1] == "help":
+                        return display_configuration_help(args.command, tailer_configuration, firebase_user)
+                    else:
 
-    if args.command == "deploy":
-        if len(args.arguments) >= 2:
-            if args.arguments[1] is not None:
-                if args.arguments[1] == "help":
-                    return display_configuration_help(args.command, tailer_configuration, firebase_user)
-                else:
+                        # # Special check for TABLE-TO-TABLE (DAG Generator) configuration
+                        # # If so, we need to process the configuration file
+                        # #
+                        # if check_table_to_table(args.arguments[1]) is True:
+                        #     print("Processing table-to-table type configuration ...")
+                        #     sql_dag_generator.process(
+                        #         configuration_file=args.arguments[1], tailer_sdk_version=tailer_sdk_version)
+                        #     return True
+
+                        # Get optional flags
+                        #
+                        cmd_line_context = None
+                        cmd_line_no_launch = False
+
+                        for remainder_index in range(2,len(args.arguments)):
+
+                            if args.arguments[remainder_index].strip() == "--context":
+                                try:
+                                    cmd_line_context = args.arguments[remainder_index + 1].strip()
+                                    print("Context provided : {}".format(cmd_line_context))
+                                except Exception:
+                                    print("\nError : Please specify a context.\n")
+                                    return False
+
+                            elif args.arguments[remainder_index].strip() == "--no-launch":
+                                cmd_line_no_launch = True
+
+                        # Retrieve configuration version
+                        #
+                        configuration_version = get_configuration_version(input_configuration=args.arguments[1])
+                        print("Configuration version : {}".format(configuration_version))
+
+                        # Process context for configuration version >= 2
+                        #
+                        read_configuration = None
+                        context_data = None
+
+                        # Everyone get contexts
+                        # if configuration_version == "2":``
+                        #
+                        ret_code, read_configuration, context_data = \
+                            process_configuration_context(
+                                input_configuration=args.arguments[1],
+                                tailer_configuration=tailer_configuration,
+                                firebase_user=firebase_user,
+                                context_choice=cmd_line_context)
 
-                    # # Special check for TABLE-TO-TABLE (DAG Generator) configuration
-                    # # If so, we need to process the configuration file
-                    # #
-                    # if check_table_to_table(args.arguments[1]) is True:
-                    #     print("Processing table-to-table type configuration ...")
-                    #     sql_dag_generator.process(
-                    #         configuration_file=args.arguments[1], tailer_sdk_version=tailer_sdk_version)
-                    #     return True
-
-                    # Get optional flags
-                    #
-                    cmd_line_context = None
-                    cmd_line_no_launch = False
-
-                    for remainder_index in range(2,len(args.arguments)):
-
-                        if args.arguments[remainder_index].strip() == "--context":
-                            try:
-                                cmd_line_context = args.arguments[remainder_index + 1].strip()
-                                print("Context provided : {}".format(cmd_line_context))
-                            except Exception:
-                                print("\nError : Please specify a context.\n")
-                                return False
+                        if ret_code is False:
+                            print("Error while processing configuration context.")
+                            return False
 
-                        elif args.arguments[remainder_index].strip() == "--no-launch":
-                            cmd_line_no_launch = True
+                        # DEBUG
+                        #
+                        # print(f"Configuration id : {read_configuration['configuration_id']}")
+
+                        # Special check for TABLE-TO-TABLE (DAG Generator) configuration
+                        # If so, we need to process the configuration file
+                        #
+                        if check_table_to_table(
+                                input_configuration=args.arguments[1],
+                                read_configuration=read_configuration) is True:
+
+                            print("Processing table-to-table type configuration ...")
+                            sql_dag_generator.process(
+                                configuration_file=args.arguments[1],
+                                read_configuration=read_configuration,
+                                tailer_sdk_version=tailer_sdk_version,
+                                cmd_line_no_launch=cmd_line_no_launch,
+                                context_data=context_data)
+                            return True
+
+                        # Check if the configuration is valid
+                        #
+                        if check_configuration(
+                                input_conf_file=args.arguments[1],
+                                tailer_configuration=tailer_configuration,
+                                read_configuration=read_configuration,
+                                firebase_user=firebase_user) is False:
 
-                    # Retrieve configuration version
-                    #
-                    configuration_version = get_configuration_version(input_configuration=args.arguments[1])
-                    print("Configuration version : {}".format(configuration_version))
-
-                    # Process context for configuration version >= 2
-                    #
-                    read_configuration = None
-                    context_data = None
-
-                    # Everyone get contexts
-                    # if configuration_version == "2":``
-                    #
-                    ret_code, read_configuration, context_data = \
-                        process_configuration_context(
-                            input_configuration=args.arguments[1],
-                            tailer_configuration=tailer_configuration,
-                            firebase_user=firebase_user,
-                            context_choice=cmd_line_context)
-
-                    if ret_code is False:
-                        print("Error while processing configuration context.")
-                        return False
-
-                    # DEBUG
-                    #
-                    # print(f"Configuration id : {read_configuration['configuration_id']}")
-
-                    # Special check for TABLE-TO-TABLE (DAG Generator) configuration
-                    # If so, we need to process the configuration file
-                    #
-                    if check_table_to_table(
-                            input_configuration=args.arguments[1],
-                            read_configuration=read_configuration) is True:
-
-                        print("Processing table-to-table type configuration ...")
-                        sql_dag_generator.process(
-                            configuration_file=args.arguments[1],
-                            read_configuration=read_configuration,
-                            tailer_sdk_version=tailer_sdk_version,
-                            cmd_line_no_launch=cmd_line_no_launch,
-                            context_data=context_data)
-                        return True
-
-                    # Check if the configuration is valid
-                    #
-                    if check_configuration(
-                            input_conf_file=args.arguments[1],
-                            tailer_configuration=tailer_configuration,
-                            read_configuration=read_configuration,
-                            firebase_user=firebase_user) is False:
-
-                        return False
-
-                    # Process Cloud Function deployment
-                    #
-                    # Only for : STS, STT, xml-conversion,
-                    #
-                    gcp_cf_deploy = process_cf_deployment(
-                                        input_configuration=args.arguments[1],
-                                        tailer_configuration=tailer_configuration,
-                                        no_gcp_cf_deploy=args.no_gcp_cf_deploy)
-
-                    # Check if GCP Project ID is present
-                    #
-                    project_profile = None
-                    if (configuration_version == "1") or (read_configuration is None):
+                            return False
 
-                        project_profile = process_project_profile(
-                                            input_conf_file=args.arguments[1],
+                        # Process Cloud Function deployment
+                        #
+                        # Only for : STS, STT, xml-conversion,
+                        #
+                        gcp_cf_deploy = process_cf_deployment(
+                                            input_configuration=args.arguments[1],
                                             tailer_configuration=tailer_configuration,
-                                            firebase_user=firebase_user)
+                                            no_gcp_cf_deploy=args.no_gcp_cf_deploy)
 
-                        if project_profile is None:
-                            return False
+                        # Check if GCP Project ID is present
+                        #
+                        project_profile = None
+                        if (configuration_version == "1") or (read_configuration is None):
+
+                            project_profile = process_project_profile(
+                                                input_conf_file=args.arguments[1],
+                                                tailer_configuration=tailer_configuration,
+                                                firebase_user=firebase_user)
 
-                    else:
+                            if project_profile is None:
+                                return False
 
-                        project_profile = get_project_profile_from_configuration(
-                                            input_conf_file=args.arguments[1],
-                                            tailer_configuration=tailer_configuration,
-                                            read_configuration=read_configuration,
-                                            firebase_user=firebase_user)
+                        else:
+
+                            project_profile = get_project_profile_from_configuration(
+                                                input_conf_file=args.arguments[1],
+                                                tailer_configuration=tailer_configuration,
+                                                read_configuration=read_configuration,
+                                                firebase_user=firebase_user)
 
-                        if project_profile is None:
+                            if project_profile is None:
+                                return False
+
+                        # Global special processing
+                        #
+                        read_configuration = configuration_special_processing(args.arguments[1],read_configuration)
+                        if read_configuration is None:
                             return False
 
-                    # Global special processing
-                    #
-                    read_configuration = configuration_special_processing(args.arguments[1],read_configuration)
-                    if read_configuration is None:
-                        return False
-
-                    print("Attempting to deploy regular configuration...")
-
-                    return deploy_configuration(
-                                args.arguments[1],
-                                tailer_configuration,
-                                firebase_user,
-                                gcp_cf_deploy,
-                                project_profile=project_profile,
-                                read_configuration=read_configuration,
-                                tailer_sdk_version=tailer_sdk_version,
-                                no_dag_execution=cmd_line_no_launch)
+                        print("Attempting to deploy regular configuration...")
+
+                        return deploy_configuration(
+                                    args.arguments[1],
+                                    tailer_configuration,
+                                    firebase_user,
+                                    gcp_cf_deploy,
+                                    project_profile=project_profile,
+                                    read_configuration=read_configuration,
+                                    tailer_sdk_version=tailer_sdk_version,
+                                    no_dag_execution=cmd_line_no_launch)
 
-            else:
-                print("Argument unknown." % args.arguments[1])
-                return False
-        else:
-            return display_configuration_help(
-                        args.command,
-                        tailer_configuration,
-                        firebase_user)
-
-    elif args.command == "create":
-        if len(args.arguments) >= 2:
-            if args.arguments[1] is not None:
-                if args.arguments[1] == "help":
-                    return display_configuration_help(
-                                args.command,
-                                tailer_configuration,
-                                firebase_user)
                 else:
+                    print("Argument unknown." % args.arguments[1])
+                    return False
+            else:
+                return display_configuration_help(
+                            args.command,
+                            tailer_configuration,
+                            firebase_user)
+
+        elif args.command == "create":
+            if len(args.arguments) >= 2:
+                if args.arguments[1] is not None:
+                    if args.arguments[1] == "help":
+                        return display_configuration_help(
+                                    args.command,
+                                    tailer_configuration,
+                                    firebase_user)
+                    else:
 
-                    # retrieve output_filename
-                    #
-                    try:
-                        output_filename = args.arguments[2]
-                    except Exception:
-                        output_filename = args.arguments[1] + ".json"
-
-                    return create_configuration(
-                                args.arguments[1],
-                                output_filename,
-                                tailer_configuration,
-                                firebase_user)
+                        # retrieve output_filename
+                        #
+                        try:
+                            output_filename = args.arguments[2]
+                        except Exception:
+                            output_filename = args.arguments[1] + ".json"
+
+                        return create_configuration(
+                                    args.arguments[1],
+                                    output_filename,
+                                    tailer_configuration,
+                                    firebase_user)
+                else:
+                    print("Argument unknown." % args.arguments[1])
+                    return False
             else:
-                print("Argument unknown." % args.arguments[1])
-                return False
-        else:
-            return display_configuration_help(
-                        args.command,
-                        tailer_configuration,
-                        firebase_user)
-
-    elif args.command == "check":
-        if len(args.arguments) >= 2:
-            if args.arguments[1] is not None:
-                if args.arguments[1] == "help":
-                    return display_configuration_help(
-                                args.command,
-                                tailer_configuration,
-                                firebase_user)
+                return display_configuration_help(
+                            args.command,
+                            tailer_configuration,
+                            firebase_user)
+
+        elif args.command == "check":
+            if len(args.arguments) >= 2:
+                if args.arguments[1] is not None:
+                    if args.arguments[1] == "help":
+                        return display_configuration_help(
+                                    args.command,
+                                    tailer_configuration,
+                                    firebase_user)
+                    else:
+                        return check_configuration(
+                                    input_conf_file=args.arguments[1],
+                                    tailer_configuration=tailer_configuration,
+                                    firebase_user=firebase_user)
                 else:
-                    return check_configuration(
-                                input_conf_file=args.arguments[1],
-                                tailer_configuration=tailer_configuration,
-                                firebase_user=firebase_user)
+                    print("Argument unknown." % args.arguments[1])
+                    return False
             else:
-                print("Argument unknown." % args.arguments[1])
-                return False
-        else:
-            return display_configuration_help(
-                        args.command,
-                        tailer_configuration,
-                        firebase_user)
-
-    return True
+                return display_configuration_help(
+                            args.command,
+                            tailer_configuration,
+                            firebase_user)
+
+        return True
+
+    except Exception as ex:
+        print(f"Error : {str(ex)}")
+        return False
```

## tailer_sdk/tailersdk.py

```diff
@@ -23,15 +23,15 @@
 import google.auth
 
 warnings.filterwarnings(
     "ignore", "Your application has authenticated using end user credentials")
 
 # Globals
 #
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 TAILER_SDK_NAME = "tailer-sdk"
 
 
 def display_tailer_header():
 
     print("")
     print("Tailer SDK")
@@ -130,25 +130,29 @@
                 #
                 tailer_configuration = tailer_config.get_tailer_configuration_file()
                 tailer_auth.reset_password(tailer_configuration=tailer_configuration)
 
     elif args.command == "create":
         if len(args.arguments) > 0:
             if (args.arguments)[0] == "configuration":
-                tailer_configuration_manager.process(args, tailer_sdk_version=__version__)
+                if tailer_configuration_manager.process(args, tailer_sdk_version=__version__) is False:
+                    raise Exception("error while processing Tailer SDK create command.")
 
     elif args.command == "check":
         if len(args.arguments) > 0:
             if (args.arguments)[0] == "configuration":
-                tailer_configuration_manager.process(args, tailer_sdk_version=__version__)
+                if tailer_configuration_manager.process(args, tailer_sdk_version=__version__) is False:
+                    raise Exception("error while processing Tailer SDK check command.")
 
     elif args.command == "deploy":
         if len(args.arguments) > 0:
             if (args.arguments)[0] == "configuration":
-                tailer_configuration_manager.process(args, tailer_sdk_version=__version__)
+                if tailer_configuration_manager.process(args, tailer_sdk_version=__version__) is False:
+                    raise Exception("error while processing Tailer SDK deploy command.")
+
             if (args.arguments)[0] == "gcp-cloud-function":
                 tailer_gcp_cf_manager.process(args)
     
     elif args.command == "help":
         tailer_help.display_help()
     else:
         tailer_help.display_help()
@@ -156,8 +160,13 @@
     # Check if there is a newer version
     #
     notify_update_tailer_sdk()
 
 
 if __name__ == "__main__":
 
-    main()
+    try:
+        main()
+        exit(0)
+    except Exception as ex:
+        print(f"\nError : {str(ex)}\n")
+        exit(1)
```

## Comparing `tailer_sdk-1.3.8.dist-info/LICENSE` & `tailer_sdk-1.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tailer_sdk-1.3.8.dist-info/METADATA` & `tailer_sdk-1.3.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tailer-sdk
-Version: 1.3.8
+Version: 1.3.9
 Summary: Tailer SDK Python Package
 Home-page: https://www.fashiondata.io/
 Author: Fashiondata Team
 Author-email: contact@fashiondata.io
 License: GPLv3
 Keywords: pip,fashiondata
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.22.0)
 Requires-Dist: firebase (>=3.0.1)
 Requires-Dist: pycryptodome (>=1.6.0)
@@ -28,14 +27,19 @@
 Requires-Dist: pkg-info (>=0.1.2)
 Requires-Dist: chardet (>=3.0.4)
 
 # Tailer SDK
 
 ## Changelog
 
+### Release 1.3.9 : 2022-11-24
+
+* TTS : support for context in SQL query.
+* Global : enhanced SDK return codes
+
 ### Release 1.3.8 : 2022-10-05
 
 * TTT : bugfix, error when applying context on a SQL file containing the variable name "TEMPLATE_CURRENT_DATE".
 
 ### Release 1.3.7 : 2022-07-28
 
 * TTT : added new criticality level -> stop.
@@ -115,8 +119,7 @@
  
 * Added support for configuration type : xml-conversion
 
 ### Release 1.2.0 : 2021-02-22
 
 * First release : moved code from Jarvis SDK
  
-
```

## Comparing `tailer_sdk-1.3.8.dist-info/RECORD` & `tailer_sdk-1.3.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 tailer_sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tailer_sdk/sql_dag_generator.py,sha256=DLerADYSSK4BjQOECCPs7jIkohEkk6hAxqGhVBN78yQ,153077
+tailer_sdk/sql_dag_generator.py,sha256=FsJS4mBva7UHtRpJkoSRL3UktBUqQ8YuM8mco2Jnydg,152004
 tailer_sdk/tailer_auth.py,sha256=sK_e1PGRJeHgfKkA9ZnZpnBc52YRvgHh-XT247SSwlg,7170
 tailer_sdk/tailer_config.py,sha256=06bKrxQ5jrAq0OBwlhG0C4n3a1y4276NxCezNoHVRPQ,16580
-tailer_sdk/tailer_configuration_manager.py,sha256=ciSbqIBsr41A6YRYlPauztKVHBXJspTEyQNAok5WAfE,35034
+tailer_sdk/tailer_configuration_manager.py,sha256=ItYGeQ36vTIg3G-GAZVUD_esjIK9zAxrSrAUEEE8Iq4,36352
 tailer_sdk/tailer_crypto.py,sha256=KoInwerwltvlnEhSn1UQu69m5JhxxHB2muX3Hi1GLFQ,2421
 tailer_sdk/tailer_gcp_cf_manager.py,sha256=ZE9Ve0Co_b-jP29UUqVPPmo2Q0uKY3AHebWlECLkxG4,4194
 tailer_sdk/tailer_help.py,sha256=B_TRaYYVwu7-4x2_eqrQ-2GaRdolKK1tX89XoRWPfpA,1192
 tailer_sdk/tailer_misc.py,sha256=IQ-q4XPBjQdt317tiWILauVrZDIzHBTyG2nktCSUsMI,9800
-tailer_sdk/tailersdk.py,sha256=JbyV9mmKlYhrOmCaBukNkdcltD2nNh1DzIOI88z7wZg,4830
-tailer_sdk-1.3.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-tailer_sdk-1.3.8.dist-info/METADATA,sha256=_EmodBmdCEBEcuxYznlZIqJPGwUMmpL7gdjScBKzrKg,3980
-tailer_sdk-1.3.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tailer_sdk-1.3.8.dist-info/entry_points.txt,sha256=OfYDJpEmY0gCF7SAivOwWjMsNBEyqtqWrdm5oPhvMZc,54
-tailer_sdk-1.3.8.dist-info/top_level.txt,sha256=jkfXqEW45U_J0psaU2NHS6_VZe5jFlAafJjXnpWlDGM,11
-tailer_sdk-1.3.8.dist-info/RECORD,,
+tailer_sdk/tailersdk.py,sha256=WKdu7wYDEED-BYh2D0-pZbp3lCKjRVIHDgqhHJoWKlg,5249
+tailer_sdk-1.3.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+tailer_sdk-1.3.9.dist-info/METADATA,sha256=8MCe4RIPz5KEKliE4tH45aWMHsCp_KQLKhCL4NHmlsQ,4073
+tailer_sdk-1.3.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tailer_sdk-1.3.9.dist-info/entry_points.txt,sha256=lk71xIQCG5SmGgwpuRCmsNhbWW5r5klk6oM-Z4PdV60,53
+tailer_sdk-1.3.9.dist-info/top_level.txt,sha256=jkfXqEW45U_J0psaU2NHS6_VZe5jFlAafJjXnpWlDGM,11
+tailer_sdk-1.3.9.dist-info/RECORD,,
```

