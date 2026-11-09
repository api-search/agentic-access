---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 8
api_specs:
- filename: dsrv-ethereum-api-openapi.yml
  format: yaml
  label: Dsrv Ethereum API
  slug: dsrv-ethereum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsrv/openapi/dsrv-ethereum-api-openapi.yml
- filename: dsrv-health-api-openapi.yml
  format: yaml
  label: Dsrv Health API
  slug: dsrv-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dsrv/openapi/dsrv-health-api-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Dsrv Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ethereum/{network}/broadcast
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ethereum/{network}/request-deposit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ethereum/{network}/request-withdraw
operation_count: 11
overview: 'Dsrv exposes 11 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dsrv
provider_slug: dsrv
slug: dsrv-agentic-access
source_filename: dsrv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: generated\nsource: openapi/dsrv-staking-hub-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 3\n    connected: 8\n  by_consequence:\n    safety-critical: 3\n    read: 8\n  human_in_the_loop_required: 3\noperations:\n- path: /ethereum/{network}/broadcast\n  method: post\n  operationId: EthereumController_broadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ethereum/{network}/income-daily\n\
  \  method: post\n  operationId: EthereumController_getIncomeDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ethereum/{network}/income-lifetime\n  method: post\n  operationId: EthereumController_getIncomeLifetime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ethereum/{network}/income-monthly\n  method: post\n  operationId: EthereumController_getIncomeMonthly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ethereum/{network}/key-stat\n  method: get\n  operationId: EthereumController_getKeyStat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ethereum/{network}/request-deposit\n\
  \  method: post\n  operationId: EthereumController_requestDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ethereum/{network}/request-withdraw\n  method: post\n  operationId: EthereumController_requestWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ethereum/{network}/transactions\n  method: post\n  operationId: EthereumController_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ethereum/{network}/validators\n  method: post\n  operationId: EthereumController_getValidators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ethereum/{network}/validators/apr\n  method: post\n  operationId: EthereumController_getValidatorApr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: AppController_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dsrv/agentic-access/dsrv-agentic-access.yml
summary_line: 11 operations · 3 acting · 3 human-in-the-loop
tags:
- Company
- Blockchain
- Infrastructure
- Staking
- Web3
---
