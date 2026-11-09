---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: xpay-sh-rda-api-openapi.yml
  format: yaml
  label: xpay-sh Rda API
  slug: xpay-sh-rda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-rda-api-openapi.yml
- filename: xpay-sh-rdas-api-openapi.yml
  format: yaml
  label: xpay-sh Rdas API
  slug: xpay-sh-rdas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-rdas-api-openapi.yml
- filename: xpay-sh-run-api-openapi.yml
  format: yaml
  label: xpay-sh Run API
  slug: xpay-sh-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-run-api-openapi.yml
- filename: xpay-sh-wallet-api-openapi.yml
  format: yaml
  label: xpay-sh Wallet API
  slug: xpay-sh-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-wallet-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xpay Sh Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallet/deposit
operation_count: 6
overview: 'xpay-sh exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: xpay-sh
provider_slug: xpay-sh
slug: xpay-sh-agentic-access
source_filename: xpay-sh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/xpay-sh-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 3\n    acting: 3\n  by_consequence:\n    read: 3\n    write: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /rdas\n  method: get\n  operationId: listRdas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rda/{identifier}\n  method: get\n  operationId: getRda\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rda\n  method: post\n  operationId:\
  \ createRda\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /run\n  method: post\n  operationId: runRda\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/balance\n  method: get\n  operationId: getWalletBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/deposit\n  method: post\n  operationId: recordDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/xpay-sh/agentic-access/xpay-sh-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Company
- Commerce
- Artificial Intelligence
- Software-as-a-Service
- Agent Readiness
---
