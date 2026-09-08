---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 2
api_specs:
- filename: bolt-financial-account-api-openapi.yml
  format: yaml
  label: Bolt Financial Account API
  slug: bolt-financial-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-account-api-openapi.yml
- filename: bolt-financial-callbacks-api-openapi.yml
  format: yaml
  label: Bolt Financial Callbacks API
  slug: bolt-financial-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-callbacks-api-openapi.yml
- filename: bolt-financial-configuration-api-openapi.yml
  format: yaml
  label: Bolt Financial Configuration API
  slug: bolt-financial-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-configuration-api-openapi.yml
- filename: bolt-financial-oauth-api-openapi.yml
  format: yaml
  label: Bolt Financial O Auth API
  slug: bolt-financial-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-oauth-api-openapi.yml
- filename: bolt-financial-orders-api-openapi.yml
  format: yaml
  label: Bolt Financial Orders API
  slug: bolt-financial-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-orders-api-openapi.yml
- filename: bolt-financial-payments-api-openapi.yml
  format: yaml
  label: Bolt Financial Payments API
  slug: bolt-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-payments-api-openapi.yml
- filename: bolt-financial-statements-api-openapi.yml
  format: yaml
  label: Bolt Financial Statements API
  slug: bolt-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-statements-api-openapi.yml
- filename: bolt-financial-subscriptions-api-openapi.yml
  format: yaml
  label: Bolt Financial Subscriptions API
  slug: bolt-financial-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-subscriptions-api-openapi.yml
- filename: bolt-financial-testing-api-openapi.yml
  format: yaml
  label: Bolt Financial Testing API
  slug: bolt-financial-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-testing-api-openapi.yml
- filename: bolt-financial-tokenizer-api-openapi.yml
  format: yaml
  label: Bolt Financial Tokenizer API
  slug: bolt-financial-tokenizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-tokenizer-api-openapi.yml
- filename: bolt-financial-transactions-api-openapi.yml
  format: yaml
  label: Bolt Financial Transactions API
  slug: bolt-financial-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-transactions-api-openapi.yml
- filename: bolt-financial-webhooks-api-openapi.yml
  format: yaml
  label: Bolt Financial Webhooks API
  slug: bolt-financial-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-webhooks-api-openapi.yml
consequence_counts:
  physical: 7
  read: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bolt Financial Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /account/payment-methods/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /guest/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /guest/payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{id}
operation_count: 16
overview: 'Bolt Financial exposes 16 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 7 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bolt Financial
provider_slug: bolt-financial
slug: bolt-financial-agentic-access
source_filename: bolt-financial-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bolt-api-reference-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 2\n    acting: 14\n  by_consequence:\n    read: 2\n    write: 7\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /account\n  method: get\n  operationId: accountGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - bolt.account.manage\n    - bolt.account.view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/addresses\n  method: post\n  operationId: accountAddressCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - bolt.account.manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/addresses/{id}\n  method: put\n  operationId: accountAddressEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bolt.account.manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/addresses/{id}\n  method: delete\n  operationId: accountAddressDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bolt.account.manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /account/payment-methods\n  method: post\n  operationId: accountAddPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bolt.account.manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/payment-methods/{id}\n  method: delete\n  operationId: accountPaymentMethodDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bolt.account.manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: post\n  operationId:\
  \ paymentsInitialize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bolt.account.manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}\n  method: post\n  operationId: paymentsAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bolt.account.manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /guest/payments\n  method: post\n  operationId: guestPaymentsInitialize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /guest/payments/{id}\n  method: post\n  operationId: guestPaymentsAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: post\n  operationId: ordersCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: oauthGetToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /callbacks/accounts\n  method: post\n  operationId: callbackAccountUpsert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /testing/accounts\n  method: post\n  operationId: testingAccountCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /testing/accounts/phones\n  method: get\n  operationId: testingAccountPhoneGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /testing/credit-cards\n  method: post\n  operationId: testingCreditCardGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/agentic-access/bolt-financial-agentic-access.yml
summary_line: 16 operations · 14 acting
tags:
- Company
- Payments
- Checkout
- E-Commerce
- Fintech
- Subscription
- Tokenization
- Fraud
- Identity
- Webhook
---
