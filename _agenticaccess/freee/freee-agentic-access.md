---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 24
api_specs:
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Deals API
  slug: freee-accounting-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Account Items API
  slug: freee-accounting-account-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Partners API
  slug: freee-accounting-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Invoices and Quotations API
  slug: freee-accounting-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Wallet Transactions API
  slug: freee-accounting-wallet-txns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee Accounting Journals and Reports API
  slug: freee-accounting-journals-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Employees API
  slug: freee-hr-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Payroll API
  slug: freee-hr-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
- filename: freee-openapi.yml
  format: yaml
  label: freee HR Attendance API
  slug: freee-hr-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/openapi/freee-openapi.yml
consequence_counts:
  read: 24
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Freee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'freee exposes 42 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: freee
provider_slug: freee
slug: freee-agentic-access
source_filename: freee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/freee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 24\n    acting: 18\n  by_consequence:\n    read: 24\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /api/1/companies\n  method: get\n  operationId: getCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/companies/{id}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - read\n    - write\n- path: /api/1/deals\n  method: get\n  operationId: getDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/deals\n  method: post\n  operationId: createDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/deals/{id}\n  method: get\n  operationId: getDeal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/deals/{id}\n  method: put\n  operationId: updateDeal\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/deals/{id}\n  method: delete\n  operationId: deleteDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/account_items\n  method: get\n  operationId: getAccountItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/account_items\n  method: post\n  operationId:\
  \ createAccountItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/account_items/{id}\n  method: get\n  operationId: getAccountItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/account_items/{id}\n  method: put\n  operationId: updateAccountItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path:\
  \ /api/1/account_items/{id}\n  method: delete\n  operationId: deleteAccountItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/partners\n  method: get\n  operationId: getPartners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/partners\n  method: post\n  operationId: createPartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - read\n    - write\n- path: /api/1/partners/{id}\n  method: get\n  operationId: getPartner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/partners/{id}\n  method: put\n  operationId: updatePartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/partners/{id}\n  method: delete\n  operationId: deletePartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/invoices\n  method: get\n  operationId: getInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/invoices/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/quotations\n  method: get\n  operationId: getQuotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/wallet_txns\n  method: get\n  operationId: getWalletTxns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/wallet_txns\n  method: post\n  operationId: createWalletTxn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/wallet_txns/{id}\n  method: get\n  operationId: getWalletTxn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/wallet_txns/{id}\n  method: delete\n  operationId: deleteWalletTxn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/walletables\n  method: get\n  operationId: getWalletables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/journals\n  method: get\n  operationId: getJournals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/manual_journals\n  method: get\n  operationId: getManualJournals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/manual_journals\n  method: post\n  operationId: createManualJournal\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /api/1/reports/trial_pl\n  method: get\n  operationId: getTrialPl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /api/1/taxes/codes\n  method: get\n  operationId: getTaxCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/users/me\n  method: get\n  operationId: getHrMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees\n  method: get\n  operationId: getEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees\n  method: post\n  operationId: createEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees/{id}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees/{id}\n  method: put\n  operationId:\
  \ updateEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees/{id}\n  method: delete\n  operationId: deleteEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/salaries/employee_payroll_statements\n  method: get\n  operationId: getEmployeePayrollStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - read\n    - write\n- path: /hr/api/v1/employees/{employee_id}/time_clocks\n  method: get\n  operationId: getTimeClocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees/{employee_id}/time_clocks\n  method: post\n  operationId: createTimeClock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees/{employee_id}/work_records/{date}\n  method: get\n  operationId: getWorkRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    -\
  \ read\n    - write\n- path: /hr/api/v1/employees/{employee_id}/work_records/{date}\n  method: put\n  operationId: updateWorkRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /hr/api/v1/employees/{employee_id}/work_records/{date}\n  method: delete\n  operationId: deleteWorkRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freee/refs/heads/main/agentic-access/freee-agentic-access.yml
summary_line: 42 operations · 18 acting
tags:
- Accounting
- Bookkeeping
- HR
- Payroll
- Invoicing
- Finance
- SaaS
- Japan
---
