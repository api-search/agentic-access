---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: thingstodoapi-com-coverage-api-openapi.yml
  format: yaml
  label: thingstodoapi-com Coverage API
  slug: thingstodoapi-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thingstodoapi-com/openapi/thingstodoapi-com-coverage-api-openapi.yml
- filename: thingstodoapi-com-events-api-openapi.yml
  format: yaml
  label: thingstodoapi-com Events API
  slug: thingstodoapi-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thingstodoapi-com/openapi/thingstodoapi-com-events-api-openapi.yml
- filename: thingstodoapi-com-keys-api-openapi.yml
  format: yaml
  label: thingstodoapi-com Keys API
  slug: thingstodoapi-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thingstodoapi-com/openapi/thingstodoapi-com-keys-api-openapi.yml
- filename: thingstodoapi-com-mcp-api-openapi.yml
  format: yaml
  label: thingstodoapi-com MCP API
  slug: thingstodoapi-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thingstodoapi-com/openapi/thingstodoapi-com-mcp-api-openapi.yml
- filename: thingstodoapi-com-search-api-openapi.yml
  format: yaml
  label: thingstodoapi-com Search API
  slug: thingstodoapi-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thingstodoapi-com/openapi/thingstodoapi-com-search-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thingstodoapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'thingstodoapi-com exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: thingstodoapi-com
provider_slug: thingstodoapi-com
slug: thingstodoapi-com-agentic-access
source_filename: thingstodoapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/thingstodoapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search\n  method: get\n  operationId: searchEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coverage\n  method: get\n  operationId:\
  \ listCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/thingstodoapi-com/agentic-access/thingstodoapi-com-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Event
- Local
- Artificial Intelligence
- JSON
- MCP
---
