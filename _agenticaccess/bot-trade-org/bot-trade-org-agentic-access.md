---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: bot-trade-org-billing-api-openapi.yml
  format: yaml
  label: BotTrade Billing API
  slug: bot-trade-org-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-billing-api-openapi.yml
- filename: bot-trade-org-market-api-openapi.yml
  format: yaml
  label: BotTrade Market API
  slug: bot-trade-org-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-market-api-openapi.yml
- filename: bot-trade-org-runs-api-openapi.yml
  format: yaml
  label: BotTrade Runs API
  slug: bot-trade-org-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-runs-api-openapi.yml
- filename: bot-trade-org-scenarios-api-openapi.yml
  format: yaml
  label: BotTrade Scenarios API
  slug: bot-trade-org-scenarios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bot-trade-org/openapi/bot-trade-org-scenarios-api-openapi.yml
consequence_counts:
  physical: 2
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bot Trade Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/runs/{id}/trades
operation_count: 15
overview: 'BotTrade exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BotTrade
provider_slug: bot-trade-org
slug: bot-trade-org-agentic-access
source_filename: bot-trade-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/bot-trade-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 5\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/billing/account\n  method: get\n  operationId: getBillingAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/account\n  method: patch\n  operationId: patchBillingAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/checkout\n  method: post\n  operationId: billingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/portal\n  method: post\n  operationId: billingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/session/{session_id}\n  method: get\n  operationId: getBillingSession\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/runs\n  method: post\n  operationId: createRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/runs/{id}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/runs/{id}/market\n  method: get\n  operationId: getRunMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/runs/{id}/publish\n  method: post\n  operationId: publish\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/runs/{id}/results\n  method: get\n  operationId: getResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/runs/{id}/step\n  method: post\n  operationId: step\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/runs/{id}/trades\n  method: get\n  operationId: listTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/runs/{id}/trades\n  method: post\n  operationId: queueTrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scenarios\n  method: get\n  operationId: listScenarios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scenarios/{id}\n  method: get\n  operationId: getScenario\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bot-trade-org/agentic-access/bot-trade-org-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Finance
- Artificial Intelligence
- Trading
- Simulation
- Benchmarks
- Company
---
