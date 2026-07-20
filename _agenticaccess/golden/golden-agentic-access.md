---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: golden-openapi-original.json
  format: json
  label: Golden Public API v2
  slug: golden-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-openapi-original.json
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Golden Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Golden exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Golden
provider_slug: golden
slug: golden-agentic-access
source_filename: golden-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/golden-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/public/entities/\n  method: get\n  operationId: public_api_entities_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/public/entities/{id}/\n  method: get\n  operationId: public_api_entities_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/public/queries/{id}/results/\n\
  \  method: get\n  operationId: public_api_queries_results_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/public/queries/permalink/{permalink}/\n  method: get\n  operationId: public_api_queries_permalink_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/public/schema/entityTypes/\n  method: get\n  operationId: public_api_schema_entityTypes_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/public/schema/entityTypes/{id}/\n  method: get\n  operationId: public_api_schema_entityTypes_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/public/schema/predicates/\n  method: get\n  operationId: public_api_schema_predicates_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/public/schema/predicates/{id}/\n  method: get\n  operationId: public_api_schema_predicates_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/agentic-access/golden-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- Knowledge Graph
- Company Data
- Data
- Entities
- Artificial Intelligence
- Search
- Business Intelligence
---
