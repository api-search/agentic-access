---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: dataforb2b-ai-dataforb2b-api-api-openapi.yml
  format: yaml
  label: dataforb2b-ai DataForB2B API
  slug: dataforb2b-ai-dataforb2b-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataforb2b-ai/openapi/dataforb2b-ai-dataforb2b-api-api-openapi.yml
- filename: dataforb2b-ai-health-api-openapi.yml
  format: yaml
  label: dataforb2b-ai Health API
  slug: dataforb2b-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataforb2b-ai/openapi/dataforb2b-ai-health-api-openapi.yml
- filename: dataforb2b-ai-search-api-openapi.yml
  format: yaml
  label: dataforb2b-ai Search API
  slug: dataforb2b-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataforb2b-ai/openapi/dataforb2b-ai-search-api-openapi.yml
- filename: dataforb2b-ai-stats-api-openapi.yml
  format: yaml
  label: dataforb2b-ai Stats API
  slug: dataforb2b-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataforb2b-ai/openapi/dataforb2b-ai-stats-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dataforb2B Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'dataforb2b-ai exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: dataforb2b-ai
provider_slug: dataforb2b-ai
slug: dataforb2b-ai-agentic-access
source_filename: dataforb2b-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/dataforb2b-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: get_stats_stats_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/people\n  method: post\n  operationId: search_people_endpoint_search_people_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/companies\n  method: post\n  operationId: search_companies_endpoint_search_companies_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/posts\n  method: post\n  operationId: search_posts_endpoint_search_posts_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dataforb2b-ai/agentic-access/dataforb2b-ai-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Data
- B2B
- Artificial Intelligence
- Analytics
---
