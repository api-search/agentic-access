---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 3
api_specs:
- filename: sparql-query-api-openapi.yml
  format: yaml
  label: SPARQL Query API
  slug: sparql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparql/refs/heads/main/openapi/sparql-query-api-openapi.yml
- filename: sparql-sparql-api-openapi.yml
  format: yaml
  label: SPARQL API
  slug: sparql-sparql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparql/refs/heads/main/openapi/sparql-sparql-api-openapi.yml
- filename: sparql-sparql-graph-api-openapi.yml
  format: yaml
  label: SPARQL Graph API
  slug: sparql-sparql-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparql/refs/heads/main/openapi/sparql-sparql-graph-api-openapi.yml
- filename: sparql-sparql-update-api-openapi.yml
  format: yaml
  label: SPARQL Update API
  slug: sparql-sparql-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparql/refs/heads/main/openapi/sparql-sparql-update-api-openapi.yml
- filename: sparql-update-api-openapi.yml
  format: yaml
  label: SPARQL Update API
  slug: sparql-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparql/refs/heads/main/openapi/sparql-update-api-openapi.yml
consequence_counts:
  read: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sparql Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'SPARQL exposes 10 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SPARQL
provider_slug: sparql
slug: sparql-agentic-access
source_filename: sparql-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/sparql-query-api-openapi.yml, openapi/sparql-sparql-api-openapi.yml, openapi/sparql-sparql-graph-api-openapi.yml,\n  openapi/sparql-sparql-update-api-openapi.yml, openapi/sparql-update-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 3\n    acting: 7\n  by_consequence:\n    read: 3\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /sparql\n  method: get\n  operationId: queryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sparql\n  method: post\n  operationId: queryPost\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sparql\n  method: get\n  operationId: sparqlQueryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sparql\n  method: post\n  operationId: sparqlQueryPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sparql-graph\n  method: get\n  operationId: graphStoreGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /sparql-graph\n  method: put\n  operationId: graphStorePut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sparql-graph\n  method: post\n  operationId: graphStorePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sparql-graph\n  method: delete\n  operationId: graphStoreDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /sparql-update\n  method: post\n  operationId: sparqlUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sparql/update\n  method: post\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparql/refs/heads/main/agentic-access/sparql-agentic-access.yml
summary_line: 10 operations · 7 acting
tags:
- Linked Data
- Query Language
- RDF
- Semantic Web
- SPARQL
- W3C
---
