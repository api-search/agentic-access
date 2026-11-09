---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: asoskill-com-authentication-api-openapi.yml
  format: yaml
  label: asoskill-com Authentication API
  slug: asoskill-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-authentication-api-openapi.yml
- filename: asoskill-com-billing-api-openapi.yml
  format: yaml
  label: asoskill-com Billing API
  slug: asoskill-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-billing-api-openapi.yml
- filename: asoskill-com-credits-api-openapi.yml
  format: yaml
  label: asoskill-com Credits API
  slug: asoskill-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-credits-api-openapi.yml
- filename: asoskill-com-data-api-openapi.yml
  format: yaml
  label: asoskill-com Data API
  slug: asoskill-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-data-api-openapi.yml
- filename: asoskill-com-mcp-api-openapi.yml
  format: yaml
  label: asoskill-com MCP API
  slug: asoskill-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-mcp-api-openapi.yml
- filename: asoskill-com-operations-api-openapi.yml
  format: yaml
  label: asoskill-com Operations API
  slug: asoskill-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-operations-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  safety-critical: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Asoskill Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /mcp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/auth/credential
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 13
overview: 'asoskill-com exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 4 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: asoskill-com
provider_slug: asoskill-com
slug: asoskill-com-agentic-access
source_filename: asoskill-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/asoskill-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 6\n    acting: 7\n  by_consequence:\n    read: 6\n    safety-critical: 2\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /\n  method: get\n  operationId: discoverApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n\
  \  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - credits\n    - data\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/autocomplete\n  method: post\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/popularity\n  method: post\n  operationId: popularity\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/lookup\n  method: post\n  operationId: lookupApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits\n  method: get\n  operationId: credits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/packs\n  method: get\n  operationId: billingPacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: checkout\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/device\n  method: post\n  operationId: startDeviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/device/token\n  method: post\n  operationId: exchangeDeviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/auth/credential\n  method: delete\n  operationId: revokeCurrentCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/asoskill-com/agentic-access/asoskill-com-agentic-access.yml
summary_line: 13 operations · 7 acting · 2 human-in-the-loop
tags:
- Company
- ASO
- App Store
- Data
---
