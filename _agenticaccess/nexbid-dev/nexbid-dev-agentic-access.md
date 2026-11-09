---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: nexbid-dev-agent-api-openapi.yml
  format: yaml
  label: nexbid-dev Agent API
  slug: nexbid-dev-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexbid-dev/openapi/nexbid-dev-agent-api-openapi.yml
- filename: nexbid-dev-attribution-api-openapi.yml
  format: yaml
  label: nexbid-dev Attribution API
  slug: nexbid-dev-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexbid-dev/openapi/nexbid-dev-attribution-api-openapi.yml
- filename: nexbid-dev-discovery-api-openapi.yml
  format: yaml
  label: nexbid-dev Discovery API
  slug: nexbid-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexbid-dev/openapi/nexbid-dev-discovery-api-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nexbid Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'nexbid-dev exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: nexbid-dev
provider_slug: nexbid-dev
slug: nexbid-dev-agentic-access
source_filename: nexbid-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/nexbid-dev-agent-openapi.json, openapi/nexbid-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /agent/snippet/{id}\n  method: get\n  operationId: getAgentSnippet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/match\n  method: get\n  operationId: matchAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /agent/track\n  method: post\n  operationId: trackBeacon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/mcp.json\n  method: get\n  operationId: getMcpDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: getAgentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agents.json\n  method: get\n  operationId: getAgentsManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/discover\n  method: post\n  operationId: discoverProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feeds\n  method: post\n  operationId: createFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/click\n  method: post\n  operationId: generateClickUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/nexbid-dev/agentic-access/nexbid-dev-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Company
- Artificial Intelligence
- Commerce
- Advertising
- Switzerland
- Open Source
---
