---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: 9bot-com-br-discovery-api-openapi.yml
  format: yaml
  label: 9bot Discovery API
  slug: 9bot-com-br-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-discovery-api-openapi.yml
- filename: 9bot-com-br-health-api-openapi.yml
  format: yaml
  label: 9bot Health API
  slug: 9bot-com-br-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-health-api-openapi.yml
- filename: 9bot-com-br-mcp-api-openapi.yml
  format: yaml
  label: 9bot MCP API
  slug: 9bot-com-br-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/9bot-com-br/openapi/9bot-com-br-mcp-api-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 9Bot Com Br Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: '9bot exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 9bot
provider_slug: 9bot-com-br
slug: 9bot-com-br-agentic-access
source_filename: 9bot-com-br-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/9bot-com-br-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 1\n    connected: 5\n  by_consequence:\n    write: 1\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: exchangeMcpMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/health\n  method: get\n  operationId: getMcpHealth\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp\n  method: get\n  operationId: getMcpMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: getOAuthProtectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getOAuthAuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server.json\n  method: get\n  operationId: getMcpRegistryManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/9bot-com-br/agentic-access/9bot-com-br-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- WhatsApp
- Automation
- Bot
- Messaging
- Integration
---
