---
acting_count: 218
action_class_counts:
  acting: 218
  connected: 120
api_specs:
- filename: antfly-ai-api-openapi.yml
  format: yaml
  label: Antfly AI API
  slug: antfly-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-ai-api-openapi.yml
- filename: antfly-cluster-management-api-openapi.yml
  format: yaml
  label: Antfly Cluster Management API
  slug: antfly-cluster-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-cluster-management-api-openapi.yml
- filename: antfly-data-operations-api-openapi.yml
  format: yaml
  label: Antfly Data Operations API
  slug: antfly-data-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-data-operations-api-openapi.yml
- filename: antfly-documents-api-openapi.yml
  format: yaml
  label: Antfly Documents API
  slug: antfly-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-documents-api-openapi.yml
- filename: antfly-index-management-api-openapi.yml
  format: yaml
  label: Antfly Index Management API
  slug: antfly-index-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-index-management-api-openapi.yml
- filename: antfly-inference-api-openapi.yml
  format: yaml
  label: Antfly Inference API
  slug: antfly-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-inference-api-openapi.yml
- filename: antfly-installed-api-openapi.yml
  format: yaml
  label: Antfly Installed API
  slug: antfly-installed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-installed-api-openapi.yml
- filename: antfly-memory-api-openapi.yml
  format: yaml
  label: Antfly Memory API
  slug: antfly-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-memory-api-openapi.yml
- filename: antfly-ml-api-openapi.yml
  format: yaml
  label: Antfly Ml API
  slug: antfly-ml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-ml-api-openapi.yml
- filename: antfly-models-api-openapi.yml
  format: yaml
  label: Antfly Models API
  slug: antfly-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-models-api-openapi.yml
- filename: antfly-packages-api-openapi.yml
  format: yaml
  label: Antfly Packages API
  slug: antfly-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-packages-api-openapi.yml
- filename: antfly-permission-api-openapi.yml
  format: yaml
  label: Antfly Permission API
  slug: antfly-permission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-permission-api-openapi.yml
- filename: antfly-personal-connections-api-openapi.yml
  format: yaml
  label: Antfly Personal Connections API
  slug: antfly-personal-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-personal-connections-api-openapi.yml
- filename: antfly-query-operations-api-openapi.yml
  format: yaml
  label: Antfly Query Operations API
  slug: antfly-query-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-query-operations-api-openapi.yml
- filename: antfly-resolver-curation-api-openapi.yml
  format: yaml
  label: Antfly Resolver Curation API
  slug: antfly-resolver-curation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-resolver-curation-api-openapi.yml
- filename: antfly-role-api-openapi.yml
  format: yaml
  label: Antfly Role API
  slug: antfly-role-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-role-api-openapi.yml
- filename: antfly-rowfilter-api-openapi.yml
  format: yaml
  label: Antfly Row Filter API
  slug: antfly-rowfilter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-rowfilter-api-openapi.yml
- filename: antfly-table-management-api-openapi.yml
  format: yaml
  label: Antfly Table Management API
  slug: antfly-table-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-table-management-api-openapi.yml
- filename: antfly-user-api-openapi.yml
  format: yaml
  label: Antfly User API
  slug: antfly-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-user-api-openapi.yml
- filename: antfly-api-key-api-openapi.yml
  format: yaml
  label: Antfly API Key API
  slug: antfly-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-api-key-api-openapi.yml
consequence_counts:
  physical: 2
  read: 120
  safety-critical: 5
  write: 211
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Antfly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/v1/extract/jobs/{job_id}/resume
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/v1/read/jobs/{job_id}/resume
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /db/v1/tables/{tableName}/repair/control-jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /extensions/v1/installed/{name}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /extensions/v1/installed/{name}/enable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /memory/v1/spaces/{space}/relationship-proposals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /memory/v1/spaces/{space}/relationship-proposals/{id}/verdict
operation_count: 338
overview: 'Antfly exposes 338 API operations that an AI agent could call, of which 218 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 120 read, 211 write, 2 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Antfly
provider_slug: antfly
slug: antfly-agentic-access
source_filename: antfly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/antfly-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 338\n  by_action_class:\n    connected: 120\n    acting: 218\n  by_consequence:\n    read: 120\n    write: 211\n    safety-critical: 5\n    physical: 2\n  human_in_the_loop_required: 5\noperations:\n- path: /db/v1/tables/{tableName}/lake/catalog\n  method: get\n  operationId: getLakeCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/lake/catalog\n  method: post\n  operationId: initializeLakeCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/lake/changes\n  method: post\n  operationId: ingestLakeChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/lake/maintenance\n  method: post\n  operationId: maintainLakeTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/lake/commits\n  method:\
  \ post\n  operationId: commitLakeCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/lake/commits/{commitId}\n  method: get\n  operationId: getLakeCommitOutcome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/cluster\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /db/v1/connections/chatgpt/authorize\n  method: post\n  operationId: authorizeChatGPT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/connections/chatgpt/attempts/{attempt_id}\n  method: get\n  operationId: getChatGPTAttempt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/connections/chatgpt/accounts\n  method: get\n  operationId: listChatGPTAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/connections/{connection_id}/chatgpt/models\n  method: get\n  operationId: listChatGPTModels\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/connections/{connection_id}/chatgpt/disconnect\n  method: post\n  operationId: disconnectChatGPT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/connections/{connection_id}/inference/{operation}\n  method: post\n  operationId: invokeInferenceConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/secrets\n  method: get\n  operationId: listSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/secrets/{key}\n  method: put\n  operationId: putSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/secrets/{key}\n  method: delete\n  operationId: deleteSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /db/v1/batch\n  method: post\n  operationId: multiBatchWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/indexes/{indexName}/graph-metrics/{metricName}:{action}\n  method: post\n  operationId: executeGraphMetricAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/databases/{databaseName}/namespaces/{namespaceName}/tables/{tableName}/indexes/{indexName}/graph-metrics/{metricName}:{action}\n  method: post\n  operationId: executeNamespaceTableGraphMetricAction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/commit\n  method: post\n  operationId: commitTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions\n  method: get\n  operationId: listTransactionSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/transactions/cleanup\n  method: post\n  operationId: cleanupTransactionSessions\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/begin\n  method: post\n  operationId: beginTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/{transaction_id}\n  method: get\n  operationId: getTransactionSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/transactions/{transaction_id}/stage\n  method: post\n  operationId: stageTransactionSession\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/{transaction_id}/read\n  method: post\n  operationId: stageTransactionRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/{transaction_id}/write\n  method: post\n  operationId: stageTransactionWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /db/v1/transactions/{transaction_id}/delete\n  method: post\n  operationId: stageTransactionDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/{transaction_id}/savepoints\n  method: post\n  operationId: createTransactionSavepoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/{transaction_id}/savepoints/{savepoint_id}/rollback\n  method: post\n  operationId: rollbackTransactionSavepoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/{transaction_id}/commit\n  method: post\n  operationId: commitTransactionSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/transactions/{transaction_id}/abort\n  method: post\n  operationId: abortTransactionSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/backup\n  method: post\n  operationId:\
  \ backup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/restore\n  method: post\n  operationId: restore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/restore/jobs\n  method: get\n  operationId: listRestoreJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/restore/jobs/{job_id}\n  method: get\n  operationId: getRestoreJob\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/restore/jobs/{job_id}\n  method: delete\n  operationId: cancelRestoreJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/backups\n  method: get\n  operationId: listBackups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/sql/connections\n  method: post\n  operationId: openSQLConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /db/v1/sql/connections/{connection_id}\n  method: delete\n  operationId: closeSQLConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/sql/prepared\n  method: post\n  operationId: prepareSQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/sql/prepared/{prepared_id}/execute\n  method: post\n  operationId: executePreparedSQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/sql/prepared/{prepared_id}\n  method: delete\n  operationId: closePreparedSQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/settings\n  method: post\n  operationId: administerSqlSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/store-roots/enroll\n  method: post\n  operationId: enrollStoreRoot\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/store-roots/enrollment-status\n  method: post\n  operationId: getStoreRootEnrollmentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/sql\n  method: post\n  operationId: executeSQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/query\n  method: post\n  operationId: globalQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/eval\n  method: post\n  operationId: evaluate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/agents/query-builder\n  method: post\n  operationId: queryBuilderAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/agents/retrieval\n  method: post\n  operationId: retrievalAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/agents/research\n  method: post\n  operationId: researchAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/agents/research/jobs\n  method: post\n  operationId: startResearchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/agents/research/jobs/{jobId}\n  method: get\n  operationId: getResearchJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /db/v1/agents/research/jobs/{jobId}/advance\n  method: post\n  operationId: advanceResearchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/agents/research/jobs/{jobId}/cancel\n  method: post\n  operationId: cancelResearchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables\n  method: get\n  operationId: listTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /db/v1/tables/{tableName}\n  method: post\n  operationId: createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}\n  method: delete\n  operationId: dropTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/query\n  method: post\n  operationId:\
  \ queryTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/constraints/status\n  method: get\n  operationId: getRelationalConstraintStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/constraints/repair\n  method: post\n  operationId: repairRelationalConstraints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/constraints/retry\n  method: post\n  operationId: retryRelationalConstraints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/constraints/retire\n  method: post\n  operationId: retireRelationalConstraints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/rows/query\n  method: post\n  operationId: queryRelationalRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/rows/mutate\n  method: post\n  operationId: mutateRelationalRows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/batch\n  method: post\n  operationId: batchWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/merge\n  method: post\n  operationId: linearMerge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/backup\n  method: post\n  operationId:\
  \ backupTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/restore\n  method: post\n  operationId: restoreTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/destination-authorization\n  method: post\n  operationId: reauthorizeTableDestinations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/schema\n  method: put\n  operationId: updateSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/schema\n  method: patch\n  operationId: patchSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/documents\n  method: post\n  operationId: scanKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/documents/{key}\n  method: get\n  operationId: lookupKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/documents/{key}/artifacts\n  method: get\n  operationId: listDocumentArtifactManifests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/artifacts\n  method: get\n  operationId: listArtifactEnrichments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/repair/issues\n  method: post\n  operationId: listTableRepairIssues\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/storage/migrations\n  method: post\n  operationId: createTableStorageMigration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/storage/migrations/{jobId}\n  method: get\n  operationId: getTableStorageMigration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/storage/migrations/{jobId}\n  method: post\n  operationId: advanceTableStorageMigration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/repair/run\n  method: post\n  operationId: runTableRepair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/repair/jobs\n  method: post\n  operationId: startTableRepairJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/repair/control-jobs\n\
  \  method: post\n  operationId: startTableRepairControlJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /db/v1/tables/{tableName}/repair/jobs/{jobId}\n  method: get\n  operationId: getTableRepairJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/repair/jobs/{jobId}/advance\n  method: post\n  operationId: advanceTableRepairJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /db/v1/tables/{tableName}/repair/jobs/{jobId}/cancel\n  method: post\n  operationId: cancelTableRepairJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/artifacts/{artifactName}/reprocess\n  method: post\n  operationId: reprocessDocumentArtifactRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/artifacts/{artifactName}/enrichment\n  method: put\n  operationId: putArtifactEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/artifacts/{artifactName}/enrichment\n  method: delete\n  operationId: deleteArtifactEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/artifacts/{artifactName}/reprocess-jobs\n  method: post\n  operationId: startDocumentArtifactReprocessJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/artifacts/{artifactName}/reprocess-jobs/{jobId}\n  method: get\n  operationId: getDocumentArtifactReprocessJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/artifacts/{artifactName}/reprocess-jobs/{jobId}/advance\n  method: post\n  operationId: advanceDocumentArtifactReprocessJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/artifacts/{artifactName}/reprocess-jobs/{jobId}/cancel\n  method: post\n  operationId: cancelDocumentArtifactReprocessJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/v1/tables/{tableName}/documents/{key}/artifacts/{artifactName}\n  method: get\n  operationId: getDocumentArtifactManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/v1/tables/{tableName}/documents/{key}/artifacts/{artifactName}/reprocess\n  method: post\n  operationId: reprocessDocumentArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (108 KB total) ---\n# Full source: https://artifacts.apis.io/antfly/agentic-access/antfly-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/antfly/agentic-access/antfly-agentic-access.yml
summary_line: 338 operations · 218 acting · 5 human-in-the-loop
tags:
- Artificial Intelligence
- Search
- Retrieval
- Vectors
- Hybrid
---
