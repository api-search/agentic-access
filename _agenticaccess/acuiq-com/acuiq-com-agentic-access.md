---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: acuiq-com-checkout-api-openapi.yml
  format: yaml
  label: AcuiQ Checkout API
  slug: acuiq-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-checkout-api-openapi.yml
- filename: acuiq-com-corpus-api-openapi.yml
  format: yaml
  label: AcuiQ Corpus API
  slug: acuiq-com-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-corpus-api-openapi.yml
- filename: acuiq-com-llms-txt-api-openapi.yml
  format: yaml
  label: AcuiQ Llms.txt API
  slug: acuiq-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-llms-txt-api-openapi.yml
- filename: acuiq-com-mcp-api-openapi.yml
  format: yaml
  label: AcuiQ MCP API
  slug: acuiq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-mcp-api-openapi.yml
- filename: acuiq-com-meridians-api-openapi.yml
  format: yaml
  label: AcuiQ Meridians API
  slug: acuiq-com-meridians-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-meridians-api-openapi.yml
- filename: acuiq-com-protocols-api-openapi.yml
  format: yaml
  label: AcuiQ Protocols API
  slug: acuiq-com-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-protocols-api-openapi.yml
- filename: acuiq-com-reviews-api-openapi.yml
  format: yaml
  label: AcuiQ Reviews API
  slug: acuiq-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-reviews-api-openapi.yml
- filename: acuiq-com-symptoms-api-openapi.yml
  format: yaml
  label: AcuiQ Symptoms API
  slug: acuiq-com-symptoms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-symptoms-api-openapi.yml
- filename: acuiq-com-wiki-api-openapi.yml
  format: yaml
  label: AcuiQ Wiki API
  slug: acuiq-com-wiki-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuiq-com/openapi/acuiq-com-wiki-api-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Acuiq Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp
operation_count: 9
overview: 'AcuiQ exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AcuiQ
provider_slug: acuiq-com
slug: acuiq-com-agentic-access
source_filename: acuiq-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/acuiq-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    physical: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/symptoms\n  method: get\n  operationId: searchSymptoms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meridians\n  method: get\n  operationId: getMeridians\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/protocols\n \
  \ method: get\n  operationId: searchProtocols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wiki\n  method: get\n  operationId: searchWiki\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reviews\n  method: post\n  operationId: submitProductRating\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: post\n  operationId: mcpServer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/corpus\n  method: get\n  operationId: getCorpus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/acuiq-com/agentic-access/acuiq-com-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Health
- Acupuncture
- Data
- Research
- Wellness
---
