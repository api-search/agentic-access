---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: notfair-co-health-api-openapi.yml
  format: yaml
  label: notfair-co Health API
  slug: notfair-co-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-health-api-openapi.yml
- filename: notfair-co-mcp-api-openapi.yml
  format: yaml
  label: notfair-co MCP API
  slug: notfair-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-mcp-api-openapi.yml
- filename: notfair-co-well-known-api-openapi.yml
  format: yaml
  label: notfair-co .well Known API
  slug: notfair-co-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Notfair Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/notfair
operation_count: 4
overview: 'notfair-co exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: notfair-co
provider_slug: notfair-co
slug: notfair-co-agentic-access
source_filename: notfair-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/notfair-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/health\n  method: get\n  operationId: getNotFairHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: getNotFairMcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/api/mcp/notfair\n\
  \  method: get\n  operationId: getNotFairProtectedResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/notfair\n  method: post\n  operationId: sendNotFairMcpMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/notfair-co/agentic-access/notfair-co-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Company
- Advertising
- Artificial Intelligence
- Marketing
- Automation
---
