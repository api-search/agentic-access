---
acting_count: 120
action_class_counts:
  acting: 120
  connected: 120
api_specs:
- filename: paystack-accept-payments-openapi.yml
  format: yaml
  label: Paystack Accept Payments API
  slug: paystack-accept-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-accept-payments-openapi.yml
- filename: paystack-subscriptions-openapi.yml
  format: yaml
  label: Paystack Subscriptions API
  slug: paystack-subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-subscriptions-openapi.yml
- filename: paystack-customers-openapi.yml
  format: yaml
  label: Paystack Customers API
  slug: paystack-customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-customers-openapi.yml
- filename: paystack-transfers-openapi.yml
  format: yaml
  label: Paystack Transfers API
  slug: paystack-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-transfers-openapi.yml
- filename: paystack-splits-subaccounts-openapi.yml
  format: yaml
  label: Paystack Splits and Subaccounts API
  slug: paystack-splits-subaccounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-splits-subaccounts-openapi.yml
- filename: paystack-dedicated-virtual-accounts-openapi.yml
  format: yaml
  label: Paystack Dedicated Virtual Accounts API
  slug: paystack-dedicated-virtual-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-dedicated-virtual-accounts-openapi.yml
- filename: paystack-products-pages-openapi.yml
  format: yaml
  label: Paystack Products and Payment Pages API
  slug: paystack-products-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-products-pages-openapi.yml
- filename: paystack-payment-requests-openapi.yml
  format: yaml
  label: Paystack Payment Requests API
  slug: paystack-payment-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-payment-requests-openapi.yml
- filename: paystack-refunds-disputes-openapi.yml
  format: yaml
  label: Paystack Refunds and Disputes API
  slug: paystack-refunds-disputes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-refunds-disputes-openapi.yml
- filename: paystack-settlements-openapi.yml
  format: yaml
  label: Paystack Settlements API
  slug: paystack-settlements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-settlements-openapi.yml
- filename: paystack-verification-openapi.yml
  format: yaml
  label: Paystack Verification API
  slug: paystack-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-verification-openapi.yml
- filename: paystack-balance-openapi.yml
  format: yaml
  label: Paystack Balance API
  slug: paystack-balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-balance-openapi.yml
- filename: paystack-integration-openapi.yml
  format: yaml
  label: Paystack Integration Settings API
  slug: paystack-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/openapi/paystack-integration-openapi.yml
- filename: paystack-webhooks-asyncapi.yml
  format: yaml
  label: Paystack Webhooks
  slug: paystack-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/asyncapi/paystack-webhooks-asyncapi.yml
consequence_counts:
  physical: 50
  read: 120
  safety-critical: 6
  write: 64
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Paystack Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscription/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscription/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transfer/disable_otp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transfer/disable_otp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transfer/disable_otp_finalize
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transfer/disable_otp_finalize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulkcharge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulkcharge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_birthday
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_birthday
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_otp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_otp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_phone
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_phone
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_pin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/submit_pin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /integration/payment_session_timeout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /integration/payment_session_timeout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentrequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentrequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentrequest/archive/{id}
operation_count: 240
overview: 'Paystack exposes 240 API operations that an AI agent could call, of which 120 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 120 read, 64 write, 50 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paystack
provider_slug: paystack
slug: paystack-agentic-access
source_filename: paystack-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/paystack-accept-payments-openapi.yml, openapi/paystack-balance-openapi.yml,\n  openapi/paystack-customers-openapi.yml, openapi/paystack-dedicated-virtual-accounts-openapi.yml,\n  openapi/paystack-integration-openapi.yml, openapi/paystack-openapi-original.yml, openapi/paystack-payment-requests-openapi.yml,\n  openapi/paystack-products-pages-openapi.yml, openapi/paystack-refunds-disputes-openapi.yml,\n  openapi/paystack-settlements-openapi.yml, openapi/paystack-splits-subaccounts-openapi.yml,\n  openapi/paystack-subscriptions-openapi.yml, openapi/paystack-transfers-openapi.yml, openapi/paystack-verification-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 240\n  by_action_class:\n\
  \    acting: 120\n    connected: 120\n  by_consequence:\n    write: 64\n    read: 120\n    physical: 50\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /transaction/initialize\n  method: post\n  operationId: transaction_initialize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/verify/{reference}\n  method: get\n  operationId: transaction_verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction\n  method: get\n  operationId: transaction_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /transaction/{id}\n  method: get\n  operationId: transaction_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/timeline/{id_or_reference}\n  method: get\n  operationId: transaction_timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/totals\n  method: get\n  operationId: transaction_totals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/export\n  method: get\n  operationId: transaction_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/charge_authorization\n  method: post\n  operationId: transaction_chargeAuthorization\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/check_authorization\n  method: post\n  operationId: transaction_checkAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/partial_debit\n  method: post\n  operationId: transaction_partialDebit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{id}/event\n  method: get\n  operationId: transaction_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}/session\n  method: get\n  operationId: transaction_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charge\n  method: post\n  operationId: charge_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge/submit_pin\n  method: post\n  operationId: charge_submitPin\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge/submit_otp\n  method: post\n  operationId: charge_submitOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge/submit_phone\n  method: post\n  operationId: charge_submitPhone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n     \
  \ purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge/submit_birthday\n  method: post\n  operationId: charge_submitBirthday\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge/submit_address\n  method: post\n  operationId: charge_submitAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /charge/{reference}\n  method: get\n  operationId: charge_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  operationId: balance_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance/ledger\n  method: get\n  operationId: balance_ledger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer\n  method: post\n  operationId: customer_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer\n\
  \  method: get\n  operationId: customer_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{code}\n  method: get\n  operationId: customer_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{code}\n  method: put\n  operationId: customer_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/set_risk_action\n  method: post\n  operationId: customer_riskAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/deactivate_authorization\n  method: post\n  operationId: customer_deactivateAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/{code}/identification\n  method: post\n  operationId: customer_validatte\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dedicated_account\n  method: post\n  operationId: dedicatedAccount_create\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dedicated_account\n  method: get\n  operationId: dedicatedAccount_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dedicated_account/{account_id}\n  method: get\n  operationId: dedicatedAccount_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dedicated_account/{account_id}\n  method: delete\n  operationId: dedicatedAccount_deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dedicated_account/available_providers\n  method: get\n  operationId: dedicatedAccount_availableProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dedicated_account/split\n  method: post\n  operationId: dedicatedAccount_addSplit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/payment_session_timeout\n  method: get\n  operationId: integration_fetchPaymentSessionTimeout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/payment_session_timeout\n\
  \  method: put\n  operationId: integration_updatePaymentSessionTimeout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/initialize\n  method: post\n  operationId: transaction_initialize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/verify/{reference}\n  method: get\n  operationId: transaction_verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /transaction\n  method: get\n  operationId: transaction_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}\n  method: get\n  operationId: transaction_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/timeline/{id_or_reference}\n  method: get\n  operationId: transaction_timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/totals\n  method: get\n  operationId: transaction_totals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/export\n  method: get\n  operationId: transaction_download\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/charge_authorization\n  method: post\n  operationId: transaction_chargeAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/check_authorization\n  method: post\n  operationId: transaction_checkAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/partial_debit\n\
  \  method: post\n  operationId: transaction_partialDebit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{id}/event\n  method: get\n  operationId: transaction_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}/session\n  method: get\n  operationId: transaction_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /split\n  method: post\n  operationId: split_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /split\n  method: get\n  operationId: split_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /split/{id}\n  method: get\n  operationId: split_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /split/{id}\n  method: put\n  operationId: split_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /split/{id}/subaccount/add\n  method: post\n  operationId: split_addSubaccount\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /split/{id}/subaccount/remove\n  method: post\n  operationId: split_removeSubaccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer\n  method: post\n  operationId: customer_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer\n  method: get\n\
  \  operationId: customer_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{code}\n  method: get\n  operationId: customer_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{code}\n  method: put\n  operationId: customer_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/set_risk_action\n  method: post\n  operationId: customer_riskAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/deactivate_authorization\n  method: post\n  operationId: customer_deactivateAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/{code}/identification\n  method: post\n  operationId: customer_validatte\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dedicated_account\n  method: post\n  operationId: dedicatedAccount_create\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dedicated_account\n  method: get\n  operationId: dedicatedAccount_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dedicated_account/{account_id}\n  method: get\n  operationId: dedicatedAccount_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dedicated_account/{account_id}\n  method: delete\n  operationId: dedicatedAccount_deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dedicated_account/available_providers\n  method: get\n  operationId: dedicatedAccount_availableProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dedicated_account/split\n  method: post\n  operationId: dedicatedAccount_addSplit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccount\n  method: post\n  operationId: subaccount_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /subaccount\n  method: get\n  operationId: subaccount_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subaccount/{code}\n  method: get\n  operationId: subaccount_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subaccount/{code}\n  method: put\n  operationId: subaccount_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plan\n  method: post\n  operationId: plan_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plan\n  method: get\n  operationId: plan_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plan/{code}\n  method: get\n  operationId: plan_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plan/{code}\n  method: put\n  operationId: plan_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription\n  method: post\n  operationId: subscription_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription\n  method: get\n  operationId: subscription_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription/{code}\n  method: get\n  operationId: subscription_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription/disable\n  method: post\n  operationId: subscription_disable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /subscription/enable\n  method: post\n  operationId: subscription_enable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/{code}/manage/link\n  method: post\n  operationId: subscription_manageLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/{code}/manage/email\n  method: post\n  operationId: subscription_manageEmail\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product\n  method: post\n  operationId: product_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product\n  method: get\n  operationId: product_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/{id}\n  method: get\n  operationId: product_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /product/{id}\n  method: put\n  operationId: product_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{id}\n  method: delete\n  operationId: product_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /page\n  method: post\n  operationId: page_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /page\n  method: get\n  operationId: page_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/{id}\n  method: get\n  operationId: page_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/{id}\n  method: put\n  operationId: page_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /page/check_slug_availability/{slug}\n  method: get\n  operationId: page_checkSlugAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/{id}/product\n  method: post\n  operationId: page_addProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentrequest\n  method: post\n  operationId: paymentRequest_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentrequest\n  method: get\n  operationId: paymentRequest_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentrequest/{id}\n  method: get\n  operationId: paymentRequest_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentrequest/{id}\n  method: put\n  operationId: paymentRequest_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentrequest/verify/{id}\n  method: get\n  operationId: paymentRequest_verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentrequest/notify/{id}\n  method: post\n  operationId: paymentRequest_notify\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentrequest/totals\n  method: get\n  operationId: paymentRequest_totals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentrequest/finalize/{id}\n  method: post\n  operationId: paymentRequest_finalize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentrequest/archive/{id}\n\
  \  method: post\n  operationId: paymentRequest_archive\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settlement\n  method: get\n  operationId: settlements_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settlement/{id}/transaction\n  method: get\n  operationId: settlements_transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transferrecipient\n  method: post\n  operationId: transferrecipient_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transferrecipient\n  method: get\n  operationId: transferrecipient_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transferrecipient/bulk\n  method: post\n  operationId: transferrecipient_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transferrecipient/{code}\n  method: get\n  operationId: transferrecipient_fetch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl\n\n# --- truncated at 32 KB (69 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/agentic-access/paystack-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystack/refs/heads/main/agentic-access/paystack-agentic-access.yml
summary_line: 240 operations · 120 acting · 6 human-in-the-loop
tags:
- Payments
- Africa
- Fintech
- Recurring Billing
- Marketplaces
- Payouts
- Mobile Money
- Stripe
---
