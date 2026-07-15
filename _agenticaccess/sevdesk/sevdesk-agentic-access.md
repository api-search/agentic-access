---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 17
api_specs:
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Contacts API
  slug: sevdesk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Invoices API
  slug: sevdesk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Orders API
  slug: sevdesk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Credit Notes API
  slug: sevdesk-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Vouchers API
  slug: sevdesk-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Bank and Transactions API
  slug: sevdesk-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Parts API
  slug: sevdesk-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Tags API
  slug: sevdesk-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
- filename: sevdesk-openapi.yml
  format: yaml
  label: sevdesk Export and Reports API
  slug: sevdesk-export-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/openapi/sevdesk-openapi.yml
consequence_counts:
  physical: 5
  read: 17
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sevdesk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoice/Factory/saveInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoice/{invoiceId}/sendViaEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Order/Factory/saveOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Order/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /Order/{orderId}
operation_count: 30
overview: 'sevdesk exposes 30 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 8 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sevdesk
provider_slug: sevdesk
slug: sevdesk-agentic-access
source_filename: sevdesk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sevdesk-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 17\n    acting: 13\n  by_consequence:\n    read: 17\n    write: 8\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /Contact\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contact\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contact/{contactId}\n  method: get\n  operationId: getContactById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contact/{contactId}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contact/{contactId}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /Contact/Factory/getNextCustomerNumber\n  method: get\n  operationId: getNextCustomerNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice\n  method: get\n  operationId: getInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice/{invoiceId}\n  method: get\n  operationId: getInvoiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice/Factory/saveInvoice\n  method: post\n  operationId: createInvoiceByFactory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoice/{invoiceId}/getPdf\n  method: get\n  operationId: invoiceGetPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoice/{invoiceId}/sendViaEmail\n  method: post\n  operationId: sendInvoiceViaEMail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Order\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Order/Factory/saveOrder\n\
  \  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Order/{orderId}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Order/{orderId}\n  method: put\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /Order/{orderId}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNote\n  method: get\n  operationId: getCreditNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNote/Factory/saveCreditNote\n  method: post\n  operationId: createcreditNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Voucher\n\
  \  method: get\n  operationId: getVouchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Voucher/Factory/saveVoucher\n  method: post\n  operationId: voucherFactorySaveVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Voucher/{voucherId}\n  method: get\n  operationId: getVoucherById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CheckAccount\n  method: get\n  operationId: getCheckAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /CheckAccount/{checkAccountId}\n  method: get\n  operationId: getCheckAccountById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CheckAccountTransaction\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CheckAccountTransaction\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Part\n  method: get\n  operationId: getParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /Part\n  method: post\n  operationId: createPart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Part/{partId}/getStock\n  method: get\n  operationId: partGetStock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Tag\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Tag/Factory/create\n  method: post\n  operationId: createTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sevdesk/refs/heads/main/agentic-access/sevdesk-agentic-access.yml
summary_line: 30 operations · 13 acting
tags:
- Accounting
- Invoicing
- Bookkeeping
- Finance
- Germany
- Vouchers
- Contacts
- SaaS
- ERP
- Financial Software
---
