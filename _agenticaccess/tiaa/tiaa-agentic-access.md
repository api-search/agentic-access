---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: tiaa-fdx-openapi.yml
  format: yaml
  label: TIAA Financial Data Exchange API
  slug: tiaa-fdx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-fdx-openapi.yml
- filename: tiaa-sia-openapi.yml
  format: yaml
  label: TIAA Secure Income Account API
  slug: tiaa-sia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-sia-openapi.yml
consequence_counts:
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tiaa Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'TIAA exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TIAA
provider_slug: tiaa
slug: tiaa-agentic-access
source_filename: tiaa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tiaa-fdx-openapi.yml, openapi/tiaa-sia-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 10\n    acting: 2\n  by_consequence:\n    read: 10\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions\n\
  \  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/positions\n  method: get\n  operationId: listPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax-forms\n  method: get\n  operationId: listTaxForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}/participants\n  method: get\n  operationId: listParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}/participants\n  method: post\n  operationId: enrollParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}/participants/{participantId}\n  method: get\n  operationId: getParticipant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}/contributions\n  method: post\n  operationId: submitContribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}/participants/{participantId}/projections\n  method: get\n  operationId: getIncomeProjection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planId}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/agentic-access/tiaa-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Finance
- Financial Data
- Fintech
- Insurance
- Investment Management
- Retirement
- Wealth Management
- Fortune 100
---
