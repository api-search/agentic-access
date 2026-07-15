---
acting_count: 257
action_class_counts:
  acting: 257
  connected: 162
api_specs:
- filename: scaleway-instance-openapi.yml
  format: yaml
  label: Scaleway Instance API
  slug: scaleway-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-instance-openapi.yml
- filename: scaleway-kubernetes-openapi.yml
  format: yaml
  label: Scaleway Kubernetes API
  slug: scaleway-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-kubernetes-openapi.yml
- filename: scaleway-iam-openapi.yml
  format: yaml
  label: Scaleway IAM API
  slug: scaleway-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-iam-openapi.yml
- filename: scaleway-load-balancer-openapi.yml
  format: yaml
  label: Scaleway Load Balancer API
  slug: scaleway-load-balancer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-load-balancer-openapi.yml
- filename: scaleway-database-openapi.yml
  format: yaml
  label: Scaleway Managed Database API
  slug: scaleway-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-database-openapi.yml
- filename: scaleway-vpc-openapi.yml
  format: yaml
  label: Scaleway VPC API
  slug: scaleway-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-vpc-openapi.yml
- filename: scaleway-serverless-containers-openapi.yml
  format: yaml
  label: Scaleway Serverless Containers API
  slug: scaleway-serverless-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-serverless-containers-openapi.yml
- filename: scaleway-serverless-functions-openapi.yml
  format: yaml
  label: Scaleway Serverless Functions API
  slug: scaleway-serverless-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-serverless-functions-openapi.yml
- filename: scaleway-secret-manager-openapi.yml
  format: yaml
  label: Scaleway Secret Manager API
  slug: scaleway-secret-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-secret-manager-openapi.yml
- filename: scaleway-transactional-email-openapi.yml
  format: yaml
  label: Scaleway Transactional Email API
  slug: scaleway-transactional-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-transactional-email-openapi.yml
consequence_counts:
  physical: 3
  read: 162
  safety-critical: 10
  write: 244
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Scaleway Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /iam/v1alpha1/saml/{saml_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /k8s/v1/regions/{region}/acls/{acl_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /k8s/v1/regions/{region}/clusters/{cluster_id}/acls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /k8s/v1/regions/{region}/clusters/{cluster_id}/acls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /k8s/v1/regions/{region}/clusters/{cluster_id}/reset-admin-token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /k8s/v1/regions/{region}/nodes/{node_id}/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rdb/v1/regions/{region}/read-replicas/{read_replica_id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /secret-manager/v1beta1/regions/{region}/secrets/{secret_id}/unprotect
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /secret-manager/v1beta1/regions/{region}/secrets/{secret_id}/versions/{revision}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transactional-email/v1alpha1/regions/{region}/domains/{domain_id}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /containers/v1/regions/{region}/containers/{container_id}/redeploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /functions/v1beta1/regions/{region}/functions/{function_id}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactional-email/v1alpha1/regions/{region}/emails
operation_count: 419
overview: 'Scaleway exposes 419 API operations that an AI agent could call, of which 257 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 162 read, 244 write, 3 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scaleway
provider_slug: scaleway
slug: scaleway-agentic-access
source_filename: scaleway-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scaleway-database-openapi.yml, openapi/scaleway-iam-openapi.yml, openapi/scaleway-instance-openapi.yml,\n  openapi/scaleway-kubernetes-openapi.yml, openapi/scaleway-load-balancer-openapi.yml, openapi/scaleway-secret-manager-openapi.yml,\n  openapi/scaleway-serverless-containers-openapi.yml, openapi/scaleway-serverless-functions-openapi.yml,\n  openapi/scaleway-transactional-email-openapi.yml, openapi/scaleway-vpc-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 419\n  by_action_class:\n    connected: 162\n    acting: 257\n  by_consequence:\n    read: 162\n    write: 244\n    safety-critical: 10\n    physical: 3\n  human_in_the_loop_required: 10\noperations:\n- path: /rdb/v1/regions/{region}/backups\n\
  \  method: get\n  operationId: ListDatabaseBackups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/backups\n  method: post\n  operationId: CreateDatabaseBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/backups/{database_backup_id}\n  method: get\n  operationId: GetDatabaseBackup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/backups/{database_backup_id}\n  method: patch\n  operationId: UpdateDatabaseBackup\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/backups/{database_backup_id}\n  method: delete\n  operationId: DeleteDatabaseBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/backups/{database_backup_id}/export\n  method: post\n  operationId: ExportDatabaseBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /rdb/v1/regions/{region}/backups/{database_backup_id}/restore\n  method: post\n  operationId: RestoreDatabaseBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/database-engines\n  method: get\n  operationId: ListDatabaseEngines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/endpoints/{endpoint_id}\n  method: get\n  operationId: GetEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/endpoints/{endpoint_id}\n  method: delete\n  operationId:\
  \ DeleteEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/endpoints/{endpoint_id}/migrate\n  method: post\n  operationId: MigrateEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances\n  method: get\n  operationId: ListInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances\n  method: post\n  operationId: CreateInstance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}\n  method: get\n  operationId: GetInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}\n  method: patch\n  operationId: UpdateInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}\n  method: delete\n  operationId: DeleteInstance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/acls\n  method: get\n  operationId: ListInstanceACLRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/acls\n  method: post\n  operationId: AddInstanceACLRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/acls\n  method:\
  \ put\n  operationId: SetInstanceACLRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/acls\n  method: delete\n  operationId: DeleteInstanceACLRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/apply-maintenance\n  method: post\n  operationId: ApplyInstanceMaintenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/certificate\n  method: get\n  operationId: GetInstanceCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/clone\n  method: post\n  operationId: CloneInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/databases\n  method: get\n  operationId: ListDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/databases\n  method: post\n  operationId: CreateDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/databases/{name}\n  method: delete\n  operationId: DeleteDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/endpoints\n  method: post\n  operationId: CreateEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/logs\n  method: get\n  operationId: ListInstanceLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/logs-details\n  method: get\n  operationId: ListInstanceLogsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/metrics\n  method: get\n  operationId: GetInstanceMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/prepare-logs\n  method: post\n  operationId: PrepareInstanceLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/privileges\n  method: get\n  operationId: ListPrivileges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/privileges\n  method: put\n  operationId: SetPrivilege\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/purge-logs\n  method: post\n  operationId: PurgeInstanceLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/renew-certificate\n  method: post\n  operationId: RenewInstanceCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/restart\n  method: post\n  operationId: RestartInstance\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/settings\n  method: post\n  operationId: AddInstanceSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/settings\n  method: put\n  operationId: SetInstanceSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/settings\n  method: delete\n  operationId: DeleteInstanceSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/snapshots\n  method: post\n  operationId: CreateSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/upgrade\n  method: post\n  operationId: UpgradeInstance\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/users\n  method: get\n  operationId: ListUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/users\n  method: post\n  operationId: CreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/users/{name}\n  method: patch\n  operationId: UpdateUser\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/instances/{instance_id}/users/{name}\n  method: delete\n  operationId: DeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/logs/{instance_log_id}\n  method: get\n  operationId: GetInstanceLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/node-types\n  method: get\n  operationId: ListNodeTypes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/read-replicas\n  method: post\n  operationId: CreateReadReplica\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/read-replicas/{read_replica_id}\n  method: get\n  operationId: GetReadReplica\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/read-replicas/{read_replica_id}\n  method: delete\n  operationId: DeleteReadReplica\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/read-replicas/{read_replica_id}/endpoints\n  method: post\n  operationId: CreateReadReplicaEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/read-replicas/{read_replica_id}/promote\n  method: post\n  operationId: PromoteReadReplica\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/read-replicas/{read_replica_id}/reset\n\
  \  method: post\n  operationId: ResetReadReplica\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rdb/v1/regions/{region}/snapshots\n  method: get\n  operationId: ListSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/snapshots/{snapshot_id}\n  method: get\n  operationId: GetSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rdb/v1/regions/{region}/snapshots/{snapshot_id}\n  method: patch\n  operationId: UpdateSnapshot\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/snapshots/{snapshot_id}\n  method: delete\n  operationId: DeleteSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rdb/v1/regions/{region}/snapshots/{snapshot_id}/create-instance\n  method: post\n  operationId: CreateInstanceFromSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /iam/v1alpha1/api-keys\n  method: get\n  operationId: ListAPIKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/api-keys\n  method: post\n  operationId: CreateAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/api-keys/{access_key}\n  method: get\n  operationId: GetAPIKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/api-keys/{access_key}\n  method: patch\n  operationId: UpdateAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/api-keys/{access_key}\n  method: delete\n  operationId: DeleteAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/applications\n  method: get\n  operationId: ListApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/applications\n  method: post\n  operationId: CreateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/applications/{application_id}\n  method: get\n  operationId: GetApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/applications/{application_id}\n  method: patch\n  operationId: UpdateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/applications/{application_id}\n  method: delete\n  operationId: DeleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/check-permissions\n  method: post\n  operationId: CheckPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/grace-periods\n  method: get\n  operationId: ListGracePeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/groups\n  method: get\n  operationId: ListGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/groups\n\
  \  method: post\n  operationId: CreateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/groups/{group_id}\n  method: get\n  operationId: GetGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/groups/{group_id}\n  method: patch\n  operationId: UpdateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/groups/{group_id}\n  method: delete\n  operationId: DeleteGroup\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/groups/{group_id}/add-member\n  method: post\n  operationId: AddGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/groups/{group_id}/add-members\n  method: post\n  operationId: AddGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /iam/v1alpha1/groups/{group_id}/members\n  method: put\n  operationId: SetGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/groups/{group_id}/remove-member\n  method: post\n  operationId: RemoveGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/jwts\n  method: get\n  operationId: ListJWTs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/jwts/{jti}\n\
  \  method: get\n  operationId: GetJWT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/jwts/{jti}\n  method: delete\n  operationId: DeleteJWT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/logs\n  method: get\n  operationId: ListLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/logs/{log_id}\n  method: get\n  operationId: GetLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/organizations/{organization_id}\n\
  \  method: get\n  operationId: GetOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/organizations/{organization_id}/alias\n  method: put\n  operationId: SetOrganizationAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/organizations/{organization_id}/login-methods\n  method: patch\n  operationId: UpdateOrganizationLoginMethods\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /iam/v1alpha1/organizations/{organization_id}/saml\n  method: get\n  operationId: GetOrganizationSaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/organizations/{organization_id}/saml\n  method: post\n  operationId: EnableOrganizationSaml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/organizations/{organization_id}/security-settings\n  method: get\n  operationId: GetOrganizationSecuritySettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/organizations/{organization_id}/security-settings\n \
  \ method: patch\n  operationId: UpdateOrganizationSecuritySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/permission-sets\n  method: get\n  operationId: ListPermissionSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/policies\n  method: get\n  operationId: ListPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/policies\n  method: post\n  operationId: CreatePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/policies/{policy_id}\n  method: get\n  operationId: GetPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/policies/{policy_id}\n  method: patch\n  operationId: UpdatePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/policies/{policy_id}\n  method: delete\n  operationId: DeletePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/policies/{policy_id}/clone\n  method: post\n  operationId: ClonePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v1alpha1/quota\n  method: get\n  operationId: ListQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/quota/{quotum_name}\n  method: get\n  operationId: GetQuotum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iam/v1alpha1/rules\n  method: get\n \n\n# --- truncated at\
  \ 32 KB (131 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/agentic-access/scaleway-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/agentic-access/scaleway-agentic-access.yml
summary_line: 419 operations · 257 acting · 10 human-in-the-loop
tags:
- AI
- Cloud Computing
- Containers
- Database
- European Cloud
- Infrastructure
- Kubernetes
- Serverless
- Storage
---
