---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: xauconnect-com-analytics-api-openapi.yml
  format: yaml
  label: XAUConnect Analytics API
  slug: xauconnect-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-analytics-api-openapi.yml
- filename: xauconnect-com-cross-chain-api-openapi.yml
  format: yaml
  label: XAUConnect Cross Chain API
  slug: xauconnect-com-cross-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-cross-chain-api-openapi.yml
- filename: xauconnect-com-meta-api-openapi.yml
  format: yaml
  label: XAUConnect Meta API
  slug: xauconnect-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-meta-api-openapi.yml
- filename: xauconnect-com-swap-api-openapi.yml
  format: yaml
  label: XAUConnect Swap API
  slug: xauconnect-com-swap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xauconnect-com/openapi/xauconnect-com-swap-api-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xauconnect Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'XAUConnect exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: XAUConnect
provider_slug: xauconnect-com
slug: xauconnect-com-agentic-access
source_filename: xauconnect-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/xauconnect-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 7\n    acting: 6\n  by_consequence:\n    read: 7\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/chains\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/tokens\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/dexes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/settings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/allowance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/quote\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap/build\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap/submit-solana\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap/record\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap/cross-chain/quote\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap/cross-chain/build\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap/cross-chain/status/{quoteId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/xauconnect-com/agentic-access/xauconnect-com-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Fintech
- DeFi
- Blockchain
- Token Launch
- Solana
---
