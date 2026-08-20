---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 2
api_specs:
- filename: clearbank-sterling-v4.json
  format: json
  label: ClearBank GBP Accounts API
  slug: clearbank-gbp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sterling-v4.json
- filename: clearbank-fps-initiate-payment-v3.json
  format: json
  label: ClearBank Faster Payments API
  slug: clearbank-faster-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fps-initiate-payment-v3.json
- filename: clearbank-chaps-v6.json
  format: json
  label: ClearBank CHAPS API
  slug: clearbank-chaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-chaps-v6.json
- filename: clearbank-mccy-accounts-v2.json
  format: json
  label: ClearBank Multi-Currency Accounts API
  slug: clearbank-multi-currency-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-mccy-accounts-v2.json
- filename: clearbank-mccy-payments-v1.json
  format: json
  label: ClearBank Multi-Currency Payments API
  slug: clearbank-multi-currency-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-mccy-payments-v1.json
- filename: clearbank-fx-orchestrator-rfq.json
  format: json
  label: ClearBank FX API
  slug: clearbank-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fx-orchestrator-rfq.json
- filename: clearbank-sepa-ct-v1.json
  format: json
  label: ClearBank SEPA Credit Transfer API
  slug: clearbank-sepa-credit-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sepa-ct-v1.json
- filename: clearbank-cop-outbound-v1.json
  format: json
  label: ClearBank Confirmation of Payee API
  slug: clearbank-confirmation-of-payee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cop-outbound-v1.json
- filename: clearbank-know-your-customer-v1.json
  format: json
  label: ClearBank Customer Due Diligence (KYC) API
  slug: clearbank-customer-due-diligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-know-your-customer-v1.json
- filename: clearbank-cross-border-v4.json
  format: json
  label: ClearBank Cross-Border Sterling Payments API
  slug: clearbank-cross-border-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cross-border-v4.json
- filename: clearbank-customers_v2_retail.json
  format: json
  label: ClearBank Retail Embedded Banking Customers API
  slug: clearbank-retail-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-customers_v2_retail.json
consequence_counts:
  physical: 16
  read: 2
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clearbank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /customers/v2/customers/{customerId}/related-parties
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fx/v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fx/v1/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/chaps/v6/customer-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/chaps/v6/institution-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/chaps/v6/return-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/cross-border-sterling/v4/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/sepa-ct/v1/customer-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/sepa-ct/v1/payment-returns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/sepa-ct/v1/recall
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/sepa-ct/v1/recall-response
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/mccy/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/mccy/payments/{batchId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/mccy/payments/{batchId}/{endToEndId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payments/fps
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payments/fps/return
operation_count: 31
overview: 'ClearBank exposes 31 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 13 write, and 16 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClearBank
provider_slug: clearbank
slug: clearbank-agentic-access
source_filename: clearbank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/clearbank-chaps-v6.json, openapi/clearbank-cop-outbound-v1.json, openapi/clearbank-cross-border-v4.json,\n  openapi/clearbank-customers_v2_retail.json, openapi/clearbank-fps-initiate-payment-v3.json,\n  openapi/clearbank-fx-orchestrator-rfq.json, openapi/clearbank-know-your-customer-v1.json,\n  openapi/clearbank-mccy-accounts-v2.json, openapi/clearbank-mccy-payments-v1.json, openapi/clearbank-sepa-ct-v1.json,\n  openapi/clearbank-sterling-v4.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 29\n    connected: 2\n  by_consequence:\n    physical: 16\n    write: 13\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /payments/chaps/v6/institution-payments\n\
  \  method: post\n  operationId: ExternalCreateInstitutionPayment-v6\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/chaps/v6/customer-payments\n  method: post\n  operationId: ExternalCreateCustomerPayment-v6\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/chaps/v6/return-payments\n  method: post\n  operationId: ExternalReturnPayment-v6\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-banking/outbound/v1/name-verification\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-banking/outbound/v1/srd/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/cross-border-sterling/v4/payments\n\
  \  method: post\n  operationId: ExternalCrossBorderCreateCustomerPayment-v7\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/customers/{customerId}\n  method: get\n  operationId: V2CustomerGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v2/customers/{customerId}/related-parties\n  method: get\n  operationId: V2RelatedPartiesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v2/customers/{customerId}/related-parties\n  method: post\n  operationId: V2RelatedPartyPost\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/customers/{customerId}/current-addresses\n  method: post\n  operationId: V2CustomersCurrentAddressPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/customers/{customerId}/related-parties/{relatedCustomerId}/{relatedPartyType}\n  method: delete\n  operationId: V2RelatedPartyDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/customers/{customerId}/identity-documents/{idCountryOfIssue}-{idType}\n  method: put\n  operationId: V2CustomerIdentityDocumentPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/customers/{customerId}/identity-documents/{idCountryOfIssue}-{idType}\n  method: delete\n  operationId: V2CustomerIdentityDocumentDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /customers/v2/customers/{customerId}/tax-residencies/{countryOfTaxResidence}\n  method: put\n  operationId: V2CustomerTaxResidencyPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/customers/{customerId}/tax-residencies/{countryOfTaxResidence}\n  method: delete\n  operationId: V2CustomerTaxResidencyDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/retail\n  method: post\n  operationId: V2RetailPost\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v2/retail/{customerId}\n  method: patch\n  operationId: V2RetailPatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payments/fps\n  method: post\n  operationId: Post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v3/payments/fps/return\n  method: post\n  operationId: PostReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fx/v1/order\n  method: post\n  operationId: Order.Create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fx/v1/quote\n  method: post\n  operationId: Order.Create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer-due-diligence/v1/retail/onboard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mccy/v2/Accounts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mccy/payments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mccy/payments/{batchId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mccy/payments/{batchId}/{endToEndId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /payments/sepa-ct/v1/customer-payments\n  method: post\n  operationId: Payment.Create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/sepa-ct/v1/recall-response\n  method: post\n  operationId: Payments.Inbound.RecallRequestResult\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/sepa-ct/v1/recall\n  method: post\n  operationId: Payment.Recall\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/sepa-ct/v1/payment-returns\n  method: post\n  operationId: Payments.Inbound.ReturnOfInboundPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/Accounts\n  method: post\n  operationId: V4InstitutionsByInstitutionIdAccountsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/agentic-access/clearbank-agentic-access.yml
summary_line: 31 operations · 29 acting
tags:
- Financial-Services
- Banking
- Banking as a Service
- Embedded Banking
- Payments
- Clearing
- Faster Payments
- CHAPS
- Multi-Currency
- Foreign Exchange
- Open Banking
- United Kingdom
- Fintech
---
