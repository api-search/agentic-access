---
acting_count: 228
action_class_counts:
  acting: 228
  connected: 263
api_specs:
- filename: thingsboard-devices-openapi.yml
  format: yaml
  label: ThingsBoard Devices API
  slug: thingsboard-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-devices-openapi.yml
- filename: thingsboard-assets-openapi.yml
  format: yaml
  label: ThingsBoard Assets API
  slug: thingsboard-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-assets-openapi.yml
- filename: thingsboard-telemetry-openapi.yml
  format: yaml
  label: ThingsBoard Telemetry API
  slug: thingsboard-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-telemetry-openapi.yml
- filename: thingsboard-alarms-openapi.yml
  format: yaml
  label: ThingsBoard Alarms API
  slug: thingsboard-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-alarms-openapi.yml
- filename: thingsboard-rule-engine-openapi.yml
  format: yaml
  label: ThingsBoard Rule Engine API
  slug: thingsboard-rule-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-rule-engine-openapi.yml
- filename: thingsboard-rpc-openapi.yml
  format: yaml
  label: ThingsBoard RPC API
  slug: thingsboard-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-rpc-openapi.yml
- filename: thingsboard-dashboards-openapi.yml
  format: yaml
  label: ThingsBoard Dashboards API
  slug: thingsboard-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-dashboards-openapi.yml
- filename: thingsboard-auth-openapi.yml
  format: yaml
  label: ThingsBoard Authentication API
  slug: thingsboard-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-auth-openapi.yml
- filename: thingsboard-tenants-openapi.yml
  format: yaml
  label: ThingsBoard Tenants and Customers API
  slug: thingsboard-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-tenants-openapi.yml
- filename: thingsboard-admin-openapi.yml
  format: yaml
  label: ThingsBoard Admin API
  slug: thingsboard-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-admin-openapi.yml
- filename: thingsboard-notifications-openapi.yml
  format: yaml
  label: ThingsBoard Notifications API
  slug: thingsboard-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-notifications-openapi.yml
- filename: thingsboard-edge-openapi.yml
  format: yaml
  label: ThingsBoard Edge API
  slug: thingsboard-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-edge-openapi.yml
- filename: thingsboard-mobile-openapi.yml
  format: yaml
  label: ThingsBoard Mobile App API
  slug: thingsboard-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-mobile-openapi.yml
- filename: thingsboard-lwm2m-openapi.yml
  format: yaml
  label: ThingsBoard LwM2M API
  slug: thingsboard-lwm2m-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-lwm2m-openapi.yml
- filename: thingsboard-ai-openapi.yml
  format: yaml
  label: ThingsBoard AI API
  slug: thingsboard-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/openapi/thingsboard-ai-openapi.yml
consequence_counts:
  read: 263
  safety-critical: 226
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 226
kind: agentic-access
layout: agentic-access
method: generated
name: Thingsboard Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/2fa/account/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/2fa/account/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/2fa/account/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/2fa/account/config/generate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/2fa/account/config/submit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/2fa/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/autoCommitSettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/admin/autoCommitSettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/jwtSettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/repositorySettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/admin/repositorySettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/repositorySettings/checkAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/securitySettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/settings/testMail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/admin/settings/testSms
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/model
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/model/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/ai/model/{modelUuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/alarm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/alarm/{alarmId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/alarm/{alarmId}/ack
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/alarm/{alarmId}/assign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/alarm/{alarmId}/assign/{assigneeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/alarm/{alarmId}/clear
operation_count: 491
overview: 'ThingsBoard exposes 491 API operations that an AI agent could call, of which 228 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 263 read, 2 write, and 226 safety-critical.


  226 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ThingsBoard
provider_slug: thingsboard
slug: thingsboard-agentic-access
source_filename: thingsboard-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/thingsboard-admin-openapi.yml, openapi/thingsboard-ai-openapi.yml, openapi/thingsboard-alarms-openapi.yml,\n  openapi/thingsboard-assets-openapi.yml, openapi/thingsboard-auth-openapi.yml, openapi/thingsboard-dashboards-openapi.yml,\n  openapi/thingsboard-devices-openapi.yml, openapi/thingsboard-edge-openapi.yml, openapi/thingsboard-lwm2m-openapi.yml,\n  openapi/thingsboard-mobile-openapi.yml, openapi/thingsboard-notifications-openapi.yml, openapi/thingsboard-rpc-openapi.yml,\n  openapi/thingsboard-rule-engine-openapi.yml, openapi/thingsboard-telemetry-openapi.yml, openapi/thingsboard-tenants-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 491\n  by_action_class:\n    connected:\
  \ 263\n    acting: 228\n  by_consequence:\n    read: 263\n    safety-critical: 226\n    write: 2\n  human_in_the_loop_required: 226\noperations:\n- path: /api/queues\n  method: get\n  operationId: getTenantQueuesByServiceType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/queues\n  method: post\n  operationId: saveQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/mobile/qr/settings\n  method: get\n  operationId: getQrCodeSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mobile/qr/settings\n\
  \  method: post\n  operationId: saveQrCodeSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/job/{id}/reprocess\n  method: post\n  operationId: reprocessJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/job/{id}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/events/{entityType}/{entityId}\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/events/{entityType}/{entityId}\n  method: post\n  operationId: getEvents_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/events/{entityType}/{entityId}/clear\n  method: post\n  operationId: clearEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/settings\n  method: post\n  operationId: saveAdminSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/settings/testSms\n  method: post\n  operationId: sendTestSms\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/settings/testMail\n\
  \  method: post\n  operationId: sendTestMail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/securitySettings\n  method: get\n  operationId: getSecuritySettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/securitySettings\n  method: post\n  operationId: saveSecuritySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n-\
  \ path: /api/admin/repositorySettings\n  method: get\n  operationId: getRepositorySettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/repositorySettings\n  method: post\n  operationId: saveRepositorySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/repositorySettings\n  method: delete\n  operationId: deleteRepositorySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/admin/repositorySettings/checkAccess\n  method: post\n  operationId: checkRepositoryAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/jwtSettings\n  method: get\n  operationId: getJwtSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/jwtSettings\n  method: post\n  operationId: saveJwtSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/autoCommitSettings\n  method: get\n  operationId: getAutoCommitSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/autoCommitSettings\n  method: post\n  operationId: saveAutoCommitSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/admin/autoCommitSettings\n  method: delete\n  operationId: deleteAutoCommitSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/usage\n  method: get\n  operationId: getTenantUsageInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/queues/{queueId}\n  method: get\n  operationId: getQueueById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/queues/{queueId}\n  method: delete\n  operationId: deleteQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/queues/name/{queueName}\n\
  \  method: get\n  operationId: getQueueByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/queueStats\n  method: get\n  operationId: getQueueStatsByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/queueStats/{queueStatsId}\n  method: get\n  operationId: getQueueStatsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/noauth/qr\n  method: get\n  operationId: getApplicationRedirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/noauth/qr/{secret}\n  method: get\n  operationId: getUserTokenByMobileSecret\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mobile/qr/deepLink\n  method: get\n  operationId: getMobileAppDeepLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mail/config/template\n  method: get\n  operationId: getClientRegistrationTemplates_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs\n  method: get\n  operationId: getJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/job/{id}\n  method: get\n  operationId: getJobById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/job/{id}\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/events/{entityType}/{entityId}/{eventType}\n  method: get\n  operationId: getEvents_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/audit/logs\n  method: get\n  operationId: getAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/audit/logs/user/{userId}\n  method: get\n  operationId: getAuditLogsByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/audit/logs/entity/{entityType}/{entityId}\n  method: get\n  operationId: getAuditLogsByEntityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/audit/logs/customer/{customerId}\n  method: get\n  operationId: getAuditLogsByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/updates\n  method: get\n  operationId: checkUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/systemInfo\n  method: get\n  operationId: getSystemInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/admin/settings/{key}\n  method: get\n  operationId: getAdminSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/repositorySettings/info\n  method: get\n  operationId: getRepositorySettingsInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/repositorySettings/exists\n  method: get\n  operationId: repositorySettingsExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/mail/oauth2/loginProcessingUrl\n  method: get\n  operationId: getMailProcessingUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/admin/mail/oauth2/code\n  method: get\n  operationId: codeProcessingUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/mail/oauth2/authorize\n  method: get\n  operationId: getAuthorizationUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/featuresInfo\n  method: get\n  operationId: getFeaturesInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/autoCommitSettings/exists\n  method: get\n  operationId: autoCommitSettingsExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/assetlinks.json\n  method: get\n \
  \ operationId: getAssetLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/apple-app-site-association\n  method: get\n  operationId: getAppleAppSiteAssociation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trendz/settings\n  method: get\n  operationId: getTrendzSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trendz/settings\n  method: post\n  operationId: saveTrendzSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/ai/model\n  method: get\n  operationId: getAiModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/model\n  method: post\n  operationId: saveAiModel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/model/chat\n  method: post\n  operationId: sendChatRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /api/ai/model/{modelUuid}\n  method: get\n  operationId: getAiModelById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/model/{modelUuid}\n  method: delete\n  operationId: deleteAiModelById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/alarm\n  method: post\n  operationId: saveAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /api/alarm/{alarmId}/comment\n  method: get\n  operationId: getAlarmComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alarm/{alarmId}/comment\n  method: post\n  operationId: saveAlarmComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/alarm/{alarmId}/clear\n  method: post\n  operationId: clearAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/alarm/{alarmId}/assign/{assigneeId}\n  method: post\n  operationId: assignAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/alarm/{alarmId}/ack\n  method: post\n  operationId: ackAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/alarms\n  method: get\n  operationId: getAllAlarmsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/alarm/{entityType}/{entityId}\n  method: get\n  operationId: getAlarmsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alarms\n  method: get\n  operationId: getAllAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alarm/{entityType}/{entityId}\n  method: get\n  operationId: getAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alarm/{alarmId}\n  method: get\n  operationId: getAlarmById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alarm/{alarmId}\n  method: delete\n  operationId:\
  \ deleteAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/alarm/types\n  method: get\n  operationId: getAlarmTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alarm/info/{alarmId}\n  method: get\n  operationId: getAlarmInfoById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alarm/highestSeverity/{entityType}/{entityId}\n  method: get\n  operationId: getHighestAlarmSeverity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/alarm/{alarmId}/comment/{commentId}\n  method: delete\n  operationId: deleteAlarmComment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/alarm/{alarmId}/assign\n  method: delete\n  operationId: unassignAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/relation\n  method: post\n  operationId: saveRelationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/relation\n  method: delete\n  operationId: deleteRelationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/relations\n  method: get\n  operationId: findByTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/relations\n  method: post\n  operationId: findByQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/relations\n  method: delete\n  operationId: deleteRelations\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/relations/info\n  method: get\n  operationId: findInfoByTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/relations/info\n  method: post\n  operationId: findInfoByQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/relation\n  method: get\n  operationId: getRelation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/relation\n  method: post\n  operationId: saveRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/relation\n  method: delete\n  operationId: deleteRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/entityViews\n  method: get\n  operationId: getEntityViewsByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/entityViews\n  method: post\n  operationId: findByQuery_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/entityView\n  method: post\n  operationId: saveEntityView\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/edge/{edgeId}/entityView/{entityViewId}\n  method: post\n  operationId: assignEntityViewToEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/edge/{edgeId}/entityView/{entityViewId}\n  method: delete\n  operationId: unassignEntityViewFromEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/edge/{edgeId}/asset/{assetId}\n  method: post\n  operationId: assignAssetToEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/edge/{edgeId}/asset/{assetId}\n  method: delete\n  operationId: unassignAssetFromEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/customer/{customerId}/entityView/{entityViewId}\n  method: post\n  operationId: assignEntityViewToCustomer\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/customer/{customerId}/asset/{assetId}\n  method: post\n  operationId: assignAssetToCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/customer/public/entityView/{entityViewId}\n  method: post\n  operationId: assignEntityViewToPublicCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/customer/public/asset/{assetId}\n  method: post\n  operationId: assignAssetToPublicCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/assets\n  method: get\n  operationId: getAssetsByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/assets\n  method: post\n  operationId: findByQuery_4\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/asset\n  method: post\n  operationId: saveAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/assetProfile\n  method: post\n  operationId: saveAssetProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/assetProfile/{assetProfileId}/default\n  method: post\n  operationId:\
  \ setDefaultAssetProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/asset/bulk_import\n  method: post\n  operationId: processAssetsBulkImport\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tenant/entityViews\n  method: get\n  operationId: getTenantEntityViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/entityViewInfos\n\
  \  method: get\n  operationId: getTenantEntityViewInfos\n  x\n\n# --- truncated at 32 KB (145 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/agentic-access/thingsboard-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingsboard/refs/heads/main/agentic-access/thingsboard-agentic-access.yml
summary_line: 491 operations · 228 acting · 226 human-in-the-loop
tags:
- IoT
- Internet of Things
- Device Management
- Telemetry
- Open Source
- Apache 2.0
- MQTT
- LwM2M
- CoAP
- Rule Engine
- Dashboards
- Edge
- Multi-tenant
- Java
- Spring
---
