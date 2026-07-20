---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 21
api_specs:
- filename: bitski-nft-service-openapi-original.json
  format: json
  label: Bitski NFT Service APIs
  slug: bitski-nft-service-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-nft-service-openapi-original.json
- filename: bitski-wallet-experience-openapi-original.json
  format: json
  label: Bitski Wallet Experience APIs
  slug: bitski-wallet-experience-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/openapi/bitski-wallet-experience-openapi-original.json
consequence_counts:
  physical: 6
  read: 21
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bitski Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/apps/{app_id}/contracts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/apps/{app_id}/fulfillments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/apps/{app_id}/fulfillments/{fulfillment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/orders/{order_id}/payments/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/users/{user_id}/payment-methods
operation_count: 35
overview: 'Bitski exposes 35 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 8 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bitski
provider_slug: bitski
slug: bitski-agentic-access
source_filename: bitski-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/bitski-nft-service-openapi-original.json, openapi/bitski-wallet-experience-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 21\n    acting: 14\n  by_consequence:\n    read: 21\n    physical: 6\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /contracts/{contract_id}/metadata\n  method: get\n  operationId: contract_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/token-metadata/{token_id}\n  method: get\n  operationId: token_metadata\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/contracts\n  method: get\n  operationId: list_contracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/contracts\n  method: post\n  operationId: create_contract\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - apps\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/contracts/{contract_id}\n  method: get\n  operationId: get_contract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - apps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/contracts/{contract_id}\n  method: patch\n  operationId: patch_contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apps\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/fulfillments\n  method: post\n  operationId: create_fulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/fulfillments/{fulfillment_id}\n  method: get\n  operationId: get_fulfillment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/fulfillments/{fulfillment_id}\n  method: patch\n  operationId: patch_fulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/gates\n  method: get\n  operationId: list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/gates\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apps\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/gates/{gate_id}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/gates/{gate_id}\n  method: put\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apps\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/token-templates\n  method: get\n  operationId: get_token_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - apps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/token-templates\n  method: post\n  operationId: create_token_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apps\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/token-templates/{token_template_id}\n  method: get\n  operationId: token_template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/token-templates/{token_template_id}\n  method: put\n  operationId: update_token_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apps\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/tokens\n  method: get\n  operationId: get_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/tokens\n  method: post\n  operationId: create_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apps\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/tokens/{token_id}\n  method: get\n  operationId: get_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - apps\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/tokens/{token_id}\n  method: patch\n  operationId: update_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - apps\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auctions/{auction_id}\n  method: get\n  operationId: get_auction_info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claim-codes/claims/unclaimed\n  method: get\n  operationId: get_unclaimed_codes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claim-codes/{claim_code_id_or_code}\n  method: get\n  operationId: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gates/check\n  method: get\n  operationId: check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders\n  method: post\n  operationId: create_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - commerce\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{order_id}\n  method: get\n  operationId: get_order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{order_id}/payments/{payment_id}\n  method: patch\n  operationId: patch_order_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - commerce\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products\n  method: get\n  operationId: list_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/products/{product_id}\n  method: get\n  operationId: get_product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{store_id}\n  method: get\n  operationId: store_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{user_id}/payment-methods\n  method: get\n  operationId: list_payment_methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{user_id}/payment-methods\n  method: post\n  operationId: add_payment_method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - commerce\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/activities\n  method: get\n  operationId: list_activities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitski/refs/heads/main/agentic-access/bitski-agentic-access.yml
summary_line: 35 operations · 14 acting
tags:
- Web3
- Crypto Wallet
- Wallet as a Service
- NFT
- Blockchain
- Authentication
- OAuth
- Payments
- Developer Tools
- Company
---
