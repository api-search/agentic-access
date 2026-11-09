---
acting_count: 52
action_class_counts:
  acting: 52
  connected: 34
api_specs:
- filename: moneyhash-accounts-api-openapi.yml
  format: yaml
  label: MoneyHash Accounts API
  slug: moneyhash-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-accounts-api-openapi.yml
- filename: moneyhash-customers-api-openapi.yml
  format: yaml
  label: MoneyHash Customers API
  slug: moneyhash-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-customers-api-openapi.yml
- filename: moneyhash-direct-api-openapi.yml
  format: yaml
  label: MoneyHash Direct API
  slug: moneyhash-direct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-direct-api-openapi.yml
- filename: moneyhash-external-api-openapi.yml
  format: yaml
  label: MoneyHash External API
  slug: moneyhash-external-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-external-api-openapi.yml
- filename: moneyhash-loyalty-api-openapi.yml
  format: yaml
  label: MoneyHash Loyalty API
  slug: moneyhash-loyalty-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-loyalty-api-openapi.yml
- filename: moneyhash-payment-links-api-openapi.yml
  format: yaml
  label: MoneyHash Payment Links API
  slug: moneyhash-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-payment-links-api-openapi.yml
- filename: moneyhash-payments-api-openapi.yml
  format: yaml
  label: MoneyHash Payments API
  slug: moneyhash-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-payments-api-openapi.yml
- filename: moneyhash-payout-api-openapi.yml
  format: yaml
  label: MoneyHash Payout API
  slug: moneyhash-payout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-payout-api-openapi.yml
- filename: moneyhash-providers-api-openapi.yml
  format: yaml
  label: MoneyHash Providers API
  slug: moneyhash-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-providers-api-openapi.yml
- filename: moneyhash-reconciliations-api-openapi.yml
  format: yaml
  label: MoneyHash Reconciliations API
  slug: moneyhash-reconciliations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-reconciliations-api-openapi.yml
- filename: moneyhash-subscriptions-api-openapi.yml
  format: yaml
  label: MoneyHash Subscriptions API
  slug: moneyhash-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-subscriptions-api-openapi.yml
- filename: moneyhash-tokens-api-openapi.yml
  format: yaml
  label: MoneyHash Tokens API
  slug: moneyhash-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-tokens-api-openapi.yml
- filename: moneyhash-transactions-api-openapi.yml
  format: yaml
  label: MoneyHash Transactions API
  slug: moneyhash-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-transactions-api-openapi.yml
consequence_counts:
  physical: 29
  read: 34
  safety-critical: 1
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Moneyhash Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1.4/accounts/reset_access_token/{account_id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/direct/payments/intent/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/direct/payments/intents/{intent_id}/card_token/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/direct/payments/intents/{intent_id}/receipt/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/direct/payments/intents/{intent_id}/update-method/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/direct/payments/intents/{intent_id}/{payment_method}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/direct/payments/intents/{intent_id}/{payment_method}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/external/payments/intent/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/external/payments/intents/{intent_id}/card_token/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/external/payments/intents/{intent_id}/receipt/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/external/payments/intents/{intent_id}/update-method/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payment_links/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payment_links/{payment_link_id}/update-quantities/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/charge-card-token/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/intent/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/intent/{intent_id}/close/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/transactions/{trx_uuid}/anomalies/{anomaly_id}/resolve/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/transactions/{trx_uuid}/capture/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/transactions/{trx_uuid}/increase-authorization/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/transactions/{trx_uuid}/pull-status/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/transactions/{trx_uuid}/refund/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payments/transactions/{trx_uuid}/void/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payout/bulk/requests/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payout/bulk/requests/{id}/cancel/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.4/payout/bulk/requests/{request_id}/items/{merchant_reference}/cancel/
operation_count: 86
overview: 'MoneyHash exposes 86 API operations that an AI agent could call, of which 52 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 22 write, 29 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MoneyHash
provider_slug: moneyhash
slug: moneyhash-agentic-access
source_filename: moneyhash-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: generated\nsource: openapi/moneyhash-api-openapi.yml, openapi/moneyhash-vault-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 86\n  by_action_class:\n    connected: 34\n    acting: 52\n  by_consequence:\n    read: 34\n    write: 22\n    safety-critical: 1\n    physical: 29\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1.2/external/payments/intents/{intent_id}/get_current_state/\n  method: post\n  operationId: v1.2_external_payments_intents_get_current_state_create\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/accounts/\n  method: get\n  operationId: v1.1_accounts_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/accounts/\n  method: post\n  operationId: v1.1_accounts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/accounts/get-from-access-token/\n  method: get\n  operationId: v1.1_accounts_get_from_access_token_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/accounts/payment_methods/\n  method: post\n  operationId: v1.1_accounts_payment_methods_create\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/accounts/reset_access_token/{account_id}/\n  method: post\n  operationId: v1.1_accounts_reset_access_token_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1.4/accounts/{account_id}/transactions/\n  method: get\n  operationId: v1.1_accounts_transactions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/customers/\n  method: get\n  operationId: v1.1_customers_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/customers/\n\
  \  method: post\n  operationId: v1.1_customers_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/customers/{customer_uuid}/\n  method: patch\n  operationId: v1.1_customers_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/customers/{customer_uuid}/\n  method: get\n  operationId: v1.1_customers_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/customers/{customer_uuid}/\n\
  \  method: delete\n  operationId: v1.1_customers_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/customers/{customer_uuid}/cards/\n  method: get\n  operationId: v1.1_customers_cards_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/customers/{customer_uuid}/cards/{card_uuid_or_id}/\n  method: delete\n  operationId: v1.1_customers_cards_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1.4/customers/{customer_uuid}/subscriptions/\n  method: get\n  operationId: v1.1_customers_subscriptions_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/customers/{customer_uuid}/transactions/\n  method: get\n  operationId: v1.1_customers_transactions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/customers/{customer_uuid}/wallets/debit/\n  method: post\n  operationId: v1.1_customers_wallets_debit_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/customers/{customer_uuid}/wallets/top-up/\n\
  \  method: post\n  operationId: v1.1_customers_wallets_top_up_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/direct/payments/intent/\n  method: post\n  operationId: v1.1_direct_payments_intent_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/direct/payments/intents/{intent_id}/\n  method: get\n  operationId: v1.1_direct_payments_intents_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/direct/payments/intents/{intent_id}/card_token/\n  method: post\n  operationId: v1.1_direct_payments_intents_card_token_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/direct/payments/intents/{intent_id}/receipt/\n  method: post\n  operationId: v1.1_direct_payments_intents_receipt_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1.4/direct/payments/intents/{intent_id}/update-method/\n  method: post\n  operationId: v1.1_direct_payments_intents_update_method_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/direct/payments/intents/{intent_id}/{payment_method}/\n  method: post\n  operationId: v1.1_direct_payments_intents_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/external/payments/intent/\n\
  \  method: post\n  operationId: v1.1_external_payments_intent_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/external/payments/intents/{intent_id}/\n  method: get\n  operationId: v1.1_external_payments_intents_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/external/payments/intents/{intent_id}/card_token/\n  method: post\n  operationId: v1.1_external_payments_intents_card_token_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n \
  \     purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/external/payments/intents/{intent_id}/receipt/\n  method: post\n  operationId: v1.1_external_payments_intents_receipt_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/external/payments/intents/{intent_id}/update-method/\n  method: post\n  operationId: v1.1_external_payments_intents_update_method_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/loyalty/earn/\n  method: post\n  operationId: v1.1_loyalty_earn_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/loyalty/earn/{id}/\n  method: get\n  operationId: v1.1_loyalty_earn_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/loyalty/earn/{id}/reverse/\n  method: post\n  operationId: v1.1_loyalty_earn_reverse_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/loyalty/eligibility/\n  method: post\n  operationId: v1.1_loyalty_eligibility_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payment_links/\n  method: post\n  operationId: v1.1_payment_links_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payment_links/{payment_link_id}/status/\n  method: get\n  operationId:\
  \ v1.1_payment_links_status_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payment_links/{payment_link_id}/update-quantities/\n  method: post\n  operationId: v1.1_payment_links_update_quantities_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/charge-card-token/\n  method: post\n  operationId: v1.1_payments_charge_card_token_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/intent/\n  method: post\n  operationId: v1.1_payments_intent_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/intent/{intent_id}/\n  method: get\n  operationId: v1.1_payments_intent_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payments/intent/{intent_id}/close/\n  method: post\n  operationId: v1.1_payments_intent_close_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/intents/{intent_id}/transactions/\n  method: get\n  operationId: v1.1_payments_intents_transactions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payments/transactions/{trx_uuid}/\n  method: get\n  operationId: v1.1_payments_transactions_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payments/transactions/{trx_uuid}/anomalies/{anomaly_id}/resolve/\n  method: post\n  operationId: v1.1_payments_transactions_anomalies_resolve_create\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/transactions/{trx_uuid}/capture/\n  method: post\n  operationId: v1.1_payments_transactions_capture_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/transactions/{trx_uuid}/increase-authorization/\n  method: post\n  operationId: v1.1_payments_transactions_increase_authorization_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/transactions/{trx_uuid}/pull-status/\n  method: post\n  operationId: v1.1_payments_transactions_pull_status_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/transactions/{trx_uuid}/refund/\n  method: post\n  operationId: v1.1_payments_transactions_refund_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payments/transactions/{trx_uuid}/void/\n  method: post\n  operationId: v1.1_payments_transactions_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payout/bulk/requests/\n  method: get\n  operationId: v1.1_payout_bulk_requests_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payout/bulk/requests/\n  method: post\n  operationId: v1.1_payout_bulk_requests_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payout/bulk/requests/{id}/\n  method: get\n  operationId: v1.1_payout_bulk_requests_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payout/bulk/requests/{id}/cancel/\n  method: post\n  operationId: v1.1_payout_bulk_requests_cancel_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1.4/payout/bulk/requests/{id}/items/\n  method: get\n  operationId: v1.1_payout_bulk_requests_items_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payout/bulk/requests/{request_id}/items/{merchant_reference}/\n  method: get\n  operationId: v1.1_payout_bulk_requests_items_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/payout/bulk/requests/{request_id}/items/{merchant_reference}/cancel/\n  method: post\n  operationId: v1.1_payout_bulk_requests_items_cancel_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payout/intent/\n  method: post\n  operationId: v1.1_payout_intent_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payout/intent/{intent_id}/close/\n  method: post\n  operationId: v1.1_payout_intent_close_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payout/transactions/{trx_uuid}/pull-status/\n\
  \  method: post\n  operationId: v1.1_payout_transactions_pull_status_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/payout/transactions/{trx_uuid}/void/\n  method: post\n  operationId: v1.1_payout_transactions_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/reconciliations/settlement-files/\n  method: post\n  operationId: v1.4_reconciliations_settlement_files_create\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/reconciliations/settlement-files/{settlement_file_id}/confirm_upload/\n  method: post\n  operationId: v1.4_reconciliations_settlement_files_confirm_upload_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/reconciliations/settlement-operations/\n  method: get\n  operationId: v1.4_reconciliations_settlement_operations_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/v1.4/subscriptions/\n  method: get\n  operationId: v1.1_subscriptions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/subscriptions/\n  method: post\n  operationId: v1.1_subscriptions_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/subscriptions/plan-groups/\n  method: get\n  operationId: v1.1_subscriptions_plan_groups_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/subscriptions/plan-groups/{plan_group_id}/\n  method: get\n  operationId: v1.1_subscriptions_plan_groups_retrieve\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/subscriptions/plans/\n  method: get\n  operationId: v1.1_subscriptions_plans_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/subscriptions/plans/\n  method: post\n  operationId: v1.1_subscriptions_plans_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/subscriptions/{subscription_id}/\n  method: get\n  operationId: v1.1_subscriptions_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1.4/subscriptions/{subscription_id}/card_token/\n  method: post\n  operationId: v1.1_subscriptions_card_token_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/subscriptions/{subscription_id}/retry-payment/\n  method: post\n  operationId: v1.1_subscriptions_retry_payment_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/subscriptions/{subscription_id}/update_amount/\n  method: post\n  operationId: v1.1_subscriptions_update_amount_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/subscriptions/{subscription_id}/update_discount/\n  method: post\n  operationId: v1.1_subscriptions_update_discount_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/subscriptions/{subscription_id}/update_plan/\n  method: post\n  operationId: v1.1_subscriptions_update_plan_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/subscriptions/{subscription_id}/update_remaining_recurring_cycles/\n  method: post\n  operationId: v1.1_subscriptions_update_remaining_recurring_cycles_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/tokens/cards/\n  method: post\n  operationId: v1.1_tokens_cards_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.4/tokens/cards/{card_uuid}/\n  method: get\n  operationId:\
  \ v1.1_tokens_cards_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/tokens/intent/{card_intent_id}/details/\n  method: get\n  operationId: v1.1_tokens_intent_details_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/transactions/{trx_uuid}/transition/\n  method: post\n  operationId: v1.1_transactions_transition_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/providers/available/\n  method: get\n  operationId: v1_providers_available_list\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/providers/connected/\n  method: get\n  operationId: v1_providers_connected_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/providers/countries/\n  method: get\n  operationId: v1_providers_countries_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/providers/sync/available/\n  method: get\n  operationId: v1_providers_sync_available_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/providers/sync/available/\n  method: post\n  operationId: v1_providers_sync_available_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/providers/sync/connected/\n  method: get\n  operationId: v1_providers_sync_connected_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.4/direct/payments/intents/{intent_id}/{payment_method}/\n  method: post\n  operationId: api_v1_direct_payments_intents_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/moneyhash/agentic-access/moneyhash-agentic-access.yml
summary_line: 86 operations · 52 acting · 1 human-in-the-loop
tags:
- Company
- Payments
- Fintech
- Orchestration
---
