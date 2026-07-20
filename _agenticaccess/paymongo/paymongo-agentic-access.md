---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 13
api_specs:
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Intents API
  slug: paymongo-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Methods API
  slug: paymongo-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payments API
  slug: paymongo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Sources API
  slug: paymongo-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Checkout Sessions API
  slug: paymongo-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Payment Links API
  slug: paymongo-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Customers API
  slug: paymongo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Refunds API
  slug: paymongo-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo QR Ph API
  slug: paymongo-qr-ph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Webhooks API
  slug: paymongo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Subscriptions & Plans API
  slug: paymongo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Money Movement API
  slug: paymongo-money-movement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Forex API
  slug: paymongo-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
- filename: paymongo-openapi.yml
  format: yaml
  label: PayMongo Fraud Detection API
  slug: paymongo-fraud-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/openapi/paymongo-openapi.yml
consequence_counts:
  read: 13
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Money-moving operations (attaching a payment, issuing a refund) default to human-in-the-loop required because they authorize or reverse funds. See research/curity/agentic-access/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Paymongo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'PayMongo exposes 28 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 15 write.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PayMongo
provider_slug: paymongo
slug: paymongo-agentic-access
source_filename: paymongo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/paymongo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Money-moving operations (attaching a payment, issuing a refund) default\n  to human-in-the-loop required because they authorize or reverse funds. See research/curity/agentic-access/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 15\n    connected: 13\n  by_consequence:\n    write: 15\n    read: 13\n  human_in_the_loop_required: 2\noperations:\n- path: /payment_intents\n  method: post\n  operationId: createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /payment_intents/{id}\n  method: get\n  operationId: retrievePaymentIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_intents/{id}/attach\n  method: post\n  operationId: attachPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /payment_methods\n  method: post\n  operationId: createPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - pii\n    audit: required\n- path: /payment_methods/{id}\n\
  \  method: get\n  operationId: retrievePaymentMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{id}\n  method: get\n  operationId: retrievePayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: post\n  operationId: createSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources/{id}\n  method: get\n\
  \  operationId: retrieveSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout_sessions\n  method: post\n  operationId: createCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout_sessions/{id}\n  method: get\n  operationId: retrieveCheckoutSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout_sessions/{id}/expire\n  method: post\n  operationId: expireCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /links/{id}\n  method: get\n  operationId: retrievePaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - pii\n    audit:\
  \ required\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: get\n  operationId: retrieveCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - pii\n    audit: required\n- path: /customers/{id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/{id}\n  method: get\n  operationId: retrieveRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qr_codes/static\n  method: post\n  operationId: createStaticQrPh\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: get\n  operationId: retrieveWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}/enable\n  method:\
  \ post\n  operationId: enableWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /webhooks/{id}/disable\n  method: post\n  operationId: disableWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymongo/refs/heads/main/agentic-access/paymongo-agentic-access.yml
summary_line: 28 operations · 15 acting · 2 human-in-the-loop
tags:
- Payments
- FinTech
- Philippines
- Southeast Asia
- GCash
- E-Wallet
- Card Payments
---
