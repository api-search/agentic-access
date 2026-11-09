---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: keenable-fetch-api-openapi.yml
  format: yaml
  label: Keenable Fetch API
  slug: keenable-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenable/openapi/keenable-fetch-api-openapi.yml
- filename: keenable-search-api-openapi.yml
  format: yaml
  label: Keenable Search API
  slug: keenable-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenable/openapi/keenable-search-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Keenable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Keenable exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Keenable
provider_slug: keenable
slug: keenable-agentic-access
source_filename: keenable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: generated\nsource: openapi/keenable-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search\n  method: post\n  operationId: search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search/public\n  method: post\n  operationId: search_post_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fetch\n  method: get\n  operationId: fetch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fetch/public\n  method: get\n  operationId: fetch_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/keenable/agentic-access/keenable-agentic-access.yml
summary_line: 4 operations
tags:
- Web Search
- AI Agents
- AI Labs
- Inference Platforms
---
