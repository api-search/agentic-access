---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 15
api_specs:
- filename: best-practice-fhir-api-openapi.yml
  format: yaml
  label: Best Practice Software FHIR API
  slug: best-practice-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/best-practice-fhir-api-openapi.yml
- filename: best-practice-registered-queries-api-openapi.yml
  format: yaml
  label: Best Practice Software Registered Queries API
  slug: best-practice-registered-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/best-practice-registered-queries-api-openapi.yml
- filename: best-practice-sites-api-openapi.yml
  format: yaml
  label: Best Practice Software Sites API
  slug: best-practice-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/best-practice-sites-api-openapi.yml
- filename: best-practice-sql-passthrough-api-openapi.yml
  format: yaml
  label: Best Practice Software SQL Passthrough API
  slug: best-practice-sql-passthrough-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/best-practice-sql-passthrough-api-openapi.yml
- filename: best-practice-tokens-api-openapi.yml
  format: yaml
  label: Best Practice Software Tokens API
  slug: best-practice-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/best-practice-tokens-api-openapi.yml
consequence_counts:
  read: 15
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Best Practice Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Best Practice Software exposes 29 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Best Practice Software
provider_slug: best-practice
slug: best-practice-agentic-access
source_filename: best-practice-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/haloconnect-desktop-openapi.json, openapi/haloconnect-integrator-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 14\n    connected: 15\n  by_consequence:\n    write: 14\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /integrator/token\n  method: post\n  operationId: obtainToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/immediate\n  method: post\n\
  \  operationId: createImmediateQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/async\n  method: post\n  operationId: createAsyncQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/registered\n  method: post\n  operationId: createRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/registered\n  method: get\n  operationId: getRegisteredQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/queries/registered/{queryId}\n  method: get\n  operationId: getRegisteredQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/queries/registered/{queryId}\n  method: delete\n  operationId: cancelRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/registered/{queryId}/results\n\
  \  method: get\n  operationId: getRegisteredQueryResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/queries/{queryId}\n  method: get\n  operationId: getQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/queries/{queryId}/results/{pageNumber}\n  method: get\n  operationId: getResultPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/fhir/R4/{fhirParameters}\n  method: get\n  operationId: getFhirQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/fhir/R4/{resource}/_search\n\
  \  method: post\n  operationId: postFhirSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/immediate\n  method: post\n  operationId: createImmediateQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/async\n  method: post\n  operationId: createAsyncQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/registered\n  method: post\n  operationId: createRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/registered\n  method: get\n  operationId: getRegisteredQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/registered/{queryId}\n  method: get\n  operationId: getRegisteredQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/registered/{queryId}\n\
  \  method: delete\n  operationId: cancelRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/registered/{queryId}/results\n  method: get\n  operationId: getRegisteredQueryResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/{queryId}\n  method: get\n  operationId: getQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/status\n  method: post\n  operationId: getQueryStatusBatch\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/{queryId}/results/{pageNumber}\n  method: get\n  operationId: getResultPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/{queryId}/results/{pageNumber}/stream\n  method: get\n  operationId: streamResultPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/fhir/R4/{fhirParameters}\n  method: get\n  operationId: getFhirQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /integrator/sites/{siteId}/fhir/R4/{resource}/_search\n  method: post\n  operationId: postFhirSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/pair-site\n  method: post\n  operationId: Integrator_PairSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/pairSite\n  method: post\n  operationId: pairSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites\n  method: get\n  operationId: getSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/agentic-access/best-practice-agentic-access.yml
summary_line: 29 operations · 14 acting
tags:
- Healthcare
- Australia
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- AU Base
- Practice Management
- General Practice
- Appointments
- Scheduling
---
