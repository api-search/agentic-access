---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 11
api_specs:
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Users & KYC API
  slug: pomelo-users-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Cards API
  slug: pomelo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Card Accounts API
  slug: pomelo-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Transactions API
  slug: pomelo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Authorizations API
  slug: pomelo-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Transfers API
  slug: pomelo-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Webhooks API
  slug: pomelo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pomelo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /cards/v1/{id}/shipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/v1
operation_count: 20
overview: 'Pomelo exposes 20 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 7 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pomelo
provider_slug: pomelo
slug: pomelo-agentic-access
source_filename: pomelo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pomelo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 9\n    connected: 11\n  by_consequence:\n    write: 7\n    read: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/v1\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/v1\n  method: get\n  operationId: searchUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/v1/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/v1/{id}\n  method: patch\n  operationId: modifyUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/v1\n\
  \  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/v1\n  method: get\n  operationId: searchCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/v1/{id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/v1/{id}\n  method: patch\n  operationId: updateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/v1/activation\n  method: post\n  operationId: activateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/v1/batches\n  method: post\n  operationId: createCardBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/v1/{id}/shipment\n  method: patch\n  operationId: updateCardShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/v1\n  method: get\n  operationId: searchCardAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/v1/{id}\n  method: get\n  operationId: getCardAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/v1/{id}/movements\n  method: get\n  operationId: listAccountMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/v1\n  method: get\n  operationId: searchTransactions\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/v1/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/v1\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/v1\n  method: get\n  operationId: searchTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/v1/{id}\n  method: get\n  operationId: getTransfer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/agentic-access/pomelo-agentic-access.yml
summary_line: 20 operations · 9 acting
tags:
- Fintech
- Card Issuing
- Embedded Finance
- Payments
- Latin America
---
