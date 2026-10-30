---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 18
api_specs:
- filename: monerium-addresses-api-openapi.yml
  format: yaml
  label: Monerium Addresses API
  slug: monerium-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-addresses-api-openapi.yml
- filename: monerium-auth-api-openapi.yml
  format: yaml
  label: Monerium Auth API
  slug: monerium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-auth-api-openapi.yml
- filename: monerium-files-api-openapi.yml
  format: yaml
  label: Monerium Files API
  slug: monerium-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-files-api-openapi.yml
- filename: monerium-ibans-api-openapi.yml
  format: yaml
  label: Monerium Ibans API
  slug: monerium-ibans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-ibans-api-openapi.yml
- filename: monerium-orders-api-openapi.yml
  format: yaml
  label: Monerium Orders API
  slug: monerium-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-orders-api-openapi.yml
- filename: monerium-profiles-api-openapi.yml
  format: yaml
  label: Monerium Profiles API
  slug: monerium-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-profiles-api-openapi.yml
- filename: monerium-signatures-api-openapi.yml
  format: yaml
  label: Monerium Signatures API
  slug: monerium-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-signatures-api-openapi.yml
- filename: monerium-start-api-openapi.yml
  format: yaml
  label: Monerium Start API
  slug: monerium-start-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-start-api-openapi.yml
- filename: monerium-swap-api-openapi.yml
  format: yaml
  label: Monerium Swap API
  slug: monerium-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-swap-api-openapi.yml
- filename: monerium-tokens-api-openapi.yml
  format: yaml
  label: Monerium Tokens API
  slug: monerium-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-tokens-api-openapi.yml
- filename: monerium-webhooks-api-openapi.yml
  format: yaml
  label: Monerium Webhooks API
  slug: monerium-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/openapi/monerium-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 18
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Monerium Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/payments
operation_count: 35
overview: 'Monerium exposes 35 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 15 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Monerium
provider_slug: monerium
slug: monerium-agentic-access
source_filename: monerium-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/monerium-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 18\n    acting: 17\n  by_consequence:\n    read: 18\n    write: 15\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: welcome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth\n  method: post\n  operationId: auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth\n  method: get\n  operationId: auth-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/context\n  method: get\n  operationId: auth-context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/token\n  method: post\n  operationId: auth-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: list-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: create-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{subscription}\n  method: patch\n  operationId: update-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /countries\n  method: get\n  operationId: get-countries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles\n  method: post\n  operationId:\
  \ create-profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles\n  method: get\n  operationId: profiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile}\n  method: get\n  operationId: profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile}/state\n  method: patch\n  operationId: close-profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile}/share\n  method: post\n  operationId: share-profile-kyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile}/details\n  method: patch\n  operationId: patch-profile-details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile}/form\n  method: patch\n  operationId: patch-profile-form\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile}/verifications\n  method: patch\n  operationId: patch-profile-verifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses\n  method: post\n  operationId: link-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses\n  method: get\n  operationId: addresses\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address}\n  method: get\n  operationId: address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances/{chain}/{address}\n  method: get\n  operationId: balances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ibans\n  method: post\n  operationId: request-iban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ibans\n  method: get\n  operationId: ibans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ibans/{iban}\n  method: get\n  operationId: iban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ibans/{iban}\n  method: patch\n  operationId: move-iban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: post\n  operationId: post-orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /orders\n  method: get\n  operationId: orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}\n  method: get\n  operationId: order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/payments\n  method: get\n  operationId: order-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/payments\n  method: post\n  operationId: post-order-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: upload-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens\n  method: get\n  operationId: tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/{chain}/{sellToken}/{buyToken}\n  method: get\n  operationId: create-swap-quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/accept\n  method: post\n  operationId: accept-swap-quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signatures\n  method: get\n  operationId: get-signatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monerium/refs/heads/main/agentic-access/monerium-agentic-access.yml
summary_line: 35 operations · 17 acting
tags:
- Payments
- Crypto
- FinTech
- DigitalCurrency
- API
---
