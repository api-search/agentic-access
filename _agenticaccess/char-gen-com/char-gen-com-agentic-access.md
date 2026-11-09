---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: char-gen-com-account-catalog-api-openapi.yml
  format: yaml
  label: CharGen Account & catalog API
  slug: char-gen-com-account-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-account-catalog-api-openapi.yml
- filename: char-gen-com-billing-api-openapi.yml
  format: yaml
  label: CharGen Billing API
  slug: char-gen-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-billing-api-openapi.yml
- filename: char-gen-com-entities-api-openapi.yml
  format: yaml
  label: CharGen Entities API
  slug: char-gen-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-entities-api-openapi.yml
- filename: char-gen-com-generations-api-openapi.yml
  format: yaml
  label: CharGen Generations API
  slug: char-gen-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-generations-api-openapi.yml
- filename: char-gen-com-ping-api-openapi.yml
  format: yaml
  label: CharGen Ping API
  slug: char-gen-com-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-ping-api-openapi.yml
- filename: char-gen-com-public-pricing-api-openapi.yml
  format: yaml
  label: CharGen Public pricing API
  slug: char-gen-com-public-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-public-pricing-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Char Gen Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /partner/v1/generations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partner/v1/billing/checkout-session
operation_count: 9
overview: 'CharGen exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 1 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CharGen
provider_slug: char-gen-com
slug: char-gen-com-agentic-access
source_filename: char-gen-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/partner-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    safety-critical: 1\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /partner/v1/generations\n  method: get\n  operationId: list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/generations\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /partner/v1/entities\n  method: post\n  operationId: createEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/billing/checkout-session\n  method: post\n  operationId: checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/public/pricing\n  method: get\n  operationId:\
  \ pricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/models\n  method: get\n  operationId: models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/generations/{id}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://artifacts.apis.io/char-gen-com/agentic-access/char-gen-com-agentic-access.yml
summary_line: 9 operations · 3 acting · 1 human-in-the-loop
tags:
- AI Art
- RPG Tools
- Character Generation
- Map Generation
- Campaign Building
- Audio Generation
---
