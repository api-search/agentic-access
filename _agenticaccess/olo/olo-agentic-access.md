---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 4
api_specs:
- filename: olo-ordering-openapi.yml
  format: yaml
  label: Olo Ordering API
  slug: olo-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-ordering-openapi.yml
- filename: olo-ordering-openapi.yml
  format: yaml
  label: Olo Rails API
  slug: olo-rails
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-ordering-openapi.yml
- filename: olo-promotions-openapi.yml
  format: yaml
  label: Olo Loyalty API
  slug: olo-loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/openapi/olo-promotions-openapi.yml
- filename: olo-webhooks-asyncapi.yml
  format: yaml
  label: Olo Webhooks
  slug: olo-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/asyncapi/olo-webhooks-asyncapi.yml
consequence_counts:
  read: 4
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Olo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Olo exposes 12 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Olo
provider_slug: olo
slug: olo-agentic-access
source_filename: olo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/olo-ordering-openapi.yml, openapi/olo-promotions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 4\n    acting: 8\n  by_consequence:\n    read: 4\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1.1/brand\n  method: get\n  operationId: getBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/users/exists\n  method: post\n  operationId: checkUserExists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/vendorexport/status\n  method: get\n  operationId: getVendorExportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/baskets/create\n  method: post\n  operationId: createBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /promotions/accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /promotions/accounts\n  method: get\n  operationId: findAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /promotions/accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /promotions/validate\n  method: post\n  operationId: validatePromotions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /promotions/redemptions\n  method: post\n  operationId: redeemPromotions\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /promotions/redemptions/{redemptionId}\n  method: delete\n  operationId: voidRedemption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /promotions/accruals\n  method: post\n  operationId: accruePoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /promotions/accruals/{accrualId}\n  method:\
  \ delete\n  operationId: voidAccrual\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olo/refs/heads/main/agentic-access/olo-agentic-access.yml
summary_line: 12 operations · 8 acting
tags:
- Food Service
- Restaurants
- Online Ordering
- Delivery
- Point of Sale
- Hospitality
- Payments
- Loyalty
- Marketing
---
