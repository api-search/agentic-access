---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: betsolutions-wallet-api.yaml
  format: yaml
  label: BetSolutions Wallet API
  slug: wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/openapi/betsolutions-wallet-api.yaml
consequence_counts:
  physical: 3
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Betsolutions Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallet/balance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallet/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallet/withdraw
operation_count: 6
overview: 'BetSolutions exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 2 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BetSolutions
provider_slug: betsolutions
slug: betsolutions-agentic-access
source_filename: betsolutions-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/betsolutions-wallet-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 1\n    acting: 5\n  by_consequence:\n    read: 1\n    physical: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /wallet/auth\n  method: get\n  operationId: authenticatePlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/deposit\n  method: post\n  operationId: depositFunds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/withdraw\n  method: post\n  operationId: withdrawFunds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/balance\n  method: post\n  operationId: getBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /game/list\n  method:\
  \ post\n  operationId: getGameList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /player/info\n  method: post\n  operationId: getPlayerInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/agentic-access/betsolutions-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
---
