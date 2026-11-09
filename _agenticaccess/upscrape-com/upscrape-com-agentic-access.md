---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: upscrape-com-pinterest-api-openapi.yml
  format: yaml
  label: upscrape-com Pinterest API
  slug: upscrape-com-pinterest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upscrape-com/openapi/upscrape-com-pinterest-api-openapi.yml
- filename: upscrape-com-system-api-openapi.yml
  format: yaml
  label: upscrape-com System API
  slug: upscrape-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upscrape-com/openapi/upscrape-com-system-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Upscrape Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'upscrape-com exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: upscrape-com
provider_slug: upscrape-com
slug: upscrape-com-agentic-access
source_filename: upscrape-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/upscrape-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ready\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/v1/pinterest/pins\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/upscrape-com/agentic-access/upscrape-com-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Web Scraping
- Data Extraction
- AI Integration
- MCP
---
