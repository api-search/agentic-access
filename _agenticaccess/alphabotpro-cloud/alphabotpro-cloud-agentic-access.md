---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 12
api_specs:
- filename: alphabotpro-cloud-checkout-api-openapi.yml
  format: yaml
  label: AlphaBotPro Checkout API
  slug: alphabotpro-cloud-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-checkout-api-openapi.yml
- filename: alphabotpro-cloud-ea-api-openapi.yml
  format: yaml
  label: AlphaBotPro Ea API
  slug: alphabotpro-cloud-ea-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-ea-api-openapi.yml
- filename: alphabotpro-cloud-expert-advisors-api-openapi.yml
  format: yaml
  label: AlphaBotPro Expert Advisors API
  slug: alphabotpro-cloud-expert-advisors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-expert-advisors-api-openapi.yml
- filename: alphabotpro-cloud-mcp-api-openapi.yml
  format: yaml
  label: AlphaBotPro MCP API
  slug: alphabotpro-cloud-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-mcp-api-openapi.yml
- filename: alphabotpro-cloud-signals-api-openapi.yml
  format: yaml
  label: AlphaBotPro Signals API
  slug: alphabotpro-cloud-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-signals-api-openapi.yml
- filename: alphabotpro-cloud-stocks-api-openapi.yml
  format: yaml
  label: AlphaBotPro Stocks API
  slug: alphabotpro-cloud-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-stocks-api-openapi.yml
- filename: alphabotpro-cloud-warroom-api-openapi.yml
  format: yaml
  label: AlphaBotPro Warroom API
  slug: alphabotpro-cloud-warroom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabotpro-cloud/openapi/alphabotpro-cloud-warroom-api-openapi.yml
consequence_counts:
  physical: 4
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alphabotpro Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/api/checkout/crypto
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/api/checkout/crypto
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/api/checkout/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/api/checkout/verify
operation_count: 16
overview: 'AlphaBotPro exposes 16 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AlphaBotPro
provider_slug: alphabotpro-cloud
slug: alphabotpro-cloud-agentic-access
source_filename: alphabotpro-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/alphabotpro-cloud-openapi.json, openapi/mcp-alphabotpro-cloud-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 12\n    acting: 4\n  by_consequence:\n    read: 12\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/mcp/catalog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/signals\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/warroom\n  method: get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/expert-advisors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/ea/{slug}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/stocks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/checkout/crypto\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/checkout/verify\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mcp/catalog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/signals\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/warroom\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/api/expert-advisors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/ea/{slug}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/stocks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/checkout/crypto\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/checkout/verify\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/alphabotpro-cloud/agentic-access/alphabotpro-cloud-agentic-access.yml
summary_line: 16 operations · 4 acting
tags:
- Company
- Trading
- Automation
- Signals
- MT5
- PropFirm
---
