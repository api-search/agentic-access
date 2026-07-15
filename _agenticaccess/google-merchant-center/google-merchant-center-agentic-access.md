---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Merchant API
  slug: google-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 3
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Merchant Center Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Google Merchant Center exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Merchant Center
provider_slug: google-merchant-center
slug: google-merchant-center-agentic-access
source_filename: google-merchant-center-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 3\n    acting: 4\n  by_consequence:\n    read: 3\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/v1/{parent}/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/content\n- path: /products/v1/{parent}/productInputs\n  method: post\n  operationId: insertProductInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/content\n- path: /products/v1/{name}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/content\n- path: /inventories/v1/{parent}/localInventories\n  method: post\n  operationId: insertLocalInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/content\n- path: /promotions/v1/{parent}/promotions\n\
  \  method: get\n  operationId: listPromotions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/content\n- path: /promotions/v1/{parent}/promotions\n  method: post\n  operationId: createPromotion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/content\n- path: /reports/v1/{parent}/reports:search\n  method: post\n  operationId: searchReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/content\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/agentic-access/google-merchant-center-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- E-Commerce
- Google Shopping
- Inventory
- Merchant Center
- Products
- Promotions
- Shopping
---
