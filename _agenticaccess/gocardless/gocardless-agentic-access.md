---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 27
api_specs:
- filename: gocardless-billing-request-flows-api-openapi.yml
  format: yaml
  label: GoCardless billing_request_flows API
  slug: gocardless-billing-request-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-billing-request-flows-api-openapi.yml
- filename: gocardless-billing-requests-api-openapi.yml
  format: yaml
  label: GoCardless billing_requests API
  slug: gocardless-billing-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-billing-requests-api-openapi.yml
- filename: gocardless-blocks-api-openapi.yml
  format: yaml
  label: GoCardless blocks API
  slug: gocardless-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-blocks-api-openapi.yml
- filename: gocardless-creditor-bank-accounts-api-openapi.yml
  format: yaml
  label: GoCardless creditor_bank_accounts API
  slug: gocardless-creditor-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-creditor-bank-accounts-api-openapi.yml
- filename: gocardless-creditors-api-openapi.yml
  format: yaml
  label: GoCardless creditors API
  slug: gocardless-creditors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-creditors-api-openapi.yml
- filename: gocardless-customer-bank-accounts-api-openapi.yml
  format: yaml
  label: GoCardless customer_bank_accounts API
  slug: gocardless-customer-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-customer-bank-accounts-api-openapi.yml
- filename: gocardless-customers-api-openapi.yml
  format: yaml
  label: GoCardless customers API
  slug: gocardless-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-customers-api-openapi.yml
- filename: gocardless-events-api-openapi.yml
  format: yaml
  label: GoCardless events API
  slug: gocardless-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-events-api-openapi.yml
- filename: gocardless-instalment-schedules-api-openapi.yml
  format: yaml
  label: GoCardless instalment_schedules API
  slug: gocardless-instalment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-instalment-schedules-api-openapi.yml
- filename: gocardless-institutions-api-openapi.yml
  format: yaml
  label: GoCardless institutions API
  slug: gocardless-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-institutions-api-openapi.yml
- filename: gocardless-mandates-api-openapi.yml
  format: yaml
  label: GoCardless mandates API
  slug: gocardless-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-mandates-api-openapi.yml
- filename: gocardless-payer-authorisations-api-openapi.yml
  format: yaml
  label: GoCardless payer_authorisations API
  slug: gocardless-payer-authorisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payer-authorisations-api-openapi.yml
- filename: gocardless-payments-api-openapi.yml
  format: yaml
  label: GoCardless payments API
  slug: gocardless-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payments-api-openapi.yml
- filename: gocardless-payouts-api-openapi.yml
  format: yaml
  label: GoCardless payouts API
  slug: gocardless-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-payouts-api-openapi.yml
- filename: gocardless-refunds-api-openapi.yml
  format: yaml
  label: GoCardless refunds API
  slug: gocardless-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-refunds-api-openapi.yml
- filename: gocardless-subscriptions-api-openapi.yml
  format: yaml
  label: GoCardless subscriptions API
  slug: gocardless-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/openapi/gocardless-subscriptions-api-openapi.yml
consequence_counts:
  physical: 5
  read: 27
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gocardless Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{id}/actions/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /refunds/{id}
operation_count: 48
overview: 'GoCardless exposes 48 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 16 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoCardless
provider_slug: gocardless
slug: gocardless-agentic-access
source_filename: gocardless-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gocardless-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 27\n    acting: 21\n  by_consequence:\n    read: 27\n    write: 16\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_bank_accounts\n  method: get\n  operationId: listCustomerBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_bank_accounts\n  method: post\n  operationId: createCustomerBankAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_bank_accounts/{id}\n  method: get\n  operationId: getCustomerBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_bank_accounts/{id}\n  method: put\n  operationId: updateCustomerBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates\n  method: get\n  operationId: listMandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mandates\n  method: post\n  operationId: createMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates/{id}\n  method: get\n  operationId: getMandate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mandates/{id}\n  method: put\n  operationId: updateMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates/{id}/actions/cancel\n\
  \  method: post\n  operationId: cancelMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{id}\n  method: put\n  operationId: updatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}/actions/cancel\n  method: post\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts\n  method: get\n  operationId: listPayouts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/{id}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{id}\n  method: get\n  operationId: getSubscription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{id}\n  method: put\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{id}/actions/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds/{id}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/{id}\n  method: put\n  operationId: updateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing_requests\n  method: get\n  operationId: listBillingRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing_requests\n  method: post\n  operationId: createBillingRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing_requests/{id}\n  method: get\n  operationId: getBillingRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing_request_flows\n  method: post\n  operationId: createBillingRequestFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing_request_flows/{id}\n  method: get\n  operationId: getBillingRequestFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditors\n  method: get\n  operationId: listCreditors\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditors/{id}\n  method: get\n  operationId: getCreditor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditor_bank_accounts\n  method: get\n  operationId: listCreditorBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditor_bank_accounts\n  method: post\n  operationId: createCreditorBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instalment_schedules\n  method: get\n  operationId: listInstalmentSchedules\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instalment_schedules\n  method: post\n  operationId: createInstalmentSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instalment_schedules/{id}\n  method: get\n  operationId: getInstalmentSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payer_authorisations\n  method: post\n  operationId: createPayerAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payer_authorisations/{id}\n  method: get\n  operationId: getPayerAuthorisation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institutions\n  method: get\n  operationId: listInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks\n  method: post\n  operationId: createBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blocks/{id}\n  method: get\n  operationId: getBlock\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/agentic-access/gocardless-agentic-access.yml
summary_line: 48 operations · 21 acting
tags:
- Payments
- Direct Debit
- Bank Debit
- Recurring Payments
- Subscription
- SEPA
- Bacs
- ACH
- Open Banking
- Fintech
---
