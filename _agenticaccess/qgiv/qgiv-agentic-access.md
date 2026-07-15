---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 11
api_specs:
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Transactions API
  slug: qgiv-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Recurring Donations API
  slug: qgiv-recurring-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Refunds API
  slug: qgiv-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Peer-to-Peer Registrations API
  slug: qgiv-peer-to-peer-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Events API
  slug: qgiv-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Account Settings API
  slug: qgiv-account-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Custom Fields API
  slug: qgiv-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Custom Amounts API
  slug: qgiv-custom-amounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Statements API
  slug: qgiv-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Report Mappings API
  slug: qgiv-report-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
consequence_counts:
  physical: 4
  read: 11
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qgiv Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reporting/refunds/after/{refundId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reporting/refunds/dates/{begin}:{end}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reporting/refunds/last/{limit}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reporting/refunds/{id}
operation_count: 34
overview: 'Qgiv exposes 34 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 19 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qgiv
provider_slug: qgiv
slug: qgiv-agentic-access
source_filename: qgiv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/qgiv-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 11\n    acting: 23\n  by_consequence:\n    read: 11\n    write: 19\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /reporting/transactions/last/{limit}\n  method: get\n  operationId: getLastTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/transactions/after/{transactionId}\n  method: get\n  operationId: getTransactionsAfterId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /reporting/transactions/dates/{begin}:{end}\n  method: get\n  operationId: getTransactionsByDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/recurring/list\n  method: post\n  operationId: listRecurringTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/recurring/{status}\n  method: post\n  operationId: listRecurringTransactionsByStatus\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/recurring/{id}\n  method: post\n  operationId: getRecurringTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/refunds/last/{limit}\n  method: post\n  operationId: getLastRefunds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/refunds/after/{refundId}\n  method: post\n  operationId: getRefundsAfterId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/refunds/dates/{begin}:{end}\n  method: post\n  operationId: getRefundsByDateRange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/refunds/{id}\n  method: post\n  operationId: getRefund\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/registrations/last/{limit}\n  method: post\n  operationId: getLastRegistrations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/registrations/dates/{begin}:{end}\n  method: post\n  operationId: getRegistrationsByDateRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/registrations/{id}\n  method: post\n  operationId: getRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/list\n  method: post\n  operationId: listEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n\
  \  method: post\n  operationId: updateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/settings\n  method: get\n  operationId: getAccountSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/settings\n  method: post\n  operationId: updateAccountSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customFields/list\n  method: post\n  operationId: listCustomFields\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customFields/create\n  method: post\n  operationId: createCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customFields/{id}\n  method: get\n  operationId: getCustomField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customFields/{id}\n  method: post\n  operationId: updateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /amounts/list\n  method: get\n  operationId: listCustomAmounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /amounts/create\n  method: post\n  operationId: createCustomAmount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /amounts/{id}\n  method: get\n  operationId: getCustomAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /amounts/{id}\n  method:\
  \ post\n  operationId: updateCustomAmount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/statements/list\n  method: post\n  operationId: listStatements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/statements/latest\n  method: post\n  operationId: getLatestStatements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /reporting/statements/{id}\n  method: post\n  operationId: getStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/mappings/list\n  method: get\n  operationId: listMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/mappings/{id}\n  method: get\n  operationId: getMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mappings/create\n  method: post\n  operationId: createMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mappings/{id}\n  method: post\n  operationId: updateMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/agentic-access/qgiv-agentic-access.yml
summary_line: 34 operations · 23 acting
tags:
- Nonprofit
- Fundraising
- Donations
- Payments
- Peer to Peer
- Events
- Bloomerang
---
