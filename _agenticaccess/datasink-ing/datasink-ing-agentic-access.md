---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: datasink-ing-documents-api-openapi.yml
  format: yaml
  label: DataSinking Documents API
  slug: datasink-ing-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-documents-api-openapi.yml
- filename: datasink-ing-exchanges-api-openapi.yml
  format: yaml
  label: DataSinking Exchanges API
  slug: datasink-ing-exchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-exchanges-api-openapi.yml
- filename: datasink-ing-feedback-api-openapi.yml
  format: yaml
  label: DataSinking Feedback API
  slug: datasink-ing-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-feedback-api-openapi.yml
- filename: datasink-ing-free-key-api-openapi.yml
  format: yaml
  label: DataSinking Free Key API
  slug: datasink-ing-free-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-free-key-api-openapi.yml
- filename: datasink-ing-stocks-api-openapi.yml
  format: yaml
  label: DataSinking Stocks API
  slug: datasink-ing-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-stocks-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Datasink Ing Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'DataSinking exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DataSinking
provider_slug: datasink-ing
slug: datasink-ing-agentic-access
source_filename: datasink-ing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/datasink-ing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/sections\n  method: get\n\
  \  operationId: listDocumentSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/batch\n  method: post\n  operationId: batchDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges\n  method: get\n  operationId: listExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks\n  method: get\n  operationId: listStocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback/{id}\n  method: get\n  operationId: getFeedbackStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free-key\n  method: post\n  operationId: getFreeKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/datasink-ing/agentic-access/datasink-ing-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Finance
- Reports
- Markdown
- Data
---
