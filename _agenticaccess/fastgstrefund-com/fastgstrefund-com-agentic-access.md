---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: fastgstrefund-com-checklist-api-openapi.yml
  format: yaml
  label: Fast GST Refund Checklist API
  slug: fastgstrefund-com-checklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-checklist-api-openapi.yml
- filename: fastgstrefund-com-generator-files-api-openapi.yml
  format: yaml
  label: Fast GST Refund Generator Files API
  slug: fastgstrefund-com-generator-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-generator-files-api-openapi.yml
- filename: fastgstrefund-com-generators-api-openapi.yml
  format: yaml
  label: Fast GST Refund Generators API
  slug: fastgstrefund-com-generators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-generators-api-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fastgstrefund Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Fast GST Refund exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fast GST Refund
provider_slug: fastgstrefund-com
slug: fastgstrefund-com-agentic-access
source_filename: fastgstrefund-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/fastgstrefund-com-openapi.json, openapi/fastgstrefund-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/generators/statement3\n  method: get\n  operationId: statement3Requirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generators/statement3\n  method: post\n  operationId: statement3CheckOrCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   scope:\n    - refund:generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/generators/annexureb\n  method: get\n  operationId: annexurebRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generators/annexureb\n  method: post\n  operationId: annexurebCheckOrCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refund:generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/generator-files/{id}\n  method: get\n  operationId: downloadGeneratedJson\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - refund:generate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generator-files/{id}\n  method: delete\n  operationId: deleteGeneratedJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refund:generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checklist\n  method: get\n  operationId: getRefundPreparationChecklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generators/statement3\n  method: get\n  operationId: statement3Requirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generators/statement3\n\
  \  method: post\n  operationId: statement3CheckOrCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refund:generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/generators/annexureb\n  method: get\n  operationId: annexurebRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generators/annexureb\n  method: post\n  operationId: annexurebCheckOrCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refund:generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/generator-files/{id}\n  method: get\n  operationId: downloadGeneratedJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - refund:generate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generator-files/{id}\n  method: delete\n  operationId: deleteGeneratedJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refund:generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checklist\n  method: get\n  operationId: getRefundPreparationChecklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fastgstrefund-com/agentic-access/fastgstrefund-com-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- GST refund
- JSON generator
- Exporters
- Chartered accountants
- SaaS companies
- Accounting practices
---
