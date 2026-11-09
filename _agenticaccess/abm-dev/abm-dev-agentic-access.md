---
acting_count: 36
action_class_counts:
  acting: 36
  connected: 34
api_specs:
- filename: abm-dev-campaigns-api-openapi.yml
  format: yaml
  label: abm-dev Campaigns API
  slug: abm-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-campaigns-api-openapi.yml
- filename: abm-dev-crm-api-openapi.yml
  format: yaml
  label: abm-dev CRM API
  slug: abm-dev-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-crm-api-openapi.yml
- filename: abm-dev-enrichment-api-openapi.yml
  format: yaml
  label: abm-dev Enrichment API
  slug: abm-dev-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-enrichment-api-openapi.yml
- filename: abm-dev-enrichment-config-api-openapi.yml
  format: yaml
  label: abm-dev Enrichment Config API
  slug: abm-dev-enrichment-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-enrichment-config-api-openapi.yml
- filename: abm-dev-field-configuration-api-openapi.yml
  format: yaml
  label: abm-dev Field Configuration API
  slug: abm-dev-field-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-field-configuration-api-openapi.yml
- filename: abm-dev-health-api-openapi.yml
  format: yaml
  label: abm-dev Health API
  slug: abm-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-health-api-openapi.yml
- filename: abm-dev-organization-api-openapi.yml
  format: yaml
  label: abm-dev Organization API
  slug: abm-dev-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-organization-api-openapi.yml
- filename: abm-dev-people-finder-api-openapi.yml
  format: yaml
  label: abm-dev People Finder API
  slug: abm-dev-people-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-people-finder-api-openapi.yml
- filename: abm-dev-webhooks-api-openapi.yml
  format: yaml
  label: abm-dev Webhooks API
  slug: abm-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 34
  safety-critical: 3
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Abm Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/api-keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/enrichment-config/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/field-config/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/organizations/signup
operation_count: 70
overview: 'abm-dev exposes 70 API operations that an AI agent could call, of which 36 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 32 write, 1 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: abm-dev
provider_slug: abm-dev
slug: abm-dev-agentic-access
source_filename: abm-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/abm-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 70\n  by_action_class:\n    acting: 36\n    connected: 34\n  by_consequence:\n    write: 32\n    read: 34\n    safety-critical: 3\n    physical: 1\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/enrichments\n  method: post\n  operationId: createEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments\n  method: get\n  operationId: listEnrichments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/stats\n  method: get\n  operationId: getEnrichmentStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/{id}\n  method: get\n  operationId: getEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/{id}\n  method: delete\n  operationId: cancelEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/{id}/stream\n  method: get\n  operationId: streamEnrichment\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/{id}/approve\n  method: post\n  operationId: approveEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/{id}/sources\n  method: get\n  operationId: getEnrichmentSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/{id}/fields\n  method: get\n  operationId: getEnrichmentFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/{id}/writeback-preview\n\
  \  method: get\n  operationId: getWritebackPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/{id}/export/excel\n  method: get\n  operationId: exportEnrichmentExcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/batches/preview\n  method: post\n  operationId: previewBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/batches/confirm\n  method: post\n  operationId: confirmBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/batches\n  method: get\n  operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/batches/{batchId}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/batches/{batchId}/members\n  method: get\n  operationId: getBatchMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/batches/{batchId}/approve\n  method: post\n  operationId: approveBatch\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/batches/{batchId}/export/excel\n  method: get\n  operationId: exportBatchExcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichments/{id}/writeback\n  method: post\n  operationId: executeWriteback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/bulk-writeback\n  method: post\n  operationId: bulkWriteback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/batches/upload\n  method: post\n  operationId: uploadBatchFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichments/batches/upload/confirm\n  method: post\n  operationId: confirmUploadBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people-finder\n  method: post\n  operationId:\
  \ createPersonFinderJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people-finder\n  method: get\n  operationId: listPersonFinderJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people-finder/{jobId}\n  method: get\n  operationId: getPersonFinderJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people-finder/{jobId}\n  method: delete\n  operationId: cancelPersonFinderJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people-finder/{jobId}/stream\n  method: get\n  operationId: streamPersonFinderJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people-finder/list/preview\n  method: post\n  operationId: previewPersonFinderList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people-finder/list/confirm\n  method: post\n  operationId: confirmPersonFinderList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people-finder/upload\n  method: post\n  operationId: uploadPersonFinderFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people-finder/upload/confirm\n  method: post\n  operationId: confirmPersonFinderUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns/preview\n  method: post\n  operationId: previewCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns/confirm\n  method: post\n  operationId: confirmCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{id}\n\
  \  method: delete\n  operationId: cancelCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns/{id}/stream\n  method: get\n  operationId: streamCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{id}/results\n  method: get\n  operationId: getCampaignResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{id}/approve\n  method: post\n  operationId: approveCampaignCandidates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns/{id}/writeback\n  method: post\n  operationId: campaignWriteback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/field-config\n  method: get\n  operationId: listFieldConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/field-config/{fieldId}\n  method: put\n  operationId: updateFieldConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/field-config/reset\n  method: post\n  operationId: resetFieldConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/enrichment-config\n  method: get\n  operationId: getEnrichmentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrichment-config\n  method: put\n  operationId: updateEnrichmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichment-config/reset\n  method: post\n  operationId: resetEnrichmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhooks/subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/subscriptions/{id}\n  method: get\n  operationId: getWebhookSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/subscriptions/{id}\n  method: patch\n  operationId: updateWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/subscriptions/{id}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/event-types\n  method: get\n  operationId: listWebhookEventTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crm/config/integrations\n  method: get\n  operationId: listCrmIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crm/config/integrations\n  method: post\n  operationId: createCrmIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crm/config/integrations/{id}\n  method: get\n  operationId: getCrmIntegration\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crm/config/integrations/{id}\n  method: delete\n  operationId: deleteCrmIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crm/config/integrations/test\n  method: post\n  operationId: testCrmIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crm/config/platforms/{platform}/health\n  method: get\n  operationId: getCrmPlatformHealth\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crm/config/platforms/{platform}/mappings\n  method: get\n  operationId: getCrmFieldMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/current\n  method: get\n  operationId: getCurrentOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/signup\n  method: post\n  operationId: signupOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys/{keyId}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys/{keyId}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/api-keys/{keyId}/rotate\n  method: post\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/detailed\n  method: get\n  operationId: detailedHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/abm-dev/agentic-access/abm-dev-agentic-access.yml
summary_line: 70 operations · 36 acting · 3 human-in-the-loop
tags:
- Account Based Marketing
- AI Agents
- Data Enrichment
- B2B
- Marketing API
---
