---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 14
api_specs:
- filename: backbase-approve-api-openapi.yml
  format: yaml
  label: BackBase Approve API
  slug: backbase-approve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-approve-api-openapi.yml
- filename: backbase-bbt-api-openapi.yml
  format: yaml
  label: BackBase Bbt API
  slug: backbase-bbt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-bbt-api-openapi.yml
- filename: backbase-patch-api-openapi.yml
  format: yaml
  label: BackBase Patch API
  slug: backbase-patch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-patch-api-openapi.yml
- filename: backbase-payment-orders-api-openapi.yml
  format: yaml
  label: BackBase Payment Orders API
  slug: backbase-payment-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-payment-orders-api-openapi.yml
- filename: backbase-test-api-openapi.yml
  format: yaml
  label: BackBase Test API
  slug: backbase-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-test-api-openapi.yml
- filename: backbase-utility-api-openapi.yml
  format: yaml
  label: BackBase Utility API
  slug: backbase-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-utility-api-openapi.yml
- filename: backbase-validate-api-openapi.yml
  format: yaml
  label: BackBase Validate API
  slug: backbase-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-validate-api-openapi.yml
- filename: backbase-wallet-api-openapi.yml
  format: yaml
  label: BackBase Wallet API
  slug: backbase-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/openapi/backbase-wallet-api-openapi.yml
consequence_counts:
  physical: 11
  read: 14
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Backbase Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-api/v2/payment-orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client-api/v2/payment-orders/bulk-approvals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-api/v2/payment-orders/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-api/v2/payment-orders/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client-api/v2/payment-orders/{paymentOrderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /client-api/v2/payment-orders/{paymentOrderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client-api/v2/payment-orders/{paymentOrderId}/approvals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /client-api/v2/payment-orders/{paymentOrderId}/approvals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-api/v2/payment-orders/{paymentOrderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallet/paymentcards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /wallet/paymentcards/{cardId}
operation_count: 26
overview: 'BackBase exposes 26 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 1 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BackBase
provider_slug: backbase
slug: backbase-agentic-access
source_filename: backbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: generated\nsource: openapi/backbase-approve-api-openapi.yml, openapi/backbase-bbt-api-openapi.yml, openapi/backbase-patch-api-openapi.yml,\n  openapi/backbase-payment-orders-api-openapi.yml, openapi/backbase-test-api-openapi.yml, openapi/backbase-utility-api-openapi.yml,\n  openapi/backbase-validate-api-openapi.yml, openapi/backbase-wallet-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 12\n    connected: 14\n  by_consequence:\n    physical: 11\n    read: 14\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /client-api/v2/payment-orders/{paymentOrderId}/approvals\n  method: put\n  operationId: putApprovalsByPaymentOrderId\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bbt/build-info\n  method: get\n  operationId: getBuildinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patch\n  method: patch\n  operationId: patchPatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders\n  method: get\n  operationId: getPaymentOrders\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-api/v2/payment-orders\n  method: post\n  operationId: postPaymentOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders/validate\n  method: post\n  operationId: postValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders/bulk-approvals\n  method:\
  \ put\n  operationId: putBulkApprovals\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders/approvals\n  method: get\n  operationId: getApprovablePaymentOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-api/v2/payment-orders/{paymentOrderId}\n  method: get\n  operationId: getPaymentOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-api/v2/payment-orders/{paymentOrderId}\n  method: put\n  operationId: putPaymentOrderById\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders/{paymentOrderId}\n  method: delete\n  operationId: deletePaymentOrderById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders/{paymentOrderId}/approvals\n  method: put\n  operationId: putApprovalsByPaymentOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders/{paymentOrderId}/cancel\n  method: post\n  operationId: postCancelByPaymentOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-api/v2/payment-orders/currencies\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-api/v2/payment-orders/rate\n  method: get\n  operationId: getRate\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test/required-boolean-query-param\n  method: get\n  operationId: getRequiredbooleanqueryparam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test/values\n  method: get\n  operationId: getValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test/headers\n  method: get\n  operationId: getHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test/date-query-params\n  method: get\n  operationId: getDatequeryparams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /client-api/v2/payment-orders/currencies\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-api/v2/payment-orders/rate\n  method: get\n  operationId: getRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-api/v2/payment-orders/validate\n  method: post\n  operationId: postValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/paymentcards\n  method: get\n  operationId: getPaymentcards\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/paymentcards\n  method: post\n  operationId: postPaymentcards\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/paymentcards/{cardId}\n  method: get\n  operationId: getCardIdByCardId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/paymentcards/{cardId}\n  method: delete\n  operationId: deleteCardIdByCardId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backbase/refs/heads/main/agentic-access/backbase-agentic-access.yml
summary_line: 26 operations · 12 acting
tags:
- Banking
- Fintech
- Digital Banking
- API Platform
- AI-Native
---
