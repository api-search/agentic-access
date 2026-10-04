---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 18
api_specs:
- filename: halo-connect-fhir-api-openapi.yml
  format: yaml
  label: Halo Connect FHIR API
  slug: halo-connect-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-fhir-api-openapi.yml
- filename: halo-connect-registered-queries-api-openapi.yml
  format: yaml
  label: Halo Connect Registered Queries API
  slug: halo-connect-registered-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-registered-queries-api-openapi.yml
- filename: halo-connect-sites-api-openapi.yml
  format: yaml
  label: Halo Connect Sites API
  slug: halo-connect-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-sites-api-openapi.yml
- filename: halo-connect-sql-passthrough-api-openapi.yml
  format: yaml
  label: Halo Connect SQL Passthrough API
  slug: halo-connect-sql-passthrough-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-sql-passthrough-api-openapi.yml
- filename: halo-connect-tokens-api-openapi.yml
  format: yaml
  label: Halo Connect Tokens API
  slug: halo-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-tokens-api-openapi.yml
consequence_counts:
  read: 18
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Halo Connect Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Halo Connect exposes 29 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Halo Connect
provider_slug: halo-connect
slug: halo-connect-agentic-access
source_filename: halo-connect-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/halo-connect-fhir-api-openapi.yml, openapi/halo-connect-registered-queries-api-openapi.yml,\n  openapi/halo-connect-sites-api-openapi.yml, openapi/halo-connect-sql-passthrough-api-openapi.yml,\n  openapi/halo-connect-tokens-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 18\n    acting: 11\n  by_consequence:\n    read: 18\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /desktop/sites/{siteId}/fhir/R4/{fhirParameters}\n  method: get\n  operationId: getFhirQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /desktop/sites/{siteId}/fhir/R4/{resource}/_search\n  method: post\n  operationId: postFhirSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/fhir/R4/{fhirParameters}\n  method: get\n  operationId: getFhirQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/fhir/R4/{resource}/_search\n  method: post\n  operationId: postFhirSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/queries/registered\n  method: post\n  operationId: createRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/registered\n  method: get\n  operationId: getRegisteredQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/queries/registered/{queryId}\n  method: get\n  operationId: getRegisteredQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /desktop/sites/{siteId}/queries/registered/{queryId}\n  method: delete\n  operationId: cancelRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/registered/{queryId}/results\n  method: get\n  operationId: getRegisteredQueryResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/registered\n  method: post\n  operationId: createRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/registered\n  method: get\n  operationId: getRegisteredQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/registered/{queryId}\n\
  \  method: get\n  operationId: getRegisteredQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/registered/{queryId}\n  method: delete\n  operationId: cancelRegisteredQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/registered/{queryId}/results\n  method: get\n  operationId: getRegisteredQueryResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/pair-site\n  method: post\n  operationId: Integrator_PairSite\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/pairSite\n  method: post\n  operationId: pairSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites\n  method: get\n  operationId: getSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /desktop/sites/{siteId}/queries/immediate\n  method: post\n  operationId: createImmediateQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/async\n  method: post\n  operationId: createAsyncQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /desktop/sites/{siteId}/queries/{queryId}\n  method: get\n  operationId: getQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /desktop/sites/{siteId}/queries/{queryId}/results/{pageNumber}\n  method: get\n  operationId: getResultPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/immediate\n  method: post\n  operationId: createImmediateQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrator/sites/{siteId}/queries/async\n  method: post\n  operationId: createAsyncQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /integrator/sites/{siteId}/queries/{queryId}\n  method: get\n  operationId: getQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/status\n  method: post\n  operationId: getQueryStatusBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/{queryId}/results/{pageNumber}\n  method: get\n  operationId: getResultPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/sites/{siteId}/queries/{queryId}/results/{pageNumber}/stream\n  method: get\n  operationId: streamResultPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrator/token\n  method: post\n  operationId: obtainToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/agentic-access/halo-connect-agentic-access.yml
summary_line: 29 operations · 11 acting
tags:
- Healthcare
- Australia
- FHIR
- HL7
- Interoperability
- EHR
- Practice Management
- Primary Care
- AU Base
- Health Data
---
