---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 8
api_specs:
- filename: kushki-card-payments-api-openapi.yml
  format: yaml
  label: Kushki Card Payments API
  slug: kushki-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-card-payments-api-openapi.yml
- filename: kushki-subscriptions-api-openapi.yml
  format: yaml
  label: Kushki Subscriptions API
  slug: kushki-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-subscriptions-api-openapi.yml
- filename: kushki-transfer-payments-api-openapi.yml
  format: yaml
  label: Kushki Transfer Payments API
  slug: kushki-transfer-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-transfer-payments-api-openapi.yml
- filename: kushki-cash-payments-api-openapi.yml
  format: yaml
  label: Kushki Cash Payments API
  slug: kushki-cash-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-cash-payments-api-openapi.yml
- filename: kushki-payouts-api-openapi.yml
  format: yaml
  label: Kushki Payouts API
  slug: kushki-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-payouts-api-openapi.yml
- filename: kushki-card-present-api-openapi.yml
  format: yaml
  label: Kushki Card Present API
  slug: kushki-card-present-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-card-present-api-openapi.yml
- filename: kushki-merchants-api-openapi.yml
  format: yaml
  label: Kushki Merchants and Branches API
  slug: kushki-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-merchants-api-openapi.yml
consequence_counts:
  physical: 13
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kushki Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card/v1/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card/v1/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card/v1/deferred
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cardpresent/v1/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cardpresent/v1/charges/{ticketNumber}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cash/v1/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /cash/v1/charges/{ticketNumber}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/transfer/v1/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/transfer/v1/init
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscriptions/v1/card/{subscriptionId}/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/v1/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/v1/init
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/charges/{ticketNumber}
operation_count: 28
overview: 'Kushki exposes 28 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 7 write, and 13 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kushki
provider_slug: kushki
slug: kushki-agentic-access
source_filename: kushki-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kushki-card-payments-api-openapi.yml, openapi/kushki-card-present-api-openapi.yml,\n  openapi/kushki-cash-payments-api-openapi.yml, openapi/kushki-merchants-api-openapi.yml, openapi/kushki-payouts-api-openapi.yml,\n  openapi/kushki-subscriptions-api-openapi.yml, openapi/kushki-transfer-payments-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 20\n    connected: 8\n  by_consequence:\n    write: 7\n    physical: 13\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /card/v1/tokens\n  method: post\n  operationId: createCardToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card/v1/charges\n  method: post\n  operationId: createCardCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card/v1/preAuthorization\n  method: post\n  operationId: preAuthorizeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card/v1/capture\n  method: post\n  operationId:\
  \ captureCardCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card/v1/deferred\n  method: post\n  operationId: createDeferredCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/charges/{ticketNumber}\n  method: delete\n  operationId: voidOrRefundCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardpresent/v1/terminals\n  method: get\n  operationId: listTerminals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardpresent/v1/terminals/{terminalId}\n  method: get\n  operationId: getTerminal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardpresent/v1/charges\n  method: post\n  operationId: createCardPresentCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /cardpresent/v1/charges/{ticketNumber}/void\n  method: post\n  operationId: voidCardPresentCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cash/v1/charges\n  method: post\n  operationId: createCashCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cash/v1/charges/{ticketNumber}\n  method: get\n  operationId: getCashCharge\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cash/v1/charges/{ticketNumber}\n  method: delete\n  operationId: cancelCashCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/v1/branches\n  method: get\n  operationId: listBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/v1/branches\n  method: post\n  operationId: createBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/v1/branches/{branchId}\n  method: get\n  operationId: getBranch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/v1/branches/{branchId}\n  method: put\n  operationId: updateBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/transfer/v1/init\n  method: post\n  operationId: initPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/transfer/v1/payouts/{payoutId}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/transfer/v1/batch\n  method: post\n  operationId: createPayoutBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/card\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/card/{subscriptionId}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/v1/card/{subscriptionId}\n  method: put\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/card/{subscriptionId}\n  method: delete\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/card/{subscriptionId}/charge\n  method: post\n  operationId: chargeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/v1/init\n  method: post\n  operationId: initTransferCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/v1/charge\n\
  \  method: post\n  operationId: confirmTransferCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/v1/charges/{ticketNumber}\n  method: get\n  operationId: getTransferCharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/agentic-access/kushki-agentic-access.yml
summary_line: 28 operations · 20 acting
tags:
- Payments
- LatAm
- Andean Region
- Card Payments
- Subscriptions
- Cash
- Bank Transfers
- Payouts
- PSE
- Webpay
- SPEI
- PIX
- OXXO
- PagoEfectivo
- Fintech
- Ecuador
- Colombia
- Peru
- Chile
- Mexico
- Brazil
---
