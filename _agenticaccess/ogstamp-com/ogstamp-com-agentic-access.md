---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: ogstamp-com-auto-api-openapi.yml
  format: yaml
  label: ogstamp-com Auto API
  slug: ogstamp-com-auto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-auto-api-openapi.yml
- filename: ogstamp-com-credits-api-openapi.yml
  format: yaml
  label: ogstamp-com Credits API
  slug: ogstamp-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-credits-api-openapi.yml
- filename: ogstamp-com-mcp-api-openapi.yml
  format: yaml
  label: ogstamp-com MCP API
  slug: ogstamp-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-mcp-api-openapi.yml
- filename: ogstamp-com-og-api-openapi.yml
  format: yaml
  label: ogstamp-com Og API
  slug: ogstamp-com-og-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-og-api-openapi.yml
- filename: ogstamp-com-packs-api-openapi.yml
  format: yaml
  label: ogstamp-com Packs API
  slug: ogstamp-com-packs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-packs-api-openapi.yml
- filename: ogstamp-com-peek-api-openapi.yml
  format: yaml
  label: ogstamp-com Peek API
  slug: ogstamp-com-peek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-peek-api-openapi.yml
- filename: ogstamp-com-recover-api-openapi.yml
  format: yaml
  label: ogstamp-com Recover API
  slug: ogstamp-com-recover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogstamp-com/openapi/ogstamp-com-recover-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ogstamp Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'ogstamp-com exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ogstamp-com
provider_slug: ogstamp-com
slug: ogstamp-com-agentic-access
source_filename: ogstamp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/ogstamp-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/og\n  method: get\n  operationId: renderOgFree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/og\n  method: post\n  operationId: renderOgPaid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/packs\n  method: get\n  operationId: listPacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/credits\n  method: get\n  operationId: creditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auto\n  method: get\n  operationId: renderOgFromUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/peek\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recover\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ogstamp-com/agentic-access/ogstamp-com-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- OpenGraph
- Image Generation
- Pay-as-you-go
- Social Media
---
