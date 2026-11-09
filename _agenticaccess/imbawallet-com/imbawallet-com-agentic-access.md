---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 10
api_specs:
- filename: imbawallet-com-auth-api-openapi.yml
  format: yaml
  label: imbawallet-com Auth API
  slug: imbawallet-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-auth-api-openapi.yml
- filename: imbawallet-com-balance-api-openapi.yml
  format: yaml
  label: imbawallet-com Balance API
  slug: imbawallet-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-balance-api-openapi.yml
- filename: imbawallet-com-cards-api-openapi.yml
  format: yaml
  label: imbawallet-com Cards API
  slug: imbawallet-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-cards-api-openapi.yml
- filename: imbawallet-com-catalog-api-openapi.yml
  format: yaml
  label: imbawallet-com Catalog API
  slug: imbawallet-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-catalog-api-openapi.yml
- filename: imbawallet-com-deposit-api-openapi.yml
  format: yaml
  label: imbawallet-com Deposit API
  slug: imbawallet-com-deposit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-deposit-api-openapi.yml
- filename: imbawallet-com-withdrawals-api-openapi.yml
  format: yaml
  label: imbawallet-com Withdrawals API
  slug: imbawallet-com-withdrawals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-withdrawals-api-openapi.yml
consequence_counts:
  physical: 4
  read: 10
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Imbawallet Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/deposit_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/partner/deposit_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/partner/withdraw_create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/purchase
operation_count: 24
overview: 'imbawallet-com exposes 24 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 10 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: imbawallet-com
provider_slug: imbawallet-com
slug: imbawallet-com-agentic-access
source_filename: imbawallet-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/agent.openapi.yaml, openapi/partner.openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 14\n    connected: 10\n  by_consequence:\n    write: 10\n    read: 10\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/v1/agent/register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/agent/token\n  method: post\n  operationId: createAgentAccessToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/partner/jwks\n  method: get\n  operationId: getSharedJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/v1/agent/webhook\n  method: patch\n  operationId: patchAgentWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/agent/hmac/rotate\n  method: post\n  operationId: rotateAgentHmac\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deposit_address\n  method: post\n  operationId: getAgentDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deposit_address\n  method: get\n  operationId: getAgentBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/card_products\n  method: post\n  operationId: listAgentCardProducts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cards\n  method: post\n  operationId: listAgentCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pin/create_card\n  method: post\n  operationId: createAgentCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pin/topup_card\n  method: post\n  operationId: topupAgentCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/offers\n  method: post\n  operationId: listAgentGiftOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/purchase\n  method: post\n  operationId: purchaseAgentGift\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/partner/token\n  method: post\n  operationId: createPartnerAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/balance\n\
  \  method: post\n  operationId: getPartnerBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partner/deposit_address\n  method: post\n  operationId: getPartnerDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/withdraw_create\n  method: post\n  operationId: createPartnerWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/partner/card_products\n  method: post\n  operationId: listPartnerCardProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partner/card_list\n  method: post\n  operationId: listPartnerCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partner/card_issue\n  method: post\n  operationId: issuePartnerCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/card_get\n  method: post\n  operationId: getPartnerCard\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partner/card_balance\n  method: post\n  operationId: getPartnerCardBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partner/card_topup\n  method: post\n  operationId: createPartnerCardTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/card_freeze\n  method: post\n  operationId: freezePartnerCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/imbawallet-com/agentic-access/imbawallet-com-agentic-access.yml
summary_line: 24 operations · 14 acting
tags:
- Fintech
- Payments
- Cryptocurrency
- Virtual Cards
- Wallets
---
