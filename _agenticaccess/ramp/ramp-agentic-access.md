---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: ramp-accounts-api-openapi.yml
  format: yaml
  label: Ramp Accounts API
  slug: ramp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-accounts-api-openapi.yml
- filename: ramp-audit-logs-api-openapi.yml
  format: yaml
  label: Ramp Audit Logs API
  slug: ramp-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-audit-logs-api-openapi.yml
- filename: ramp-bills-api-openapi.yml
  format: yaml
  label: Ramp Bills API
  slug: ramp-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-bills-api-openapi.yml
- filename: ramp-cards-api-openapi.yml
  format: yaml
  label: Ramp Cards API
  slug: ramp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-cards-api-openapi.yml
- filename: ramp-departments-api-openapi.yml
  format: yaml
  label: Ramp Departments API
  slug: ramp-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-departments-api-openapi.yml
- filename: ramp-locations-api-openapi.yml
  format: yaml
  label: Ramp Locations API
  slug: ramp-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-locations-api-openapi.yml
- filename: ramp-reimbursements-api-openapi.yml
  format: yaml
  label: Ramp Reimbursements API
  slug: ramp-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-reimbursements-api-openapi.yml
- filename: ramp-statements-api-openapi.yml
  format: yaml
  label: Ramp Statements API
  slug: ramp-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-statements-api-openapi.yml
- filename: ramp-transactions-api-openapi.yml
  format: yaml
  label: Ramp Transactions API
  slug: ramp-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-transactions-api-openapi.yml
- filename: ramp-users-api-openapi.yml
  format: yaml
  label: Ramp Users API
  slug: ramp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-users-api-openapi.yml
- filename: ramp-vendors-api-openapi.yml
  format: yaml
  label: Ramp Vendors API
  slug: ramp-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-vendors-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ramp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Ramp exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ramp
provider_slug: ramp
slug: ramp-agentic-access
source_filename: ramp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ramp-developer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /accounting/accounts\n  method: get\n  operationId: listAccountingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/vendors\n  method: get\n  operationId: listAccountingVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting:read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cards:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - users:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /departments\n  method: get\n  operationId: listDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - departments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - locations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reimbursements\n  method: get\n  operationId: listReimbursements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reimbursements:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills\n  method: get\n  operationId: listBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - bills:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /statements\n  method: get\n  operationId: listStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - statements:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit-logs/events\n  method: get\n  operationId: listAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - audit:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/agentic-access/ramp-agentic-access.yml
summary_line: 12 operations
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursement
---
