---
acting_count: 0
action_class_counts:
  connected: 2
api_specs:
- filename: fed-spend-com-contracts-api-openapi.yml
  format: yaml
  label: Fed-Spend Contracts API
  slug: fed-spend-com-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fed-spend-com/openapi/fed-spend-com-contracts-api-openapi.yml
- filename: fed-spend-com-search-api-openapi.yml
  format: yaml
  label: Fed-Spend Search API
  slug: fed-spend-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fed-spend-com/openapi/fed-spend-com-search-api-openapi.yml
consequence_counts:
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fed Spend Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Fed-Spend exposes 2 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fed-Spend
provider_slug: fed-spend-com
slug: fed-spend-com-agentic-access
source_filename: fed-spend-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/fed-spend-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 2\n  by_consequence:\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{id}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fed-spend-com/agentic-access/fed-spend-com-agentic-access.yml
summary_line: 2 operations
tags:
- Business Intelligence
- Government
- Federal Spending
- Data Analytics
- Contract Intelligence
- Company
---
