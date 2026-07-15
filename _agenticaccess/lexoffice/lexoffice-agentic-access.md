---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 22
api_specs:
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Contacts API
  slug: lexoffice-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Invoices API
  slug: lexoffice-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Quotations API
  slug: lexoffice-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Order Confirmations API
  slug: lexoffice-order-confirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Delivery Notes API
  slug: lexoffice-delivery-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Credit Notes API
  slug: lexoffice-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Dunnings API
  slug: lexoffice-dunnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Vouchers API
  slug: lexoffice-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Event Subscriptions API
  slug: lexoffice-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Payments API
  slug: lexoffice-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
- filename: lexoffice-openapi.yml
  format: yaml
  label: lexoffice Profile and Metadata API
  slug: lexoffice-profile-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/openapi/lexoffice-openapi.yml
consequence_counts:
  physical: 2
  read: 22
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lexoffice Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order-confirmations
operation_count: 35
overview: 'lexoffice exposes 35 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 11 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: lexoffice
provider_slug: lexoffice
slug: lexoffice-agentic-access
source_filename: lexoffice-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lexoffice-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 22\n    acting: 13\n  by_consequence:\n    read: 22\n    write: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /invoices/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{id}/document\n  method: get\n  operationId: getInvoiceDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotations\n  method: post\n  operationId: createQuotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotations/{id}\n  method: get\n  operationId: getQuotation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /order-confirmations\n  method: post\n  operationId: createOrderConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order-confirmations/{id}\n  method: get\n  operationId: getOrderConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delivery-notes\n  method: post\n  operationId: createDeliveryNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /delivery-notes/{id}\n  method: get\n  operationId: getDeliveryNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit-notes\n  method: post\n  operationId: createCreditNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credit-notes/{id}\n  method: get\n  operationId: getCreditNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dunnings/{id}\n  method: get\n  operationId: getDunning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /down-payment-invoices/{id}\n  method: get\n  operationId: getDownPaymentInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vouchers\n  method: post\n  operationId: createVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vouchers/{id}\n  method: get\n  operationId: getVoucher\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vouchers/{id}\n  method: put\n  operationId: updateVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vouchers/{id}\n  method: delete\n  operationId: deleteVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voucherlist\n  method: get\n  operationId: listVouchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /files/{id}\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event-subscriptions\n  method: get\n  operationId: listEventSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event-subscriptions\n  method: post\n  operationId: createEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event-subscriptions/{id}\n  method: get\n  operationId: getEventSubscription\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event-subscriptions/{id}\n  method: delete\n  operationId: deleteEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{voucherId}\n  method: get\n  operationId: getPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-conditions\n  method: get\n  operationId: listPaymentConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posting-categories\n  method: get\n  operationId: listPostingCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring-templates\n  method: get\n  operationId: listRecurringTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring-templates/{id}\n  method: get\n  operationId: getRecurringTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexoffice/refs/heads/main/agentic-access/lexoffice-agentic-access.yml
summary_line: 35 operations · 13 acting
tags:
- Accounting
- Invoicing
- Bookkeeping
- Finance
- Germany
- Vouchers
- Contacts
- SaaS
- Financial Software
---
