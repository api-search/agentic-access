---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: apuchat-com-channels-api-openapi.yml
  format: yaml
  label: Apuchat Channels API
  slug: apuchat-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-channels-api-openapi.yml
- filename: apuchat-com-healthz-api-openapi.yml
  format: yaml
  label: Apuchat Healthz API
  slug: apuchat-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-healthz-api-openapi.yml
- filename: apuchat-com-info-api-openapi.yml
  format: yaml
  label: Apuchat Info API
  slug: apuchat-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-info-api-openapi.yml
- filename: apuchat-com-stats-api-openapi.yml
  format: yaml
  label: Apuchat Stats API
  slug: apuchat-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-stats-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apuchat Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Apuchat exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apuchat
provider_slug: apuchat-com
slug: apuchat-com-agentic-access
source_filename: apuchat-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/apuchat-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 3\n    acting: 2\n  by_consequence:\n    read: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/info\n  method: get\n  operationId: getServiceInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: healthCheck\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/channels\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/channels/{id}/join\n  method: post\n  operationId: joinChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/apuchat-com/agentic-access/apuchat-com-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Artificial Intelligence
- Communications
- Multi-Agent
- MCP
- Chat
---
