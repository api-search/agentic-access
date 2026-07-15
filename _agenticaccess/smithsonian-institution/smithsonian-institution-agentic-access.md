---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: smithsonian-open-access-openapi.yml
  format: yaml
  label: Smithsonian Open Access API
  slug: open-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/openapi/smithsonian-open-access-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smithsonian Institution Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Smithsonian Institution exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Smithsonian Institution
provider_slug: smithsonian-institution
slug: smithsonian-institution-agentic-access
source_filename: smithsonian-institution-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smithsonian-open-access-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/content\n  method: get\n  operationId: getContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/category_search\n  method: get\n  operationId:\
  \ searchByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/terms\n  method: get\n  operationId: searchTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/metrics/stats\n  method: get\n  operationId: getMetricsStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithsonian-institution/refs/heads/main/agentic-access/smithsonian-institution-agentic-access.yml
summary_line: 5 operations
tags:
- Collections
- Cultural Heritage
- Museums
- Open Data
- Art
- Natural History
- Research
---
