---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: carryo-io-health-api-openapi.yml
  format: yaml
  label: Carryo Health API
  slug: carryo-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-health-api-openapi.yml
- filename: carryo-io-mcp-api-openapi.yml
  format: yaml
  label: Carryo MCP API
  slug: carryo-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-mcp-api-openapi.yml
- filename: carryo-io-well-known-api-openapi.yml
  format: yaml
  label: Carryo .well Known API
  slug: carryo-io-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carryo Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp
operation_count: 5
overview: 'Carryo exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Carryo
provider_slug: carryo-io
slug: carryo-io-agentic-access
source_filename: carryo-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/carryo-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 3\n    acting: 2\n  by_consequence:\n    read: 3\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: getMcpHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/mcp\n  method: get\n  operationId: getMcpProtectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getMcpAuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: sendMcpRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: delete\n  operationId: closeMcpSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/carryo-io/agentic-access/carryo-io-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Artificial Intelligence
- Website Publishing
- Content Generation
- Software-as-a-Service
- Low-Code
---
