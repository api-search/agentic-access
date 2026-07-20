---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Contacts API
  slug: bexio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Sales Order Management API
  slug: bexio-sales-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Accounting API
  slug: bexio-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Items API
  slug: bexio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Projects & Time Tracking API
  slug: bexio-projects-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Files API
  slug: bexio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Purchase API
  slug: bexio-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Payroll API
  slug: bexio-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Banking API
  slug: bexio-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
consequence_counts:
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the modeled OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. bexio writes affect real financial records (invoices, journal entries, payroll), so write operations default to human-in-the-loop required. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Bexio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'bexio exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 12 write.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bexio
provider_slug: bexio
slug: bexio-agentic-access
source_filename: bexio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/bexio-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the modeled OpenAPI. A governance starting point for exposing this API to AI agents - review\n  and bind audience per deployment. bexio writes affect real financial records (invoices,\n  journal entries, payroll), so write operations default to human-in-the-loop required.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 12\n    connected: 8\n  by_consequence:\n    write: 12\n    read: 8\n  human_in_the_loop_required: 12\noperations:\n- path: /contact\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact/{id}\n  method: post\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/{id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kb_offer\n  method: get\n  operationId: listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kb_offer\n  method: post\n  operationId: createOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kb_order\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kb_order\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kb_invoice\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kb_invoice\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kb_invoice/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kb_invoice/{id}/pdf\n\
  \  method: get\n  operationId: getInvoicePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /article\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /article\n  method: post\n  operationId: createArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/manual_entries\n  method: post\n  operationId: createManualEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pr_project\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timesheet\n  method: post\n  operationId: createTimesheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ required\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banking/accounts\n  method: get\n  operationId: listBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/agentic-access/bexio-agentic-access.yml
summary_line: 20 operations · 12 acting · 12 human-in-the-loop
tags:
- Accounting
- ERP
- Invoicing
- SMB
- Switzerland
---
