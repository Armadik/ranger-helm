# ranger-admin

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square)

The Helm chart for ranger

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.helm.sh/stable | postgresql | 8.6.4 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| configMountPath | string | `/opt/ranger-admin/install.properties` |  |
| conf.DB_FLAVOR | string | `"POSTGRES"` |  |
| conf.JAVA_BIN | string | `"java"` |  |
| conf.JAVA_ORACLE | string | `"Java(TM) SE Runtime Environment"` |  |
| conf.JAVA_VERSION_REQUIRED | string | `"1.8"` |  |
| conf.LOGFILE | string | `"/opt/ranger-admin/logfile"` |  |
| conf.LOGFILES | string | `"$LOGFILE"` |  |
| conf.PATCH_RETRY_INTERVAL | int | `120` |  |
| conf.PYTHON_COMMAND_INVOKER | string | `"python3"` |  |
| conf.RANGER_ADMIN_LOGBACK_CONF_FILE | string | `nil` |  |
| conf.RANGER_ADMIN_LOG_DIR | string | `"$PWD"` |  |
| conf.RANGER_PID_DIR_PATH | string | `"/tmp/ranger"` |  |
| conf.SQL_CONNECTOR_JAR | string | `"/usr/share/java/postgresql-connector-java.jar"` |  |
| conf.STALE_PATCH_ENTRY_HOLD_TIME | int | `10` |  |
| conf.TMPFILE | string | `"/opt/ranger-admin/.fi_tmp"` |  |
| conf.XAPOLICYMGR_DIR | string | `"$PWD"` |  |
| conf.admin_keytab | string | `nil` |  |
| conf.admin_principal | string | `nil` |  |
| conf.app_home | string | `"/opt/ranger-admin/ews/webapp"` |  |
| conf.audit_cloudwatch_log_group | string | `nil` |  |
| conf.audit_cloudwatch_log_stream_prefix | string | `nil` |  |
| conf.audit_cloudwatch_region | string | `nil` |  |
| conf.audit_elasticsearch_bootstrap_enabled | bool | `true` |  |
| conf.audit_elasticsearch_index | string | `nil` |  |
| conf.audit_elasticsearch_password | string | `nil` |  |
| conf.audit_elasticsearch_port | string | `nil` |  |
| conf.audit_elasticsearch_protocol | string | `nil` |  |
| conf.audit_elasticsearch_urls | string | `nil` |  |
| conf.audit_elasticsearch_user | string | `nil` |  |
| conf.audit_solr_acl_user_list_sasl | string | `"solr,infra-solr"` |  |
| conf.audit_solr_bootstrap_enabled | bool | `true` |  |
| conf.audit_solr_collection_name | string | `"ranger_audits"` |  |
| conf.audit_solr_config_name | string | `"ranger_audits"` |  |
| conf.audit_solr_configset_location | string | `nil` |  |
| conf.audit_solr_max_shards_per_node | int | `1` |  |
| conf.audit_solr_no_replica | int | `1` |  |
| conf.audit_solr_no_shards | int | `1` |  |
| conf.audit_solr_password | string | `"SOLR_PASSWORD"` |  |
| conf.audit_solr_urls | string | `"localhost:8123"` |  |
| conf.audit_solr_user | string | `"SOLR_USER"` |  |
| conf.audit_solr_zookeepers | string | `nil` |  |
| conf.audit_store | string | `"solr"` |  |
| conf.authServiceHostName | string | `"localhost"` |  |
| conf.authServicePort | int | `5151` |  |
| conf.authentication_method | string | `"LDAP"` |  |
| conf.cookie_domain | string | `nil` |  |
| conf.cookie_path | string | `"/"` |  |
| conf.db_host | string | `"ranger-local-postgresql:5432"` |  |
| conf.db_name | string | `"ranger"` |  |
| conf.db_override_connection_string | string | `nil` |  |
| conf.db_password | string | `"ranger"` |  |
| conf.db_root_password | string | `"ranger"` |  |
| conf.db_root_user | string | `"ranger"` |  |
| conf.db_ssl_auth_type | string | `"2-way"` |  |
| conf.db_ssl_certificate_file | string | `nil` |  |
| conf.db_ssl_enabled | bool | `false` |  |
| conf.db_ssl_required | bool | `false` |  |
| conf.db_ssl_verifyServerCertificate | bool | `false` |  |
| conf.db_user | string | `"ranger"` |  |
| conf.hadoop_conf | string | `"/etc/hadoop-default"` |  |
| conf.is_override_db_connection_string | bool | `false` |  |
| conf.javax_net_ssl_keyStore | string | `nil` |  |
| conf.javax_net_ssl_keyStorePassword | string | `nil` |  |
| conf.javax_net_ssl_keyStore_type | string | `"jks"` |  |
| conf.javax_net_ssl_trustStore | string | `nil` |  |
| conf.javax_net_ssl_trustStorePassword | string | `nil` |  |
| conf.javax_net_ssl_trustStore_type | string | `"jks"` |  |
| conf.keyadmin_password | string | `"RANGER_KEYADMIN_PASSWORD"` |  |
| conf.lookup_keytab | string | `nil` |  |
| conf.lookup_principal | string | `nil` |  |
| conf.policymgr_external_url | string | `"http://localhost:6080"` |  |
| conf.policymgr_http_enabled | bool | `true` |  |
| conf.policymgr_https_keystore_file | string | `nil` |  |
| conf.policymgr_https_keystore_keyalias | string | `"rangeradmin"` |  |
| conf.policymgr_https_keystore_password | string | `nil` |  |
| conf.policymgr_supportedcomponents | string | `"hdfs,yarn"` |  |
| conf.rangerAdmin_password | string | `"RANGER_ADMIN_PASSWORD"` |  |
| conf.rangerTagsync_password | string | `"RANGER_TAGSYNC_PASSWORD"` |  |
| conf.rangerUsersync_password | string | `"RANGER_USERSYNC_PASSWORD"` |  |
| conf.ranger_admin_max_heap_size | string | `"4g"` |  |
| conf.ranger_unixauth_keystore | string | `"keystore.jks"` |  |
| conf.ranger_unixauth_keystore_password | string | `"password"` |  |
| conf.ranger_unixauth_truststore | string | `"cacerts"` |  |
| conf.ranger_unixauth_truststore_password | string | `"changeit"` |  |
| conf.remoteLoginEnabled | bool | `true` |  |
| conf.spnego_keytab | string | `nil` |  |
| conf.spnego_principal | string | `nil` |  |
| conf.sso_enabled | bool | `false` |  |
| conf.sso_providerurl | string | `"https://127.0.0.1:8443/gateway/knoxsso/api/v1/websso"` |  |
| conf.sso_publickey | string | `nil` |  |
| conf.token_valid | int | `30` |  |
| conf.unix_group | string | `"ranger"` |  |
| conf.unix_user | string | `"ranger"` |  |
| conf.unix_user_pwd | string | `nil` |  |
| conf.xa_ldap_ad_base_dn | string | `nil` |  |
| conf.xa_ldap_ad_bind_dn | string | `nil` |  |
| conf.xa_ldap_ad_bind_password | string | `nil` |  |
| conf.xa_ldap_ad_domain | string | `nil` |  |
| conf.xa_ldap_ad_referral | string | `nil` |  |
| conf.xa_ldap_ad_url | string | `nil` |  |
| conf.xa_ldap_ad_userSearchFilter | string | `nil` |  |
| conf.xa_ldap_base_dn | string | `nil` |  |
| conf.xa_ldap_bind_dn | string | `nil` |  |
| conf.xa_ldap_bind_password | string | `"LDAP_TUZ_PASSWORD"` |  |
| conf.xa_ldap_groupRoleAttribute | string | `nil` |  |
| conf.xa_ldap_groupSearchBase | string | `nil` |  |
| conf.xa_ldap_groupSearchFilter | string | `nil` |  |
| conf.xa_ldap_referral | string | `nil` |  |
| conf.xa_ldap_url | string | `nil` |  |
| conf.xa_ldap_userDNpattern | string | `nil` |  |
| conf.xa_ldap_userSearchFilter | string | `nil` |  |
| extraEnv[0].name | string | `"JAVA_OPTS"` |  |
| extraEnv[0].value | string | `" -Dcom.sun.management.jmxremote -Dcom.sun.management.jmxremote.port=6081 -Dcom.sun.management.jmxremote.local.only=false -Dcom.sun.management.jmxremote.authenticate=false -javaagent:/usr/share/java/jmx_prometheus_javaagent.jar=6088:/opt/ranger-admin/jmx_prometheus_javaagent.yaml -Dcom.sun.management.jmxremote.ssl=false "` |  |
| fullnameOverride | string | `"ranger-admin"` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"armadik/ranger-admin"` |  |
| image.tag | string | `"2.4.0"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts | list | `[]` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `"ranger-admin"` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| postgresql.enabled | bool | `true` |  |
| postgresql.postgresqlDatabase | string | `"ranger"` |  |
| postgresql.postgresqlPassword | string | `"ranger"` |  |
| postgresql.postgresqlUsername | string | `"ranger"` |  |
| ranger_usersync.conf.AUTH_SSL_ENABLED | bool | `false` |  |
| ranger_usersync.conf.AUTH_SSL_KEYSTORE_FILE | string | `"/etc/ranger/usersync/conf/cert/unixauthservice.jks"` |  |
| ranger_usersync.conf.AUTH_SSL_KEYSTORE_PASSWORD | int | `12345` |  |
| ranger_usersync.conf.AUTH_SSL_TRUSTSTORE_FILE | string | `nil` |  |
| ranger_usersync.conf.AUTH_SSL_TRUSTSTORE_PASSWORD | string | `nil` |  |
| ranger_usersync.conf.CRED_KEYSTORE_FILENAME | string | `"/etc/ranger/usersync/conf/rangerusersync.jceks"` |  |
| ranger_usersync.conf.GROUP_BASED_ROLE_ASSIGNMENT_RULES | string | `nil` |  |
| ranger_usersync.conf.JVM_METRICS_ENABLED | bool | `false` |  |
| ranger_usersync.conf.JVM_METRICS_FILENAME | string | `"ranger_usersync_metric.json"` |  |
| ranger_usersync.conf.JVM_METRICS_FILEPATH | string | `"logs"` |  |
| ranger_usersync.conf.JVM_METRICS_FREQUENCY_TIME_IN_MILLIS | int | `10000` |  |
| ranger_usersync.conf.MIN_UNIX_GROUP_ID_TO_SYNC | int | `500` |  |
| ranger_usersync.conf.MIN_UNIX_USER_ID_TO_SYNC | int | `1000` |  |
| ranger_usersync.conf.ROLE_ASSIGNMENT_LIST_DELIMITER | string | `"&"` |  |
| ranger_usersync.conf.SYNC_GROUP_MEMBER_ATTRIBUTE_NAME | string | `nil` |  |
| ranger_usersync.conf.SYNC_GROUP_OBJECT_CLASS | string | `nil` |  |
| ranger_usersync.conf.SYNC_GROUP_SEARCH_ENABLED | string | `nil` |  |
| ranger_usersync.conf.SYNC_GROUP_SEARCH_SCOPE | string | `nil` |  |
| ranger_usersync.conf.SYNC_GROUP_USER_MAP_SYNC_ENABLED | string | `nil` |  |
| ranger_usersync.conf.SYNC_INTERVAL | int | `15` |  |
| ranger_usersync.conf.SYNC_LDAP_BIND_DN | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_BIND_PASSWORD | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_DELTASYNC | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_GROUPNAME_CASE_CONVERSION | string | `"none"` |  |
| ranger_usersync.conf.SYNC_LDAP_GROUP_SEARCH_FILTER | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_REFERRAL | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_SEARCH_BASE | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_URL | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_USERNAME_CASE_CONVERSION | string | `"none"` |  |
| ranger_usersync.conf.SYNC_LDAP_USER_GROUP_NAME_ATTRIBUTE | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_USER_NAME_ATTRIBUTE | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_USER_OBJECT_CLASS | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_USER_SEARCH_BASE | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_USER_SEARCH_FILTER | string | `nil` |  |
| ranger_usersync.conf.SYNC_LDAP_USER_SEARCH_SCOPE | string | `nil` |  |
| ranger_usersync.conf.SYNC_SOURCE | string | `"ldap"` |  |
| ranger_usersync.conf.USERNAME_GROUPNAME_ASSIGNMENT_LIST_DELIMITER | string | `","` |  |
| ranger_usersync.conf.USERSYNC_PID_DIR_PATH | string | `"/opt/ranger-usersync/"` |  |
| ranger_usersync.conf.USERS_GROUPS_ASSIGNMENT_LIST_DELIMITER | string | `":"` |  |
| ranger_usersync.conf.hadoop_conf | string | `"/etc/hadoop-default"` |  |
| ranger_usersync.conf.logdir | string | `"logs"` |  |
| ranger_usersync.conf.rangerUsersync_password | string | `"RANGER_USERSYNC_PASSWORD"` |  |
| ranger_usersync.conf.ranger_base_dir | string | `"/etc/ranger"` |  |
| ranger_usersync.conf.unix_group | string | `"ranger"` |  |
| ranger_usersync.conf.unix_user | string | `"ranger"` |  |
| ranger_usersync.conf.usersync_keytab | string | `nil` |  |
| ranger_usersync.conf.usersync_principal | string | `nil` |  |
| ranger_usersync.enabled | bool | `false` |  |
| ranger_usersync.extraEnv | list | `[]` |  |
| ranger_usersync.image.pullPolicy | string | `"Always"` |  |
| ranger_usersync.image.repository | string | `"armadik/ranger-usersync"` |  |
| ranger_usersync.image.tag | string | `"2.4.0"` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | int | `4` |  |
| resources.limits.memory | string | `"8Gi"` |  |
| resources.requests.cpu | int | `2` |  |
| resources.requests.memory | string | `"4Gi"` |  |
| securityContext | object | `{}` |  |
| service.port | int | `6080` |  |
| service.type | string | `"ClusterIP"` |  |
| commonLabels | object | `{}` | Labels to add to all deployed objects |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `""` |  |
| servicemonitor.create | bool | `true` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.13.1](https://github.com/norwoodj/helm-docs/releases/v1.13.1)
