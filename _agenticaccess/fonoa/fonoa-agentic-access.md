---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 2
api_specs:
- filename: fonoa-validate-openapi.yml
  format: yaml
  label: Fonoa Validate API
  slug: validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-validate-openapi.yml
- filename: fonoa-tax-engine-openapi.yml
  format: yaml
  label: Fonoa Tax Engine API
  slug: tax-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-tax-engine-openapi.yml
- filename: fonoa-e-invoicing-openapi.yml
  format: yaml
  label: Fonoa E-Invoicing API
  slug: e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-e-invoicing-openapi.yml
- filename: fonoa-onboarding-openapi.yml
  format: yaml
  label: Fonoa Onboarding API
  slug: onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/openapi/fonoa-onboarding-openapi.yml
consequence_counts:
  read: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fonoa Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Fonoa exposes 10 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fonoa
provider_slug: fonoa
slug: fonoa-agentic-access
source_filename: fonoa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fonoa-e-invoicing-openapi.yml, openapi/fonoa-onboarding-openapi.yml, openapi/fonoa-tax-engine-openapi.yml,\n  openapi/fonoa-validate-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 8\n    connected: 2\n  by_consequence:\n    write: 8\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/transactions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboarding/v2/companies\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tax/v2/calculations\n  method: post\n  operationId: Requestataxrate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookup/v2/single-validations\n  method: post\n  operationId: RequestavalidationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /lookup/v2/batch-validations\n  method: post\n  operationId: RequestbatchvalidationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookup/v2/batch-validations/{batch_id}\n  method: get\n  operationId: GetresultofbatchvalidationV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/v2/batch-validations/{batch_id}\n  method: delete\n  operationId: CancelbatchvalidationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /lookup/v2/single-validations/{validation_id}\n  method: get\n  operationId: GetresultofvalidationV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/v2/single-validations/{validation_id}\n  method: delete\n  operationId: DeleteresultofvalidationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookup/v2/tin-search\n  method: post\n  operationId: RequestTINsearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fonoa/refs/heads/main/agentic-access/fonoa-agentic-access.yml
summary_line: 10 operations · 8 acting
tags:
- Tax
- VAT
- GST
- E-Invoicing
- Tax Automation
- Tax Compliance
- Tax Calculation
- Tax ID Validation
- Invoice Generation
- Global Tax
- Indirect Tax
- FinTech
---
