---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 28
api_specs:
- filename: zvid-io-api-keys-api-openapi.yml
  format: yaml
  label: zvid-io API Keys API
  slug: zvid-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-api-keys-api-openapi.yml
- filename: zvid-io-authoring-api-openapi.yml
  format: yaml
  label: zvid-io Authoring API
  slug: zvid-io-authoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-authoring-api-openapi.yml
- filename: zvid-io-bulk-render-api-openapi.yml
  format: yaml
  label: zvid-io Bulk Render API
  slug: zvid-io-bulk-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-bulk-render-api-openapi.yml
- filename: zvid-io-credits-api-openapi.yml
  format: yaml
  label: zvid-io Credits API
  slug: zvid-io-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-credits-api-openapi.yml
- filename: zvid-io-library-api-openapi.yml
  format: yaml
  label: zvid-io Library API
  slug: zvid-io-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-library-api-openapi.yml
- filename: zvid-io-projects-api-openapi.yml
  format: yaml
  label: zvid-io Projects API
  slug: zvid-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-projects-api-openapi.yml
- filename: zvid-io-render-api-openapi.yml
  format: yaml
  label: zvid-io Render API
  slug: zvid-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-render-api-openapi.yml
- filename: zvid-io-stock-api-openapi.yml
  format: yaml
  label: zvid-io Stock API
  slug: zvid-io-stock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-stock-api-openapi.yml
- filename: zvid-io-templates-api-openapi.yml
  format: yaml
  label: zvid-io Templates API
  slug: zvid-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-templates-api-openapi.yml
- filename: zvid-io-uploads-api-openapi.yml
  format: yaml
  label: zvid-io Uploads API
  slug: zvid-io-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-uploads-api-openapi.yml
- filename: zvid-io-user-api-openapi.yml
  format: yaml
  label: zvid-io User API
  slug: zvid-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-user-api-openapi.yml
- filename: zvid-io-webhooks-api-openapi.yml
  format: yaml
  label: zvid-io Webhooks API
  slug: zvid-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-webhooks-api-openapi.yml
- filename: zvid-io-zvid-api-api-openapi.yml
  format: yaml
  label: zvid-io Zvid API
  slug: zvid-io-zvid-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-zvid-api-api-openapi.yml
consequence_counts:
  physical: 1
  read: 28
  safety-critical: 1
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Zvid Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/api-keys/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/webhooks/{id}/test
operation_count: 52
overview: 'zvid-io exposes 52 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 22 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: zvid-io
provider_slug: zvid-io
slug: zvid-io-agentic-access
source_filename: zvid-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/zvid-io-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 28\n    acting: 24\n  by_consequence:\n    read: 28\n    write: 22\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/user/profile\n  method: get\n  operationId: getUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/credits/balance\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /api/credits/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/credits/usage-stats\n  method: get\n  operationId: getUsageStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/api-keys/{id}\n  method: put\n  operationId: updateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/api-keys/{id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/api-keys/{id}/stats\n  method: get\n  operationId: getApiKeyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/creative-plan/api-key\n\
  \  method: post\n  operationId: planCreativeVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/render/api-key\n  method: post\n  operationId: submitRenderJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/jobs\n  method: get\n  operationId: listRenderJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/jobs/{id}\n  method: get\n  operationId: getRenderJob\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/image/api-key\n  method: post\n  operationId: submitImageRenderJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/render/bulk/api-key\n  method: post\n  operationId: submitBulkRender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/render/image/bulk/api-key\n  method: post\n  operationId: submitImageBulkRender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/render/bulk\n  method: get\n  operationId: listBulkRenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/bulk/{id}\n  method: get\n  operationId: getBulkRender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/templates\n  method: post\n  operationId: createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/templates/{id}\n  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/templates/{id}\n  method: put\n  operationId: updateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/templates/{id}\n  method: delete\n  operationId: deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/templates/{id}/preview\n  method: post\n  operationId: previewTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/{id}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}/deliveries\n\
  \  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/uploads\n  method: get\n  operationId: listUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/uploads/{id}\n  method: delete\n  operationId: deleteUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{id}\n  method: put\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/projects/{id}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/templates/{id}/duplicate\n  method: post\n  operationId: duplicateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/render/validate/api-key\n  method: post\n  operationId: validateRenderJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/render/schema/api-key\n  method: get\n  operationId: getRenderSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/elements/api-key\n  method:\
  \ get\n  operationId: listRenderElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/elements/{type}/api-key\n  method: get\n  operationId: getRenderElement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/examples/api-key\n  method: get\n  operationId: listRenderExamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/examples/{name}/api-key\n  method: get\n  operationId: getRenderExample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/render/repair/api-key\n  method: post\n  operationId: repairRenderProject\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/preferences\n  method: get\n  operationId: getMcpPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stock/search\n  method: get\n  operationId: searchStockMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/library/{kind}\n  method: get\n  operationId: listLibraryItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/library/{kind}/{slug}\n  method: get\n  operationId: getLibraryItem\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/library/{kind}/{slug}/content\n  method: get\n  operationId: getLibraryContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/zvid-io/agentic-access/zvid-io-agentic-access.yml
summary_line: 52 operations · 24 acting · 1 human-in-the-loop
tags:
- Company
- Video
- Automation
- Media
---
