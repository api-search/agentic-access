---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 12
api_specs:
- filename: flexyield-io-agents-api-openapi.yml
  format: yaml
  label: flexyield-io Agents API
  slug: flexyield-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-agents-api-openapi.yml
- filename: flexyield-io-data-api-openapi.yml
  format: yaml
  label: flexyield-io Data API
  slug: flexyield-io-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-data-api-openapi.yml
- filename: flexyield-io-keys-api-openapi.yml
  format: yaml
  label: flexyield-io Keys API
  slug: flexyield-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-keys-api-openapi.yml
- filename: flexyield-io-rpc-api-openapi.yml
  format: yaml
  label: flexyield-io Rpc API
  slug: flexyield-io-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-rpc-api-openapi.yml
- filename: flexyield-io-statements-api-openapi.yml
  format: yaml
  label: flexyield-io Statements API
  slug: flexyield-io-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-statements-api-openapi.yml
- filename: flexyield-io-toolbox-api-openapi.yml
  format: yaml
  label: flexyield-io Toolbox API
  slug: flexyield-io-toolbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-toolbox-api-openapi.yml
- filename: flexyield-io-x402-api-openapi.yml
  format: yaml
  label: flexyield-io X402 API
  slug: flexyield-io-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexyield-io/openapi/flexyield-io-x402-api-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Flexyield Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/adopt
operation_count: 18
overview: 'flexyield-io exposes 18 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: flexyield-io
provider_slug: flexyield-io
slug: flexyield-io-agentic-access
source_filename: flexyield-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/flexyield-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 6\n    connected: 12\n  by_consequence:\n    write: 5\n    read: 12\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /rpc/{chain}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /toolbox/gas/{chain}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /toolbox/tx/{chain}/{hash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /toolbox/ens/resolve/{name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /toolbox/ens/reverse/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /toolbox/prices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /toolbox/abi/{chain}/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /toolbox/decode/{chain}/{address}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{chain}/balances/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{chain}/history/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/statements\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/statements/{period}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/receipts/{tx_hash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/bind/start\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/bind\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/adopt\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/flexyield-io/agentic-access/flexyield-io-agentic-access.yml
summary_line: 18 operations · 6 acting · 1 human-in-the-loop
tags:
- Blockchain
- API Gateway
- Unified Billing
- Multi-Chain
- Free Tier
---
