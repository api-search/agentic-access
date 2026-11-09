---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 18
api_specs:
- filename: pdfs-build-delegated-agents-api-openapi.yml
  format: yaml
  label: pdfs-build Delegated agents API
  slug: pdfs-build-delegated-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-delegated-agents-api-openapi.yml
- filename: pdfs-build-embedded-editor-api-openapi.yml
  format: yaml
  label: pdfs-build Embedded editor API
  slug: pdfs-build-embedded-editor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-embedded-editor-api-openapi.yml
- filename: pdfs-build-legacy-v1-api-openapi.yml
  format: yaml
  label: pdfs-build Legacy v1 API
  slug: pdfs-build-legacy-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-legacy-v1-api-openapi.yml
- filename: pdfs-build-render-jobs-api-openapi.yml
  format: yaml
  label: pdfs-build Render jobs API
  slug: pdfs-build-render-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-render-jobs-api-openapi.yml
- filename: pdfs-build-render-logs-api-openapi.yml
  format: yaml
  label: pdfs-build Render logs API
  slug: pdfs-build-render-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-render-logs-api-openapi.yml
- filename: pdfs-build-rendering-api-openapi.yml
  format: yaml
  label: pdfs-build Rendering API
  slug: pdfs-build-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-rendering-api-openapi.yml
- filename: pdfs-build-template-gallery-api-openapi.yml
  format: yaml
  label: pdfs-build Template gallery API
  slug: pdfs-build-template-gallery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-template-gallery-api-openapi.yml
- filename: pdfs-build-templates-api-openapi.yml
  format: yaml
  label: pdfs-build Templates API
  slug: pdfs-build-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-templates-api-openapi.yml
- filename: pdfs-build-webhooks-api-openapi.yml
  format: yaml
  label: pdfs-build Webhooks API
  slug: pdfs-build-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfs-build/openapi/pdfs-build-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  safety-critical: 2
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Pdfs Build Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/organizations/{organizationId}/delegated/grants/{grantId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/organizations/{organizationId}/embed-sessions/{sessionId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/organizations/{organizationId}/webhooks/{endpointId}/test
operation_count: 38
overview: 'pdfs-build exposes 38 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 17 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: pdfs-build
provider_slug: pdfs-build
slug: pdfs-build-agentic-access
source_filename: pdfs-build-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/pdfs-build-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 18\n    acting: 20\n  by_consequence:\n    read: 18\n    write: 17\n    physical: 1\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v2/organizations/{organizationId}/templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/templates\n  method: post\n  operationId: createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/templates/{externalId}\n  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/templates/{externalId}\n  method: patch\n  operationId: updateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/templates/{externalId}/publish\n  method: post\n  operationId: publishTemplate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/templates/{externalId}/unpublish\n  method: post\n  operationId: unpublishTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/templates/{externalId}/render\n  method: post\n  operationId: renderTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/templates/{externalId}/batches\n  method: post\n  operationId: createRenderBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/renders/{jobId}\n  method: get\n  operationId: getRenderJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/renders/{jobId}/pdf\n  method: get\n  operationId: getRenderJobPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/batches/{batchId}\n\
  \  method: get\n  operationId: getRenderBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/templates/{externalId}/logs\n  method: get\n  operationId: listTemplateLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/logs\n  method: get\n  operationId: listLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/logs/{logId}\n  method: get\n  operationId: getLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/webhooks\n  method: get\n\
  \  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/webhooks\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/webhooks/{endpointId}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/webhooks/{endpointId}\n\
  \  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/webhooks/{endpointId}/rotate-secret\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/webhooks/{endpointId}/test\n  method: post\n  operationId: testWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/webhooks/{endpointId}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/templates/{externalId}/embed-sessions\n  method: post\n  operationId: createEmbedSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/embed-sessions/{sessionId}\n  method: delete\n  operationId: revokeEmbedSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/organizations/{organizationId}/gallery\n  method: get\n  operationId: listGalleryTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/gallery/{galleryId}/preview\n  method: get\n  operationId: previewGalleryTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/templates/from-gallery\n  method: post\n  operationId: createTemplateFromGallery\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/delegated/tickets\n  method: post\n  operationId: createDelegatedTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organizations/{organizationId}/delegated/grants\n  method: get\n  operationId: listDelegatedGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organizations/{organizationId}/delegated/grants/{grantId}\n  method: delete\n  operationId: revokeDelegatedGrant\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/render\n  method: post\n  operationId: renderTemplateV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: get\n  operationId: listTemplatesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates\n  method: post\n  operationId: createTemplateV1\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/{id}\n  method: get\n  operationId: getTemplateV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/{id}/publish\n  method: post\n  operationId: publishTemplateV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/{id}/unpublish\n  method: post\n  operationId: unpublishTemplateV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/{id}/logs\n  method: get\n  operationId: listTemplateLogsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/logs\n  method: get\n  operationId: listLogsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/logs/{id}\n  method: get\n  operationId: getLogV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/pdfs-build/agentic-access/pdfs-build-agentic-access.yml
summary_line: 38 operations · 20 acting · 2 human-in-the-loop
tags:
- PDF
- Template Engine
- Rendering
- Software-as-a-Service
- Document Generation
---
