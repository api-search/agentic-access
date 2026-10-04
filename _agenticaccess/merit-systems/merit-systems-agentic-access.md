---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: merit-systems-balances-api-openapi.yml
  format: yaml
  label: Merit Systems Balances API
  slug: merit-systems-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-balances-api-openapi.yml
- filename: merit-systems-invite-codes-api-openapi.yml
  format: yaml
  label: Merit Systems Invite Codes API
  slug: merit-systems-invite-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-invite-codes-api-openapi.yml
- filename: merit-systems-organizations-api-openapi.yml
  format: yaml
  label: Merit Systems Organizations API
  slug: merit-systems-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-organizations-api-openapi.yml
- filename: merit-systems-payments-api-openapi.yml
  format: yaml
  label: Merit Systems Payments API
  slug: merit-systems-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-payments-api-openapi.yml
- filename: merit-systems-search-api-openapi.yml
  format: yaml
  label: Merit Systems Search API
  slug: merit-systems-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-search-api-openapi.yml
- filename: merit-systems-send-api-openapi.yml
  format: yaml
  label: Merit Systems Send API
  slug: merit-systems-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/openapi/merit-systems-send-api-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Merit Systems Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/send
operation_count: 9
overview: 'Merit Systems exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Merit Systems
provider_slug: merit-systems
slug: merit-systems-agentic-access
source_filename: merit-systems-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/merit-systems-balances-api-openapi.yml, openapi/merit-systems-invite-codes-api-openapi.yml,\n  openapi/merit-systems-organizations-api-openapi.yml, openapi/merit-systems-payments-api-openapi.yml,\n  openapi/merit-systems-search-api-openapi.yml, openapi/merit-systems-send-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /users/{login}/balance\n  method: get\n  operationId: getUserBalanceByLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /user/{user_id}/balance\n  method: get\n  operationId: getUserBalanceByGithubId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/balance\n  method: get\n  operationId: getRepoBalanceByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repositories/{repo_id}/balance\n  method: get\n  operationId: getRepoBalanceByRepoId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invite-codes\n  method: post\n  operationId: invite-codes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations\n  method: get\n  operationId: organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{user_id}/payments\n  method: get\n  operationId: getPaymentsBySender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/send\n  method: post\n  operationId: send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merit-systems/refs/heads/main/agentic-access/merit-systems-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Company
- Agentic Commerce
- Payments
- x402
- Micropayments
- MCP
- Stablecoins
- API Discovery
- Open Source
- Developer Tools
---
