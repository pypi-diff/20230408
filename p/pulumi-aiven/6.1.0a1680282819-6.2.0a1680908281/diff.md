# Comparing `tmp/pulumi_aiven-6.1.0a1680282819.tar.gz` & `tmp/pulumi_aiven-6.2.0a1680908281.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.1.0a1680282819.tar", last modified: Fri Mar 31 17:19:31 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.2.0a1680908281.tar", last modified: Fri Apr  7 23:07:21 2023, max compression
```

## Comparing `pulumi_aiven-6.1.0a1680282819.tar` & `pulumi_aiven-6.2.0a1680908281.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:19:31.321583 pulumi_aiven-6.1.0a1680282819/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-31 17:19:31.321583 pulumi_aiven-6.1.0a1680282819/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:19:31.317583 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   599198 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    73507 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:19:31.321583 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    73192 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    74761 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    73222 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    78050 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    76154 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    76710 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75554 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    74440 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    75063 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74183 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)   892539 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71601 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74559 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29938 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    53402 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:19:31.321583 pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-03-31 17:19:31.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-03-31 17:19:31.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:19:31.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:19:31.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-31 17:19:31.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-31 17:19:31.000000 pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 17:19:31.321583 pulumi_aiven-6.1.0a1680282819/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-31 17:19:30.000000 pulumi_aiven-6.1.0a1680282819/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:07:21.766697 pulumi_aiven-6.2.0a1680908281/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-07 23:07:21.766697 pulumi_aiven-6.2.0a1680908281/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:07:21.766697 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   599198 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73507 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:07:21.766697 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73192 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74761 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73222 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78050 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76154 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76710 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75554 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74440 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75063 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74183 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   892539 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71601 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74559 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29938 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53402 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:07:21.766697 pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:07:21.766697 pulumi_aiven-6.2.0a1680908281/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-07 23:07:21.000000 pulumi_aiven-6.2.0a1680908281/setup.py
```

### Comparing `pulumi_aiven-6.1.0a1680282819/PKG-INFO` & `pulumi_aiven-6.2.0a1680908281/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.1.0a1680282819
+Version: 6.2.0a1680908281
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_aiven-6.1.0a1680282819/README.md` & `pulumi_aiven-6.2.0a1680908281/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/__init__.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_team.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/flink.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_cassanda.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_project.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_service_component.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/get_transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/grafana.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/open_search.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/outputs.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/pg.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/project.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/project_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/provider.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/redis.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.1.0a1680282819
+Version: 6.2.0a1680908281
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_aiven-6.1.0a1680282819/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.2.0a1680908281/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.1.0a1680282819/setup.py` & `pulumi_aiven-6.2.0a1680908281/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.1.0a1680282819"
-PLUGIN_VERSION = "6.1.0-alpha.1680282819+b47976e5"
+VERSION = "6.2.0a1680908281"
+PLUGIN_VERSION = "6.2.0-alpha.1680908281+c795a662"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
```

