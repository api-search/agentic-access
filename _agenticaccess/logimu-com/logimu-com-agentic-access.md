---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: logimu-com-coding-agents-json-api-openapi.yml
  format: yaml
  label: logimu-com Coding Agents.json API
  slug: logimu-com-coding-agents-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logimu-com/openapi/logimu-com-coding-agents-json-api-openapi.yml
- filename: logimu-com-deprecations-json-api-openapi.yml
  format: yaml
  label: logimu-com Deprecations.json API
  slug: logimu-com-deprecations-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logimu-com/openapi/logimu-com-deprecations-json-api-openapi.yml
- filename: logimu-com-rankings-json-api-openapi.yml
  format: yaml
  label: logimu-com Rankings.json API
  slug: logimu-com-rankings-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logimu-com/openapi/logimu-com-rankings-json-api-openapi.yml
- filename: logimu-com-subscribe-api-openapi.yml
  format: yaml
  label: logimu-com Subscribe API
  slug: logimu-com-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logimu-com/openapi/logimu-com-subscribe-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Logimu Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscribe
operation_count: 4
overview: 'logimu-com exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: logimu-com
provider_slug: logimu-com
slug: logimu-com-agentic-access
source_filename: logimu-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/logimu-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/rankings.json\n  method: get\n  operationId: getRankings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deprecations.json\n  method: get\n  operationId: getDeprecations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/coding-agents.json\n\
  \  method: get\n  operationId: getCodingAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribe\n  method: post\n  operationId: subscribeAlerts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/logimu-com/agentic-access/logimu-com-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Company
- E-Commerce
- Data API
- Amazon
- Walmart
---
