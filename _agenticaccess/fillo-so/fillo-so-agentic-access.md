---
acting_count: 37
action_class_counts:
  acting: 37
  connected: 28
api_specs:
- filename: fillo-so-agents-api-openapi.yml
  format: yaml
  label: Fillo Agents API
  slug: fillo-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-agents-api-openapi.yml
- filename: fillo-so-credentials-api-openapi.yml
  format: yaml
  label: Fillo Credentials API
  slug: fillo-so-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-credentials-api-openapi.yml
- filename: fillo-so-deliveries-api-openapi.yml
  format: yaml
  label: Fillo Deliveries API
  slug: fillo-so-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-deliveries-api-openapi.yml
- filename: fillo-so-fillo-management-api-api-openapi.yml
  format: yaml
  label: Fillo Fillo Management API
  slug: fillo-so-fillo-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-fillo-management-api-api-openapi.yml
- filename: fillo-so-forms-api-openapi.yml
  format: yaml
  label: Fillo Forms API
  slug: fillo-so-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-forms-api-openapi.yml
- filename: fillo-so-insights-api-openapi.yml
  format: yaml
  label: Fillo Insights API
  slug: fillo-so-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-insights-api-openapi.yml
- filename: fillo-so-integrations-api-openapi.yml
  format: yaml
  label: Fillo Integrations API
  slug: fillo-so-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-integrations-api-openapi.yml
- filename: fillo-so-members-api-openapi.yml
  format: yaml
  label: Fillo Members API
  slug: fillo-so-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-members-api-openapi.yml
- filename: fillo-so-respondents-api-openapi.yml
  format: yaml
  label: Fillo Respondents API
  slug: fillo-so-respondents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-respondents-api-openapi.yml
- filename: fillo-so-responses-api-openapi.yml
  format: yaml
  label: Fillo Responses API
  slug: fillo-so-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-responses-api-openapi.yml
- filename: fillo-so-settings-api-openapi.yml
  format: yaml
  label: Fillo Settings API
  slug: fillo-so-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-settings-api-openapi.yml
- filename: fillo-so-storage-api-openapi.yml
  format: yaml
  label: Fillo Storage API
  slug: fillo-so-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-storage-api-openapi.yml
- filename: fillo-so-webhooks-api-openapi.yml
  format: yaml
  label: Fillo Webhooks API
  slug: fillo-so-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-webhooks-api-openapi.yml
- filename: fillo-so-workspace-api-openapi.yml
  format: yaml
  label: Fillo Workspace API
  slug: fillo-so-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-workspace-api-openapi.yml
consequence_counts:
  physical: 1
  read: 28
  safety-critical: 6
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Fillo So Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/manage/agents/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/manage/forms/{form}/integrations/{provider}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/manage/forms/{form}/storage/folder
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/manage/project/identity
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/manage/sync-tokens/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/manage/tokens/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/manage/forms/{form}/deliveries/redeliver
operation_count: 65
overview: 'Fillo exposes 65 API operations that an AI agent could call, of which 37 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 30 write, 1 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fillo
provider_slug: fillo-so
slug: fillo-so-agentic-access
source_filename: fillo-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/fillo-so-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    connected: 28\n    acting: 37\n  by_consequence:\n    read: 28\n    write: 30\n    safety-critical: 6\n    physical: 1\n  human_in_the_loop_required: 6\noperations:\n- path: /api/v1\n  method: get\n  operationId: discoverFilloApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms\n  method: get\n  operationId: listForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/manage/forms/{form}\n  method: get\n  operationId: getForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}\n  method: patch\n  operationId: renameForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/versions\n  method: get\n  operationId: listFormVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/settings\n  method: get\n  operationId: getFormSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/settings\n  method: patch\n  operationId: updateFormSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/webhooks\n  method: get\n  operationId: listFormWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/webhooks\n  method: post\n  operationId: createFormWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/webhooks/{id}\n  method: patch\n  operationId: updateFormWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/webhooks/{id}\n  method: delete\n  operationId: deleteFormWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/responses\n  method: get\n  operationId: listFormResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/responses/export\n  method: get\n  operationId: exportFormResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/responses/summary\n  method: get\n  operationId: summarizeFormResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/responses/{id}\n  method: get\n  operationId: getResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/responses/{id}\n  method: delete\n  operationId: deleteResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/respondents\n  method: get\n  operationId: findRespondents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/respondents/{id}/responses\n  method: get\n  operationId: listRespondentResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/unpublish\n  method: post\n  operationId: unpublishForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/discard\n\
  \  method: post\n  operationId: discardFormDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/duplicate\n  method: post\n  operationId: duplicateForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/storage\n  method: get\n  operationId: getFormStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/storage\n  method: put\n  operationId:\
  \ setFormStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/storage/folder\n  method: get\n  operationId: listFormStorageFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/storage/folder\n  method: put\n  operationId: setFormStorageFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/storage/folder\n  method: delete\n \
  \ operationId: resetFormStorageFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/manage/forms/{form}/insights\n  method: get\n  operationId: getFormInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/drafts\n  method: get\n  operationId: listFormDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/deliveries\n  method: get\n  operationId: getFormDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/deliveries/retry\n  method: post\n  operationId: retryFormDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/deliveries/redeliver\n  method: post\n  operationId: redeliverFormResponses\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/responses/release\n  method: post\n  operationId: releaseHeldResponses\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/integrations/{provider}\n  method: get\n  operationId: getFormIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/forms/{form}/integrations/{provider}\n  method: put\n  operationId: setFormIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/forms/{form}/integrations/{provider}\n  method: delete\n\
  \  operationId: disableFormIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/manage/integrations/connections\n  method: get\n  operationId: listIntegrationConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/integrations/connections/{provider}\n  method: put\n  operationId: selectIntegrationConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/manage/integrations/connections/{provider}\n  method: delete\n  operationId: detachIntegrationConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/integrations/accounts/{id}\n  method: delete\n  operationId: removeIntegrationAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/integrations/discord/accounts/{id}\n  method: patch\n  operationId: renameDiscordChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/integrations/discord/servers/{guildId}\n  method: delete\n  operationId: disconnectDiscordServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/integrations/hubspot/properties\n  method: get\n  operationId: listHubspotProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/integrations/hubspot/pipelines\n  method: get\n  operationId: listHubspotPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/respondents/{id}\n  method: delete\n  operationId: forgetRespondent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/members\n  method: get\n  operationId: listWorkspaceMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/members/invites\n  method: post\n  operationId: inviteWorkspaceMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/manage/members/invites/{id}\n  method: delete\n  operationId: cancelWorkspaceInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/members/{id}\n  method: patch\n  operationId: setMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/members/{id}\n  method: delete\n  operationId: removeWorkspaceMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/workspace\n  method: patch\n  operationId: renameWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/project\n  method: patch\n  operationId: renameProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/project/code-sync\n  method: get\n  operationId: getCodeSyncPolicy\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/project/code-sync\n  method: patch\n  operationId: setCodeSyncPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/project/origins\n  method: get\n  operationId: listAllowedOrigins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/project/origins\n  method: put\n  operationId: setAllowedOrigins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/project/identity\n  method: get\n  operationId: getIdentityVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/project/identity\n  method: post\n  operationId: enableIdentityVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/project/identity\n  method: delete\n  operationId: disableIdentityVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/manage/tokens\n  method: get\n  operationId: listConnectorTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/tokens/{id}\n  method: delete\n  operationId: revokeConnectorToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/manage/sync-tokens\n  method: get\n  operationId: listSyncTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/sync-tokens\n  method: post\n  operationId:\
  \ createSyncToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/manage/sync-tokens/{id}\n  method: delete\n  operationId: revokeSyncToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/manage/agents\n  method: get\n  operationId: listAgentGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manage/agents/{id}\n  method: delete\n  operationId: revokeAgentGrant\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/fillo-so/agentic-access/fillo-so-agentic-access.yml
summary_line: 65 operations · 37 acting · 6 human-in-the-loop
tags:
- Forms
- Form Builder
- Developer Tools
- Embeddable Widgets
- Webhooks
- Validation
- File Uploads
- SDK
- CLI
- Management API
---
