---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 19
api_specs:
- filename: datanomik-openbanking-openapi.json
  format: json
  label: Datanomik OpenBanking API
  slug: datanomik-openbanking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-openbanking-openapi.json
- filename: datanomik-remuneration-openapi.json
  format: json
  label: Datanomik Treasury / Remuneration API
  slug: datanomik-treasury-remuneration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-remuneration-openapi.json
consequence_counts:
  read: 19
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Datanomik Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Datanomik exposes 21 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Datanomik
provider_slug: datanomik
slug: datanomik-agentic-access
source_filename: datanomik-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/datanomik-openbanking-openapi.json, openapi/datanomik-remuneration-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 19\n    acting: 2\n  by_consequence:\n    read: 19\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accounts/position\n  method: get\n  operationId: account-position\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions\n  method: post\n  operationId: create-manual-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}\n  method: get\n  operationId: detail-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/general-owners/{id}\n  method: get\n  operationId: detail-general-owner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{paymentId}/receipt\n  method: get\n  operationId: get_v1-payments-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pix-transactions/{pixTransactionId}/receipt\n  method: get\n  operationId: get_v1-pix-transactions-1\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/investments/movements/{movementId}/receipt\n  method: get\n  operationId: get_v1-investments-movements-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-slips\n  method: get\n  operationId: get_v1-payments-2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: get\n  operationId: list-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/details\n  method: get\n  operationId: get_v1-applications-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/links/sync/assets/{linkId}\n  method: post\n  operationId: list-assets-copy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/balances/history\n  method: get\n  operationId: list-balances-copy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/general-owners\n  method: get\n  operationId: list-general-owners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/investments/movements\n  method: get\n  operationId: get_v1-investments-movements\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/investments/history\n  method: get\n  operationId: list-investments-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/investments\n  method: get\n  operationId: list-investments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments\n  method: get\n  operationId: get_v1-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pix-transactions\n  method: get\n  operationId: get_v1-pix-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/accounts/\n  method: get\n  operationId: detail-remuneration-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions\n  method: get\n  operationId: list-remunerated-account-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/accounts\n  method: get\n  operationId: list-remuneration-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/agentic-access/datanomik-agentic-access.yml
summary_line: 21 operations · 2 acting
tags:
- Company
- Open Finance
- Open Banking
- Treasury Management
- Cash Management
- Payments
- PIX
- Financial Data
- Bank Connectivity
- Brazil
- LatAm
- Fintech
---
