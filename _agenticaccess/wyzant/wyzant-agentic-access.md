---
acting_count: 0
action_class_counts:
  connected: 2
api_specs:
- filename: wyzant-data-feed-api-openapi.yml
  format: yaml
  label: Wyzant Data Feed API
  slug: wyzant-data-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wyzant/refs/heads/main/openapi/wyzant-data-feed-api-openapi.yml
- filename: wyzant-search-api-openapi.yml
  format: yaml
  label: Wyzant Search API
  slug: wyzant-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wyzant/refs/heads/main/openapi/wyzant-search-api-openapi.yml
consequence_counts:
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wyzant Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Wyzant exposes 2 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wyzant
provider_slug: wyzant
slug: wyzant-agentic-access
source_filename: wyzant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/wyzant-data-feed-api-openapi.yml, openapi/wyzant-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 2\n  by_consequence:\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /feeds/downloadFeed\n  method: get\n  operationId: downloadTutorFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: post\n  operationId: searchTutors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyzant/refs/heads/main/agentic-access/wyzant-agentic-access.yml
summary_line: 2 operations
tags:
- Tutoring
- Education
- Marketplace
- Tutors
- EdTech
- Affiliates
- Partner API
- Data Feed
---
