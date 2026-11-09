---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 10
api_specs:
- filename: aitwire-com-api-keys-api-openapi.yml
  format: yaml
  label: aitwire-com API Keys API
  slug: aitwire-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-api-keys-api-openapi.yml
- filename: aitwire-com-attribution-api-openapi.yml
  format: yaml
  label: aitwire-com Attribution API
  slug: aitwire-com-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-attribution-api-openapi.yml
- filename: aitwire-com-authority-api-openapi.yml
  format: yaml
  label: aitwire-com Authority API
  slug: aitwire-com-authority-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-authority-api-openapi.yml
- filename: aitwire-com-billing-api-openapi.yml
  format: yaml
  label: aitwire-com Billing API
  slug: aitwire-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-billing-api-openapi.yml
- filename: aitwire-com-drift-api-openapi.yml
  format: yaml
  label: aitwire-com Drift API
  slug: aitwire-com-drift-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-drift-api-openapi.yml
- filename: aitwire-com-entities-api-openapi.yml
  format: yaml
  label: aitwire-com Entities API
  slug: aitwire-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-entities-api-openapi.yml
- filename: aitwire-com-scans-api-openapi.yml
  format: yaml
  label: aitwire-com Scans API
  slug: aitwire-com-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-scans-api-openapi.yml
- filename: aitwire-com-webhooks-api-openapi.yml
  format: yaml
  label: aitwire-com Webhooks API
  slug: aitwire-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitwire-com/openapi/aitwire-com-webhooks-api-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Aitwire Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /webhooks/{id}
operation_count: 17
overview: 'aitwire-com exposes 17 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: aitwire-com
provider_slug: aitwire-com
slug: aitwire-com-agentic-access
source_filename: aitwire-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/aitwire-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 10\n    acting: 7\n  by_consequence:\n    read: 10\n    write: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /entities\n  method: get\n  operationId: listEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{id}\n  method: get\n  operationId: getEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{id}\n\
  \  method: put\n  operationId: upsertEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scans\n  method: get\n  operationId: listScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/run\n  method: post\n  operationId: runScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authority/graph\n  method: get\n  operationId: getAuthorityGraph\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /governance/drift/events\n  method: get\n  operationId: listDriftEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attribution/summary\n  method: get\n  operationId: getAttributionSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/scopes\n  method: get\n  operationId: listAvailableScopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage\n  method: get\n  operationId: getUsageStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aitwire-com/agentic-access/aitwire-com-agentic-access.yml
summary_line: 17 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- IoT
- Connectivity
- Industrial
---
