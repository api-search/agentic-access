---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 10
api_specs:
- filename: billdesk-authentication-api-openapi.yml
  format: yaml
  label: BillDesk Authentication API
  slug: billdesk-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-authentication-api-openapi.yml
- filename: billdesk-card-account-api-openapi.yml
  format: yaml
  label: BillDesk Card Account API
  slug: billdesk-card-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-card-account-api-openapi.yml
- filename: billdesk-guest-checkout-altid-api-openapi.yml
  format: yaml
  label: BillDesk Guest Checkout (AltID) API
  slug: billdesk-guest-checkout-altid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-guest-checkout-altid-api-openapi.yml
- filename: billdesk-invoice-api-openapi.yml
  format: yaml
  label: BillDesk Invoice API
  slug: billdesk-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-invoice-api-openapi.yml
- filename: billdesk-mandate-api-openapi.yml
  format: yaml
  label: BillDesk Mandate API
  slug: billdesk-mandate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-mandate-api-openapi.yml
- filename: billdesk-order-api-openapi.yml
  format: yaml
  label: BillDesk Order API
  slug: billdesk-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-order-api-openapi.yml
- filename: billdesk-payment-links-api-openapi.yml
  format: yaml
  label: BillDesk Payment Links API
  slug: billdesk-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-payment-links-api-openapi.yml
- filename: billdesk-penny-drop-api-openapi.yml
  format: yaml
  label: BillDesk Penny Drop API
  slug: billdesk-penny-drop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-penny-drop-api-openapi.yml
- filename: billdesk-refund-api-openapi.yml
  format: yaml
  label: BillDesk Refund API
  slug: billdesk-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-refund-api-openapi.yml
- filename: billdesk-settlement-api-openapi.yml
  format: yaml
  label: BillDesk Settlement API
  slug: billdesk-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-settlement-api-openapi.yml
- filename: billdesk-transaction-api-openapi.yml
  format: yaml
  label: BillDesk Transaction API
  slug: billdesk-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-transaction-api-openapi.yml
- filename: billdesk-validate-vpa-api-openapi.yml
  format: yaml
  label: BillDesk Validate VPA API
  slug: billdesk-validate-vpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/openapi/billdesk-validate-vpa-api-openapi.yml
consequence_counts:
  physical: 14
  read: 10
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Billdesk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/authentications/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/authentications/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/orders/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/refunds/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/refunds/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/transactions/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/transactions/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/ve1_2/upi/validatevpa
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pgsi/ve1_2/invoice/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pgsi/ve1_2/mandatetokens/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pgsi/ve1_2/mandatetokens/update/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /resend
operation_count: 31
overview: 'BillDesk exposes 31 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 7 write, and 14 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BillDesk
provider_slug: billdesk
slug: billdesk-agentic-access
source_filename: billdesk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/billdesk-linkpay-openapi.yml, openapi/billdesk-pa-settlements-openapi.yml, openapi/billdesk-payments-openapi.yml,\n  openapi/billdesk-penny-drop-openapi.yml, openapi/billdesk-recurring-openapi.yml, openapi/billdesk-tokenization-openapi.yml,\n  openapi/billdesk-validate-vpa-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 21\n    connected: 10\n  by_consequence:\n    physical: 14\n    read: 10\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /create\n  method: post\n  operationId: create-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete\n  method: post\n  operationId: delete-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fetch\n  method: post\n  operationId: retrieve-link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resend\n  method: post\n  operationId: resend-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pasettlements/v1_2/settlements/get\n  method: post\n  operationId: retrieve-settlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/ve1_2/authentications/create\n  method: post\n  operationId: createAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/ve1_2/authentications/get\n  method: post\n  operationId: retrieveAuthentication\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/ve1_2/authentications/validate\n  method: post\n  operationId: validateAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/ve1_2/orders/create\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/ve1_2/refunds/create\n\
  \  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/ve1_2/refunds/get\n  method: post\n  operationId: retrieveRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/ve1_2/transactions/create\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/ve1_2/transactions/get\n  method: post\n  operationId: post-payments-v1_2-transactions-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/ve1_2/transactions/update\n  method: post\n  operationId: updateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgsi/ve1_2/mandatetokens/create\n  method: post\n  operationId: createMandateToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgsi/ve1_2/mandatetokens/update/create\n  method: post\n  operationId: modify-mandate-token\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgauth/ve1_2/accountvalidation\n  method: post\n  operationId: pennydrop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgsi/ve1_2/invoice/create\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgsi/ve1_2/invoice/get\n  method: post\n  operationId: retriveInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pgsi/ve1_2/mandates/create\n  method: post\n  operationId: createMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgsi/ve1_2/mandates/delete\n  method: post\n  operationId: deleteMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgsi/ve1_2/mandates/get\n  method: post\n  operationId: retrieveMandate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pgsi/ve1_2/mandates/list\n  method: post\n  operationId: listMandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pgsi/ve1_2/mandates/modify\n  method: post\n \
  \ operationId: modifyMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgsi/ve1_2/mandates/update\n  method: post\n  operationId: updateMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/ve1_2/altid/get\n  method: post\n  operationId: retrievealtid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenizer/ve1_2/token/create\n  method: post\n  operationId: createCardAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokenizer/ve1_2/token/delete\n  method: post\n  operationId: deleteCardAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokenizer/ve1_2/token/list\n  method: post\n  operationId: listCardAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenizer/ve1_2/token/retrieve\n  method: post\n  operationId: retrieveCardAccount\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/ve1_2/upi/validatevpa\n  method: post\n  operationId: validatVPA\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/agentic-access/billdesk-agentic-access.yml
summary_line: 31 operations · 21 acting
tags:
- Payments
- India
- Payment Gateway
- UPI
- Recurring Payments
- Mandates
- Net Banking
- Bill Payments
- Fintech
---
