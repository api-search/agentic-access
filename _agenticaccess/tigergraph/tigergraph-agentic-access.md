---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph REST++ Data API (Vertices & Edges)
  slug: tigergraph-restpp-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Query API (Run GSQL Queries)
  slug: tigergraph-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Schema API
  slug: tigergraph-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Auth & Tokens API
  slug: tigergraph-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Savanna (Cloud) API
  slug: tigergraph-savanna-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
consequence_counts:
  read: 13
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tigergraph Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'TigerGraph exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TigerGraph
provider_slug: tigergraph
slug: tigergraph-agentic-access
source_filename: tigergraph-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tigergraph-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 13\n    acting: 9\n  by_consequence:\n    read: 13\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/echo\n  method: get\n  operationId: echoGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/echo\n  method: post\n  operationId: echoPost\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/requesttoken\n  method: post\n  operationId: requestToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/endpoints/{graph_name}\n  method: get\n  operationId: listEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gsql/v1/schema\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/ddl/{graph_name}\n  method: post\n  operationId: runLoadingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/graph/{graph_name}\n  method: post\n  operationId: upsertGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /restpp/graph/{graph_name}/vertices/{vertex_type}\n  method: get\n  operationId: listVertices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/graph/{graph_name}/vertices/{vertex_type}\n  method: delete\n  operationId: deleteVertices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/graph/{graph_name}/vertices/{vertex_type}/{vertex_id}\n  method: get\n  operationId: getVertex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/graph/{graph_name}/vertices/{vertex_type}/{vertex_id}\n  method: delete\n  operationId: deleteVertex\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/graph/{graph_name}/edges/{source_type}/{source_id}\n  method: get\n  operationId: listEdges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/graph/{graph_name}/edges/{source_type}/{source_id}/{edge_type}/{target_type}/{target_id}\n  method: get\n  operationId: getEdge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/graph/{graph_name}/edges/{source_type}/{source_id}/{edge_type}/{target_type}/{target_id}\n  method: delete\n  operationId: deleteEdge\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/query/{graph_name}/{query_name}\n  method: get\n  operationId: runInstalledQueryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/query/{graph_name}/{query_name}\n  method: post\n  operationId: runInstalledQueryPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/interpreted_query/{graph_name}\n  method: post\n  operationId: runInterpretedQuery\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restpp/path/{graph_name}\n  method: get\n  operationId: shortestPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/allpaths/{graph_name}\n  method: get\n  operationId: allPaths\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restpp/statistics/{graph_name}\n  method: get\n  operationId: getStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/agentic-access/tigergraph-agentic-access.yml
summary_line: 22 operations · 9 acting
tags:
- Graph Database
- Analytics
- GSQL
- REST++
- Graph Analytics
---
