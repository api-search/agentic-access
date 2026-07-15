---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 15
api_specs:
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Expenses API
  slug: fyle-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Reports API
  slug: fyle-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Advances API
  slug: fyle-advances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Categories API
  slug: fyle-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Projects API
  slug: fyle-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Cost Centers API
  slug: fyle-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Employees API
  slug: fyle-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Merchants API
  slug: fyle-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Corporate Cards & Transactions API
  slug: fyle-corporate-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Webhooks API
  slug: fyle-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
- filename: fyle-openapi.yml
  format: yaml
  label: Fyle Files & Receipts API
  slug: fyle-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-openapi.yml
consequence_counts:
  read: 15
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fyle Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'Fyle exposes 40 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 25 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fyle
provider_slug: fyle
slug: fyle-agentic-access
source_filename: fyle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fyle-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 15\n    acting: 25\n  by_consequence:\n    read: 15\n    write: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /admin/expenses\n  method: get\n  operationId: listAdminExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/expenses\n  method: post\n  operationId: upsertAdminExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/expenses/accounting_export_summary/bulk\n  method: post\n  operationId: bulkUpsertAccountingExportSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spender/expenses\n  method: get\n  operationId: listSpenderExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spender/expenses\n  method: post\n  operationId: createSpenderExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spender/expenses/attach_receipt\n  method: post\n  operationId: attachReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spender/expenses/create_from_receipt\n  method: post\n  operationId: createExpenseFromReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/reports\n  method: get\n  operationId: listAdminReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /admin/reports\n  method: post\n  operationId: upsertAdminReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/reports/mark_paid/bulk\n  method: post\n  operationId: bulkMarkReportsPaid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spender/reports\n  method: get\n  operationId: listSpenderReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spender/reports\n\
  \  method: post\n  operationId: createSpenderReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spender/reports/add_expenses\n  method: post\n  operationId: addExpensesToReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spender/reports/submit\n  method: post\n  operationId: submitReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /admin/advance_requests\n  method: get\n  operationId: listAdvanceRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/advance_requests\n  method: post\n  operationId: upsertAdvanceRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/categories\n  method: post\n  operationId: upsertCategory\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/categories/bulk\n  method: post\n  operationId: bulkUpsertCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/projects\n  method: post\n  operationId: upsertProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/projects/bulk\n  method: post\n  operationId: bulkUpsertProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/cost_centers\n  method: get\n  operationId: listCostCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/cost_centers\n  method: post\n  operationId: upsertCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/cost_centers/bulk\n  method: post\n  operationId: bulkUpsertCostCenters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/employees\n  method: post\n  operationId: upsertEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/employees/invite/bulk\n  method: post\n  operationId: bulkInviteEmployees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spender/merchants\n  method: get\n  operationId: listMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spender/merchants\n  method: post\n  operationId: bulkUpsertMerchants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/corporate_cards\n  method: get\n  operationId:\
  \ listCorporateCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/corporate_card_transactions\n  method: get\n  operationId: listCorporateCardTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/corporate_card_transactions\n  method: post\n  operationId: upsertCorporateCardTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /admin/subscriptions\n  method: post\n  operationId: upsertSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/scheduled_callbacks\n  method: get\n  operationId: listScheduledCallbacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/scheduled_callbacks\n  method: post\n  operationId: upsertScheduledCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/files\n\
  \  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/files\n  method: post\n  operationId: createFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/files/generate_urls/bulk\n  method: post\n  operationId: bulkGenerateFileUrls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/agentic-access/fyle-agentic-access.yml
summary_line: 40 operations · 25 acting
tags:
- Expense Management
- Spend Management
- Corporate Cards
- Fintech
- Accounting
- Receipts
---
