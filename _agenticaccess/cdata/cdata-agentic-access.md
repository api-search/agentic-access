---
acting_count: 45
action_class_counts:
  acting: 45
  connected: 31
api_specs:
- filename: cdata-mcp-api-openapi.yml
  format: yaml
  label: CData Connect AI MCP Server
  slug: mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-mcp-api-openapi.yml
- filename: cdata-account-api-openapi.yml
  format: yaml
  label: CData Account API
  slug: cdata-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-account-api-openapi.yml
- filename: cdata-cache-api-openapi.yml
  format: yaml
  label: CData Cache API
  slug: cdata-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-cache-api-openapi.yml
- filename: cdata-connection-api-openapi.yml
  format: yaml
  label: CData Connection API
  slug: cdata-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-connection-api-openapi.yml
- filename: cdata-data-explorer-api-openapi.yml
  format: yaml
  label: CData Data Explorer API
  slug: cdata-data-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-data-explorer-api-openapi.yml
- filename: cdata-job-api-openapi.yml
  format: yaml
  label: CData Job API
  slug: cdata-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-job-api-openapi.yml
- filename: cdata-jobs-api-openapi.yml
  format: yaml
  label: CData Jobs API
  slug: cdata-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-jobs-api-openapi.yml
- filename: cdata-log-api-openapi.yml
  format: yaml
  label: CData Log API
  slug: cdata-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-log-api-openapi.yml
- filename: cdata-metadata-api-openapi.yml
  format: yaml
  label: CData Metadata API
  slug: cdata-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-metadata-api-openapi.yml
- filename: cdata-query-api-openapi.yml
  format: yaml
  label: CData Query API
  slug: cdata-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-query-api-openapi.yml
- filename: cdata-service-accounts-api-openapi.yml
  format: yaml
  label: CData Service Accounts API
  slug: cdata-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-service-accounts-api-openapi.yml
- filename: cdata-users-api-openapi.yml
  format: yaml
  label: CData Users API
  slug: cdata-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-users-api-openapi.yml
- filename: cdata-odata-api-openapi.yml
  format: yaml
  label: CData O Data API
  slug: cdata-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-odata-api-openapi.yml
- filename: cdata-open-api-api-openapi.yml
  format: yaml
  label: CData Open API
  slug: cdata-open-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-open-api-api-openapi.yml
consequence_counts:
  read: 31
  safety-critical: 1
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Cdata Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /job/{jobId}/stop
operation_count: 76
overview: 'CData exposes 76 API operations that an AI agent could call, of which 45 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 44 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CData
provider_slug: cdata
slug: cdata-agentic-access
source_filename: cdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/cdata-account-api-openapi.yml, openapi/cdata-cache-api-openapi.yml, openapi/cdata-connection-api-openapi.yml,\n  openapi/cdata-data-explorer-api-openapi.yml, openapi/cdata-job-api-openapi.yml, openapi/cdata-jobs-api-openapi.yml,\n  openapi/cdata-log-api-openapi.yml, openapi/cdata-mcp-api-openapi.yml, openapi/cdata-metadata-api-openapi.yml,\n  openapi/cdata-odata-api-openapi.yml, openapi/cdata-open-api-api-openapi.yml, openapi/cdata-query-api-openapi.yml,\n  openapi/cdata-service-accounts-api-openapi.yml, openapi/cdata-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 76\n  by_action_class:\n    connected: 31\n    acting: 45\n  by_consequence:\n    read: 31\n    write:\
  \ 44\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /poweredby/account/list\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poweredby/account/{accountIdOrExternalId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poweredby/account/create\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poweredby/account/update/{subAccountId}\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poweredby/account/delete/{id}\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/cacheConnection\n  method: post\n  operationId: updateCacheConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/cacheConnection/formLink\n\
  \  method: post\n  operationId: generateCacheConnectionURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poweredby/connection/create\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poweredby/connection/list\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poweredby/sources/list\n  method: get\n  operationId: listDataSources\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poweredby/connection/edit/{connectionId}\n  method: post\n  operationId: editConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poweredby/connection/delete/{id}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poweredby/{connectionId}/metadata\n  method: delete\n  operationId: clearConnectionMetadata\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poweredby/dataExplorer\n  method: post\n  operationId: generateDataExplorerURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/list\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /job/create\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/{jobId}/update\n  method: put\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/{jobId}/delete\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/{jobId}/run\n  method: post\n  operationId: runJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/{jobId}/stop\n  method: post\n  operationId: stopJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /poweredby/jobs\n  method: post\n  operationId: generateJobsURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /log/query/list\n  method: post\n  operationId: listQueryLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /log/query/get/{queryId}\n  method: get\n  operationId: getQueryLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /log/audit/list\n  method: post\n  operationId: listAuditLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: postMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/connections/{connectionId}\n  method: post\n  operationId: postMcpConnectionsByConnectionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs\n  method: get\n  operationId: getCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas\n\
  \  method: get\n  operationId: getSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables\n  method: get\n  operationId: getTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /columns\n  method: get\n  operationId: getColumns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /primaryKeys\n  method: get\n  operationId: getPrimaryKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /importedKeys\n  method: get\n  operationId: getImportedKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /exportedKeys\n  method: get\n  operationId: getExportedKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indexes\n  method: get\n  operationId: getIndexes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /procedures\n  method: get\n  operationId: getProcedures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /procedureParameters\n  method: get\n  operationId: getProcedureParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspaceName}\n  method: get\n  operationId: getByWorkspaceName\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspaceName}/$metadata\n  method: get\n  operationId: getByWorkspaceName$metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspaceName}/{resourcePath}\n  method: get\n  operationId: getByWorkspaceNameByResourcePath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspaceName}/{resourcePath}\n  method: delete\n  operationId: deleteByWorkspaceNameByResourcePath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspaceName}/{resourcePath}\n\
  \  method: post\n  operationId: postByWorkspaceNameByResourcePath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspaceName}/{resourcePath}\n  method: patch\n  operationId: patchByWorkspaceNameByResourcePath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{version}/{workspaceName}\n  method: get\n  operationId: getByVersionByWorkspaceName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: post\n\
  \  operationId: postQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch\n  method: post\n  operationId: postBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exec\n  method: post\n  operationId: postExec\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts\n\
  \  method: post\n  operationId: createServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts\n  method: get\n  operationId: listServiceAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:service-accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-accounts/{id}\n  method: get\n  operationId: getServiceAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:service-accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-accounts/{id}\n  method: patch\n  operationId:\
  \ updateServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts/{id}\n  method: delete\n  operationId: deleteServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts/{id}/roles\n  method: post\n  operationId: assignServiceAccountRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts/{id}/roles\n  method: get\n  operationId: listServiceAccountRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:service-accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-accounts/{id}/roles/{role_id}\n  method: delete\n  operationId: removeServiceAccountRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts/{id}/permissions\n  method: post\n  operationId: assignServiceAccountPermission\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts/{id}/permissions\n  method: get\n  operationId: listServiceAccountPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:service-accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-accounts/{id}/permissions/{permission_id}\n  method: delete\n  operationId: removeServiceAccountPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts/{id}/workspaces/{workspace_id}/roles\n  method: post\n  operationId: assignServiceAccountWorkspaceRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-accounts/{id}/workspaces/{workspace_id}/roles\n  method: get\n  operationId: listServiceAccountWorkspaceRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:service-accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-accounts/{id}/workspaces/{workspace_id}/roles/{role_id}\n  method: delete\n  operationId: removeServiceAccountWorkspaceRole\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:service-accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:users:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/batch\n  method: post\n  operationId:\
  \ batchCreateUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:users:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method:\
  \ delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/roles\n  method: post\n  operationId: assignUserRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/roles\n  method: get\n  operationId: listUserRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:users:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /users/{id}/roles/{role_id}\n  method: delete\n  operationId: removeUserRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/permissions\n  method: post\n  operationId: assignUserPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/permissions\n  method: get\n  operationId: listUserPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   scope:\n    - management:users:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/permissions/{permission_id}\n  method: delete\n  operationId: removeUserPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/workspaces/{workspace_id}/roles\n  method: post\n  operationId: assignUserWorkspaceRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/workspaces/{workspace_id}/roles\n  method:\
  \ get\n  operationId: listUserWorkspaceRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - management:users:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/workspaces/{workspace_id}/roles/{role_id}\n  method: delete\n  operationId: removeUserWorkspaceRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - management:users:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/agentic-access/cdata-agentic-access.yml
summary_line: 76 operations · 45 acting · 1 human-in-the-loop
tags:
- Data
- Data Access
- Data Connectivity
- Database
- NoSQL
- SQL
---
