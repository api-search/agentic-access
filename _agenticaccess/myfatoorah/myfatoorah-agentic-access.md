---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: myfatoorah-invoicing-api-openapi.yml
  format: yaml
  label: MyFatoorah Invoicing API
  slug: myfatoorah-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-invoicing-api-openapi.yml
- filename: myfatoorah-payment-status-api-openapi.yml
  format: yaml
  label: MyFatoorah Payment Status API
  slug: myfatoorah-payment-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-payment-status-api-openapi.yml
- filename: myfatoorah-payments-api-openapi.yml
  format: yaml
  label: MyFatoorah Payments API
  slug: myfatoorah-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-payments-api-openapi.yml
- filename: myfatoorah-recurring-api-openapi.yml
  format: yaml
  label: MyFatoorah Recurring API
  slug: myfatoorah-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-recurring-api-openapi.yml
- filename: myfatoorah-refunds-api-openapi.yml
  format: yaml
  label: MyFatoorah Refunds API
  slug: myfatoorah-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-refunds-api-openapi.yml
- filename: myfatoorah-sessions-api-openapi.yml
  format: yaml
  label: MyFatoorah Sessions API
  slug: myfatoorah-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-sessions-api-openapi.yml
- filename: myfatoorah-shipping-api-openapi.yml
  format: yaml
  label: MyFatoorah Shipping API
  slug: myfatoorah-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-shipping-api-openapi.yml
- filename: myfatoorah-suppliers-api-openapi.yml
  format: yaml
  label: MyFatoorah Suppliers API
  slug: myfatoorah-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-suppliers-api-openapi.yml
- filename: myfatoorah-webhooks-api-openapi.yml
  format: yaml
  label: MyFatoorah Webhooks API
  slug: myfatoorah-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/openapi/myfatoorah-webhooks-api-openapi.yml
consequence_counts:
  physical: 7
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Myfatoorah Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /CancelRecurringPayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ExecutePayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /GetRefundStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /InitiatePayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /MakeRefund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /MakeSupplierRefund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /SendPayment
operation_count: 14
overview: 'MyFatoorah exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 2 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MyFatoorah
provider_slug: myfatoorah
slug: myfatoorah-agentic-access
source_filename: myfatoorah-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/myfatoorah-invoicing-api-openapi.yml, openapi/myfatoorah-payment-status-api-openapi.yml,\n  openapi/myfatoorah-payments-api-openapi.yml, openapi/myfatoorah-recurring-api-openapi.yml,\n  openapi/myfatoorah-refunds-api-openapi.yml, openapi/myfatoorah-sessions-api-openapi.yml, openapi/myfatoorah-shipping-api-openapi.yml,\n  openapi/myfatoorah-suppliers-api-openapi.yml, openapi/myfatoorah-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 9\n    connected: 5\n  by_consequence:\n    physical: 7\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /SendPayment\n  method: post\n  operationId: sendPayment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetPaymentStatus\n  method: post\n  operationId: getPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /InitiatePayment\n  method: post\n  operationId: initiatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ExecutePayment\n  method: post\n\
  \  operationId: executePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetRecurringPayment\n  method: post\n  operationId: getRecurringPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CancelRecurringPayment\n  method: post\n  operationId: cancelRecurringPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /MakeRefund\n  method: post\n  operationId: makeRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetRefundStatus\n  method: post\n  operationId: getRefundStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /MakeSupplierRefund\n  method: post\n  operationId: makeSupplierRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /InitiateSession\n  method: post\n  operationId: initiateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CancelToken\n  method: post\n  operationId: cancelToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetCities\n  method: post\n  operationId: getCities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GetSuppliers\n  method: post\n  operationId: getSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GetWebhooks\n  method: post\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myfatoorah/refs/heads/main/agentic-access/myfatoorah-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Payments
- Payment Gateway
- Kuwait
- GCC
- MENA
- KNET
- mada
- Benefits
- Invoices
- Cards
- Fintech
---
