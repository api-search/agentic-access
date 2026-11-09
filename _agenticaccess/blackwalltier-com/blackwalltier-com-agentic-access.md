---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: blackwalltier-com-forecast-api-openapi.yml
  format: yaml
  label: blackwalltier-com Forecast API
  slug: blackwalltier-com-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blackwalltier-com/openapi/blackwalltier-com-forecast-api-openapi.yml
- filename: blackwalltier-com-keys-api-openapi.yml
  format: yaml
  label: blackwalltier-com Keys API
  slug: blackwalltier-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blackwalltier-com/openapi/blackwalltier-com-keys-api-openapi.yml
- filename: blackwalltier-com-receipts-api-openapi.yml
  format: yaml
  label: blackwalltier-com Receipts API
  slug: blackwalltier-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blackwalltier-com/openapi/blackwalltier-com-receipts-api-openapi.yml
- filename: blackwalltier-com-usage-api-openapi.yml
  format: yaml
  label: blackwalltier-com Usage API
  slug: blackwalltier-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blackwalltier-com/openapi/blackwalltier-com-usage-api-openapi.yml
consequence_counts:
  read: 3
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blackwalltier Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'blackwalltier-com exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: blackwalltier-com
provider_slug: blackwalltier-com
slug: blackwalltier-com-agentic-access
source_filename: blackwalltier-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/blackwalltier-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 4\n    connected: 3\n  by_consequence:\n    write: 4\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/forecast\n  method: post\n  operationId: createForecast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/receipts/{id}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipts/verify\n  method: post\n  operationId: verifyReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/forecast/{id}/outcome\n  method: patch\n  operationId: reportOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/blackwalltier-com/agentic-access/blackwalltier-com-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- Company
- Artificial Intelligence
- Security
- Policy
- Risk Management
---
