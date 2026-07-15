---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: Xero-OpenAPI
  format: yaml
  label: Xero Accounting API
  slug: api
  spec_type: OpenAPI
  url: https://github.com/XeroAPI/Xero-OpenAPI
consequence_counts:
  physical: 3
  read: 9
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xero Accounting Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /BankTransfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /BatchPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Invoices
operation_count: 17
overview: 'Xero Accounting exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 5 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Xero Accounting
provider_slug: xero-accounting
slug: xero-accounting-agentic-access
source_filename: xero-accounting-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/xero-accounting-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    write: 5\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /Accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Accounts\n  method: put\n  operationId: createAccount\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Accounts/{AccountID}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Accounts/{AccountID}\n  method: post\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Accounts/{AccountID}\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Accounts/{AccountID}/Attachments\n\
  \  method: get\n  operationId: getAccountAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /BankTransactions\n  method: get\n  operationId: getBankTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /BankTransactions\n  method: put\n  operationId: createBankTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /BankTransactions/{BankTransactionID}\n  method: get\n  operationId: getBankTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /BankTransfers\n  method: get\n  operationId: getBankTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /BankTransfers\n  method: put\n  operationId: createBankTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /BatchPayments\n  method: get\n  operationId: getBatchPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /BatchPayments\n  method: put\n  operationId: createBatchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Contacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Contacts\n  method: put\n  operationId: createContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Invoices\n  method: get\n  operationId: getInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n\
  \    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n- path: /Invoices\n  method: put\n  operationId: createInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accounting.attachments\n    - accounting.contacts\n    - accounting.journals.read\n    - accounting.reports.read\n    - accounting.settings\n    - accounting.transactions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/agentic-access/xero-accounting-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Financial Reporting
- SaaS
---
