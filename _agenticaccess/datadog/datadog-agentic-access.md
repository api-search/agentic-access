---
acting_count: 324
action_class_counts:
  acting: 324
  connected: 234
api_specs:
- filename: datadog-api-openapi.yml
  format: yaml
  label: Datadog API
  slug: datadog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-api-openapi.yml
- filename: datadog-metrics-openapi.yml
  format: yaml
  label: Datadog Metrics API
  slug: datadog-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-metrics-openapi.yml
- filename: datadog-logs-openapi.yml
  format: yaml
  label: Datadog Logs API
  slug: datadog-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-logs-openapi.yml
- filename: datadog-events-openapi.yml
  format: yaml
  label: Datadog Events API
  slug: datadog-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-events-openapi.yml
- filename: datadog-monitors-openapi.yml
  format: yaml
  label: Datadog Monitors API
  slug: datadog-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-monitors-openapi.yml
- filename: datadog-incidents-openapi.yml
  format: yaml
  label: Datadog Incidents API
  slug: datadog-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/openapi/datadog-incidents-openapi.yml
consequence_counts:
  physical: 22
  read: 234
  safety-critical: 4
  write: 298
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Datadog Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/logs/config/archives/{archive_id}/readers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/logs/config/restriction_queries/{restriction_query_id}/roles
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/roles/{role_id}/permissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/users/{user_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v2/apm/config/retention-filters-execution-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v2/app-builder/apps/{app_id}/deployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/app-builder/apps/{app_id}/deployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/ci/pipeline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/dora/deployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/dora/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/dora/incident
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/incidents/{incident_id}/relationships/integrations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v2/incidents/{incident_id}/relationships/integrations/{integration_metadata_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/incidents/{incident_id}/relationships/integrations/{integration_metadata_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/incidents/{incident_id}/relationships/todos
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v2/incidents/{incident_id}/relationships/todos/{todo_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/incidents/{incident_id}/relationships/todos/{todo_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/logs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/logs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v2/logs/config/archive-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/rum/applications/{app_id}/relationships/retention_filters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/sensitive-data-scanner/config
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/team/{team_id}/memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v2/team/{team_id}/memberships/{user_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/team/{team_id}/memberships/{user_id}
operation_count: 558
overview: 'Datadog exposes 558 API operations that an AI agent could call, of which 324 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 234 read, 298 write, 22 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Datadog
provider_slug: datadog
slug: datadog-agentic-access
source_filename: datadog-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/datadog-api-openapi.yml, openapi/datadog-events-openapi.yml, openapi/datadog-incidents-openapi.yml,\n  openapi/datadog-logs-openapi.yml, openapi/datadog-metrics-openapi.yml, openapi/datadog-monitors-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 558\n  by_action_class:\n    acting: 324\n    connected: 234\n  by_consequence:\n    write: 298\n    read: 234\n    physical: 22\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v2/actions/connections\n  method: post\n  operationId: CreateActionConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/actions/connections/{connection_id}\n  method: delete\n  operationId: DeleteActionConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/actions/connections/{connection_id}\n  method: get\n  operationId: GetActionConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/actions/connections/{connection_id}\n  method: patch\n  operationId: UpdateActionConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/agentless_scanning/accounts/aws\n  method: get\n  operationId: ListAwsScanOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/agentless_scanning/accounts/aws\n  method: post\n  operationId: CreateAwsScanOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/agentless_scanning/accounts/aws/{account_id}\n  method: delete\n  operationId: DeleteAwsScanOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/agentless_scanning/accounts/aws/{account_id}\n  method: patch\n  operationId: UpdateAwsScanOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/agentless_scanning/ondemand/aws\n  method: get\n  operationId: ListAwsOnDemandTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/agentless_scanning/ondemand/aws\n  method: post\n  operationId: CreateAwsOnDemandTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/agentless_scanning/ondemand/aws/{task_id}\n  method: get\n  operationId: GetAwsOnDemandTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/api_keys\n  method: get\n  operationId: ListAPIKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/api_keys\n  method: post\n  operationId: CreateAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v2/api_keys/{api_key_id}\n  method: delete\n  operationId: DeleteAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/api_keys/{api_key_id}\n  method: get\n  operationId: GetAPIKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/api_keys/{api_key_id}\n  method: patch\n  operationId: UpdateAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apicatalog/api\n\
  \  method: get\n  operationId: ListAPIs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apm_api_catalog_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/apicatalog/api/{id}\n  method: delete\n  operationId: DeleteOpenAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apm_api_catalog_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apicatalog/api/{id}/openapi\n  method: get\n  operationId: GetOpenAPI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apm_api_catalog_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/apicatalog/api/{id}/openapi\n  method: put\n  operationId: UpdateOpenAPI\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apm_api_catalog_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apicatalog/openapi\n  method: post\n  operationId: CreateOpenAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apm_api_catalog_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apm/config/metrics\n  method: get\n  operationId: ListSpansMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/apm/config/metrics\n  method: post\n  operationId: CreateSpansMetric\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apm/config/metrics/{metric_id}\n  method: delete\n  operationId: DeleteSpansMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apm/config/metrics/{metric_id}\n  method: get\n  operationId: GetSpansMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/apm/config/metrics/{metric_id}\n  method: patch\n  operationId: UpdateSpansMetric\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apm/config/retention-filters\n  method: get\n  operationId: ListApmRetentionFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/apm/config/retention-filters\n  method: post\n  operationId: CreateApmRetentionFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apm/config/retention-filters-execution-order\n  method: put\n  operationId: ReorderApmRetentionFilters\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apm/config/retention-filters/{filter_id}\n  method: delete\n  operationId: DeleteApmRetentionFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/apm/config/retention-filters/{filter_id}\n  method: get\n  operationId: GetApmRetentionFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/apm/config/retention-filters/{filter_id}\n\
  \  method: put\n  operationId: UpdateApmRetentionFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/app-builder/apps\n  method: delete\n  operationId: DeleteApps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/app-builder/apps\n  method: get\n  operationId: ListApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/app-builder/apps\n  method: post\n  operationId: CreateApp\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/app-builder/apps/{app_id}\n  method: delete\n  operationId: DeleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/app-builder/apps/{app_id}\n  method: get\n  operationId: GetApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/app-builder/apps/{app_id}\n  method: patch\n  operationId: UpdateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/app-builder/apps/{app_id}/deployment\n  method: delete\n  operationId: UnpublishApp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/app-builder/apps/{app_id}/deployment\n  method: post\n  operationId: PublishApp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/application_keys\n  method: get\n  operationId: ListApplicationKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/application_keys/{app_key_id}\n  method: delete\n  operationId: DeleteApplicationKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/application_keys/{app_key_id}\n  method: get\n  operationId: GetApplicationKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/application_keys/{app_key_id}\n  method: patch\n  operationId: UpdateApplicationKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/audit/events\n  method: get\n  operationId: ListAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/audit/events/search\n  method: post\n  operationId: SearchAuditLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authn_mappings\n  method: get\n  operationId: ListAuthNMappings\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authn_mappings\n  method: post\n  operationId: CreateAuthNMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authn_mappings/{authn_mapping_id}\n  method: delete\n  operationId: DeleteAuthNMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/authn_mappings/{authn_mapping_id}\n  method: get\n  operationId: GetAuthNMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/authn_mappings/{authn_mapping_id}\n  method: patch\n  operationId: UpdateAuthNMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases\n  method: get\n  operationId: SearchCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cases_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cases\n  method: post\n  operationId: CreateCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases/projects\n  method: get\n  operationId: GetProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cases_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cases/projects\n  method: post\n  operationId: CreateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases/projects/{project_id}\n  method: delete\n  operationId: DeleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases/projects/{project_id}\n  method: get\n  operationId: GetProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cases_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cases/{case_id}\n  method: get\n  operationId: GetCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cases_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cases/{case_id}/archive\n  method: post\n  operationId: ArchiveCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v2/cases/{case_id}/assign\n  method: post\n  operationId: AssignCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases/{case_id}/priority\n  method: post\n  operationId: UpdatePriority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases/{case_id}/status\n  method: post\n  operationId: UpdateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases/{case_id}/unarchive\n  method: post\n  operationId: UnarchiveCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cases/{case_id}/unassign\n  method: post\n  operationId: UnassignCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cases_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/catalog/entity\n  method:\
  \ get\n  operationId: ListCatalogEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apm_service_catalog_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/catalog/entity\n  method: post\n  operationId: UpsertCatalogEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apm_service_catalog_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/catalog/entity/{entity_id}\n  method: delete\n  operationId: DeleteCatalogEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apm_service_catalog_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/catalog/relation\n  method: get\n  operationId: ListCatalogRelation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apm_service_catalog_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/ci/pipeline\n  method: post\n  operationId: CreateCIAppPipelineEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/ci/pipelines/analytics/aggregate\n  method: post\n  operationId: AggregateCIAppPipelineEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ci_visibility_read\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/ci/pipelines/events\n  method: get\n  operationId: ListCIAppPipelineEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ci_visibility_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/ci/pipelines/events/search\n  method: post\n  operationId: SearchCIAppPipelineEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ci_visibility_read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/ci/tests/analytics/aggregate\n  method: post\n  operationId: AggregateCIAppTestEvents\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - ci_visibility_read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/ci/tests/events\n  method: get\n  operationId: ListCIAppTestEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ci_visibility_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/ci/tests/events/search\n  method: post\n  operationId: SearchCIAppTestEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ci_visibility_read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cloud_security_management/custom_frameworks\n\
  \  method: post\n  operationId: CreateCustomFramework\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - security_monitoring_rules_read\n    - security_monitoring_rules_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cloud_security_management/custom_frameworks/{handle}/{version}\n  method: delete\n  operationId: DeleteCustomFramework\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - security_monitoring_rules_read\n    - security_monitoring_rules_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cloud_security_management/custom_frameworks/{handle}/{version}\n\
  \  method: get\n  operationId: GetCustomFramework\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - security_monitoring_rules_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cloud_security_management/custom_frameworks/{handle}/{version}\n  method: put\n  operationId: UpdateCustomFramework\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - security_monitoring_rules_read\n    - security_monitoring_rules_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cloud_security_management/resource_filters\n  method: get\n  operationId: GetResourceEvaluationFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - security_monitoring_filters_read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cloud_security_management/resource_filters\n  method: put\n  operationId: UpdateResourceEvaluationFilters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - security_monitoring_filters_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/container_images\n  method: get\n  operationId: ListContainerImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/containers\n  method: get\n  operationId: ListContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cost/aws_cur_config\n  method:\
  \ get\n  operationId: ListCostAWSCURConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cloud_cost_management_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cost/aws_cur_config\n  method: post\n  operationId: CreateCostAWSCURConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/aws_cur_config/{cloud_account_id}\n  method: delete\n  operationId: DeleteCostAWSCURConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/aws_cur_config/{cloud_account_id}\n  method: patch\n  operationId: UpdateCostAWSCURConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/azure_uc_config\n  method: get\n  operationId: ListCostAzureUCConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cloud_cost_management_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cost/azure_uc_config\n  method: post\n  operationId: CreateCostAzureUCConfigs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/azure_uc_config/{cloud_account_id}\n  method: delete\n  operationId: DeleteCostAzureUCConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/azure_uc_config/{cloud_account_id}\n  method: patch\n  operationId: UpdateCostAzureUCConfigs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/budget\n  method: put\n  operationId: UpsertBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/budget/{budget_id}\n  method: delete\n  operationId: DeleteBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cost/budget/{budget_id}\n  method: get\n  operationId: GetBudget\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cloud_cost_management_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cost/budgets\n  method: get\n  operationId: ListBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cloud_cost_management_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cost/custom_costs\n  method: get\n  operationId: ListCustomCostsFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cloud_cost_management_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/cost/custom_costs\n  method: put\n  operationId: UploadCustomCostsFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cloud_cost_management_write\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: co\n\n# --- truncated at 32 KB (179 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/agentic-access/datadog-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/agentic-access/datadog-agentic-access.yml
summary_line: 558 operations · 324 acting · 4 human-in-the-loop
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
---
