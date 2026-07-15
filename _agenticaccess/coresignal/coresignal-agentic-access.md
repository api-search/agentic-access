---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: coresignal-multi-source-company-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Company API
  slug: multi-source-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-company-api-openapi.yml
- filename: coresignal-multi-source-employee-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Employee API
  slug: multi-source-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-employee-api-openapi.yml
- filename: coresignal-multi-source-jobs-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Jobs API
  slug: multi-source-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-jobs-api-openapi.yml
consequence_counts:
  read: 3
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coresignal Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Coresignal exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coresignal
provider_slug: coresignal
slug: coresignal-agentic-access
source_filename: coresignal-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/coresignal-multi-source-company-api-openapi.yml, openapi/coresignal-multi-source-employee-api-openapi.yml,\n  openapi/coresignal-multi-source-jobs-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 8\n    connected: 3\n  by_consequence:\n    write: 8\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /search/filter\n  method: post\n  operationId: searchCompaniesByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /search/es_dsl\n  method: post\n  operationId: searchCompaniesByEsDsl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/{id}\n  method: get\n  operationId: collectCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk_collect\n  method: post\n  operationId: bulkCollectCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/filter\n  method: post\n  operationId:\
  \ searchEmployeesByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/es_dsl\n  method: post\n  operationId: searchEmployeesByEsDsl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/{id}\n  method: get\n  operationId: collectEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk_collect\n  method: post\n  operationId: bulkCollectEmployees\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/filter\n  method: post\n  operationId: searchJobsByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/es_dsl\n  method: post\n  operationId: searchJobsByEsDsl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/{id}\n  method: get\n  operationId: collectJob\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/agentic-access/coresignal-agentic-access.yml
summary_line: 11 operations · 8 acting
tags:
- Agentic Search
- B2B Data
- Companies
- Company Data
- Data as a Service
- Elasticsearch
- Employee Data
- Employees
- Enrichment
- Firmographics
- Job Postings
- Jobs
- Lead Generation
- People Data
- Sales Intelligence
- Talent Intelligence
- Web Data
---
