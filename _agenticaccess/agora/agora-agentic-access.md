---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: agora-accounts-api-openapi.yml
  format: yaml
  label: Agora Accounts API
  slug: agora-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/openapi/agora-accounts-api-openapi.yml
- filename: agora-auth-api-openapi.yml
  format: yaml
  label: Agora Auth API
  slug: agora-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/openapi/agora-auth-api-openapi.yml
- filename: agora-metrics-api-openapi.yml
  format: yaml
  label: Agora Metrics API
  slug: agora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/openapi/agora-metrics-api-openapi.yml
- filename: agora-routes-api-openapi.yml
  format: yaml
  label: Agora Routes API
  slug: agora-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/openapi/agora-routes-api-openapi.yml
- filename: agora-transactions-api-openapi.yml
  format: yaml
  label: Agora Transactions API
  slug: agora-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/openapi/agora-transactions-api-openapi.yml
consequence_counts:
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agora Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Agora exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agora
provider_slug: agora
slug: agora-agentic-access
source_filename: agora-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/agora-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 4\n    connected: 8\n  by_consequence:\n    write: 4\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v0/auth/token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/metrics\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/metrics/total-supply\n  method: get\n  operationId: totalsupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/metrics/circulating-supply\n  method: get\n  operationId: circulatingsupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/accounts\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/accounts\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/accounts/{accountId}\n  method: put\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/routes\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/routes\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/routes/{routeId}\n  method:\
  \ get\n  operationId: getbyid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/transactions\n  method: get\n  operationId: list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/transactions/{txnId}\n  method: get\n  operationId: getbyid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/agentic-access/agora-agentic-access.yml
summary_line: 12 operations · 4 acting
tags:
- Company
- Fintech
- Stablecoins
- Digital Dollar
- Payments
- Cryptocurrency
- Blockchain
- AUSD
---
