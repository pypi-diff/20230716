# Comparing `tmp/balcony-0.1.5.tar.gz` & `tmp/balcony-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.5.tar", max compression
+gzip compressed data, was "balcony-0.1.6.tar", max compression
```

## Comparing `balcony-0.1.5.tar` & `balcony-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.5/LICENSE
--rw-r--r--   0        0        0     1890 2023-06-22 10:24:32.348247 balcony-0.1.5/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.5/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.5/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.5/balcony/aws.py
--rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.5/balcony/botocore_utils.py
--rw-r--r--   0        0        0    21689 2023-06-27 20:58:05.108582 balcony-0.1.5/balcony/cli.py
--rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.5/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.5/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.5/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.5/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.5/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.5/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.5/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.5/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.5/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.5/balcony/custom_tf_import_configs/_example_import_conf.yaml
--rw-r--r--   0        0        0     2026 2023-06-27 20:56:32.969434 balcony-0.1.5/balcony/custom_tf_import_configs/ec2.yaml
--rw-r--r--   0        0        0      312 2023-06-27 00:04:18.331870 balcony-0.1.5/balcony/custom_tf_import_configs/ecs.yaml
--rw-r--r--   0        0        0     1079 2023-06-27 12:36:49.277772 balcony-0.1.5/balcony/custom_tf_import_configs/iam.yaml
--rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.5/balcony/custom_tf_import_configs/rds.yaml
--rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.5/balcony/custom_tf_import_configs/s3.yaml
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.5/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.5/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.5/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.5/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.5/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.5/balcony/errors.py
--rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.5/balcony/nodes.py
--rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.5/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.5/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.5/balcony/relations.py
--rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.5/balcony/terraform_import/__init__.py
--rw-r--r--   0        0        0     6929 2023-06-27 11:42:12.855449 balcony-0.1.5/balcony/terraform_import/importer.py
--rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.5/balcony/terraform_import/models.py
--rw-r--r--   0        0        0     2654 2023-06-27 11:55:46.303705 balcony-0.1.5/balcony/terraform_import/parsers.py
--rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.5/balcony/terraform_import/wizard.py
--rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.5/balcony/test.py
--rw-r--r--   0        0        0     6108 2023-06-27 10:22:17.365596 balcony-0.1.5/balcony/utils.py
--rw-r--r--   0        0        0     2171 2023-06-27 11:55:23.845723 balcony-0.1.5/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.5/balcony/yaml_validators.py
--rw-r--r--   0        0        0      748 2023-06-27 20:59:39.659932 balcony-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4993 1970-01-01 00:00:00.000000 balcony-0.1.5/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 balcony-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3621 2023-06-27 21:55:30.541972 balcony-0.1.6/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.6/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.6/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.6/balcony/aws.py
+-rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.6/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    22612 2023-07-16 15:42:35.736562 balcony-0.1.6/balcony/cli.py
+-rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.6/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.6/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.6/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.6/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.6/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.6/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.6/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.6/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.6/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.6/balcony/custom_tf_import_configs/_example_import_conf.yaml
+-rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.6/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      312 2023-06-27 00:04:18.331870 balcony-0.1.6/balcony/custom_tf_import_configs/ecs.yaml
+-rw-r--r--   0        0        0     1897 2023-07-16 10:50:18.867726 balcony-0.1.6/balcony/custom_tf_import_configs/iam.yaml
+-rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.6/balcony/custom_tf_import_configs/rds.yaml
+-rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.6/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     3388 2023-07-16 17:09:09.656301 balcony-0.1.6/balcony/custom_tf_import_configs/vpc.yaml
+-rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.6/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.6/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.6/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.6/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.6/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.6/balcony/errors.py
+-rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.6/balcony/nodes.py
+-rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.6/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.6/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.6/balcony/relations.py
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.6/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0     9506 2023-07-16 17:10:19.590346 balcony-0.1.6/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.6/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     3666 2023-07-16 16:00:20.534235 balcony-0.1.6/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.6/balcony/terraform_import/wizard.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.6/balcony/test.py
+-rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.6/balcony/utils.py
+-rw-r--r--   0        0        0     2171 2023-06-27 11:55:23.845723 balcony-0.1.6/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.6/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      748 2023-07-16 17:17:23.467052 balcony-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4911 1970-01-01 00:00:00.000000 balcony-0.1.6/setup.py
+-rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 balcony-0.1.6/PKG-INFO
```

### Comparing `balcony-0.1.5/LICENSE` & `balcony-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/__init__.py` & `balcony-0.1.6/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/aws.py` & `balcony-0.1.6/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/botocore_utils.py` & `balcony-0.1.6/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/cli.py` & `balcony-0.1.6/balcony/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import textwrap
 from utils import (
     get_all_available_services,
     ifind_similar_names_in_list,
     _create_boto_session,
+    is_terraform_aws_resource_type
 )
 from config import (
     get_logger,
     get_rich_console,
     set_log_level_at_runtime,
     clear_relations_cache,
     BALCONY_RELATIONS_DIR
@@ -28,22 +29,24 @@
     generate_import_block_for_resource,
     get_importable_resources,
 )
 from terraform_import.wizard import (
     interactive_help,
 )
 from rich.padding import Padding
+import re
 
 console = get_rich_console()
 logger = get_logger(__name__)
 session = _create_boto_session()
 balcony_aws = BalconyAWS(session)
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_enable=False)
 
 
+
 @app.callback()
 def _main_app_callback(
     debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug messages."),
 ):
     if debug:
         set_log_level_at_runtime(logging.DEBUG)
 
@@ -376,24 +379,24 @@
     no_args_is_help=True,
     short_help="Generate Terraform import blocks for a given AWS Service and Resource Node.",
     help="""
     Visit Balcony Terraform Import Documentation: https://oguzhan-yilmaz.github.io/balcony/terraform-import/ to learn more.\n
     """,
 )
 def terraform_import_command(
-    service: Optional[str] = typer.Argument(
+    service_or_tf_resource_type: Optional[str] = typer.Argument(
         None,
         show_default=False,
-        help="Name of the AWS Service (e.g. ec2, s3, rds)",
+        help="Name of the AWS Service (ec2, iam) or Terraform Type (aws_iam_user)",
         autocompletion=_complete_service_name,
     ),
     resource_node: Optional[str] = typer.Argument(
         None,
         show_default=False,
-        help="Name of the AWS Resource Node. (e.g. Instances, Buckets, DBInstances)",
+        help="Name of the AWS Resource Node (Instances, Buckets, DBInstances)",
         autocompletion=_complete_resource_node_name,
     ),
     debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug messages."),
     follow_pagination: bool = typer.Option(
         False,
         "--paginate",
         "-p",
@@ -426,63 +429,74 @@
             "[underline][yellow bold][WARNING][/] [bold][--paginate, -p][/] option [bold red]is NOT set[/]. You're likely to get incomplete data.[/]"
         )
 
     if list_available_resources:
         service_resource_list = get_importable_resources()
 
         def render_importable_resources(service_and_resource_tuples: List[Tuple]):
-            header = f"[bold green]{'service':<15} {'resource_name':<45}[/]\n".format()
+            header = f"[bold green]{'TerraformResourceType':<30} {'Service':>15} {'Resource':45}[/]\n".format()
             result = header
 
-            for i, (service_name, resource_name) in enumerate(
+            for i, (terraform_type, service_name, resource_name) in enumerate(
                 service_and_resource_tuples
             ):
-
-                cur_line = f"{service_name:<15} {resource_name:<45}"
+                cur_line = f"{terraform_type:<30} {service_name:>15} {resource_name:45}"
                 if i % 2:
                     cur_line = f"[bold]{cur_line}[/]"
                 result += cur_line + "\n"
             return result
 
         rendered_service_resource_list = render_importable_resources(
             service_resource_list
         )
         console.print(rendered_service_resource_list)
         return  # list option is enabled, do not run the actual importing code.
 
-    if (not service) or (not resource_node):
-        _list_service_or_resource(service, resource_node, screen_pager=screen)
+    is_terraform_r_type_given = is_terraform_aws_resource_type(service_or_tf_resource_type) and resource_node is None
+    if is_terraform_r_type_given:
+        logger.debug(f"Terraform resource type is given: {service_or_tf_resource_type} instead of service and resource node.")
+        pass
+    elif (not service_or_tf_resource_type) or (not resource_node):
+        _list_service_or_resource(service_or_tf_resource_type, resource_node, screen_pager=screen)
         console.print(f"[red bold]Please pick a Service and Resource Node[/]")
         return
 
-    import_blocks = generate_import_block_for_resource(
-        balcony_aws,
-        service,
-        resource_node,
-        follow_pagination=follow_pagination,
-    )
+    import_blocks = None
+    if is_terraform_r_type_given:
+        import_blocks = generate_import_block_for_resource(
+            balcony_aws,
+            terraform_resource_type=service_or_tf_resource_type,
+            follow_pagination=follow_pagination
+        )
+    else:
+        import_blocks = generate_import_block_for_resource(
+            balcony_aws,
+            service=service_or_tf_resource_type,
+            resource_node=resource_node,
+            follow_pagination=follow_pagination,
+        )
 
     if not import_blocks:
-        logger.debug(f"No import blocks generated for {service}.{resource_node}")
+        logger.debug(f"No import blocks generated for {service_or_tf_resource_type}.{resource_node}")
 
         fail_msg = textwrap.dedent(
             f"""
-            No terraform import blocks generated for [bold]{service}.{resource_node}[/]. Some checks:
+            No terraform import blocks generated for [bold]{service_or_tf_resource_type}.{resource_node}[/]. Some checks:
                 
                 - [underline]Run the balcony with [bold]--debug[/] flag to see more info.[/]
-                    Run     [bold]balcony terraform-import --debug {service} {resource_node}[/]
+                    Run     [bold]balcony terraform-import --debug {service_or_tf_resource_type} {resource_node}[/]
                     
                 - [underline]Do you have the correct AWS credentials and Region?[/]
                     Run     [bold]printenv | grep ^AWS_[/]
                 
                 - [underline]Is the resource node name correct?[/]
-                    Run     [bold]balcony aws {service}[/]      to see available resource nodes.
+                    Run     [bold]balcony aws {service_or_tf_resource_type}[/]      to see available resource nodes.
                 
                 - [underline]You may not have any resources in your AWS Account, check it first:[/]
-                    Run     [bold]balcony aws {service} {resource_node} -d[/] 
+                    Run     [bold]balcony aws {service_or_tf_resource_type} {resource_node} -d[/] 
             """
         ).strip()
         console.print(Padding(fail_msg, (1, 1)))
         raise typer.Exit(-1)
 
     if output_file:
         output_filepath = Path(output_file).resolve()
@@ -493,15 +507,15 @@
     else:
         if screen:
             with console.pager(styles=True):
                 console.print("\n".join(import_blocks))
         else:            
             console.print("\n".join(import_blocks))
 
-    return import_blocks
+    return  # import_blocks
 
 
 @app.command(
     "terraform-wizard",
     no_args_is_help=True,
     short_help="Wizard that helps you to create the correct import-configuration interactively for the 'terraform-import' command.",
     help="""
```

### Comparing `balcony-0.1.5/balcony/config.py` & `balcony-0.1.6/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_nodes/codebuild.py` & `balcony-0.1.6/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_nodes/ecs.py` & `balcony-0.1.6/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_nodes/iam.py` & `balcony-0.1.6/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.6/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_nodes/s3.py` & `balcony-0.1.6/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_nodes/ses.py` & `balcony-0.1.6/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_nodes/ssm.py` & `balcony-0.1.6/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_tf_import_configs/ec2.yaml` & `balcony-0.1.6/balcony/custom_tf_import_configs/ec2.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -52,8 +52,16 @@
 
   - id_generator_jinja2_template: '{{ GroupId }}'
     jmespath_query: '[].SecurityGroups[]'
     operation_name: DescribeSecurityGroups
     resource_node: SecurityGroups
     service: ec2
     to_resource_name_jinja2_template: '{{ GroupName ~ ''-'' ~ VpcId }}'
-    to_resource_type: aws_security_group
+    to_resource_type: aws_security_group
+
+  - id_generator_jinja2_template: '{{ AssociationId }}'
+    jmespath_query: '[].Addresses[]'
+    operation_name: DescribeAddresses
+    resource_node: Addresses
+    service: ec2
+    to_resource_name_jinja2_template: '{{ AssociationId }}'
+    to_resource_type: aws_eip_association
```

### Comparing `balcony-0.1.5/balcony/custom_tf_import_configs/iam.yaml` & `balcony-0.1.6/balcony/custom_tf_import_configs/iam.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+maintainers:
+- name: Oguzhan Yilmaz
+
 import_configurations:
 - id_generator_jinja2_template: '{{ UserName }}'
   jmespath_query: '[].Users[]'
   operation_name: ListUsers
   resource_node: User
   service: iam
   to_resource_name_jinja2_template: '{{ UserName }}'
@@ -27,9 +30,31 @@
   jmespath_query: '[].Policies[]'
   operation_name: ListPolicies
   resource_node: Policy
   service: iam
   to_resource_name_jinja2_template: '{{ PolicyName or PolicyId }}'
   to_resource_type: aws_iam_policy
 
-maintainers:
-- name: Oguzhan Yilmaz
+- id_generator_jinja2_template: '{{ RoleName }}'
+  jmespath_query: '[].Roles[]'
+  operation_name: ListRoles
+  resource_node: Role
+  service: iam
+  to_resource_name_jinja2_template: '{{ ''role-'' ~ RoleName }}'
+  to_resource_type: aws_iam_role
+
+- id_generator_jinja2_template: '{{ GroupName ~ '':'' ~ PolicyName }}'
+  jmespath_query: '[]'
+  operation_name: GetGroupPolicy
+  resource_node: GroupPolicy
+  service: iam
+  to_resource_name_jinja2_template: '{{ GroupName ~ ''-'' ~ PolicyName }}'
+  to_resource_type: aws_iam_group_policy
+
+- id_generator_jinja2_template: '{{ UserName ~ '':''  ~ PolicyName }}'
+  jmespath_query: '[]'
+  operation_name: GetUserPolicy
+  resource_node: UserPolicy
+  service: iam
+  to_resource_name_jinja2_template: '{{ UserName ~ ''-'' ~ PolicyName }}'
+  to_resource_type: aws_iam_user_policy
+
```

### Comparing `balcony-0.1.5/balcony/custom_tf_import_configs/rds.yaml` & `balcony-0.1.6/balcony/custom_tf_import_configs/rds.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.6/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/custom_yamls/iam.yaml` & `balcony-0.1.6/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/nodes.py` & `balcony-0.1.6/balcony/nodes.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/reader.py` & `balcony-0.1.6/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/registries.py` & `balcony-0.1.6/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/relations.py` & `balcony-0.1.6/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/terraform_import/importer.py` & `balcony-0.1.6/balcony/terraform_import/importer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 import re
 import textwrap
-from typing import List, Union
+from typing import Dict, List, Tuple, Union
 import jmespath
-from terraform_import.parsers import parse_custom_tf_import_config
+from terraform_import.models import TerraformImportConfig
+from terraform_import.parsers import parse_custom_terraform_import_configs_from_files, _TERRAFORM_TYPES_KEY
 from config import get_logger
 from aws import BalconyAWS
 from jinja2 import Environment
 
 logger = get_logger(__name__)
+_terraform_import_configurations = None
+
+
+def get_custom_terraform_import_config_dict() -> Dict:
+    global _terraform_import_configurations
+    if _terraform_import_configurations:
+        return _terraform_import_configurations
+
+    _terraform_import_configurations = parse_custom_terraform_import_configs_from_files()
+    return _terraform_import_configurations
 
 
 def extract_resource_tags_as_kwargs(data: dict) -> dict:
     tags_as_kwargs = {}
     tag_list = data.get("Tags", [])
     if not tag_list or not isinstance(tag_list, list):
         return tags_as_kwargs
@@ -33,35 +44,36 @@
         # if there's add it as tag_Name variable
         tags_as_kwargs = extract_resource_tags_as_kwargs(data)
         kwargs.update(tags_as_kwargs)
         rendered_output = template.render(**kwargs).strip()
         result.append(rendered_output)
     elif isinstance(data, list):
         # if the data is a list, render the template for each item
-        kwargs = data.copy()
+        kwargs = {"data": data}
         for an_item in data:
             kwargs["item"] = an_item
-            kwargs["data"] = an_item
             rendered_output = template.render(**kwargs).strip()
-            result.append(rendered_output)
+            rendered_list = [_.strip() for _ in rendered_output.split(' ') if _]
+            result.extend(rendered_list)
     elif isinstance(data, str):
         kwargs = {
             "item": data,
             "data": data,
         }
         rendered_output = template.render(**kwargs).strip()
         result.append(rendered_output)
     return result
 
 
 def gen_resource_name_and_import_id_from_op_data_(
     operation_data, jmespath_query, to_resource_name_tpl, id_generator_tpl
 ):
     result = []
-    if jmespath_query:
+    is_basic_j2_template = '{%' not in to_resource_name_tpl.lstrip()
+    if jmespath_query and is_basic_j2_template:
         # filter the operation data if jmespath_query is given
         # and render them one by one
         list_of_resource_data = jmespath.search(jmespath_query, operation_data)
         logger.debug(f"Filtered data using jmespath query: {jmespath_query}")
 
         for a_resource_data in list_of_resource_data:
             resource_name_list = render_jinja2_template_with_data(
@@ -73,27 +85,25 @@
             result.extend(list(zip(resource_name_list, import_id_list)))
 
         return result
     else:
         # no jmespath query given, use the whole operation data
         # assumes there's multiple lines of output from the template
 
-        resource_name_multiline = render_jinja2_template_with_data(
-            a_resource_data, to_resource_name_tpl
-        )[0]  # FIXME: later
-        import_id_multiline = render_jinja2_template_with_data(
-            a_resource_data, id_generator_tpl
-        )[0]  # FIXME: later
+        multiline_resource_name_list = render_jinja2_template_with_data(
+            operation_data, to_resource_name_tpl
+        )
+        multiline_import_id_list = render_jinja2_template_with_data(
+            operation_data, id_generator_tpl
+        )
         # split them on newlines
-        resource_name_list = [ro for ro in resource_name_multiline.split("\n") if ro]
-        import_id_list = [ro for ro in import_id_multiline.split("\n") if ro]
 
-        logger.debug(f"{resource_name_list=}    {import_id_list=}")
-        assert len(resource_name_list) == len(import_id_list)
-        return list(zip(resource_name_list, import_id_list))
+        assert len(multiline_resource_name_list) == len(multiline_import_id_list)
+        r = list(zip(multiline_resource_name_list, multiline_import_id_list))
+        return r
 
 
 def generate_terraform_import_block(to_resource_type, to_resource_name, import_id):
     jinja_tmpl = textwrap.dedent(
         """
     import {
         to = {{ to_resource_type }}.{{ to_resource_name }}
@@ -108,83 +118,135 @@
         to_resource_type=to_resource_type,
         import_id=import_id,
         to_resource_name=to_resource_name,
     ).strip()
     return rendered_output
 
 
-def get_importable_resources():
-    custom_tf_config_dict = parse_custom_tf_import_config()
+def get_importable_resources() -> List[Tuple[str, str]]:
+    custom_tf_config_dict = get_custom_terraform_import_config_dict()
 
     importable_services_and_resources = []
     for service_name, resource_config_dict in custom_tf_config_dict.items():
-        for resource_node_name, resource_config in resource_config_dict.items():
-            importable_services_and_resources.append((service_name, resource_node_name))
-    return importable_services_and_resources
+        if service_name == _TERRAFORM_TYPES_KEY:
+            continue  # skip the _terraform_types cache key
+        for resource_node_name, resource_config_list in resource_config_dict.items():
+            for resource_config in resource_config_list:
+                terraform_resource_type = resource_config.to_resource_type
+                importable_services_and_resources.append((terraform_resource_type, service_name, resource_node_name))
+    return list(sorted(importable_services_and_resources, key=lambda x: x[1]+x[2]))
 
 
-def generate_import_block_for_resource(
-    balcony_client: BalconyAWS,
-    service: str,
-    resource_node: str,
-    follow_pagination: bool = False,
-):
+def sanitize_resource_name_and_import_ids(list_of_tuples):
+    result = []
+    for resource_name, import_id in list_of_tuples:
+        # change anything that's not a letter, number, dash or underscore to underscore
+        sanitized_resource_name = re.sub(r"[^A-Za-z0-9\-_]", "_", resource_name)
+        # allow / in the import id
+        # sanitized_import_id = re.sub(r"[^A-Za-z0-9\-_/]", "_", import_id)
+        if sanitized_resource_name and import_id:
+            result.append((sanitized_resource_name, import_id))
+    return result
+
+
+def get_import_config_for(
+    service: str = None,
+    resource_node: str = None,
+    terraform_resource_type: str = None,
+) -> List[TerraformImportConfig]:
+    custom_tf_config_dict = get_custom_terraform_import_config_dict()
+
+    if service and resource_node:
+        config_for_resource_node = custom_tf_config_dict.get(service, {}).get(
+            resource_node, []
+        )
+        return config_for_resource_node
+    elif terraform_resource_type:
+        config_list_for_tf_type = custom_tf_config_dict.get(_TERRAFORM_TYPES_KEY, {}).get(
+            terraform_resource_type, False
+        )
+        if not config_list_for_tf_type:
+            return False
+        return config_list_for_tf_type
+    return False
+
 
+def generate_import_block_from_import_config(
+    balcony_client: BalconyAWS,
+    tf_import_config: TerraformImportConfig,
+    follow_pagination: bool = False
+) -> List[str]:
     tf_import_blocks: List[str] = []
-    custom_tf_config_dict = parse_custom_tf_import_config()
-    config_for_resource_node = custom_tf_config_dict.get(service, {}).get(
-        resource_node, False
-    )
-    if not config_for_resource_node:
+
+    operation_name = tf_import_config.operation_name
+    service = tf_import_config.service
+    resource_node = tf_import_config.resource_node
+    jmespath_query = tf_import_config.jmespath_query
+
+    if not tf_import_config:
         logger.debug(
             f"[red bold]No custom terraform import config found for {service}.{resource_node}. Please check out docs https://oguzhan-yilmaz.github.io/balcony/ for more info on developing it your own."
         )
         return False
 
-    # read the data
-    operation_name = config_for_resource_node.operation_name
-
-    jmespath_query = config_for_resource_node.jmespath_query
-
+    # read the operation
     operation_data = balcony_client.read_operation(
         service_name=service,
         resource_node_name=resource_node,
         operation_name=operation_name,
-        follow_pagination=follow_pagination,  # TODO: remove the comment after
+        follow_pagination=follow_pagination,
     )
 
     if not operation_data:
-        logger.debug(f"No data found for {service}/{resource_node}/{operation_name}.")
+        logger.debug(f"No data found for {service}.{resource_node}.{operation_name}.")
         return False
 
     resource_name_and_import_ids = gen_resource_name_and_import_id_from_op_data_(
         operation_data,
         jmespath_query,
-        config_for_resource_node.to_resource_name_jinja2_template,
-        config_for_resource_node.id_generator_jinja2_template,
+        tf_import_config.to_resource_name_jinja2_template,
+        tf_import_config.id_generator_jinja2_template,
     )
 
-    def sanitize_resource_name_and_import_ids(list_of_tuples):
-        result = []
-        for resource_name, import_id in list_of_tuples:
-            # change anything that's not a letter, number, dash or underscore to underscore
-            sanitized_resource_name = re.sub(r"[^A-Za-z0-9\-_]", "_", resource_name)
-
-            if sanitized_resource_name and import_id:
-                result.append((sanitized_resource_name, import_id))
-        return result
-
     # Replace unsupported chars from the to-resource-name with underscore
     sanitized_resource_name_and_import_ids = sanitize_resource_name_and_import_ids(
         resource_name_and_import_ids
     )
 
     logger.debug(
         f"Found {len(sanitized_resource_name_and_import_ids)} resources to import."
     )
     for a_tuple in sanitized_resource_name_and_import_ids:
         to_resource_name, import_id = a_tuple
         tf_import_block = generate_terraform_import_block(
-            config_for_resource_node.to_resource_type, to_resource_name, import_id
+            tf_import_config.to_resource_type, to_resource_name, import_id
         )
         tf_import_blocks.append(tf_import_block)
     return tf_import_blocks
+
+
+
+def generate_import_block_for_resource(
+    balcony_client: BalconyAWS,
+    service: str = None,
+    resource_node: str = None,
+    terraform_resource_type: str = None,
+    follow_pagination: bool = False,
+):
+    resulting_tf_import_blocks = []
+    tf_import_configs = get_import_config_for(service, resource_node, terraform_resource_type)
+    if not tf_import_configs:
+        logger.debug(
+            f"[red bold]No custom terraform import config found for {service}.{resource_node}. Please check out docs https://oguzhan-yilmaz.github.io/balcony/ for more info on developing it your own."
+        )
+        return False
+
+    for tf_import_config in tf_import_configs:
+        tf_import_blocks = generate_import_block_from_import_config(balcony_client, tf_import_config, follow_pagination)
+        if not tf_import_blocks:
+            logger.debug(
+                f"[red bold]No data found for {tf_import_config.to_resource_type} — {tf_import_config.resource_node}.{tf_import_config.operation_name}."
+            )
+            return False
+        resulting_tf_import_blocks.extend(tf_import_blocks)
+        
+    return resulting_tf_import_blocks
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `balcony-0.1.5/balcony/terraform_import/models.py` & `balcony-0.1.6/balcony/terraform_import/models.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/terraform_import/parsers.py` & `balcony-0.1.6/balcony/terraform_import/parsers.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     TerraformImportConfig,
 )
 from typing import Union, Tuple
 import yaml
 from collections import defaultdict
 
 logger = get_logger(__name__)
+_TERRAFORM_TYPES_KEY='_terraform_types'
 
 
 def parse_json_to_tf_import_config(
     input_configuration_dict: str,
 ) -> Union[bool, CustomTerraformImportConfigFile]:
     try:
         return CustomTerraformImportConfigFile(**input_configuration_dict)
@@ -41,22 +42,20 @@
         with open(yaml_file_path, "r") as f:
             input_data = yaml.load(f, Loader=yaml.FullLoader)
         return CustomTerraformImportConfigFile(**input_data), None
     except Exception as e:
         return False, e
 
 
-def parse_custom_tf_import_config():
+def parse_custom_terraform_import_configs_from_files():
+    terraform_configurations_dict = defaultdict(lambda: defaultdict(dict))
 
-    custom_terraform_config_dict = defaultdict(lambda: defaultdict(dict))
-
-    parse_directories = [
-        YAML_TF_IMPORT_CONFIGS_DIRECTORY,
-    ]
-    if USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY:
+    parse_directories = [YAML_TF_IMPORT_CONFIGS_DIRECTORY,] # noqa
+    _are_same_directories = USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY == YAML_TF_IMPORT_CONFIGS_DIRECTORY.as_posix()
+    if USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY and not _are_same_directories:
         # might not be defined
         parse_directories.append(USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY)
 
     for yaml_directory in parse_directories:
         config_filenames = find_all_yaml_files(yaml_directory)
         logger.debug(
             f"Terraform Import Configuration Registry: Found {len(config_filenames)} yaml files in {yaml_directory}. Starting to parse & validate them."
@@ -65,11 +64,23 @@
         for conf_filename in config_filenames:
             conf, error = parse_yaml_file_to_tf_import_config(conf_filename)
             if error:
                 logger.error(f"Error while parsing {conf_filename}: {error}")
                 continue
             for tf_config in conf.import_configurations:
                 # doing it this way allows overrides from the user defined configs
-                custom_terraform_config_dict[tf_config.service][
-                    tf_config.resource_node
-                ] = tf_config
-    return custom_terraform_config_dict
+                r_node = terraform_configurations_dict.get(tf_config.service, {}).get(tf_config.resource_node, False)
+                if r_node is False:
+                    terraform_configurations_dict[tf_config.service][
+                        tf_config.resource_node
+                    ] = [tf_config]
+                else:
+                    terraform_configurations_dict[tf_config.service][
+                        tf_config.resource_node
+                    ].append(tf_config)
+                # add it to _TERRAFORM_TYPES_KEY
+                tf_conf_list = terraform_configurations_dict[_TERRAFORM_TYPES_KEY].get(tf_config.to_resource_type, [])
+                if not tf_conf_list:
+                    terraform_configurations_dict[_TERRAFORM_TYPES_KEY][tf_config.to_resource_type] = [tf_config]
+                else:
+                    terraform_configurations_dict[_TERRAFORM_TYPES_KEY][tf_config.to_resource_type].append(tf_config)
+    return terraform_configurations_dict
```

### Comparing `balcony-0.1.5/balcony/terraform_import/wizard.py` & `balcony-0.1.6/balcony/terraform_import/wizard.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/test.py` & `balcony-0.1.6/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/utils.py` & `balcony-0.1.6/balcony/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import Counter
-from re import finditer, compile
+from re import finditer, compile, match
 import textwrap
 from typing import List
 import inflect
 import os
 import boto3
 from config import get_logger, YAML_IGNORE_PREFIX
 import botocore
@@ -12,14 +12,27 @@
 
 inflect_engine = inflect.engine()  # used for singular/plural word comparing
 logger = get_logger(__name__)
 
 _camel_case_regex_compiled = compile(
     r".+?(?:(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|$)"
 )
+_terraform_aws_resource_type_pattern_compiled = compile(r"^aws_[a-zA-Z0-9_-]+$")
+
+
+def is_terraform_aws_resource_type(resource_type: str) -> bool:
+    """Check for terraform aws resource type being valid
+
+    Args:
+        resource_type (str): Check for terraform aws resource type being valid
+
+    Returns:
+        bool: is resource type valid
+    """
+    return bool(match(_terraform_aws_resource_type_pattern_compiled, resource_type))
 
 
 def find_all_yaml_files(directory: str) -> List[str]:
     """Find all .yaml files in a directory with the exception of files starting with "_".
 
     Args:
         directory (str): Directory to search for yaml files
```

### Comparing `balcony-0.1.5/balcony/yaml_config.py` & `balcony-0.1.6/balcony/yaml_config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/balcony/yaml_validators.py` & `balcony-0.1.6/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.5/pyproject.toml` & `balcony-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balcony"
-version = "0.1.5"
+version = "0.1.6"
 description = "Read any resource in your AWS Account. You can generate terraform code for them, too."
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
```

