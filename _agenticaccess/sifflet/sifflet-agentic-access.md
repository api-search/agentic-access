---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 28
api_specs:
- filename: sifflet-assets-api-openapi.yml
  format: yaml
  label: Sifflet Assets API
  slug: sifflet-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-assets-api-openapi.yml
- filename: sifflet-calendars-api-openapi.yml
  format: yaml
  label: Sifflet Calendars API
  slug: sifflet-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-calendars-api-openapi.yml
- filename: sifflet-credentials-api-openapi.yml
  format: yaml
  label: Sifflet Credentials API
  slug: sifflet-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-credentials-api-openapi.yml
- filename: sifflet-dbt-integration-api-openapi.yml
  format: yaml
  label: Sifflet dbt integration API
  slug: sifflet-dbt-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-dbt-integration-api-openapi.yml
- filename: sifflet-declarative-assets-and-lineage-api-openapi.yml
  format: yaml
  label: Sifflet Declarative Assets and Lineage API
  slug: sifflet-declarative-assets-and-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-declarative-assets-and-lineage-api-openapi.yml
- filename: sifflet-domains-api-openapi.yml
  format: yaml
  label: Sifflet Domains API
  slug: sifflet-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-domains-api-openapi.yml
- filename: sifflet-external-catalog-api-openapi.yml
  format: yaml
  label: Sifflet External Catalog API
  slug: sifflet-external-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-external-catalog-api-openapi.yml
- filename: sifflet-notification-rules-api-openapi.yml
  format: yaml
  label: Sifflet Notification Rules API
  slug: sifflet-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-notification-rules-api-openapi.yml
- filename: sifflet-rule-api-openapi.yml
  format: yaml
  label: Sifflet Rule API
  slug: sifflet-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-rule-api-openapi.yml
- filename: sifflet-rule-run-api-openapi.yml
  format: yaml
  label: Sifflet Rule Run API
  slug: sifflet-rule-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-rule-run-api-openapi.yml
- filename: sifflet-sources-deprecated-api-openapi.yml
  format: yaml
  label: Sifflet Sources (deprecated) API
  slug: sifflet-sources-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-sources-deprecated-api-openapi.yml
- filename: sifflet-sources-v2-api-openapi.yml
  format: yaml
  label: Sifflet Sources (v2) API
  slug: sifflet-sources-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-sources-v2-api-openapi.yml
- filename: sifflet-teams-api-openapi.yml
  format: yaml
  label: Sifflet Teams API
  slug: sifflet-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-teams-api-openapi.yml
- filename: sifflet-users-api-openapi.yml
  format: yaml
  label: Sifflet Users API
  slug: sifflet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-users-api-openapi.yml
- filename: sifflet-workspace-api-openapi.yml
  format: yaml
  label: Sifflet Workspace API
  slug: sifflet-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-workspace-api-openapi.yml
consequence_counts:
  read: 28
  safety-critical: 1
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Sifflet Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/users/{id}/reset-password
operation_count: 67
overview: 'Sifflet exposes 67 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 38 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sifflet
provider_slug: sifflet
slug: sifflet-agentic-access
source_filename: sifflet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/sifflet-backend-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 67\n  by_action_class:\n    acting: 39\n    connected: 28\n  by_consequence:\n    write: 38\n    read: 28\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/assets\n  method: patch\n  operationId: publicEditAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assets/get-asset-with-uri\n  method: post\n  operationId: publicGetAsset\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/search\n  method: post\n  operationId: publicGetAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/sync\n  method: post\n  operationId: publicSyncAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assets/{name}\n  method: delete\n  operationId: publicDeleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calendars\n  method: get\n  operationId: publicGetCalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendars\n  method: post\n  operationId: publicCreateCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calendars/{id}\n  method: delete\n  operationId: publicDeleteCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/calendars/{id}\n  method: get\n  operationId: publicGetCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendars/{id}\n  method: patch\n  operationId: publicUpdateCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials\n  method: get\n  operationId: publicGetAllCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credentials\n  method: post\n  operationId: publicCreateCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/{name}\n  method: delete\n  operationId: publicDeleteCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/{name}\n  method: get\n  operationId: publicGetCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credentials/{name}\n  method: patch\n  operationId: publicUpdateCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains\n  method: get\n  operationId: publicGetDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains\n  method: post\n  operationId: publicCreateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}\n  method: delete\n  operationId: publicDeleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/domains/{id}\n  method: get\n  operationId: publicGetDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{id}\n  method: patch\n  operationId: publicUpdateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external-catalog/import\n  method: post\n  operationId: publicImportExternalCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/metadata/dbt/{projectName}/{target}\n\
  \  method: post\n  operationId: uploadDbtMetadataFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification-rules\n  method: get\n  operationId: publicGetNotificationRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification-rules\n  method: post\n  operationId: publicCreateNotificationRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification-rules/{id}\n  method: delete\n  operationId:\
  \ publicDeleteNotificationRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification-rules/{id}\n  method: get\n  operationId: publicGetNotificationRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notification-rules/{id}\n  method: patch\n  operationId: publicUpdateNotificationRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules\n  method: get\n  operationId: getAllRule\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/_all-as-code\n  method: get\n  operationId: getAllMonitorsAsCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/runs/{runId}/decrypt\n  method: get\n  operationId: decryptRuleRunGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/{id}/_run\n  method: post\n  operationId: siffletRuleManualRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules/{id}/decrypt\n  method: get\n\
  \  operationId: decryptRuleGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/{id}/details\n  method: get\n  operationId: getSiffletRuleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/{id}/info\n  method: get\n  operationId: getSiffletRuleInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/{id}/overview\n  method: get\n  operationId: getSiffletRuleOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/{id}/runs\n  method: get\n  operationId: getSiffletRuleRuns\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules/{id}/runs/{runId}\n  method: get\n  operationId: getSiffletRuleRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources\n  method: post\n  operationId: publicCreateSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/search\n  method: post\n  operationId: publicGetSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources/test-connection\n  method: post\n  operationId: testSourceConnection\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/{id}\n  method: delete\n  operationId: publicDeleteSourceById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/{id}\n  method: get\n  operationId: publicGetSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources/{id}\n  method: patch\n  operationId: publicEditSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources/{id}/run\n  method: post\n  operationId: publicSourceIngestionManualRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/teams\n  method: get\n  operationId: publicGetTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teams\n  method: post\n  operationId: publicCreateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/teams/{id}\n  method: delete\n  operationId: publicDeleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/teams/{id}\n  method: get\n  operationId: publicGetTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teams/{id}\n  method: patch\n  operationId: publicUpdateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/users\n  method: get\n  operationId: publicGetUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: post\n  operationId: publicCreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{id}\n  method: delete\n  operationId: publicDeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{id}\n  method: get\n  operationId: publicGetUser\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{id}\n  method: patch\n  operationId: publicUpdateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{id}/reset-password\n  method: post\n  operationId: publicResetUserPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/sources\n  method: get\n  operationId: publicGetSourcesV2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sources\n  method: post\n  operationId: publicCreateSourceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/run-subsource\n  method: post\n  operationId: publicRunSubsourceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/test-connection\n  method: post\n  operationId: publicTestSourceConnectionV2\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/test-subsource-connection\n  method: post\n  operationId: publicTestSubsourceConnectionV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/test-subsource-connection-by-uri\n  method: post\n  operationId: publicTestSubsourceConnectionByUriV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/sources/{id}\n  method: delete\n  operationId: publicDeleteSourceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/{id}\n  method: get\n  operationId: publicGetSourceV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sources/{id}\n  method: patch\n  operationId: publicEditSourceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/{id}/run\n  method: post\n  operationId: publicRunSourceV2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/{id}/schemas\n  method: get\n  operationId: publicGetSourceSchemaList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sources/{id}/test-connection\n  method: post\n  operationId: publicTestExistingSourceConnectionV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/agentic-access/sifflet-agentic-access.yml
summary_line: 67 operations · 39 acting · 1 human-in-the-loop
tags:
- Company
- Data Analytics
- Data Observability
- Data Quality
- Data Catalog
- Data Lineage
- Data Governance
- Monitoring
- Metadata
- AI Agents
---
